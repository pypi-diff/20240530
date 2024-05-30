# Comparing `tmp/agency_swarm-0.2.3.tar.gz` & `tmp/agency_swarm-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agency_swarm-0.2.3.tar", last modified: Sat May 25 17:26:10 2024, max compression
+gzip compressed data, was "agency_swarm-0.2.5.tar", last modified: Thu May 30 05:16:08 2024, max compression
```

## Comparing `agency_swarm-0.2.3.tar` & `agency_swarm-0.2.5.tar`

### file list

```diff
@@ -1,193 +1,195 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.799035 agency_swarm-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.767035 agency_swarm-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.775035 agency_swarm-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/.github/workflows/close-issues.yml
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12151 2024-05-25 17:26:10.799035 agency_swarm-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.775035 agency_swarm-0.2.3/agency_swarm/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.775035 agency_swarm-0.2.3/agency_swarm/agency/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47586 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/agency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.779035 agency_swarm-0.2.3/agency_swarm/agency/genesis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.779035 agency_swarm-0.2.3/agency_swarm/agency/genesis/AgentCreator/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/AgentCreator/AgentCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/AgentCreator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/AgentCreator/instructions.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.779035 agency_swarm-0.2.3/agency_swarm/agency/genesis/AgentCreator/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/AgentCreator/tools/CreateAgentTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/AgentCreator/tools/ImportAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/AgentCreator/tools/ReadManifesto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.779035 agency_swarm-0.2.3/agency_swarm/agency/genesis/AgentCreator/tools/util/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/AgentCreator/tools/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/AgentCreator/tools/util/get_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/GenesisAgency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.779035 agency_swarm-0.2.3/agency_swarm/agency/genesis/GenesisCEO/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/GenesisCEO/GenesisCEO.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/GenesisCEO/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/GenesisCEO/instructions.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.779035 agency_swarm-0.2.3/agency_swarm/agency/genesis/GenesisCEO/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/GenesisCEO/tools/CreateAgencyFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/GenesisCEO/tools/FinalizeAgency.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/GenesisCEO/tools/ReadRequirements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.779035 agency_swarm-0.2.3/agency_swarm/agency/genesis/OpenAPICreator/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/OpenAPICreator/OpenAPICreator.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/OpenAPICreator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/OpenAPICreator/instructions.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.779035 agency_swarm-0.2.3/agency_swarm/agency/genesis/OpenAPICreator/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/OpenAPICreator/tools/CreateToolsFromOpenAPISpec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.783035 agency_swarm-0.2.3/agency_swarm/agency/genesis/ToolCreator/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/ToolCreator/ToolCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/ToolCreator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/ToolCreator/instructions.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.783035 agency_swarm-0.2.3/agency_swarm/agency/genesis/ToolCreator/tools/
--rw-r--r--   0 runner    (1001) docker     (127)    10957 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/ToolCreator/tools/CreateTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/ToolCreator/tools/TestTool.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/manifesto.md
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agency/genesis/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.783035 agency_swarm-0.2.3/agency_swarm/agents/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.783035 agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/
--rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/BrowsingAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/instructions.md
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.783035 agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/ClickElement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/ExportFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/GoBack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/ReadURL.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/Scroll.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/SelectDropdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/SendKeys.py
--rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/SolveCaptcha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/WebPageSummarizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.783035 agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/util/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/util/get_b64_screenshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/util/highlights.py
--rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/util/selenium.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.787035 agency_swarm-0.2.3/agency_swarm/agents/Devid/
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/Devid/Devid.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/Devid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/Devid/instructions.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.787035 agency_swarm-0.2.3/agency_swarm/agents/Devid/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/Devid/tools/ChangeFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/Devid/tools/CheckCurrentDir.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/Devid/tools/CommandExecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/Devid/tools/DirectoryNavigator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/Devid/tools/FileMover.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/Devid/tools/FileReader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/Devid/tools/FileWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/Devid/tools/ListDir.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/Devid/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.787035 agency_swarm-0.2.3/agency_swarm/agents/Devid/tools/util/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/Devid/tools/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/Devid/tools/util/format_file_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31758 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/agents/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.787035 agency_swarm-0.2.3/agency_swarm/messages/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/messages/message_output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.787035 agency_swarm-0.2.3/agency_swarm/threads/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/threads/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/threads/thread_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.787035 agency_swarm-0.2.3/agency_swarm/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/tools/BaseTool.py
--rw-r--r--   0 runner    (1001) docker     (127)    15774 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/tools/ToolFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.791035 agency_swarm-0.2.3/agency_swarm/tools/oai/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/tools/oai/CodeInterpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/tools/oai/FileSearch.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/tools/oai/Retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/tools/oai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.791035 agency_swarm-0.2.3/agency_swarm/user/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/user/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.791035 agency_swarm-0.2.3/agency_swarm/util/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.791035 agency_swarm-0.2.3/agency_swarm/util/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/util/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/util/cli/create_agent_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/util/cli/import_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.791035 agency_swarm-0.2.3/agency_swarm/util/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/util/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/util/helpers/get_available_agent_descriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/util/helpers/list_available_agents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/util/oai.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/util/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/util/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/util/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/agency_swarm/util/streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.799035 agency_swarm-0.2.3/agency_swarm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12151 2024-05-25 17:26:10.000000 agency_swarm-0.2.3/agency_swarm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-05-25 17:26:10.000000 agency_swarm-0.2.3/agency_swarm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 17:26:10.000000 agency_swarm-0.2.3/agency_swarm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-25 17:26:10.000000 agency_swarm-0.2.3/agency_swarm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-25 17:26:10.000000 agency_swarm-0.2.3/agency_swarm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-25 17:26:10.000000 agency_swarm-0.2.3/agency_swarm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.791035 agency_swarm-0.2.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.795035 agency_swarm-0.2.3/docs/advanced-usage/
--rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/docs/advanced-usage/agencies.md
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/docs/advanced-usage/agents.md
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/docs/advanced-usage/azure-openai.md
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/docs/advanced-usage/open-source-models.md
--rw-r--r--   0 runner    (1001) docker     (127)    10461 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/docs/advanced-usage/tools.md
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/docs/api.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.795035 agency_swarm-0.2.3/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   721476 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/docs/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/docs/deployment.md
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.795035 agency_swarm-0.2.3/docs/introduction/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/docs/introduction/showcase.md
--rw-r--r--   0 runner    (1001) docker     (127)     6177 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/docs/quick_start.md
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.795035 agency_swarm-0.2.3/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    49298 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/notebooks/Agency_Swarm_with_Open_Source_Model.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/notebooks/agency_async.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/notebooks/azure.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    20289 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/notebooks/genesis_agency.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    44294 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/notebooks/web_browser_agent.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 17:26:10.799035 agency_swarm-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.795035 agency_swarm-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.771035 agency_swarm-0.2.3/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.799035 agency_swarm-0.2.3/tests/data/files/
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/tests/data/files/csv-test.csv
--rw-r--r--   0 runner    (1001) docker     (127)   102408 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/tests/data/files/generated_data.json
--rw-r--r--   0 runner    (1001) docker     (127)    12064 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/tests/data/files/test-docx.docx
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/tests/data/files/test-html.html
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/tests/data/files/test-md.md
--rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/tests/data/files/test-pdf.pdf
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/tests/data/files/test-txt.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/tests/data/files/test-xml.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.799035 agency_swarm-0.2.3/tests/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/tests/data/schemas/ga4.json
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/tests/data/schemas/get-headers-params.json
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/tests/data/schemas/get-weather.json
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/tests/data/schemas/relevance.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.799035 agency_swarm-0.2.3/tests/data/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/tests/data/tools/ExampleTool1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:26:10.799035 agency_swarm-0.2.3/tests/demos/
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/tests/demos/demo_gradio.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/tests/demos/streaming_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/tests/demos/term_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)    20806 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/tests/test_agency.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-05-25 17:26:06.000000 agency_swarm-0.2.3/tests/test_tool_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.241084 agency_swarm-0.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.209085 agency_swarm-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.217085 agency_swarm-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/.github/workflows/close-issues.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12199 2024-05-30 05:16:08.241084 agency_swarm-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.217085 agency_swarm-0.2.5/agency_swarm/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.217085 agency_swarm-0.2.5/agency_swarm/agency/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54101 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/agency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.221085 agency_swarm-0.2.5/agency_swarm/agency/genesis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.221085 agency_swarm-0.2.5/agency_swarm/agency/genesis/AgentCreator/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/AgentCreator/AgentCreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/AgentCreator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/AgentCreator/instructions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.221085 agency_swarm-0.2.5/agency_swarm/agency/genesis/AgentCreator/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/AgentCreator/tools/CreateAgentTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/AgentCreator/tools/ImportAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/AgentCreator/tools/ReadManifesto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.221085 agency_swarm-0.2.5/agency_swarm/agency/genesis/AgentCreator/tools/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/AgentCreator/tools/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/AgentCreator/tools/util/get_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/GenesisAgency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.221085 agency_swarm-0.2.5/agency_swarm/agency/genesis/GenesisCEO/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/GenesisCEO/GenesisCEO.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/GenesisCEO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/GenesisCEO/instructions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.221085 agency_swarm-0.2.5/agency_swarm/agency/genesis/GenesisCEO/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/GenesisCEO/tools/CreateAgencyFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/GenesisCEO/tools/FinalizeAgency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/GenesisCEO/tools/ReadRequirements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.221085 agency_swarm-0.2.5/agency_swarm/agency/genesis/OpenAPICreator/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/OpenAPICreator/OpenAPICreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/OpenAPICreator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/OpenAPICreator/instructions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.221085 agency_swarm-0.2.5/agency_swarm/agency/genesis/OpenAPICreator/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/OpenAPICreator/tools/CreateToolsFromOpenAPISpec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.225085 agency_swarm-0.2.5/agency_swarm/agency/genesis/ToolCreator/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/ToolCreator/ToolCreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/ToolCreator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/ToolCreator/instructions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.225085 agency_swarm-0.2.5/agency_swarm/agency/genesis/ToolCreator/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    10952 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/ToolCreator/tools/CreateTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/ToolCreator/tools/TestTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/manifesto.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agency/genesis/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.225085 agency_swarm-0.2.5/agency_swarm/agents/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.225085 agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/
+-rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/BrowsingAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/instructions.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.225085 agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/ClickElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/ExportFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/GoBack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/ReadURL.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/Scroll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/SelectDropdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/SendKeys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/SolveCaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/WebPageSummarizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.229085 agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/util/get_b64_screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/util/highlights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/util/selenium.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.229085 agency_swarm-0.2.5/agency_swarm/agents/Devid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/Devid/Devid.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/Devid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/Devid/instructions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.229085 agency_swarm-0.2.5/agency_swarm/agents/Devid/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/Devid/tools/ChangeFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/Devid/tools/CheckCurrentDir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/Devid/tools/CommandExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/Devid/tools/DirectoryNavigator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/Devid/tools/FileMover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/Devid/tools/FileReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/Devid/tools/FileWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/Devid/tools/ListDir.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/Devid/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.229085 agency_swarm-0.2.5/agency_swarm/agents/Devid/tools/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/Devid/tools/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/Devid/tools/util/format_file_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31978 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/agents/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.229085 agency_swarm-0.2.5/agency_swarm/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/messages/message_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.229085 agency_swarm-0.2.5/agency_swarm/threads/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16409 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/threads/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/threads/thread_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.229085 agency_swarm-0.2.5/agency_swarm/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/tools/BaseTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12908 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/tools/ToolFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.233085 agency_swarm-0.2.5/agency_swarm/tools/oai/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/tools/oai/CodeInterpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/tools/oai/FileSearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/tools/oai/Retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/tools/oai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.233085 agency_swarm-0.2.5/agency_swarm/user/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/user/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.233085 agency_swarm-0.2.5/agency_swarm/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.233085 agency_swarm-0.2.5/agency_swarm/util/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/util/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/util/cli/create_agent_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/util/cli/import_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/util/files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.233085 agency_swarm-0.2.5/agency_swarm/util/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/util/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/util/helpers/get_available_agent_descriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/util/helpers/list_available_agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/util/oai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/util/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/util/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/util/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/agency_swarm/util/streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.241084 agency_swarm-0.2.5/agency_swarm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12199 2024-05-30 05:16:08.000000 agency_swarm-0.2.5/agency_swarm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-30 05:16:08.000000 agency_swarm-0.2.5/agency_swarm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 05:16:08.000000 agency_swarm-0.2.5/agency_swarm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 05:16:08.000000 agency_swarm-0.2.5/agency_swarm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-30 05:16:08.000000 agency_swarm-0.2.5/agency_swarm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 05:16:08.000000 agency_swarm-0.2.5/agency_swarm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.233085 agency_swarm-0.2.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.237084 agency_swarm-0.2.5/docs/advanced-usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/docs/advanced-usage/agencies.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/docs/advanced-usage/agents.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/docs/advanced-usage/azure-openai.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/docs/advanced-usage/open-source-models.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10461 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/docs/advanced-usage/tools.md
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/docs/api.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.237084 agency_swarm-0.2.5/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   721476 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/docs/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/docs/deployment.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.237084 agency_swarm-0.2.5/docs/introduction/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/docs/introduction/showcase.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/docs/quick_start.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.237084 agency_swarm-0.2.5/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    49298 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/notebooks/Agency_Swarm_with_Open_Source_Model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/notebooks/agency_async.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/notebooks/azure.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    20289 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/notebooks/genesis_agency.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    44294 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/notebooks/web_browser_agent.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 05:16:08.241084 agency_swarm-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.237084 agency_swarm-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.213085 agency_swarm-0.2.5/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.241084 agency_swarm-0.2.5/tests/data/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/tests/data/files/csv-test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   102408 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/tests/data/files/generated_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12064 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/tests/data/files/test-docx.docx
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/tests/data/files/test-html.html
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/tests/data/files/test-md.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/tests/data/files/test-pdf.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/tests/data/files/test-txt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/tests/data/files/test-xml.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.241084 agency_swarm-0.2.5/tests/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/tests/data/schemas/ga4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/tests/data/schemas/get-headers-params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/tests/data/schemas/get-weather.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/tests/data/schemas/relevance.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.241084 agency_swarm-0.2.5/tests/data/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/tests/data/tools/ExampleTool1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:08.241084 agency_swarm-0.2.5/tests/demos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/tests/demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/tests/demos/demo_gradio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/tests/demos/streaming_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/tests/demos/term_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20970 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/tests/test_agency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7083 2024-05-30 05:16:04.000000 agency_swarm-0.2.5/tests/test_tool_factory.py
```

### Comparing `agency_swarm-0.2.3/.github/workflows/close-issues.yml` & `agency_swarm-0.2.5/.github/workflows/close-issues.yml`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/.github/workflows/docs.yml` & `agency_swarm-0.2.5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/.github/workflows/publish.yml` & `agency_swarm-0.2.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/.github/workflows/test.yml` & `agency_swarm-0.2.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/.gitignore` & `agency_swarm-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/CONTRIBUTING.md` & `agency_swarm-0.2.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/LICENSE` & `agency_swarm-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/PKG-INFO` & `agency_swarm-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agency-swarm
-Version: 0.2.3
+Version: 0.2.5
 Summary: An open source agent orchestration framework built on top of the latest OpenAI Assistants API.
 Home-page: https://github.com/VRSEN/agency-swarm
 Author: VRSEN
 Author-email: VRSEN <arseny9795@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Arsenii Shatokhin
@@ -30,20 +30,21 @@
 Project-URL: homepage, https://github.com/VRSEN/agency-swarm
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai==1.30.3
-Requires-Dist: instructor==1.3.1
+Requires-Dist: openai==1.30.4
+Requires-Dist: instructor==1.3.2
+Requires-Dist: datamodel-code-generator==0.25.6
 Requires-Dist: deepdiff==6.7.1
-Requires-Dist: termcolor==2.3.0
-Requires-Dist: python-dotenv==1.0.0
-Requires-Dist: rich==13.7.0
+Requires-Dist: termcolor==2.4.0
+Requires-Dist: python-dotenv==1.0.1
+Requires-Dist: rich==13.7.1
 Requires-Dist: jsonref==1.1.0
 
 # 🐝 Agency Swarm
 
 [![Framework](https://firebasestorage.googleapis.com/v0/b/vrsen-ai/o/public%2Fyoutube%2FFramework.png?alt=media&token=ae76687f-0347-4e0c-8342-4c5d31e3f050)](https://youtu.be/M5Pa0pLgyYU?si=f-cQV8FoiGd98uuk)
 
 ## Overview
```

### Comparing `agency_swarm-0.2.3/README.md` & `agency_swarm-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agency/agency.py` & `agency_swarm-0.2.5/agency_swarm/agency/agency.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import inspect
 import json
 import os
 import queue
 import threading
+import time
 import uuid
 from enum import Enum
 from typing import List, TypedDict, Callable, Any, Dict, Literal, Union, Optional
 
 from openai.types.beta.threads import Message
 from openai.types.beta.threads.runs import RunStep
 from pydantic import Field, field_validator, model_validator
@@ -15,15 +16,18 @@
 
 from agency_swarm.agents import Agent
 from agency_swarm.messages import MessageOutput
 from agency_swarm.messages.message_output import MessageOutputLive
 from agency_swarm.threads import Thread
 from agency_swarm.tools import BaseTool, FileSearch, CodeInterpreter
 from agency_swarm.user import User
+from agency_swarm.util.files import determine_file_type
 from agency_swarm.util.shared_state import SharedState
+from openai.types.beta.threads.runs.tool_call import ToolCall, FunctionToolCall, CodeInterpreterToolCall, FileSearchToolCall
+
 
 from agency_swarm.util.streaming import AgencyEventHandler
 
 console = Console()
 
 
 class SettingsCallbacks(TypedDict):
@@ -62,19 +66,19 @@
             agency_chart: The structure defining the hierarchy and interaction of agents within the agency.
             shared_instructions (str, optional): A path to a file containing shared instructions for all agents. Defaults to an empty string.
             shared_files (Union[str, List[str]], optional): A path to a folder or a list of folders containing shared files for all agents. Defaults to None.
             async_mode (str, optional): The mode for asynchronous message processing. Defaults to None.
             settings_path (str, optional): The path to the settings file for the agency. Must be json. If file does not exist, it will be created. Defaults to None.
             settings_callbacks (SettingsCallbacks, optional): A dictionary containing functions to load and save settings for the agency. The keys must be "load" and "save". Both values must be defined. Defaults to None.
             threads_callbacks (ThreadsCallbacks, optional): A dictionary containing functions to load and save threads for the agency. The keys must be "load" and "save". Both values must be defined. Defaults to None.
-            temperature (float, optional): The temperature value to use for the agents. Agent specific values will override this. Defaults to 0.3.
-            top_p (float, optional): The top_p value to use for the agents. Agent specific values will override this. Defaults to None.
-            max_prompt_tokens (int, optional): The maximum number of tokens allowed in the prompt for each agent. Agent specific values will override this. Defaults to None.
-            max_completion_tokens (int, optional): The maximum number of tokens allowed in the completion for each agent. Agent specific values will override this. Defaults to None.
-            truncation_strategy (dict, optional): The truncation strategy to use for the completion for each agent. Agent specific values will override this. Defaults to None.
+            temperature (float, optional): The temperature value to use for the agents. Agent-specific values will override this. Defaults to 0.3.
+            top_p (float, optional): The top_p value to use for the agents. Agent-specific values will override this. Defaults to None.
+            max_prompt_tokens (int, optional): The maximum number of tokens allowed in the prompt for each agent. Agent-specific values will override this. Defaults to None.
+            max_completion_tokens (int, optional): The maximum number of tokens allowed in the completion for each agent. Agent-specific values will override this. Defaults to None.
+            truncation_strategy (dict, optional): The truncation strategy to use for the completion for each agent. Agent-specific values will override this. Defaults to None.
 
         This constructor initializes various components of the Agency, including CEO, agents, threads, and user interactions. It parses the agency chart to set up the organizational structure and initializes the messaging tools, agents, and threads necessary for the operation of the agency. Additionally, it prepares a main thread for user interactions.
         """
         self.async_mode = async_mode
         if self.async_mode == "threading":
             from agency_swarm.threads.thread_async import ThreadAsync
             self.ThreadType = ThreadAsync
@@ -218,62 +222,111 @@
         }"""
 
         if dark_mode:
             js = js.replace("{theme}", "dark")
         else:
             js = js.replace("{theme}", "light")
 
-        message_file_ids = []
+        attachments = []
+        images = []
         message_file_names = None
+        uploading_files = False
         recipient_agents = [agent.name for agent in self.main_recipients]
         recipient_agent = self.main_recipients[0]
 
         with gr.Blocks(js=js) as demo:
             chatbot_queue = queue.Queue()
             chatbot = gr.Chatbot(height=height)
             with gr.Row():
                 with gr.Column(scale=9):
                     dropdown = gr.Dropdown(label="Recipient Agent", choices=recipient_agents,
                                            value=recipient_agent.name)
                     msg = gr.Textbox(label="Your Message", lines=4)
                 with gr.Column(scale=1):
-                    file_upload = gr.Files(label="Files", type="filepath")
+                    file_upload = gr.Files(label="OpenAI Files", type="filepath")
             button = gr.Button(value="Send", variant="primary")
 
             def handle_dropdown_change(selected_option):
                 nonlocal recipient_agent
                 recipient_agent = self._get_agent_by_name(selected_option)
 
             def handle_file_upload(file_list):
-                nonlocal message_file_ids
+                nonlocal attachments
                 nonlocal message_file_names
-                message_file_ids = []
+                nonlocal uploading_files
+                nonlocal images
+                uploading_files = True
+                attachments = []
                 message_file_names = []
                 if file_list:
                     try:
                         for file_obj in file_list:
+                            file_type = determine_file_type(file_obj.name)
+                            purpose = "assistants" if file_type != "vision" else "vision"
+                            tools = [{"type": "code_interpreter"}] if file_type == "assistants.code_interpreter" else [{"type": "file_search"}]
+
                             with open(file_obj.name, 'rb') as f:
                                 # Upload the file to OpenAI
                                 file = self.main_thread.client.files.create(
                                     file=f,
-                                    purpose="assistants"
+                                    purpose=purpose
                                 )
-                            message_file_ids.append(file.id)
+
+                            if file_type == "vision":
+                                images.append({
+                                    "type": "image_file",
+                                    "image_file": {"file_id": file.id}
+                                })
+                            else:
+                                attachments.append({
+                                    "file_id": file.id,
+                                    "tools": tools
+                                })
+
                             message_file_names.append(file.filename)
                             print(f"Uploaded file ID: {file.id}")
-                        return message_file_ids
+                        return attachments
                     except Exception as e:
                         print(f"Error: {e}")
                         return str(e)
+                    finally:
+                        uploading_files = False
 
+                uploading_files = False
                 return "No files uploaded"
 
             def user(user_message, history):
                 if not user_message.strip():
                     return user_message, history
+                
+                nonlocal message_file_names
+                nonlocal uploading_files
+                nonlocal images
+                nonlocal attachments
+                nonlocal recipient_agent
+
+                # Check if attachments contain file search or code interpreter types
+                def check_and_add_tools_in_attachments(attachments, recipient_agent):
+                    for attachment in attachments:
+                        for tool in attachment.get("tools", []):
+                            if tool["type"] == "file_search":
+                                if not any(isinstance(t, FileSearch) for t in recipient_agent.tools):
+                                    # Add FileSearch tool if it does not exist
+                                    recipient_agent.tools.append(FileSearch)
+                                    recipient_agent.client.beta.assistants.update(recipient_agent.id, tools=recipient_agent.get_oai_tools())
+                                    print("Added FileSearch tool to recipient agent to analyze the file.")
+                            elif tool["type"] == "code_interpreter":
+                                if not any(isinstance(t, CodeInterpreter) for t in recipient_agent.tools):
+                                    # Add CodeInterpreter tool if it does not exist
+                                    recipient_agent.tools.append(CodeInterpreter)
+                                    recipient_agent.client.beta.assistants.update(recipient_agent.id, tools=recipient_agent.get_oai_tools())
+                                    print("Added CodeInterpreter tool to recipient agent to analyze the file.")
+                    return None
+
+                check_and_add_tools_in_attachments(attachments, recipient_agent)
 
                 if history is None:
                     history = []
 
                 original_user_message = user_message
 
                 # Append the user message with a placeholder for bot response
@@ -320,27 +373,53 @@
                     chatbot_queue.put(self.message_output.get_formatted_content())
 
                 @override
                 def on_text_delta(self, delta, snapshot):
                     chatbot_queue.put(delta.value)
 
                 @override
-                def on_tool_call_created(self, tool_call):
-                    # TODO: add support for code interpreter and retirieval tools
+                def on_tool_call_created(self, tool_call: ToolCall):
+                    if isinstance(tool_call, dict):
+                        if "type" not in tool_call:
+                            tool_call["type"] = "function"
+                        
+                        if tool_call["type"] == "function":
+                            tool_call = FunctionToolCall(**tool_call)
+                        elif tool_call["type"] == "code_interpreter":
+                            tool_call = CodeInterpreterToolCall(**tool_call)
+                        elif tool_call["type"] == "file_search" or tool_call["type"] == "retrieval":
+                            tool_call = FileSearchToolCall(**tool_call)
+                        else:
+                            raise ValueError("Invalid tool call type: " + tool_call["type"])
+
+                    # TODO: add support for code interpreter and retrieval tools
                     if tool_call.type == "function":
                         chatbot_queue.put("[new_message]")
                         self.message_output = MessageOutput("function", self.recipient_agent_name, self.agent_name,
                                                             str(tool_call.function))
                         chatbot_queue.put(self.message_output.get_formatted_header() + "\n")
 
                 @override
-                def on_tool_call_done(self, snapshot):
+                def on_tool_call_done(self, snapshot: ToolCall):
+                    if isinstance(snapshot, dict):
+                        if "type" not in snapshot:
+                            snapshot["type"] = "function"
+                        
+                        if snapshot["type"] == "function":
+                            snapshot = FunctionToolCall(**snapshot)
+                        elif snapshot["type"] == "code_interpreter":
+                            snapshot = CodeInterpreterToolCall(**snapshot)
+                        elif snapshot["type"] == "file_search":
+                            snapshot = FileSearchToolCall(**snapshot)
+                        else:
+                            raise ValueError("Invalid tool call type: " + snapshot["type"])
+                        
                     self.message_output = None
 
-                    # TODO: add support for code interpreter and retirieval tools
+                    # TODO: add support for code interpreter and retrieval tools
                     if snapshot.type != "function":
                         return
 
                     chatbot_queue.put(str(snapshot.function))
 
                     if snapshot.function.name == "SendMessage":
                         try:
@@ -382,26 +461,46 @@
                     cls.message_output = None
                     chatbot_queue.put("[end]")
 
             def bot(original_message, history):
                 if not original_message:
                     return "", history
 
-                nonlocal message_file_ids
+                nonlocal attachments
                 nonlocal message_file_names
                 nonlocal recipient_agent
-                print("Message files: ", message_file_ids)
-                # Replace this with your actual chatbot logic
+                nonlocal images
+                nonlocal uploading_files
+
+                if uploading_files:
+                    history.append([None, "Uploading files... Please wait."])
+                    yield "", history
+                    return "", history
+
+                print("Message files: ", attachments)
+                print("Images: ", images)
+                
+                if images and len(images) > 0:
+                    original_message = [
+                        {
+                            "type": "text",
+                            "text": original_message,
+                        },
+                        *images
+                    ]
+
 
                 completion_thread = threading.Thread(target=self.get_completion_stream, args=(
-                    original_message, GradioEventHandler, message_file_ids, recipient_agent))
+                    original_message, GradioEventHandler, [], recipient_agent, "", attachments, None))
                 completion_thread.start()
 
-                message_file_ids = []
+                attachments = []
                 message_file_names = []
+                images = []
+                uploading_files = False
 
                 new_message = True
                 while True:
                     try:
                         bot_message = chatbot_queue.get(block=True)
 
                         if bot_message == "[end]":
@@ -499,22 +598,48 @@
 
             @override
             def on_text_delta(self, delta, snapshot):
                 self.message_output.cprint_update(snapshot.value)
 
             @override
             def on_tool_call_created(self, tool_call):
+                if isinstance(tool_call, dict):
+                    if "type" not in tool_call:
+                        tool_call["type"] = "function"
+                    
+                    if tool_call["type"] == "function":
+                        tool_call = FunctionToolCall(**tool_call)
+                    elif tool_call["type"] == "code_interpreter":
+                        tool_call = CodeInterpreterToolCall(**tool_call)
+                    elif tool_call["type"] == "file_search" or tool_call["type"] == "retrieval":
+                        tool_call = FileSearchToolCall(**tool_call)
+                    else:
+                        raise ValueError("Invalid tool call type: " + tool_call["type"])
+
                 # TODO: add support for code interpreter and retirieval tools
 
                 if tool_call.type == "function":
                     self.message_output = MessageOutputLive("function", self.recipient_agent_name, self.agent_name,
                                                             str(tool_call.function))
 
             @override
             def on_tool_call_delta(self, delta, snapshot):
+                if isinstance(snapshot, dict):
+                    if "type" not in snapshot:
+                        snapshot["type"] = "function"
+                    
+                    if snapshot["type"] == "function":
+                        snapshot = FunctionToolCall(**snapshot)
+                    elif snapshot["type"] == "code_interpreter":
+                        snapshot = CodeInterpreterToolCall(**snapshot)
+                    elif snapshot["type"] == "file_search":
+                        snapshot = FileSearchToolCall(**snapshot)
+                    else:
+                        raise ValueError("Invalid tool call type: " + snapshot["type"])
+                    
                 self.message_output.cprint_update(str(snapshot.function))
 
             @override
             def on_tool_call_done(self, snapshot):
                 self.message_output = None
 
                 # TODO: add support for code interpreter and retrieval tools
@@ -840,15 +965,15 @@
             agent_descriptions += recipient_agent.description + "\n"
 
         outer_self = self
 
         class SendMessage(BaseTool):
             my_primary_instructions: str = Field(...,
                                                  description="Please repeat your primary instructions step-by-step, including both completed "
-                                                             "and the following next steps that you need to perfrom. For multi-step, complex tasks, first break them down "
+                                                             "and the following next steps that you need to perform. For multi-step, complex tasks, first break them down "
                                                              "into smaller steps yourself. Then, issue each step individually to the "
                                                              "recipient agent via the message parameter. Each identified step should be "
                                                              "sent in separate message. Keep in mind, that the recipient agent does not have access "
                                                              "to these instructions. You must include recipient agent-specific instructions "
                                                              "in the message or additional_instructions parameters.")
             recipient: recipients = Field(..., description=agent_descriptions)
             message: str = Field(...,
```

### Comparing `agency_swarm-0.2.3/agency_swarm/agency/genesis/AgentCreator/instructions.md` & `agency_swarm-0.2.5/agency_swarm/agency/genesis/AgentCreator/instructions.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agency/genesis/AgentCreator/tools/CreateAgentTemplate.py` & `agency_swarm-0.2.5/agency_swarm/agency/genesis/AgentCreator/tools/CreateAgentTemplate.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agency/genesis/AgentCreator/tools/ImportAgent.py` & `agency_swarm-0.2.5/agency_swarm/agency/genesis/AgentCreator/tools/ImportAgent.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agency/genesis/AgentCreator/tools/ReadManifesto.py` & `agency_swarm-0.2.5/agency_swarm/agency/genesis/AgentCreator/tools/ReadManifesto.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agency/genesis/AgentCreator/tools/util/get_modules.py` & `agency_swarm-0.2.5/agency_swarm/agency/genesis/AgentCreator/tools/util/get_modules.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agency/genesis/GenesisAgency.py` & `agency_swarm-0.2.5/agency_swarm/agency/genesis/GenesisAgency.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             if with_browsing:
                 from agency_swarm.agents.BrowsingAgent import BrowsingAgent
                 browsing_agent = BrowsingAgent()
 
                 browsing_agent.instructions += ("""\n
 # BrowsingAgent's Primary instructions
 1. Browse the web to find the API documentation requested by the user. Prefer searching google directly for this API documentation page.
-2. Navigate to the API documentation page and ensure that it contains the necessary API endpoints descriptions. You can use the AnalyzeContent tool to check if the page contains the necessary API descriptions. If not, try perfrom another search in google and keep browsing until you find the right page.
+2. Navigate to the API documentation page and ensure that it contains the necessary API endpoints descriptions. You can use the AnalyzeContent tool to check if the page contains the necessary API descriptions. If not, try perform another search in google and keep browsing until you find the right page.
 3. If you have confirmed that the page contains the necessary API documentation, export the page with ExportFile tool. Then, send the file_id back to the user along with a brief description of the API.
 4. Repeat these steps for each new agent, as requested by the user.
                 """)
                 kwargs['agency_chart'].append(openapi_creator)
                 kwargs['agency_chart'].append([openapi_creator, browsing_agent])
 
         if 'shared_instructions' not in kwargs:
```

### Comparing `agency_swarm-0.2.3/agency_swarm/agency/genesis/GenesisCEO/GenesisCEO.py` & `agency_swarm-0.2.5/agency_swarm/agency/genesis/GenesisCEO/GenesisCEO.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agency/genesis/GenesisCEO/instructions.md` & `agency_swarm-0.2.5/agency_swarm/agency/genesis/GenesisCEO/instructions.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agency/genesis/GenesisCEO/tools/CreateAgencyFolder.py` & `agency_swarm-0.2.5/agency_swarm/agency/genesis/GenesisCEO/tools/CreateAgencyFolder.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agency/genesis/GenesisCEO/tools/FinalizeAgency.py` & `agency_swarm-0.2.5/agency_swarm/agency/genesis/GenesisCEO/tools/FinalizeAgency.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agency/genesis/GenesisCEO/tools/ReadRequirements.py` & `agency_swarm-0.2.5/agency_swarm/agency/genesis/GenesisCEO/tools/ReadRequirements.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agency/genesis/OpenAPICreator/instructions.md` & `agency_swarm-0.2.5/agency_swarm/agency/genesis/OpenAPICreator/instructions.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agency/genesis/OpenAPICreator/tools/CreateToolsFromOpenAPISpec.py` & `agency_swarm-0.2.5/agency_swarm/agency/genesis/OpenAPICreator/tools/CreateToolsFromOpenAPISpec.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agency/genesis/ToolCreator/instructions.md` & `agency_swarm-0.2.5/agency_swarm/agency/genesis/ToolCreator/instructions.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agency/genesis/ToolCreator/tools/CreateTool.py` & `agency_swarm-0.2.5/agency_swarm/agency/genesis/ToolCreator/tools/CreateTool.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
 
         n = 0
         code = ""
         content = ""
         while n < 3:
             resp = client.chat.completions.create(
                 messages=messages,
-                model="gpt-4-turbo",
+                model="gpt-4o",
                 temperature=0,
             )
 
             content = resp.choices[0].message.content
 
             messages.append(
                 {
```

### Comparing `agency_swarm-0.2.3/agency_swarm/agency/genesis/ToolCreator/tools/TestTool.py` & `agency_swarm-0.2.5/agency_swarm/agency/genesis/ToolCreator/tools/TestTool.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agency/genesis/manifesto.md` & `agency_swarm-0.2.5/agency_swarm/agency/genesis/manifesto.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agency/genesis/util.py` & `agency_swarm-0.2.5/agency_swarm/agency/genesis/util.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/BrowsingAgent.py` & `agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/BrowsingAgent.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/instructions.md` & `agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/instructions.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/ClickElement.py` & `agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/ClickElement.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/ExportFile.py` & `agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/ExportFile.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/ReadURL.py` & `agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/ReadURL.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/Scroll.py` & `agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/Scroll.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/SelectDropdown.py` & `agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/SelectDropdown.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/SendKeys.py` & `agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/SendKeys.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/SolveCaptcha.py` & `agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/SolveCaptcha.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/WebPageSummarizer.py` & `agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/WebPageSummarizer.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/util/highlights.py` & `agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/util/highlights.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agents/BrowsingAgent/tools/util/selenium.py` & `agency_swarm-0.2.5/agency_swarm/agents/BrowsingAgent/tools/util/selenium.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agents/Devid/Devid.py` & `agency_swarm-0.2.5/agency_swarm/agents/Devid/Devid.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agents/Devid/instructions.md` & `agency_swarm-0.2.5/agency_swarm/agents/Devid/instructions.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agents/Devid/tools/ChangeFile.py` & `agency_swarm-0.2.5/agency_swarm/agents/Devid/tools/ChangeFile.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agents/Devid/tools/CommandExecutor.py` & `agency_swarm-0.2.5/agency_swarm/agents/Devid/tools/CommandExecutor.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agents/Devid/tools/DirectoryNavigator.py` & `agency_swarm-0.2.5/agency_swarm/agents/Devid/tools/DirectoryNavigator.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agents/Devid/tools/FileMover.py` & `agency_swarm-0.2.5/agency_swarm/agents/Devid/tools/FileMover.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agents/Devid/tools/FileReader.py` & `agency_swarm-0.2.5/agency_swarm/agents/Devid/tools/FileReader.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agents/Devid/tools/FileWriter.py` & `agency_swarm-0.2.5/agency_swarm/agents/Devid/tools/FileWriter.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,34 +11,34 @@
 import re
 
 from .util import format_file_deps
 
 history = [
             {
                 "role": "system",
-                "content": "As a top-tier software engineer focused on developing programs incrementally, you are entrusted with the creation or modification of files based on user requirements. It's imperative to operate under the assumption that all necessary dependencies are pre-installed and accessible, and the file in question will be deployed in an appropriate environment. Furthermore, it is presumed that all other modules or files upon which this file relies are accurate and error-free. Your output should be encapsulated within a code block, without specifying the programming language. Prior to embarking on the coding process, you must outine a methodical, step-by-step plan to precisely fulfill the requirements—no more, no less. It is crucial to ensure that the final code block is a complete file, without any truncation. This file should embody a flawless, fully operational program, inclusive of all requisite imports and functions, devoid of any placeholders, unless specified otherwise by the user."
+                "content": "As a top-tier software engineer focused on developing programs incrementally, you are entrusted with the creation or modification of files based on user requirements. It's imperative to operate under the assumption that all necessary dependencies are pre-installed and accessible, and the file in question will be deployed in an appropriate environment. Furthermore, it is presumed that all other modules or files upon which this file relies are accurate and error-free. Your output should be encapsulated within a code block, without specifying the programming language. Prior to embarking on the coding process, you must outline a methodical, step-by-step plan to precisely fulfill the requirements — no more, no less. It is crucial to ensure that the final code block is a complete file, without any truncation. This file should embody a flawless, fully operational program, inclusive of all requisite imports and functions, devoid of any placeholders, unless specified otherwise by the user."
             },
         ]
 
 
 class FileWriter(BaseTool):
     """This tools allows you to write new files or modify existing files according to specified requirements. In 'write' mode, it creates a new file or overwrites an existing one. In 'modify' mode, it modifies an existing file according to the provided requirements.
     Note: This tool does not have access to other files within the project. You must provide all necessary details to ensure that the generated file can be used in conjunction with other files in this project."""
     file_path: str = Field(
         ..., description="The path of the file to write or modify. Will create directories if they don't exist."
     )
     requirements: str = Field(
         ...,
-        description="The comprehensive requirements explaning how the file should be written or modified. This should be a detailed description of what the file should contain, inlcuding example inputs, desired behaviour and ideal outputs. It must not contain any code or implementation details."
+        description="The comprehensive requirements explaining how the file should be written or modified. This should be a detailed description of what the file should contain, including example inputs, desired behaviour and ideal outputs. It must not contain any code or implementation details."
     )
     details: str = Field(
         None, description="Additional details like error messages, or class, function, and variable names from other files that this file depends on."
     )
     documentation: Optional[str] = Field(
-        None, description="Relevant documentation extracted with the myfiles_browser tool. You must pass all the relevant code from the documentaion, as this tool does not have access to those files."
+        None, description="Relevant documentation extracted with the myfiles_browser tool. You must pass all the relevant code from the documentation, as this tool does not have access to those files."
     )
     mode: Literal["write", "modify"] = Field(
         ..., description="The mode of operation for the tool. 'write' is used to create a new file or overwrite an existing one. 'modify' is used to modify an existing file."
     )
     file_dependencies: List[str] = Field(
         [],
         description="Paths to other files that the file being written depends on.",
@@ -98,15 +98,15 @@
         messages.insert(0, history[0])
 
         n = 0
         error_message = ""
         while n < 3:
             resp = client.chat.completions.create(
                 messages=messages,
-                model="gpt-4-turbo",
+                model="gpt-4o",
                 temperature=0,
             )
 
             content = resp.choices[0].message.content
 
             messages.append(
                 {
@@ -186,15 +186,15 @@
 
     def validate_content(self, v):
         client = get_openai_client()
 
         llm_validator(
             statement="Check if the code is bug-free. Code should be considered in isolation, with the understanding that it is part of a larger, fully developed program that strictly adheres to these standards of completeness and correctness. All files, elements, components, functions, or modules referenced within this snippet are assumed to exist in other parts of the project and are also devoid of any errors, ensuring a cohesive and error-free integration across the entire software solution. Certain placeholders may be present.",
                       client=client,
-                      model="gpt-4-turbo",
+                      model="gpt-4o",
                       temperature=0,
                       allow_override=False
                       )(v)
 
         return v
 
     @field_validator("requirements", mode="after")
@@ -214,15 +214,15 @@
 
         return v
 
     @field_validator("details", mode="after")
     @classmethod
     def validate_details(cls, v):
         if len(v) == 0:
-            raise ValueError("Details are required. Remember this tool does not have access to other files. Please provide additional details like relevant documentation, error messages, or class, function, and variable names from other files that this file depends on.")
+            raise ValueError("Details are required. Remember: this tool does not have access to other files. Please provide additional details like relevant documentation, error messages, or class, function, and variable names from other files that this file depends on.")
         return v
 
     @field_validator("documentation", mode="after")
     @classmethod
     def validate_documentation(cls, v):
         # check if documentation contains code
         pattern = r'(```)((.*\n){5,})(```)'
```

### Comparing `agency_swarm-0.2.3/agency_swarm/agents/Devid/tools/ListDir.py` & `agency_swarm-0.2.5/agency_swarm/agents/Devid/tools/ListDir.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agents/Devid/tools/util/format_file_deps.py` & `agency_swarm-0.2.5/agency_swarm/agents/Devid/tools/util/format_file_deps.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/agents/agent.py` & `agency_swarm-0.2.5/agency_swarm/agents/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             tools_folder: str = None,
             files_folder: Union[List[str], str] = None,
             schemas_folder: Union[List[str], str] = None,
             api_headers: Dict[str, Dict[str, str]] = None,
             api_params: Dict[str, Dict[str, str]] = None,
             file_ids: List[str] = None,
             metadata: Dict[str, str] = None,
-            model: str = "gpt-4-turbo",
+            model: str = "gpt-4o",
             validation_attempts: int = 1,
             max_prompt_tokens: int = None,
             max_completion_tokens: int = None,
             truncation_strategy: dict = None,
             examples: List[ExampleMessage] = None,
     ):
         """
@@ -103,15 +103,15 @@
             response_format (Dict, optional): The response format for the OpenAI API. Defaults to None.
             tools_folder (str, optional): Path to a directory containing tools associated with the agent. Each tool must be defined in a separate file. File must be named as the class name of the tool. Defaults to None.
             files_folder (Union[List[str], str], optional): Path or list of paths to directories containing files associated with the agent. Defaults to None.
             schemas_folder (Union[List[str], str], optional): Path or list of paths to directories containing OpenAPI schemas associated with the agent. Defaults to None.
             api_headers (Dict[str,Dict[str, str]], optional): Headers to be used for the openapi requests. Each key must be a full filename from schemas_folder. Defaults to an empty dictionary.
             api_params (Dict[str, Dict[str, str]], optional): Extra params to be used for the openapi requests. Each key must be a full filename from schemas_folder. Defaults to an empty dictionary.
             metadata (Dict[str, str], optional): Metadata associated with the agent. Defaults to an empty dictionary.
-            model (str, optional): The model identifier for the OpenAI API. Defaults to "gpt-4-turbo-preview".
+            model (str, optional): The model identifier for the OpenAI API. Defaults to "gpt-4o".
             validation_attempts (int, optional): Number of attempts to validate the response with response_validator function. Defaults to 1.
             max_prompt_tokens (int, optional): Maximum number of tokens allowed in the prompt. Defaults to None.
             max_completion_tokens (int, optional): Maximum number of tokens allowed in the completion. Defaults to None.
             truncation_strategy (TruncationStrategy, optional): Truncation strategy for the OpenAI API. Defaults to None.
             examples (List[Dict], optional): A list of example messages for the agent. Defaults to None.
 
         This constructor sets up the agent with its unique properties, initializes the OpenAI client, reads instructions if provided, and uploads any associated files.
@@ -190,17 +190,22 @@
             else:
                 self.response_format = self.response_format or self.assistant.response_format
             self.tool_resources = self.tool_resources or self.assistant.tool_resources.model_dump()
             self.metadata = self.metadata or self.assistant.metadata
             self.model = self.model or self.assistant.model
             self.tool_resources = self.tool_resources or self.assistant.tool_resources.model_dump()
 
-            # update assistant if parameters are different
-            if not self._check_parameters(self.assistant.model_dump()):
-                self._update_assistant()
+            for tool in self.assistant.tools:
+                # update assistants created with v1
+                if tool.type == "retrieval":
+                    self.client.beta.assistants.update(self.id, tools=self.get_oai_tools())
+
+            # # update assistant if parameters are different
+            # if not self._check_parameters(self.assistant.model_dump()):
+            #     self._update_assistant()
 
             return self
 
         # load assistant from settings
         if os.path.exists(path):
             with open(path, 'r') as f:
                 settings = json.load(f)
@@ -209,15 +214,15 @@
                     if assistant_settings['name'] == self.name:
                         try:
                             self.assistant = self.client.beta.assistants.retrieve(assistant_settings['id'])
                             self.id = assistant_settings['id']
 
                             # update assistant if parameters are different
                             if not self._check_parameters(self.assistant.model_dump()):
-                                print("Updating assistant... " + self.name)
+                                print("Updating agent... " + self.name)
                                 self._update_assistant()
 
                             if self.assistant.tool_resources:
                                 self.tool_resources = self.assistant.tool_resources.model_dump()
 
                             self._update_settings()
                             return self
```

### Comparing `agency_swarm-0.2.3/agency_swarm/cli.py` & `agency_swarm-0.2.5/agency_swarm/cli.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/messages/message_output.py` & `agency_swarm-0.2.5/agency_swarm/messages/message_output.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/threads/thread.py` & `agency_swarm-0.2.5/agency_swarm/threads/thread.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                                    recipient_agent,
                                    additional_instructions,
                                    event_handler,
                                    tool_choice,
                                    yield_messages=False)
 
     def get_completion(self,
-                       message: str,
+                       message: str | List[dict],
                        message_files: List[str] = None,
                        attachments: Optional[List[dict]] = None,
                        recipient_agent=None,
                        additional_instructions: str = None,
                        event_handler: type(AgencyEventHandler) = None,
                        tool_choice: AssistantToolChoice = None,
                        yield_messages: bool = False
```

### Comparing `agency_swarm-0.2.3/agency_swarm/threads/thread_async.py` & `agency_swarm-0.2.5/agency_swarm/threads/thread_async.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/tools/BaseTool.py` & `agency_swarm-0.2.5/agency_swarm/tools/BaseTool.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,19 +9,14 @@
 
 class BaseTool(OpenAISchema, ABC):
     shared_state: ClassVar[SharedState] = None
     caller_agent: Any = None
     event_handler: Any = None
     one_call_at_a_time: bool = False
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)   
-        # Exclude 'run' method from Pydantic model fields
-        # self.model_fields.pop("run", None)
-
     @classmethod
     @property
     def openai_schema(cls):
         schema = super(BaseTool, cls).openai_schema
 
         properties = schema.get("parameters", {}).get("properties", {})
 
@@ -38,14 +33,17 @@
         if "event_handler" in required:
             required.remove("event_handler")
         if "one_call_at_a_time" in required:
             required.remove("one_call_at_a_time")
 
         return schema
 
-    def model_dump(self, **kwargs):
-        return super().model_dump(exclude={"caller_agent", "shared_state", "event_handler", "one_call_at_a_time"},
-                                  **kwargs)
+    def model_dump(self, exclude=None, **kwargs):
+        if exclude is None:
+            exclude = {"caller_agent", "shared_state", "event_handler", "one_call_at_a_time"}
+        else:
+            exclude.update({"caller_agent", "shared_state", "event_handler", "one_call_at_a_time"})
+        return super().model_dump(exclude=exclude, **kwargs)
 
     @abstractmethod
     def run(self, **kwargs):
         pass
```

### Comparing `agency_swarm-0.2.3/agency_swarm/tools/ToolFactory.py` & `agency_swarm-0.2.5/agency_swarm/tools/ToolFactory.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,28 @@
+from enum import Enum
 import importlib.util
 import inspect
 import json
 import os
+from pathlib import Path
 import sys
 from importlib import import_module
 from typing import Any, Dict, List, Type, Union
+import typing
 
 import jsonref
 from jsonref import requests
 from pydantic import create_model, Field
 
 from .BaseTool import BaseTool
-from ..util.schema import reference_schema
+from ..util.schema import dereference_schema, reference_schema
+
+from datamodel_code_generator import DataModelType, PythonVersion
+from datamodel_code_generator.model import get_data_model_types
+from datamodel_code_generator.parser.jsonschema import JsonSchemaParser
 
 
 class ToolFactory:
 
     @staticmethod
     def from_langchain_tools(tools: List) -> List[Type[BaseTool]]:
         """
@@ -68,116 +75,53 @@
             callback
         )
 
 
     @staticmethod
     def from_openai_schema(schema: Dict[str, Any], callback: Any) -> Type[BaseTool]:
         """
-        Converts an OpenAI schema into a BaseTool. Nested propoerties without refs are not supported yet.
+        Converts an OpenAI schema into a BaseTool.
 
         Parameters:
             schema: The OpenAI schema to convert.
             callback: The function to run when the tool is called.
 
         Returns:
             A BaseTool.
         """
-        def resolve_ref(ref: str, defs: Dict[str, Any]) -> Any:
-            # Extract the key from the reference
-            key = ref.split('/')[-1]
-            if key in defs:
-                return defs[key]
-            else:
-                raise ValueError(f"Reference '{ref}' not found in definitions")
-
-        def create_fields(schema: Dict[str, Any], type_mapping: Dict[str, Type[Any]], required_fields: List[str],
-                          defs: Dict[str, Any]) -> Dict[str, Any]:
-            fields = {}
-
-            for prop, details in schema.items():
-                alias = None
-                if prop.startswith('_'):
-                    alias = prop
-                    prop = prop.lstrip('_')
-
-                json_type = details['type'] if 'type' in details else 'any'
-
-                if json_type in type_mapping:
-                    field_type = type_mapping[json_type]
-                    field_description = details.get('description', '')
-                    is_required = prop in required_fields
-                    field_default = ... if is_required else None
-
-                    if json_type == 'array':
-                        items_schema = details.get('items', {})
-                        if 'type' in items_schema:
-                            item_type = type_mapping[items_schema['type']]
-                            field_type = List[item_type]
-                        elif 'properties' in items_schema:  # Handling direct nested object in array
-                            nested_properties = items_schema['properties']
-                            nested_required = items_schema.get('required', [])
-                            nested_model_name = items_schema.get('title', f"{prop}Item")
-                            nested_fields = create_fields(nested_properties, type_mapping, nested_required, defs)
-                            nested_model = create_model(nested_model_name, **nested_fields)
-                            field_type = List[nested_model]
-                        elif '$ref' in items_schema:
-                            ref_model = resolve_ref(items_schema['$ref'], defs)
-                            field_type = List[ref_model]
-                        else:
-                            raise ValueError("Array items must have a 'type', 'properties', or '$ref'")
-                    elif json_type == 'object':
-                        if 'properties' in details:
-                            nested_properties = details['properties']
-                            nested_required = details.get('required', [])
-                            nested_model_name = details.get('title', f"{prop}Model")
-                            nested_fields = create_fields(nested_properties, type_mapping, nested_required, defs)
-                            field_type = create_model(nested_model_name, **nested_fields)
-                        elif '$ref' in details:
-                            ref_model = resolve_ref(details['$ref'], defs)
-                            field_type = ref_model
-                        else:
-                            raise ValueError("Object must have 'properties' or '$ref'")
-
-                    fields[prop] = (
-                    field_type, Field(default=field_default, description=field_description, alias=alias))
-                else:
-                    raise ValueError(f"Unsupported type '{json_type}' for property '{prop}'")
-
-            return fields
-
-        type_mapping = {
-            'string': str,
-            'integer': int,
-            'number': float,
-            'boolean': bool,
-            'array': List,
-            'object': dict,
-            'null': type(None),
-            'any': Any,
-        }
-
-        schema = reference_schema(schema)
-
-        name = schema['name']
-        description = schema['description']
-        properties = schema['parameters']['properties']
-        required_fields = schema['parameters'].get('required', [])
-
-        # Add definitions ($defs) to type_mapping
-        defs = {k: create_model(k, **create_fields(v['properties'], type_mapping, v.get('required', []), {})) for k, v
-                in schema['parameters'].get('$defs', {}).items()}
-        type_mapping.update(defs)
+        data_model_types = get_data_model_types(
+            DataModelType.PydanticV2BaseModel,
+            target_python_version=PythonVersion.PY_37
+        )
 
-        fields = create_fields(properties, type_mapping, required_fields, defs)
+        parser = JsonSchemaParser(
+            json.dumps(schema['parameters']),
+            data_model_type=data_model_types.data_model,
+            data_model_root_type=data_model_types.root_model,
+            data_model_field_type=data_model_types.field_model,
+            data_type_manager_type=data_model_types.data_type_manager,
+            dump_resolve_reference_action=data_model_types.dump_resolve_reference_action,
+            use_schema_description=True,
+            validation=False,
+            class_name='Model',
+            # custom_template_dir=Path('/Users/vrsen/Projects/agency-swarm/agency-swarm/agency_swarm/tools/data_schema_templates')
+        )
 
-        # Dynamically creating the Pydantic model
-        model = create_model(name, **fields)
+        result = parser.parse()
 
-        tool = type(name, (BaseTool, model), {
-            "__doc__": description,
+        # # Execute the result to extract the model
+        exec_globals = {}
+        exec(result, exec_globals)
+        model = exec_globals.get('Model')
+
+        if not model:
+            raise ValueError(f"Could not extract model from schema {schema['name']}")
+        
+        tool = type(schema['name'], (BaseTool, model), {
+            "__doc__": schema.get('description', ""),
             "run": callback,
         })
 
         return tool
 
     @staticmethod
     def from_openapi_schema(schema: Union[str, dict], headers: Dict[str, str] = None, params: Dict[str, Any] = None) \
@@ -255,40 +199,44 @@
                 )
                 if req_body:
                     schema["properties"]["requestBody"] = req_body
 
                 spec_params = spec.get("parameters", [])
                 if spec_params:
                     param_properties = {}
+                    required_params = []
                     for param in spec_params:
                         if "schema" not in param and "type" in param:
                             param["schema"] = {"type": param["type"]}
                         param_properties[param["name"]] = param["schema"]
                         if "description" in param:
                             param_properties[param["name"]]["description"] = param["description"]
-                        if "required" in param:
-                            param_properties[param["name"]]["required"] = param["required"]
+                        if "required" in param and param["required"]:
+                            required_params.append(param["name"])
                         if "example" in param:
                             param_properties[param["name"]]["example"] = param["example"]
                         if "examples" in param:
                             param_properties[param["name"]]["examples"] = param["examples"]
+                    
                     schema["properties"]["parameters"] = {
                         "type": "object",
                         "properties": param_properties,
+                        "required": required_params
                     }
 
                 function = {
                     "name": function_name,
                     "description": desc,
                     "parameters": schema,
                 }
 
                 tools.append(ToolFactory.from_openai_schema(function, callback))
 
         return tools
+    
     @staticmethod
     def from_file(file_path: str) -> Type[BaseTool]:
         """Dynamically imports a BaseTool class from a Python file within a package structure.
 
         Parameters:
             file_path: The file path to the Python file containing the BaseTool class.
```

### Comparing `agency_swarm-0.2.3/agency_swarm/util/cli/create_agent_template.py` & `agency_swarm-0.2.5/agency_swarm/util/cli/create_agent_template.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/util/cli/import_agent.py` & `agency_swarm-0.2.5/agency_swarm/util/cli/import_agent.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/util/helpers/get_available_agent_descriptions.py` & `agency_swarm-0.2.5/agency_swarm/util/helpers/get_available_agent_descriptions.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/util/helpers/list_available_agents.py` & `agency_swarm-0.2.5/agency_swarm/util/helpers/list_available_agents.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/util/oai.py` & `agency_swarm-0.2.5/agency_swarm/util/oai.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/util/openapi.py` & `agency_swarm-0.2.5/agency_swarm/util/openapi.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/util/schema.py` & `agency_swarm-0.2.5/agency_swarm/util/schema.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm/util/streaming.py` & `agency_swarm-0.2.5/agency_swarm/util/streaming.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/agency_swarm.egg-info/PKG-INFO` & `agency_swarm-0.2.5/agency_swarm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agency-swarm
-Version: 0.2.3
+Version: 0.2.5
 Summary: An open source agent orchestration framework built on top of the latest OpenAI Assistants API.
 Home-page: https://github.com/VRSEN/agency-swarm
 Author: VRSEN
 Author-email: VRSEN <arseny9795@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Arsenii Shatokhin
@@ -30,20 +30,21 @@
 Project-URL: homepage, https://github.com/VRSEN/agency-swarm
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai==1.30.3
-Requires-Dist: instructor==1.3.1
+Requires-Dist: openai==1.30.4
+Requires-Dist: instructor==1.3.2
+Requires-Dist: datamodel-code-generator==0.25.6
 Requires-Dist: deepdiff==6.7.1
-Requires-Dist: termcolor==2.3.0
-Requires-Dist: python-dotenv==1.0.0
-Requires-Dist: rich==13.7.0
+Requires-Dist: termcolor==2.4.0
+Requires-Dist: python-dotenv==1.0.1
+Requires-Dist: rich==13.7.1
 Requires-Dist: jsonref==1.1.0
 
 # 🐝 Agency Swarm
 
 [![Framework](https://firebasestorage.googleapis.com/v0/b/vrsen-ai/o/public%2Fyoutube%2FFramework.png?alt=media&token=ae76687f-0347-4e0c-8342-4c5d31e3f050)](https://youtu.be/M5Pa0pLgyYU?si=f-cQV8FoiGd98uuk)
 
 ## Overview
```

### Comparing `agency_swarm-0.2.3/agency_swarm.egg-info/SOURCES.txt` & `agency_swarm-0.2.5/agency_swarm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 agency_swarm/tools/oai/CodeInterpreter.py
 agency_swarm/tools/oai/FileSearch.py
 agency_swarm/tools/oai/Retrieval.py
 agency_swarm/tools/oai/__init__.py
 agency_swarm/user/__init__.py
 agency_swarm/user/user.py
 agency_swarm/util/__init__.py
+agency_swarm/util/files.py
 agency_swarm/util/oai.py
 agency_swarm/util/openapi.py
 agency_swarm/util/schema.py
 agency_swarm/util/shared_state.py
 agency_swarm/util/streaming.py
 agency_swarm/util/cli/__init__.py
 agency_swarm/util/cli/create_agent_template.py
@@ -140,10 +141,11 @@
 tests/data/files/test-txt.txt
 tests/data/files/test-xml.xml
 tests/data/schemas/ga4.json
 tests/data/schemas/get-headers-params.json
 tests/data/schemas/get-weather.json
 tests/data/schemas/relevance.json
 tests/data/tools/ExampleTool1.py
+tests/demos/__init__.py
 tests/demos/demo_gradio.py
 tests/demos/streaming_demo.py
 tests/demos/term_demo.py
```

### Comparing `agency_swarm-0.2.3/docs/advanced-usage/agencies.md` & `agency_swarm-0.2.5/docs/advanced-usage/agencies.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 
 An `Agency` is a collection of Agents that can communicate with one another. 
 
 ### Benefits of using an Agency
 
 Here are the primary benefits of using an Agency, instead of an individual agent:
 
-1. **Less halluconations**: When agents are part of an agency, they can supervise one another and recover from mistakes or unexpected circumstances.
-2. **More complex tasks**: The more agents you add, the longer the seqeunce of actions they can perfrom before retuning the result back to the user.
+1. **Fewer hallucinations**: When agents are part of an agency, they can supervise one another and recover from mistakes or unexpected circumstances.
+2. **More complex tasks**: The more agents you add, the longer the sequence of actions they can perform before returning the result back to the user.
 3. **Scalability**: As the complexity of your integration increases, you can keep adding more and more agents. 
 
     !!! tip
-        It is recommended to start from as few agents as possible, fine tune them until they are working as expected, and only then add new agents to the agency. If you add too many agents at first, it will be difficult to debug and understand what is going on.
+        It is recommended to start with as few agents as possible, fine-tune them until they are working as expected, and only then add new agents to the agency. If you add too many agents at first, it will be difficult to debug and understand what is going on.
 
 ## Communication Flows
 
-Unlike all other frameworks, communication flows in Agency Swarm are **not hierarchical** or **sequential**. Instead, they are **uniform**. You can define them however you want. But keep in mind that they are established from left to right inside the `agency_chart`. So, in the example below, the CEO can initiate communication and send tasks to the Developer and the Virtual Assistant, and they can respond in to him in the same thread, but the Developer or the VA cannot initiate a conversation and assign tasks to the CEO. You can add as many levels of communication as you want.
+Unlike all other frameworks, communication flows in Agency Swarm are **not hierarchical** or **sequential**. Instead, they are **uniform**. You can define them however you want. But keep in mind that they are established from left to right inside the `agency_chart`. So, in the example below, the CEO can initiate communication and send tasks to the Developer and the Virtual Assistant, and they can respond back to him in the same thread, but the Developer or the VA cannot initiate a conversation and assign tasks to the CEO. You can add as many levels of communication as you want.
 
 ```python
 from agency_swarm import Agency
 
 agency = Agency([
     ceo, dev  # CEO and Developer will be the entry point for communication with the user
     [ceo, dev],  # CEO can initiate communication with Developer
     [ceo, va],   # CEO can initiate communication with Virtual Assistant
     [dev, va]    # Developer can initiate communication with Virtual Assistant
 ])
 ```
 
-All agents added inside the top level list of `agency_chart` without being part of a second list, can talk to the user.
+All agents added inside the top-level list of `agency_chart` without being part of a second list, can talk to the user.
 
 ## Streaming Responses
 
 To stream the conversation between agents, you can use the `get_completion_stream` method with your event handler like below. The process is extremely similar to the one in the [official documentation](https://platform.openai.com/docs/assistants/overview/step-4-create-a-run?context=with-streaming).
 
 The only difference is that you must extend the `AgencyEventHandler` class, which has 2 additional properties: `agent_name` and `recipient_agent_name`, to get the names of the agents communicating with each other. (See the `on_text_created` below.)
 
@@ -105,15 +105,15 @@
 
 If you would like to use a different file path for the settings, other than default `settings.json`, you can specify a `settings_path` parameter. All your agent states will then be saved and loaded from this file. If this file does not exist, it will be created, along with new Assistants on your OpenAI account.
 
 ```python
 agency = Agency([ceo], settings_path='my_settings.json') 
 ```
 
-### Temperture and Max Token Controls
+### Temperature and Max Token Controls
 
 You can also specify parameters like `temperature`, `top_p`, `max_completion_tokens`,  `max_prompt_tokens` and `truncation_strategy`, parameters for the entire agency. These parameters will be used as default values for all agents in the agency, however, you can still override them for individual agents by specifying them in the agent's constructor.
 
 ```python
 agency = Agency([ceo], temperature=0.3, max_prompt_tokens=25000) 
 ```
 
@@ -144,16 +144,16 @@
 
 ### Running the Agency from your terminal
 
 ```bash
 agency.run_demo()
 ```
 
-To talk to one of the top level agents when running the agency from your terminal, you can use **mentions feature**, similar to how you would use it inside ChatGPT. Simply mention the agent name in the message like `@Developer I want you to build me a website`. The message will then be sent to the Developer agent, instead of the CEO. You can also use tab to autocomplete the agent name after the `@` symbol.
+To talk to one of the top-level agents when running the agency from your terminal, you can use **mentions feature**, similar to how you would use it inside ChatGPT. Simply mention the agent name in the message like `@Developer I want you to build me a website`. The message will then be sent to the Developer agent, instead of the CEO. You can also use tab to autocomplete the agent name after the `@` symbol.
 
 ## Deleting the Agency
 
 If you would like to delete the agency and all its agents with all associated files and vector stores, you can use the `delete` method.
 
 ```python
 agency.delete()
-```
+```
```

### Comparing `agency_swarm-0.2.3/docs/advanced-usage/agents.md` & `agency_swarm-0.2.5/docs/advanced-usage/agents.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/docs/advanced-usage/azure-openai.md` & `agency_swarm-0.2.5/docs/advanced-usage/azure-openai.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/docs/advanced-usage/open-source-models.md` & `agency_swarm-0.2.5/docs/advanced-usage/open-source-models.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/docs/advanced-usage/tools.md` & `agency_swarm-0.2.5/docs/advanced-usage/tools.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/docs/assets/logo.png` & `agency_swarm-0.2.5/docs/assets/logo.png`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/docs/contributing.md` & `agency_swarm-0.2.5/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/docs/deployment.md` & `agency_swarm-0.2.5/docs/deployment.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/docs/examples.md` & `agency_swarm-0.2.5/docs/examples.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/docs/index.md` & `agency_swarm-0.2.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/docs/quick_start.md` & `agency_swarm-0.2.5/docs/quick_start.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Quick Start
 
 When it comes to getting started with Agency Swarm, you have two options:
 
 1. **Start from Scratch**: This is the best option if you want to get a feel for the framework and understand how it works. You can start by creating your own agents and tools, and then use them to create your own agencies.
-2. **Use Genesis Swarm**: This is the best option if you want to get started quickly and don't want to spend time creating your own agents and tools. You can use the Genesis Agency to create your agent templates and tools, and then fine tune them to your needs.
+2. **Use Genesis Swarm**: This is the best option if you want to get started quickly and don't want to spend time creating your own agents and tools. You can use the Genesis Agency to create your agent templates and tools, and then fine-tune them to your needs.
 3. **Create agent templates with CLI**: This is the best option if you want to create a structured environment for each agent and tool. See [Advanced Agents](advanced-usage/agents.md) for more information.
 
 ### Installation
 
 ```python
 pip install agency-swarm
 ```
@@ -121,24 +121,24 @@
     ```
 
 2. **Chat with Genesis CEO**: Provide as much context as possible to Genesis Agency. Make sure to include:
     - Your mission and goals.
     - The agents you want to involve and their communication flows.
     - Which tools or APIs each agent should have access to, if any.
 
-3. **Fine Tune**: After Genesis has created your agents for you, you will see all the agent folders in the same directory where you ran the `genesis` command. You can then fine tune the agents and tools as per your requirements. To do so, follow these steps:  
+3. **Fine Tune**: After Genesis has created your agents for you, you will see all the agent folders in the same directory where you ran the `genesis` command. You can then fine-tune the agents and tools as per your requirements. To do so, follow these steps:  
 
 
       1. **Adjust Tools**: Modify the tools in the `tools` directories of each agent as per your requirements.
       2. **Adjust Instructions**: Modify the agents in the `agents` directories as per your requirements.
-      3. **Run Agency**: Run the `agency.py` file, send your tasks and see how they perfrom.
+      3. **Run Agency**: Run the `agency.py` file, send your tasks and see how they perform.
       4. **Repeat**: Repeat the process until your agents are performing as expected.
 
     !!! note "Agent Development is an Iterative Process"
-        Right now, all agent development is iterative. You will need to constantly monitor and adust your system until it works as expected. In the future, this will become less of a problem, as larger and smarter models are released.
+        Right now, all agent development is iterative. You will need to constantly monitor and adjust your system until it works as expected. In the future, this will become less of a problem, as larger and smarter models are released.
 
 ## Next Steps
 
 - Learn how to create more Tools, Agents and Agencies
 - Deploy in Production
```

### Comparing `agency_swarm-0.2.3/mkdocs.yml` & `agency_swarm-0.2.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/notebooks/Agency_Swarm_with_Open_Source_Model.ipynb` & `agency_swarm-0.2.5/notebooks/Agency_Swarm_with_Open_Source_Model.ipynb`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/notebooks/agency_async.ipynb` & `agency_swarm-0.2.5/notebooks/agency_async.ipynb`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/notebooks/azure.ipynb` & `agency_swarm-0.2.5/notebooks/azure.ipynb`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/notebooks/genesis_agency.ipynb` & `agency_swarm-0.2.5/notebooks/genesis_agency.ipynb`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/notebooks/web_browser_agent.ipynb` & `agency_swarm-0.2.5/notebooks/web_browser_agent.ipynb`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/pyproject.toml` & `agency_swarm-0.2.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 license = { file = "LICENSE" }
 classifiers = [
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
-    "openai==1.30.3",
-    "instructor==1.3.1",
+    "openai==1.30.4",
+    "instructor==1.3.2",
+    "datamodel-code-generator==0.25.6",
     "deepdiff==6.7.1",
-    "termcolor==2.3.0",
-    "python-dotenv==1.0.0",
-    "rich==13.7.0",
+    "termcolor==2.4.0",
+    "python-dotenv==1.0.1",
+    "rich==13.7.1",
     "jsonref==1.1.0"
 ]
 requires-python = ">=3.7"
 urls = { homepage = "https://github.com/VRSEN/agency-swarm" }
 
 [project.scripts]
 agency-swarm = "agency_swarm.cli:main"
```

### Comparing `agency_swarm-0.2.3/run_tests.py` & `agency_swarm-0.2.5/run_tests.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/setup.py` & `agency_swarm-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your requirements file
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='agency-swarm',
-    version='0.2.3',
+    version='0.2.5',
     author='VRSEN',
     author_email='arseny9795@gmail.com',
     description='An opensource agent orchestration framework built on top of the latest OpenAI Assistants API.',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/VRSEN/agency-swarm',
     packages=find_packages(exclude=['tests', 'tests.*']),
```

### Comparing `agency_swarm-0.2.3/tests/data/files/csv-test.csv` & `agency_swarm-0.2.5/tests/data/files/csv-test.csv`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/tests/data/files/generated_data.json` & `agency_swarm-0.2.5/tests/data/files/generated_data.json`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/tests/data/files/test-docx.docx` & `agency_swarm-0.2.5/tests/data/files/test-docx.docx`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/tests/data/files/test-html.html` & `agency_swarm-0.2.5/tests/data/files/test-html.html`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/tests/data/files/test-pdf.pdf` & `agency_swarm-0.2.5/tests/data/files/test-pdf.pdf`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/tests/data/schemas/ga4.json` & `agency_swarm-0.2.5/tests/data/schemas/ga4.json`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/tests/data/schemas/get-headers-params.json` & `agency_swarm-0.2.5/tests/data/schemas/get-headers-params.json`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/tests/data/schemas/get-weather.json` & `agency_swarm-0.2.5/tests/data/schemas/get-weather.json`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/tests/data/schemas/relevance.json` & `agency_swarm-0.2.5/tests/data/schemas/relevance.json`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/tests/demos/demo_gradio.py` & `agency_swarm-0.2.5/tests/demos/demo_gradio.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import gradio as gr
 
 sys.path.insert(0, './agency-swarm')
 
 from agency_swarm import set_openai_key, Agent
 
 from agency_swarm.agency.agency import Agency
-from agency_swarm.tools.oai import FileSearch
+from agency_swarm.tools.oai import FileSearch, CodeInterpreter
 
 ceo = Agent(name="CEO",
             description="Responsible for client communication, task planning and management.",
             instructions="Analyze uploaded files with myfiles_browser tool.", # can be a file like ./instructions.md
-            tools=[FileSearch])
+            tools=[FileSearch, CodeInterpreter])
 
 
 test_agent = Agent(name="Test Agent1",
                      description="Responsible for testing.",
                      instructions="Read files with myfiles_browser tool.", # can be a file like ./instructions.md
                      tools=[FileSearch])
 
@@ -27,11 +27,11 @@
 
 
 
 agency = Agency([
     ceo, test_agent, test_agent2
 ], shared_instructions="")
 
-# agency.demo_gradio()
+agency.demo_gradio()
 
-print(agency.get_completion("Hello", recipient_agent=test_agent, yield_messages=False))
+# print(agency.get_completion("Hello", recipient_agent=test_agent, yield_messages=False))
```

### Comparing `agency_swarm-0.2.3/tests/demos/streaming_demo.py` & `agency_swarm-0.2.5/tests/demos/streaming_demo.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/tests/demos/term_demo.py` & `agency_swarm-0.2.5/tests/demos/term_demo.py`

 * *Files identical despite different names*

### Comparing `agency_swarm-0.2.3/tests/test_agency.py` & `agency_swarm-0.2.5/tests/test_agency.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,18 +278,18 @@
             @override
             @classmethod
             def on_all_streams_end(cls):
                 nonlocal num_on_all_streams_end_calls
                 num_on_all_streams_end_calls += 1
 
         message = self.__class__.agency.get_completion_stream(
-            "Please tell TestAgent1 to tell TestAgent 2 to use test tool.",
+            "Please tell TestAgent1 to tell TestAgent2 to use TestTool.",
             event_handler=EventHandler,
-            additional_instructions="Your message to TestAgent1 should be exactly as follows: "
-                                    "'Please tell TestAgent2 to use test tool.'",
+            additional_instructions="\n\n**Your message to TestAgent1 should be exactly as follows:** "
+                                    "'Please tell TestAgent2 to use TestTool.'",
             tool_choice={"type": "function", "function": {"name": "SendMessage"}})
 
         # self.assertFalse('error' in message.lower())
 
         self.assertTrue(test_tool_used)
         self.assertTrue(test_agent2_used)
         self.assertTrue(num_on_all_streams_end_calls == 1)
@@ -362,14 +362,19 @@
             self.assertTrue(agent.id in [settings['id'] for settings in previous_loaded_agents_settings])
 
     def test_7_init_async_agency(self):
         """it should initialize agency with agents"""
         # reset loaded thread ids
         self.__class__.loaded_thread_ids = {}
 
+        # Set ids for all agents to None
+        self.__class__.ceo.id = None
+        self.__class__.agent1.id = None
+        self.__class__.agent2.id = None
+
         self.__class__.agency = Agency([
             self.__class__.ceo,
             [self.__class__.ceo, self.__class__.agent1],
             [self.__class__.agent1, self.__class__.agent2]],
             shared_instructions="",
             settings_callbacks=self.__class__.settings_callbacks,
             threads_callbacks=self.__class__.threads_callbacks,
```

