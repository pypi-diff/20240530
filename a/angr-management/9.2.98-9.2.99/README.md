# Comparing `tmp/angr-management-9.2.98.tar.gz` & `tmp/angr_management-9.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angr-management-9.2.98.tar", last modified: Tue Apr  9 17:03:08 2024, max compression
+gzip compressed data, was "angr_management-9.2.99.tar", last modified: Tue Apr 16 17:02:59 2024, max compression
```

## Comparing `angr-management-9.2.98.tar` & `angr_management-9.2.99.tar`

### file list

```diff
@@ -1,409 +1,409 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.116837 angr-management-9.2.98/
--rw-r--r--   0 vsts      (1001) docker     (127)     1326 2024-04-09 17:01:35.000000 angr-management-9.2.98/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)     5023 2024-04-09 17:03:08.116837 angr-management-9.2.98/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     3414 2024-04-09 17:01:35.000000 angr-management-9.2.98/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.116837 angr-management-9.2.98/angr_management.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     5023 2024-04-09 17:03:07.000000 angr-management-9.2.98/angr_management.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)    15707 2024-04-09 17:03:07.000000 angr-management-9.2.98/angr_management.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-09 17:03:07.000000 angr-management-9.2.98/angr_management.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-09 17:03:07.000000 angr-management-9.2.98/angr_management.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      571 2024-04-09 17:03:07.000000 angr-management-9.2.98/angr_management.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-04-09 17:03:07.000000 angr-management-9.2.98/angr_management.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:07.968837 angr-management-9.2.98/angrmanagement/
--rw-r--r--   0 vsts      (1001) docker     (127)      270 2024-04-09 17:01:43.000000 angr-management-9.2.98/angrmanagement/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8451 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:07.968837 angr-management-9.2.98/angrmanagement/config/
--rw-r--r--   0 vsts      (1001) docker     (127)     1586 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27335 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/config/color_schemes.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/config/config_entry.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26486 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/config/config_manager.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:07.968837 angr-management-9.2.98/angrmanagement/daemon/
--rw-r--r--   0 vsts      (1001) docker     (127)      775 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/daemon/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2561 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/daemon/client.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5051 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/daemon/server.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5168 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/daemon/url_handler.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:07.972837 angr-management-9.2.98/angrmanagement/data/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11400 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/analysis_options.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2102 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/breakpoint.py
--rw-r--r--   0 vsts      (1001) docker     (127)      962 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/function_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)      267 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/highlight_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/indirect_jump.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14536 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/instance.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:07.972837 angr-management-9.2.98/angrmanagement/data/jobs/
--rw-r--r--   0 vsts      (1001) docker     (127)      903 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/jobs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3470 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/jobs/cfg_generation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      704 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/jobs/code_tagging.py
--rw-r--r--   0 vsts      (1001) docker     (127)      637 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/jobs/ddg_generation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/jobs/decompile_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10957 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/jobs/dependency_analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)      893 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/jobs/flirt_signature_recognition.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3628 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/jobs/job.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6291 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/jobs/loading.py
--rw-r--r--   0 vsts      (1001) docker     (127)      702 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/jobs/prototype_finding.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1511 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/jobs/simgr_explore.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1397 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/jobs/simgr_step.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3821 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/jobs/variable_recovery.py
--rw-r--r--   0 vsts      (1001) docker     (127)      513 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/jobs/vfg_generation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1882 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/library_docs.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3019 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/log.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3838 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/object_container.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4417 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/tagged_interval_map.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1179 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/data/trace.py
--rw-r--r--   0 vsts      (1001) docker     (127)      306 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/errors.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:07.976837 angr-management-9.2.98/angrmanagement/logic/
--rw-r--r--   0 vsts      (1001) docker     (127)      966 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/logic/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:07.976837 angr-management-9.2.98/angrmanagement/logic/commands/
--rw-r--r--   0 vsts      (1001) docker     (127)      227 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/logic/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2056 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/logic/commands/command.py
--rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/logic/commands/command_manager.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:07.976837 angr-management-9.2.98/angrmanagement/logic/debugger/
--rw-r--r--   0 vsts      (1001) docker     (127)      226 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/logic/debugger/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10828 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/logic/debugger/bintrace.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5926 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/logic/debugger/debugger.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3060 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/logic/debugger/simgr.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:07.976837 angr-management-9.2.98/angrmanagement/logic/disassembly/
--rw-r--r--   0 vsts      (1001) docker     (127)      206 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/logic/disassembly/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13363 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/logic/disassembly/info_dock.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1858 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/logic/disassembly/jump_history.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5466 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/logic/singleton.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7675 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/logic/threads.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5658 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/logic/url_scheme.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:07.980836 angr-management-9.2.98/angrmanagement/plugins/
--rw-r--r--   0 vsts      (1001) docker     (127)     1110 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:07.984837 angr-management-9.2.98/angrmanagement/plugins/ail2asm/
--rw-r--r--   0 vsts      (1001) docker     (127)       94 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/ail2asm/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10345 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/ail2asm/ail2arm32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1381 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/ail2asm/asm_output.py
--rw-r--r--   0 vsts      (1001) docker     (127)      262 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/ail2asm/plugin.toml
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:07.984837 angr-management-9.2.98/angrmanagement/plugins/angr_binsync/
--rw-r--r--   0 vsts      (1001) docker     (127)      124 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/angr_binsync/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      271 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/angr_binsync/plugin.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     7399 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/base_plugin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:07.988837 angr-management-9.2.98/angrmanagement/plugins/binharness/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/binharness/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1240 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/binharness/bhinstance.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1210 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/binharness/binharness_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (127)      289 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/binharness/plugin.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     3207 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/binharness/run_target_dialog.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1718 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/binharness/stream_view.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:07.988837 angr-management-9.2.98/angrmanagement/plugins/coverage/
--rw-r--r--   0 vsts      (1001) docker     (127)      103 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/coverage/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9825 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/coverage/coverage.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4676 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/coverage/parse_trace.py
--rw-r--r--   0 vsts      (1001) docker     (127)      283 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/coverage/plugin.toml
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:07.992837 angr-management-9.2.98/angrmanagement/plugins/decompiler_poison/
--rw-r--r--   0 vsts      (1001) docker     (127)     6073 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/decompiler_poison/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      294 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/decompiler_poison/plugin.toml
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:07.992837 angr-management-9.2.98/angrmanagement/plugins/dep_viewer/
--rw-r--r--   0 vsts      (1001) docker     (127)      116 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/dep_viewer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1973 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/dep_viewer/dep_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (127)      289 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/dep_viewer/plugin.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     2797 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/dep_viewer/sinks.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:07.992837 angr-management-9.2.98/angrmanagement/plugins/execution_statistics_viewer/
--rw-r--r--   0 vsts      (1001) docker     (127)      151 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/execution_statistics_viewer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5389 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/execution_statistics_viewer/execution_statistics_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (127)      316 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/execution_statistics_viewer/plugin.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     3852 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/load.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:07.996837 angr-management-9.2.98/angrmanagement/plugins/memory_checker/
--rw-r--r--   0 vsts      (1001) docker     (127)      107 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/memory_checker/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2820 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/memory_checker/memory_checker.py
--rw-r--r--   0 vsts      (1001) docker     (127)      287 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/memory_checker/plugin.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     3998 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/plugin_description.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22658 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/plugin_manager.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:07.996837 angr-management-9.2.98/angrmanagement/plugins/precise_diffing/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/precise_diffing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      841 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/precise_diffing/diff_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11585 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/precise_diffing/function_diff.py
--rw-r--r--   0 vsts      (1001) docker     (127)      294 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/precise_diffing/plugin.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     6850 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/precise_diffing/precisediff_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7279 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/precise_diffing/settings_dialog.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1092 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/sample_plugin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:07.996837 angr-management-9.2.98/angrmanagement/plugins/source_importer/
--rw-r--r--   0 vsts      (1001) docker     (127)     1642 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/source_importer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      283 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/source_importer/plugin.toml
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.000837 angr-management-9.2.98/angrmanagement/plugins/source_viewer/
--rw-r--r--   0 vsts      (1001) docker     (127)      130 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/source_viewer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      291 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/source_viewer/plugin.toml
--rw-r--r--   0 vsts      (1001) docker     (127)    10729 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/source_viewer/source_viewer_plugin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.004837 angr-management-9.2.98/angrmanagement/plugins/trace_viewer/
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/trace_viewer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8589 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/trace_viewer/afl_qemu_bitmap.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4677 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/trace_viewer/multi_trace.py
--rw-r--r--   0 vsts      (1001) docker     (127)      304 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/trace_viewer/plugin.toml
--rw-r--r--   0 vsts      (1001) docker     (127)    19741 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/trace_viewer/qtrace_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14564 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/trace_viewer/trace_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9407 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/trace_viewer/trace_statistics.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.004837 angr-management-9.2.98/angrmanagement/plugins/value_search/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/value_search/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1030 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/value_search/constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/value_search/plugin.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     6636 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/value_search/qsearch_table.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4714 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/value_search/search_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4106 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/value_search/value_search_plugin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.004837 angr-management-9.2.98/angrmanagement/plugins/varec/
--rw-r--r--   0 vsts      (1001) docker     (127)       82 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/varec/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      286 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/varec/plugin.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     6570 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/plugins/varec/varec.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:07.960837 angr-management-9.2.98/angrmanagement/resources/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.004837 angr-management-9.2.98/angrmanagement/resources/fonts/
--rw-r--r--   0 vsts      (1001) docker     (127)   340712 2024-04-09 17:01:35.000000 angr-management-9.2.98/angrmanagement/resources/fonts/DejaVuSansMono.ttf
--rw-r--r--   0 vsts      (1001) docker     (127)   212880 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/fonts/SourceCodePro-Regular.ttf
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.016837 angr-management-9.2.98/angrmanagement/resources/images/
--rw-r--r--   0 vsts      (1001) docker     (127)   100896 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/images/angr-ds.png
--rw-r--r--   0 vsts      (1001) docker     (127)   143434 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/images/angr-splash.png
--rw-r--r--   0 vsts      (1001) docker     (127)   165662 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/images/angr.ico
--rw-r--r--   0 vsts      (1001) docker     (127)    79574 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/images/angr.png
--rw-r--r--   0 vsts      (1001) docker     (127)    11090 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/images/benchmark-icon.png
--rw-r--r--   0 vsts      (1001) docker     (127)     9627 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/images/error-icon.png
--rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/images/run-icon.svg
--rw-r--r--   0 vsts      (1001) docker     (127)     9671 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/images/toolbar-docker-open.png
--rw-r--r--   0 vsts      (1001) docker     (127)   176067 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/images/toolbar-file-open.ico
--rw-r--r--   0 vsts      (1001) docker     (127)   103065 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/images/toolbar-file-save.png
--rw-r--r--   0 vsts      (1001) docker     (127)     1219 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/images/toolbar-forward.png
--rw-r--r--   0 vsts      (1001) docker     (127)     1200 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/images/toolbar-previous.png
--rw-r--r--   0 vsts      (1001) docker     (127)     1891 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/images/toolbar-show-alignment.png
--rw-r--r--   0 vsts      (1001) docker     (127)    25190 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/images/warning-icon.png
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.016837 angr-management-9.2.98/angrmanagement/resources/themes/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.016837 angr-management-9.2.98/angrmanagement/resources/themes/Catppuccin Mocha/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.016837 angr-management-9.2.98/angrmanagement/resources/themes/Catppuccin Mocha/images/
--rw-r--r--   0 vsts      (1001) docker     (127)      708 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Catppuccin Mocha/images/close.svg
--rw-r--r--   0 vsts      (1001) docker     (127)     1219 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Catppuccin Mocha/images/drawing-pin.svg
--rw-r--r--   0 vsts      (1001) docker     (127)      293 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Catppuccin Mocha/images/minimize-button.svg
--rw-r--r--   0 vsts      (1001) docker     (127)      416 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Catppuccin Mocha/images/provenance.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      170 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Catppuccin Mocha/images/tab-menu.svg
--rw-r--r--   0 vsts      (1001) docker     (127)      500 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Catppuccin Mocha/theme.css
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.016837 angr-management-9.2.98/angrmanagement/resources/themes/Dark/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.020837 angr-management-9.2.98/angrmanagement/resources/themes/Dark/images/
--rw-r--r--   0 vsts      (1001) docker     (127)      708 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Dark/images/close.svg
--rw-r--r--   0 vsts      (1001) docker     (127)     1219 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Dark/images/drawing-pin.svg
--rw-r--r--   0 vsts      (1001) docker     (127)      293 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Dark/images/minimize-button.svg
--rw-r--r--   0 vsts      (1001) docker     (127)      363 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Dark/images/provenance.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      170 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Dark/images/tab-menu.svg
--rw-r--r--   0 vsts      (1001) docker     (127)      500 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Dark/theme.css
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.020837 angr-management-9.2.98/angrmanagement/resources/themes/Dracula/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.020837 angr-management-9.2.98/angrmanagement/resources/themes/Dracula/images/
--rw-r--r--   0 vsts      (1001) docker     (127)      708 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Dracula/images/close.svg
--rw-r--r--   0 vsts      (1001) docker     (127)     1219 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Dracula/images/drawing-pin.svg
--rw-r--r--   0 vsts      (1001) docker     (127)      293 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Dracula/images/minimize-button.svg
--rw-r--r--   0 vsts      (1001) docker     (127)      415 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Dracula/images/provenance.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      170 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Dracula/images/tab-menu.svg
--rw-r--r--   0 vsts      (1001) docker     (127)      500 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Dracula/theme.css
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.024837 angr-management-9.2.98/angrmanagement/resources/themes/Light/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.024837 angr-management-9.2.98/angrmanagement/resources/themes/Light/images/
--rw-r--r--   0 vsts      (1001) docker     (127)      694 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Light/images/close.svg
--rw-r--r--   0 vsts      (1001) docker     (127)     1219 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Light/images/drawing-pin-light.svg
--rw-r--r--   0 vsts      (1001) docker     (127)     1006 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Light/images/drawing-pin.svg
--rw-r--r--   0 vsts      (1001) docker     (127)      293 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Light/images/minimize-button.svg
--rw-r--r--   0 vsts      (1001) docker     (127)      337 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Light/images/provenance.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      170 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Light/images/tab-menu.svg
--rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/Light/theme.css
--rw-r--r--   0 vsts      (1001) docker     (127)     7502 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/resources/themes/base.css
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.028837 angr-management-9.2.98/angrmanagement/ui/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3837 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/awesome_tooltip_event_filter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.028837 angr-management-9.2.98/angrmanagement/ui/css/
--rw-r--r--   0 vsts      (1001) docker     (127)     4136 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/css/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.040837 angr-management-9.2.98/angrmanagement/ui/dialogs/
--rw-r--r--   0 vsts      (1001) docker     (127)      512 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1952 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/about.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11010 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/analysis_options.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6536 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/assemble_patch.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4888 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/breakpoint.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9795 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/command_palette.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5124 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/data_dep_graph_search.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6179 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/dependson.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2528 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/env_config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1026 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/fs_mount.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1939 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/func_doc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5309 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4762 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/hook.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1727 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/input_prompt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2641 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/jumpto.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19621 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/load_binary.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1479 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/load_docker_prompt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4287 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/load_plugins.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15342 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/new_state.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10062 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/preferences.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3441 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/rename.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4003 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/rename_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9608 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/rename_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6459 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/retype_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2973 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/set_comment.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11317 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/socket_config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5913 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/type_editor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3416 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/welcome.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2786 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/dialogs/xref.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.044837 angr-management-9.2.98/angrmanagement/ui/documents/
--rw-r--r--   0 vsts      (1001) docker     (127)      106 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/documents/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5999 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/documents/qcodedocument.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1129 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/icons.py
--rw-r--r--   0 vsts      (1001) docker     (127)    37584 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/main_window.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.048837 angr-management-9.2.98/angrmanagement/ui/menus/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/menus/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1340 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/menus/analyze_menu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4251 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/menus/disasm_insn_context_menu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2733 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/menus/disasm_label_context_menu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2575 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/menus/disasm_options_menu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3489 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/menus/file_menu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1086 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/menus/function_context_menu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      820 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/menus/help_menu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      958 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/menus/log_menu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5225 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/menus/menu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      508 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/menus/plugin_menu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6044 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/menus/view_menu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2178 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/toolbar_manager.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.052837 angr-management-9.2.98/angrmanagement/ui/toolbars/
--rw-r--r--   0 vsts      (1001) docker     (127)      383 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/toolbars/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9051 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/toolbars/debug_toolbar.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2072 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/toolbars/feature_map_toolbar.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1313 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/toolbars/file_toolbar.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/toolbars/function_table_toolbar.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3576 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/toolbars/nav_toolbar.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2556 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/toolbars/toolbar.py
--rw-r--r--   0 vsts      (1001) docker     (127)      651 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/toolbars/toolbar_action.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2483 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/toolbars/toolbar_dock.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7437 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/view_manager.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.064837 angr-management-9.2.98/angrmanagement/ui/views/
--rw-r--r--   0 vsts      (1001) docker     (127)     1351 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/views/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5973 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/views/breakpoints_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6366 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/views/call_explorer_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21141 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/views/code_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3678 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/views/console_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9781 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/views/data_dep_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4635 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/views/dep_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)    38085 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/views/disassembly_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2314 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/views/functions_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)    72410 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/views/hex_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18156 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/views/interaction_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1233 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/views/log_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1149 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/views/patches_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6239 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/views/proximity_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5257 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/views/registers_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6067 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/views/stack_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1524 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/views/states_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4112 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/views/strings_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4924 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/views/symexec_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1229 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/views/trace_map_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4809 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/views/traces_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5125 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/views/types_view.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9710 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/views/view.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.092837 angr-management-9.2.98/angrmanagement/ui/widgets/
--rw-r--r--   0 vsts      (1001) docker     (127)      987 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2435 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/filesystem_table.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1523 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qaddress_input.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6119 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qast_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14284 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qblock.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25547 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qblock_code.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2199 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qblock_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24777 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qccode_edit.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10063 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qccode_highlighter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1494 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qcolor_option.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2095 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qconstraint_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10223 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qdatadep_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7110 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qdatadepgraph_block.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9805 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qdecomp_options.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4447 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qdep_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7674 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qdepgraph_block.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3715 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qdisasm_base_control.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12665 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qdisasm_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4831 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qdisasm_statusbar.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26979 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qfeature_map.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2833 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qfiledesc_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1353 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qfont_option.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1934 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qfunction_combobox.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5922 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qfunction_header.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20238 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qfunction_table.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11772 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qgraph.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11714 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qgraph_arrow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1214 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qgraph_object.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1080 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qicon_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9249 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qinst_annotation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11637 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qinstruction.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1753 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qipython_widget.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20717 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qlinear_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8606 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qlog_widget.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9752 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qmemory_data_block.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5488 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qmemory_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9628 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qminimap.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19882 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qoperand.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5087 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qpatch_table.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4671 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qpathtree.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5187 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qphivariable.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5100 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qproximity_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12132 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qproximitygraph_block.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5600 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qregister_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9769 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qsimulation_manager_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12162 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qsimulation_managers.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5464 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qstate_block.py
--rw-r--r--   0 vsts      (1001) docker     (127)      909 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qstate_combobox.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6199 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qstate_table.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8582 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qstring_table.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4799 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qsymexec_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15555 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qtrace_map.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4544 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qtypedef.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3480 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qunknown_block.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4278 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qvariable.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2417 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qvextemps_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10602 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/qxref_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1721 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/widgets/state_inspector.py
--rw-r--r--   0 vsts      (1001) docker     (127)    38533 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/ui/workspace.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.096837 angr-management-9.2.98/angrmanagement/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)     8191 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      757 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/utils/block_objects.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3562 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/utils/cfg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      357 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/utils/daemon_thread.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1655 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/utils/edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2387 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/utils/env.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1314 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/utils/func.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11456 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/utils/graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30785 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/utils/graph_layouter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2451 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/utils/io.py
--rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/utils/layout.py
--rw-r--r--   0 vsts      (1001) docker     (127)      672 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/utils/monkeypatch_stdio.py
--rw-r--r--   0 vsts      (1001) docker     (127)    42616 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/utils/namegen.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11676 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/utils/tree_graph_layouter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.096837 angr-management-9.2.98/angrmanagement/vendor/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.112837 angr-management-9.2.98/angrmanagement/vendor/qtconsole/
--rw-r--r--   0 vsts      (1001) docker     (127)       48 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       73 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       72 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/_version.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14176 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/ansi_code_processor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6295 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/base_frontend_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3733 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/bracket_matcher.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10683 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/call_tip_widget.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1971 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/client.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8839 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/comms.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12909 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/completion_html.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2234 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/completion_plain.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8151 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/completion_widget.py
--rw-r--r--   0 vsts      (1001) docker     (127)   104717 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/console_widget.py
--rw-r--r--   0 vsts      (1001) docker     (127)    34810 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/frontend_widget.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9947 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/history_console_widget.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2874 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/inprocess.py
--rw-r--r--   0 vsts      (1001) docker     (127)      169 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/ipython_widget.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24994 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/jupyter_widget.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1813 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/kernel_mixins.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3793 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/kill_ring.py
--rw-r--r--   0 vsts      (1001) docker     (127)    38376 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/mainwindow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2602 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/manager.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9110 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/pygments_highlighter.py
--rw-r--r--   0 vsts      (1001) docker     (127)      540 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/qstringhelpers.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17176 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/qtconsoleapp.py
--rw-r--r--   0 vsts      (1001) docker     (127)      184 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/rich_ipython_widget.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18469 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/rich_jupyter_widget.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8638 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/rich_text.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3801 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/styles.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2394 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/svg.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8349 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/usage.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8354 2024-04-09 17:01:36.000000 angr-management-9.2.98/angrmanagement/vendor/qtconsole/util.py
--rw-r--r--   0 vsts      (1001) docker     (127)      596 2024-04-09 17:01:43.000000 angr-management-9.2.98/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     1430 2024-04-09 17:03:08.116837 angr-management-9.2.98/setup.cfg
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:03:08.112837 angr-management-9.2.98/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)     2053 2024-04-09 17:01:36.000000 angr-management-9.2.98/tests/test_qaddress_input.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5241 2024-04-09 17:01:36.000000 angr-management-9.2.98/tests/test_rename_functions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3681 2024-04-09 17:01:36.000000 angr-management-9.2.98/tests/test_rename_variables.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3487 2024-04-09 17:01:36.000000 angr-management-9.2.98/tests/test_tagged_interval_map.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3220 2024-04-09 17:01:36.000000 angr-management-9.2.98/tests/test_views_open.py
--rw-r--r--   0 vsts      (1001) docker     (127)      873 2024-04-09 17:01:36.000000 angr-management-9.2.98/tests/test_workflow.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.089766 angr_management-9.2.99/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1326 2024-04-16 17:01:31.000000 angr_management-9.2.99/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)     5023 2024-04-16 17:02:59.089766 angr_management-9.2.99/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     3414 2024-04-16 17:01:31.000000 angr_management-9.2.99/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.085766 angr_management-9.2.99/angr_management.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5023 2024-04-16 17:02:58.000000 angr_management-9.2.99/angr_management.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)    15707 2024-04-16 17:02:58.000000 angr_management-9.2.99/angr_management.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-16 17:02:58.000000 angr_management-9.2.99/angr_management.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-16 17:02:58.000000 angr_management-9.2.99/angr_management.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      571 2024-04-16 17:02:58.000000 angr_management-9.2.99/angr_management.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-04-16 17:02:58.000000 angr_management-9.2.99/angr_management.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:58.985766 angr_management-9.2.99/angrmanagement/
+-rw-r--r--   0 vsts      (1001) docker     (127)      270 2024-04-16 17:01:35.000000 angr_management-9.2.99/angrmanagement/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8451 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:58.989766 angr_management-9.2.99/angrmanagement/config/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1586 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27335 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/config/color_schemes.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/config/config_entry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26486 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/config/config_manager.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:58.989766 angr_management-9.2.99/angrmanagement/daemon/
+-rw-r--r--   0 vsts      (1001) docker     (127)      775 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/daemon/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2561 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/daemon/client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5051 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/daemon/server.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5168 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/daemon/url_handler.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:58.993765 angr_management-9.2.99/angrmanagement/data/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11400 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/analysis_options.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2102 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/breakpoint.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      962 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/function_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      267 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/highlight_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/indirect_jump.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14536 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/instance.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:58.993765 angr_management-9.2.99/angrmanagement/data/jobs/
+-rw-r--r--   0 vsts      (1001) docker     (127)      903 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/jobs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3470 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/jobs/cfg_generation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      704 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/jobs/code_tagging.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      637 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/jobs/ddg_generation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/jobs/decompile_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10957 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/jobs/dependency_analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      893 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/jobs/flirt_signature_recognition.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3628 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/jobs/job.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6291 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/jobs/loading.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      702 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/jobs/prototype_finding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1511 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/jobs/simgr_explore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1397 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/jobs/simgr_step.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3821 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/jobs/variable_recovery.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      513 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/jobs/vfg_generation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1882 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/library_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3019 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3838 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/object_container.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4417 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/tagged_interval_map.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1179 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/data/trace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      306 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/errors.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:58.997765 angr_management-9.2.99/angrmanagement/logic/
+-rw-r--r--   0 vsts      (1001) docker     (127)      966 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/logic/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:58.997765 angr_management-9.2.99/angrmanagement/logic/commands/
+-rw-r--r--   0 vsts      (1001) docker     (127)      227 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/logic/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2056 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/logic/commands/command.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/logic/commands/command_manager.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:58.997765 angr_management-9.2.99/angrmanagement/logic/debugger/
+-rw-r--r--   0 vsts      (1001) docker     (127)      226 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/logic/debugger/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10828 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/logic/debugger/bintrace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5926 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/logic/debugger/debugger.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3060 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/logic/debugger/simgr.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:58.997765 angr_management-9.2.99/angrmanagement/logic/disassembly/
+-rw-r--r--   0 vsts      (1001) docker     (127)      206 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/logic/disassembly/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13363 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/logic/disassembly/info_dock.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1858 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/logic/disassembly/jump_history.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5466 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/logic/singleton.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7675 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/logic/threads.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5658 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/logic/url_scheme.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.001766 angr_management-9.2.99/angrmanagement/plugins/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1110 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.001766 angr_management-9.2.99/angrmanagement/plugins/ail2asm/
+-rw-r--r--   0 vsts      (1001) docker     (127)       94 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/ail2asm/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10345 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/ail2asm/ail2arm32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1381 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/ail2asm/asm_output.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      262 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/ail2asm/plugin.toml
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.001766 angr_management-9.2.99/angrmanagement/plugins/angr_binsync/
+-rw-r--r--   0 vsts      (1001) docker     (127)      124 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/angr_binsync/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      271 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/angr_binsync/plugin.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     7399 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/base_plugin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.001766 angr_management-9.2.99/angrmanagement/plugins/binharness/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/binharness/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1240 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/binharness/bhinstance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1210 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/binharness/binharness_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      289 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/binharness/plugin.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     3207 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/binharness/run_target_dialog.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1718 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/binharness/stream_view.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.005766 angr_management-9.2.99/angrmanagement/plugins/coverage/
+-rw-r--r--   0 vsts      (1001) docker     (127)      103 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/coverage/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9825 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/coverage/coverage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4676 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/coverage/parse_trace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      283 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/coverage/plugin.toml
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.005766 angr_management-9.2.99/angrmanagement/plugins/decompiler_poison/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6073 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/decompiler_poison/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      294 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/decompiler_poison/plugin.toml
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.005766 angr_management-9.2.99/angrmanagement/plugins/dep_viewer/
+-rw-r--r--   0 vsts      (1001) docker     (127)      116 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/dep_viewer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1973 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/dep_viewer/dep_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      289 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/dep_viewer/plugin.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     2797 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/dep_viewer/sinks.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.005766 angr_management-9.2.99/angrmanagement/plugins/execution_statistics_viewer/
+-rw-r--r--   0 vsts      (1001) docker     (127)      151 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/execution_statistics_viewer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5389 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/execution_statistics_viewer/execution_statistics_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      316 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/execution_statistics_viewer/plugin.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     3852 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/load.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.005766 angr_management-9.2.99/angrmanagement/plugins/memory_checker/
+-rw-r--r--   0 vsts      (1001) docker     (127)      107 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/memory_checker/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2820 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/memory_checker/memory_checker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      287 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/memory_checker/plugin.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     3998 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/plugin_description.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22658 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/plugin_manager.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.009765 angr_management-9.2.99/angrmanagement/plugins/precise_diffing/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/precise_diffing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      841 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/precise_diffing/diff_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11585 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/precise_diffing/function_diff.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      294 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/precise_diffing/plugin.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     6850 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/precise_diffing/precisediff_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7279 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/precise_diffing/settings_dialog.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1092 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/sample_plugin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.009765 angr_management-9.2.99/angrmanagement/plugins/source_importer/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1642 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/source_importer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      283 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/source_importer/plugin.toml
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.009765 angr_management-9.2.99/angrmanagement/plugins/source_viewer/
+-rw-r--r--   0 vsts      (1001) docker     (127)      130 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/source_viewer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      291 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/source_viewer/plugin.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)    10729 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/source_viewer/source_viewer_plugin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.009765 angr_management-9.2.99/angrmanagement/plugins/trace_viewer/
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/trace_viewer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8589 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/trace_viewer/afl_qemu_bitmap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4677 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/trace_viewer/multi_trace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      304 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/trace_viewer/plugin.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)    19741 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/trace_viewer/qtrace_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14564 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/trace_viewer/trace_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9407 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/trace_viewer/trace_statistics.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.013765 angr_management-9.2.99/angrmanagement/plugins/value_search/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/value_search/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1030 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/value_search/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/value_search/plugin.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     6636 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/value_search/qsearch_table.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4714 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/value_search/search_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4106 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/value_search/value_search_plugin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.013765 angr_management-9.2.99/angrmanagement/plugins/varec/
+-rw-r--r--   0 vsts      (1001) docker     (127)       82 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/varec/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      286 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/varec/plugin.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     6570 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/plugins/varec/varec.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:58.981765 angr_management-9.2.99/angrmanagement/resources/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.013765 angr_management-9.2.99/angrmanagement/resources/fonts/
+-rw-r--r--   0 vsts      (1001) docker     (127)   340712 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/fonts/DejaVuSansMono.ttf
+-rw-r--r--   0 vsts      (1001) docker     (127)   212880 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/fonts/SourceCodePro-Regular.ttf
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.017766 angr_management-9.2.99/angrmanagement/resources/images/
+-rw-r--r--   0 vsts      (1001) docker     (127)   100896 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/images/angr-ds.png
+-rw-r--r--   0 vsts      (1001) docker     (127)   143434 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/images/angr-splash.png
+-rw-r--r--   0 vsts      (1001) docker     (127)   165662 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/images/angr.ico
+-rw-r--r--   0 vsts      (1001) docker     (127)    79574 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/images/angr.png
+-rw-r--r--   0 vsts      (1001) docker     (127)    11090 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/images/benchmark-icon.png
+-rw-r--r--   0 vsts      (1001) docker     (127)     9627 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/images/error-icon.png
+-rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/images/run-icon.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)     9671 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/images/toolbar-docker-open.png
+-rw-r--r--   0 vsts      (1001) docker     (127)   176067 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/images/toolbar-file-open.ico
+-rw-r--r--   0 vsts      (1001) docker     (127)   103065 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/images/toolbar-file-save.png
+-rw-r--r--   0 vsts      (1001) docker     (127)     1219 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/images/toolbar-forward.png
+-rw-r--r--   0 vsts      (1001) docker     (127)     1200 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/images/toolbar-previous.png
+-rw-r--r--   0 vsts      (1001) docker     (127)     1891 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/images/toolbar-show-alignment.png
+-rw-r--r--   0 vsts      (1001) docker     (127)    25190 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/images/warning-icon.png
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.017766 angr_management-9.2.99/angrmanagement/resources/themes/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.021766 angr_management-9.2.99/angrmanagement/resources/themes/Catppuccin Mocha/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.021766 angr_management-9.2.99/angrmanagement/resources/themes/Catppuccin Mocha/images/
+-rw-r--r--   0 vsts      (1001) docker     (127)      708 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Catppuccin Mocha/images/close.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1219 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Catppuccin Mocha/images/drawing-pin.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)      293 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Catppuccin Mocha/images/minimize-button.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)      416 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Catppuccin Mocha/images/provenance.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      170 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Catppuccin Mocha/images/tab-menu.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)      500 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Catppuccin Mocha/theme.css
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.021766 angr_management-9.2.99/angrmanagement/resources/themes/Dark/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.021766 angr_management-9.2.99/angrmanagement/resources/themes/Dark/images/
+-rw-r--r--   0 vsts      (1001) docker     (127)      708 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Dark/images/close.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1219 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Dark/images/drawing-pin.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)      293 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Dark/images/minimize-button.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)      363 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Dark/images/provenance.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      170 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Dark/images/tab-menu.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)      500 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Dark/theme.css
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.021766 angr_management-9.2.99/angrmanagement/resources/themes/Dracula/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.025766 angr_management-9.2.99/angrmanagement/resources/themes/Dracula/images/
+-rw-r--r--   0 vsts      (1001) docker     (127)      708 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Dracula/images/close.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1219 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Dracula/images/drawing-pin.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)      293 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Dracula/images/minimize-button.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)      415 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Dracula/images/provenance.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      170 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Dracula/images/tab-menu.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)      500 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Dracula/theme.css
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.025766 angr_management-9.2.99/angrmanagement/resources/themes/Light/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.025766 angr_management-9.2.99/angrmanagement/resources/themes/Light/images/
+-rw-r--r--   0 vsts      (1001) docker     (127)      694 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Light/images/close.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1219 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Light/images/drawing-pin-light.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1006 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Light/images/drawing-pin.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)      293 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Light/images/minimize-button.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)      337 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Light/images/provenance.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      170 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Light/images/tab-menu.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/Light/theme.css
+-rw-r--r--   0 vsts      (1001) docker     (127)     7502 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/resources/themes/base.css
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.025766 angr_management-9.2.99/angrmanagement/ui/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3837 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/awesome_tooltip_event_filter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.029766 angr_management-9.2.99/angrmanagement/ui/css/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4136 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/css/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.033766 angr_management-9.2.99/angrmanagement/ui/dialogs/
+-rw-r--r--   0 vsts      (1001) docker     (127)      512 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1952 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/about.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11010 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/analysis_options.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6536 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/assemble_patch.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4888 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/breakpoint.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9795 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/command_palette.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5124 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/data_dep_graph_search.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6179 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/dependson.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2528 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/env_config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1026 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/fs_mount.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1939 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/func_doc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5309 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4762 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/hook.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1727 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/input_prompt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2641 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/jumpto.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19621 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/load_binary.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1479 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/load_docker_prompt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4287 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/load_plugins.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15342 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/new_state.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10062 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/preferences.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3441 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/rename.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4003 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/rename_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9608 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/rename_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6459 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/retype_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2973 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/set_comment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11317 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/socket_config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5913 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/type_editor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3416 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/welcome.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2786 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/dialogs/xref.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.033766 angr_management-9.2.99/angrmanagement/ui/documents/
+-rw-r--r--   0 vsts      (1001) docker     (127)      106 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/documents/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5999 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/documents/qcodedocument.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1129 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/icons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    37584 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/main_window.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.037766 angr_management-9.2.99/angrmanagement/ui/menus/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/menus/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1340 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/menus/analyze_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4251 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/menus/disasm_insn_context_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2733 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/menus/disasm_label_context_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2575 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/menus/disasm_options_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3489 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/menus/file_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1086 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/menus/function_context_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      820 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/menus/help_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      958 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/menus/log_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5225 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/menus/menu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      508 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/menus/plugin_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6044 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/menus/view_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2178 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/toolbar_manager.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.041766 angr_management-9.2.99/angrmanagement/ui/toolbars/
+-rw-r--r--   0 vsts      (1001) docker     (127)      383 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/toolbars/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9051 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/toolbars/debug_toolbar.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2072 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/toolbars/feature_map_toolbar.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1313 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/toolbars/file_toolbar.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/toolbars/function_table_toolbar.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3576 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/toolbars/nav_toolbar.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2556 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/toolbars/toolbar.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      651 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/toolbars/toolbar_action.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2483 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/toolbars/toolbar_dock.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7437 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/view_manager.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.049766 angr_management-9.2.99/angrmanagement/ui/views/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1351 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/views/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5973 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/views/breakpoints_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6366 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/views/call_explorer_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21141 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/views/code_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3678 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/views/console_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9781 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/views/data_dep_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4635 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/views/dep_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    38085 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/views/disassembly_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2314 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/views/functions_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    72410 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/views/hex_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18156 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/views/interaction_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1233 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/views/log_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1149 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/views/patches_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6239 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/views/proximity_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5257 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/views/registers_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6067 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/views/stack_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1524 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/views/states_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4112 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/views/strings_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4924 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/views/symexec_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1229 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/views/trace_map_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4809 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/views/traces_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5125 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/views/types_view.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9710 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/views/view.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.069766 angr_management-9.2.99/angrmanagement/ui/widgets/
+-rw-r--r--   0 vsts      (1001) docker     (127)      987 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2435 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/filesystem_table.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1523 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qaddress_input.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6119 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qast_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14284 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qblock.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25547 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qblock_code.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2199 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qblock_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24777 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qccode_edit.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10063 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qccode_highlighter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1494 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qcolor_option.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2095 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qconstraint_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10223 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qdatadep_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7110 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qdatadepgraph_block.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9805 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qdecomp_options.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4447 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qdep_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7674 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qdepgraph_block.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3715 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qdisasm_base_control.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12665 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qdisasm_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4831 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qdisasm_statusbar.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26979 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qfeature_map.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2833 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qfiledesc_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1353 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qfont_option.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1934 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qfunction_combobox.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5922 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qfunction_header.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20238 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qfunction_table.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11772 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qgraph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11714 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qgraph_arrow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1214 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qgraph_object.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1080 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qicon_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9249 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qinst_annotation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11637 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qinstruction.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1753 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qipython_widget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20717 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qlinear_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8606 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qlog_widget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9752 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qmemory_data_block.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5488 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qmemory_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9628 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qminimap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19882 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qoperand.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5087 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qpatch_table.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4671 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qpathtree.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5187 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qphivariable.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5100 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qproximity_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12132 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qproximitygraph_block.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5600 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qregister_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9769 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qsimulation_manager_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12162 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qsimulation_managers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5464 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qstate_block.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      909 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qstate_combobox.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6199 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qstate_table.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8582 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qstring_table.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4799 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qsymexec_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15555 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qtrace_map.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4544 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qtypedef.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3480 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qunknown_block.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4278 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qvariable.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2417 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qvextemps_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10602 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/qxref_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1721 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/widgets/state_inspector.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    38533 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/ui/workspace.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.073766 angr_management-9.2.99/angrmanagement/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)     8191 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      757 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/utils/block_objects.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3562 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/utils/cfg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      357 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/utils/daemon_thread.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1655 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/utils/edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2387 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/utils/env.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1314 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/utils/func.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11456 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/utils/graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30785 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/utils/graph_layouter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2451 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/utils/io.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/utils/layout.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      672 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/utils/monkeypatch_stdio.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    42616 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/utils/namegen.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11676 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/utils/tree_graph_layouter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.073766 angr_management-9.2.99/angrmanagement/vendor/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.085766 angr_management-9.2.99/angrmanagement/vendor/qtconsole/
+-rw-r--r--   0 vsts      (1001) docker     (127)       48 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       73 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       72 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/_version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14176 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/ansi_code_processor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6295 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/base_frontend_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3733 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/bracket_matcher.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10683 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/call_tip_widget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1971 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8839 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/comms.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12909 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/completion_html.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2234 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/completion_plain.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8151 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/completion_widget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   104717 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/console_widget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34810 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/frontend_widget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9947 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/history_console_widget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2874 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/inprocess.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      169 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/ipython_widget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24994 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/jupyter_widget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1813 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/kernel_mixins.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3793 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/kill_ring.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    38376 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/mainwindow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2602 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/manager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9110 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/pygments_highlighter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      540 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/qstringhelpers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17176 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/qtconsoleapp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      184 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/rich_ipython_widget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18469 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/rich_jupyter_widget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8638 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/rich_text.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3801 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/styles.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2394 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/svg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8349 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/usage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8354 2024-04-16 17:01:31.000000 angr_management-9.2.99/angrmanagement/vendor/qtconsole/util.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      596 2024-04-16 17:01:35.000000 angr_management-9.2.99/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1430 2024-04-16 17:02:59.089766 angr_management-9.2.99/setup.cfg
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:59.085766 angr_management-9.2.99/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2053 2024-04-16 17:01:31.000000 angr_management-9.2.99/tests/test_qaddress_input.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5241 2024-04-16 17:01:31.000000 angr_management-9.2.99/tests/test_rename_functions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3681 2024-04-16 17:01:31.000000 angr_management-9.2.99/tests/test_rename_variables.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3487 2024-04-16 17:01:31.000000 angr_management-9.2.99/tests/test_tagged_interval_map.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3220 2024-04-16 17:01:31.000000 angr_management-9.2.99/tests/test_views_open.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      873 2024-04-16 17:01:31.000000 angr_management-9.2.99/tests/test_workflow.py
```

### Comparing `angr-management-9.2.98/LICENSE` & `angr_management-9.2.99/LICENSE`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/PKG-INFO` & `angr_management-9.2.99/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: angr-management
-Version: 9.2.98
+Version: 9.2.99
 Summary: GUI for angr
 Home-page: https://github.com/angr/angr-management
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PySide6>=6.4.2
 Requires-Dist: PySide6-QtAds>=4.2.1
 Requires-Dist: QtAwesome
 Requires-Dist: QtPy
-Requires-Dist: angr[angrDB]==9.2.98
+Requires-Dist: angr[angrDB]==9.2.99
 Requires-Dist: bidict
 Requires-Dist: ipython
 Requires-Dist: pyqodeng>=0.0.10
 Requires-Dist: requests[socks]
 Requires-Dist: tomlkit
 Requires-Dist: pyobjc-framework-Cocoa; platform_system == "Darwin"
 Requires-Dist: thefuzz[speedup]
@@ -35,15 +35,15 @@
 Requires-Dist: binharness~=0.1.0; extra == "binharness"
 Provides-Extra: bintrace
 Requires-Dist: bintrace; extra == "bintrace"
 Provides-Extra: pyinstaller
 Requires-Dist: pyinstaller==6.5.0; extra == "pyinstaller"
 Requires-Dist: pillow; platform_system == "Darwin" and extra == "pyinstaller"
 Requires-Dist: keystone-engine; extra == "pyinstaller"
-Requires-Dist: archr==9.2.98; platform_system == "Linux" and extra == "pyinstaller"
+Requires-Dist: archr==9.2.99; platform_system == "Linux" and extra == "pyinstaller"
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-xdist; extra == "testing"
 
 # angr Management
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `angr-management-9.2.98/README.md` & `angr_management-9.2.99/README.md`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angr_management.egg-info/PKG-INFO` & `angr_management-9.2.99/angr_management.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: angr-management
-Version: 9.2.98
+Version: 9.2.99
 Summary: GUI for angr
 Home-page: https://github.com/angr/angr-management
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PySide6>=6.4.2
 Requires-Dist: PySide6-QtAds>=4.2.1
 Requires-Dist: QtAwesome
 Requires-Dist: QtPy
-Requires-Dist: angr[angrDB]==9.2.98
+Requires-Dist: angr[angrDB]==9.2.99
 Requires-Dist: bidict
 Requires-Dist: ipython
 Requires-Dist: pyqodeng>=0.0.10
 Requires-Dist: requests[socks]
 Requires-Dist: tomlkit
 Requires-Dist: pyobjc-framework-Cocoa; platform_system == "Darwin"
 Requires-Dist: thefuzz[speedup]
@@ -35,15 +35,15 @@
 Requires-Dist: binharness~=0.1.0; extra == "binharness"
 Provides-Extra: bintrace
 Requires-Dist: bintrace; extra == "bintrace"
 Provides-Extra: pyinstaller
 Requires-Dist: pyinstaller==6.5.0; extra == "pyinstaller"
 Requires-Dist: pillow; platform_system == "Darwin" and extra == "pyinstaller"
 Requires-Dist: keystone-engine; extra == "pyinstaller"
-Requires-Dist: archr==9.2.98; platform_system == "Linux" and extra == "pyinstaller"
+Requires-Dist: archr==9.2.99; platform_system == "Linux" and extra == "pyinstaller"
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-xdist; extra == "testing"
 
 # angr Management
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `angr-management-9.2.98/angr_management.egg-info/SOURCES.txt` & `angr_management-9.2.99/angr_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angr_management.egg-info/requires.txt` & `angr_management-9.2.99/angr_management.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 PySide6>=6.4.2
 PySide6-QtAds>=4.2.1
 QtAwesome
 QtPy
-angr[angrDB]==9.2.98
+angr[angrDB]==9.2.99
 bidict
 ipython
 pyqodeng>=0.0.10
 requests[socks]
 tomlkit
 thefuzz[speedup]
 binsync==4.0.0
@@ -32,12 +32,12 @@
 pyinstaller==6.5.0
 keystone-engine
 
 [pyinstaller:platform_system == "Darwin"]
 pillow
 
 [pyinstaller:platform_system == "Linux"]
-archr==9.2.98
+archr==9.2.99
 
 [testing]
 pytest
 pytest-xdist
```

### Comparing `angr-management-9.2.98/angrmanagement/__main__.py` & `angr_management-9.2.99/angrmanagement/__main__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/config/__init__.py` & `angr_management-9.2.99/angrmanagement/config/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/config/color_schemes.py` & `angr_management-9.2.99/angrmanagement/config/color_schemes.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/config/config_entry.py` & `angr_management-9.2.99/angrmanagement/config/config_entry.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/config/config_manager.py` & `angr_management-9.2.99/angrmanagement/config/config_manager.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/daemon/__init__.py` & `angr_management-9.2.99/angrmanagement/daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/daemon/client.py` & `angr_management-9.2.99/angrmanagement/daemon/client.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/daemon/server.py` & `angr_management-9.2.99/angrmanagement/daemon/server.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/daemon/url_handler.py` & `angr_management-9.2.99/angrmanagement/daemon/url_handler.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/data/analysis_options.py` & `angr_management-9.2.99/angrmanagement/data/analysis_options.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/data/breakpoint.py` & `angr_management-9.2.99/angrmanagement/data/breakpoint.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/data/function_graph.py` & `angr_management-9.2.99/angrmanagement/data/function_graph.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/data/instance.py` & `angr_management-9.2.99/angrmanagement/data/instance.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/data/jobs/__init__.py` & `angr_management-9.2.99/angrmanagement/data/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/data/jobs/cfg_generation.py` & `angr_management-9.2.99/angrmanagement/data/jobs/cfg_generation.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/data/jobs/code_tagging.py` & `angr_management-9.2.99/angrmanagement/data/jobs/code_tagging.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/data/jobs/ddg_generation.py` & `angr_management-9.2.99/angrmanagement/data/jobs/ddg_generation.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/data/jobs/decompile_function.py` & `angr_management-9.2.99/angrmanagement/data/jobs/decompile_function.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/data/jobs/dependency_analysis.py` & `angr_management-9.2.99/angrmanagement/data/jobs/dependency_analysis.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/data/jobs/flirt_signature_recognition.py` & `angr_management-9.2.99/angrmanagement/data/jobs/flirt_signature_recognition.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/data/jobs/job.py` & `angr_management-9.2.99/angrmanagement/data/jobs/job.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/data/jobs/loading.py` & `angr_management-9.2.99/angrmanagement/data/jobs/loading.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/data/jobs/prototype_finding.py` & `angr_management-9.2.99/angrmanagement/data/jobs/prototype_finding.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/data/jobs/simgr_explore.py` & `angr_management-9.2.99/angrmanagement/data/jobs/simgr_explore.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/data/jobs/simgr_step.py` & `angr_management-9.2.99/angrmanagement/data/jobs/simgr_step.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/data/jobs/variable_recovery.py` & `angr_management-9.2.99/angrmanagement/data/jobs/variable_recovery.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/data/jobs/vfg_generation.py` & `angr_management-9.2.99/angrmanagement/data/jobs/vfg_generation.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/data/library_docs.py` & `angr_management-9.2.99/angrmanagement/data/library_docs.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/data/log.py` & `angr_management-9.2.99/angrmanagement/data/log.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/data/object_container.py` & `angr_management-9.2.99/angrmanagement/data/object_container.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/data/tagged_interval_map.py` & `angr_management-9.2.99/angrmanagement/data/tagged_interval_map.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/data/trace.py` & `angr_management-9.2.99/angrmanagement/data/trace.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/logic/__init__.py` & `angr_management-9.2.99/angrmanagement/logic/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/logic/commands/command.py` & `angr_management-9.2.99/angrmanagement/logic/commands/command.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/logic/commands/command_manager.py` & `angr_management-9.2.99/angrmanagement/logic/commands/command_manager.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/logic/debugger/bintrace.py` & `angr_management-9.2.99/angrmanagement/logic/debugger/bintrace.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/logic/debugger/debugger.py` & `angr_management-9.2.99/angrmanagement/logic/debugger/debugger.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/logic/debugger/simgr.py` & `angr_management-9.2.99/angrmanagement/logic/debugger/simgr.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/logic/disassembly/info_dock.py` & `angr_management-9.2.99/angrmanagement/logic/disassembly/info_dock.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/logic/disassembly/jump_history.py` & `angr_management-9.2.99/angrmanagement/logic/disassembly/jump_history.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/logic/singleton.py` & `angr_management-9.2.99/angrmanagement/logic/singleton.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/logic/threads.py` & `angr_management-9.2.99/angrmanagement/logic/threads.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/logic/url_scheme.py` & `angr_management-9.2.99/angrmanagement/logic/url_scheme.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/__init__.py` & `angr_management-9.2.99/angrmanagement/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/ail2asm/ail2arm32.py` & `angr_management-9.2.99/angrmanagement/plugins/ail2asm/ail2arm32.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/ail2asm/asm_output.py` & `angr_management-9.2.99/angrmanagement/plugins/ail2asm/asm_output.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/base_plugin.py` & `angr_management-9.2.99/angrmanagement/plugins/base_plugin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/binharness/bhinstance.py` & `angr_management-9.2.99/angrmanagement/plugins/binharness/bhinstance.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/binharness/binharness_plugin.py` & `angr_management-9.2.99/angrmanagement/plugins/binharness/binharness_plugin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/binharness/run_target_dialog.py` & `angr_management-9.2.99/angrmanagement/plugins/binharness/run_target_dialog.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/binharness/stream_view.py` & `angr_management-9.2.99/angrmanagement/plugins/binharness/stream_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/coverage/coverage.py` & `angr_management-9.2.99/angrmanagement/plugins/coverage/coverage.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/coverage/parse_trace.py` & `angr_management-9.2.99/angrmanagement/plugins/coverage/parse_trace.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/decompiler_poison/__init__.py` & `angr_management-9.2.99/angrmanagement/plugins/decompiler_poison/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/dep_viewer/dep_plugin.py` & `angr_management-9.2.99/angrmanagement/plugins/dep_viewer/dep_plugin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/dep_viewer/sinks.py` & `angr_management-9.2.99/angrmanagement/plugins/dep_viewer/sinks.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/execution_statistics_viewer/execution_statistics_viewer.py` & `angr_management-9.2.99/angrmanagement/plugins/execution_statistics_viewer/execution_statistics_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/load.py` & `angr_management-9.2.99/angrmanagement/plugins/load.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/memory_checker/memory_checker.py` & `angr_management-9.2.99/angrmanagement/plugins/memory_checker/memory_checker.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/plugin_description.py` & `angr_management-9.2.99/angrmanagement/plugins/plugin_description.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/plugin_manager.py` & `angr_management-9.2.99/angrmanagement/plugins/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/precise_diffing/diff_view.py` & `angr_management-9.2.99/angrmanagement/plugins/precise_diffing/diff_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/precise_diffing/function_diff.py` & `angr_management-9.2.99/angrmanagement/plugins/precise_diffing/function_diff.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/precise_diffing/precisediff_plugin.py` & `angr_management-9.2.99/angrmanagement/plugins/precise_diffing/precisediff_plugin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/precise_diffing/settings_dialog.py` & `angr_management-9.2.99/angrmanagement/plugins/precise_diffing/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/sample_plugin.py` & `angr_management-9.2.99/angrmanagement/plugins/sample_plugin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/source_importer/__init__.py` & `angr_management-9.2.99/angrmanagement/plugins/source_importer/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/source_viewer/source_viewer_plugin.py` & `angr_management-9.2.99/angrmanagement/plugins/source_viewer/source_viewer_plugin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/trace_viewer/afl_qemu_bitmap.py` & `angr_management-9.2.99/angrmanagement/plugins/trace_viewer/afl_qemu_bitmap.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/trace_viewer/multi_trace.py` & `angr_management-9.2.99/angrmanagement/plugins/trace_viewer/multi_trace.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/trace_viewer/qtrace_viewer.py` & `angr_management-9.2.99/angrmanagement/plugins/trace_viewer/qtrace_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/trace_viewer/trace_plugin.py` & `angr_management-9.2.99/angrmanagement/plugins/trace_viewer/trace_plugin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/trace_viewer/trace_statistics.py` & `angr_management-9.2.99/angrmanagement/plugins/trace_viewer/trace_statistics.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/value_search/constants.py` & `angr_management-9.2.99/angrmanagement/plugins/value_search/constants.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/value_search/qsearch_table.py` & `angr_management-9.2.99/angrmanagement/plugins/value_search/qsearch_table.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/value_search/search_view.py` & `angr_management-9.2.99/angrmanagement/plugins/value_search/search_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/value_search/value_search_plugin.py` & `angr_management-9.2.99/angrmanagement/plugins/value_search/value_search_plugin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/plugins/varec/varec.py` & `angr_management-9.2.99/angrmanagement/plugins/varec/varec.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/fonts/DejaVuSansMono.ttf` & `angr_management-9.2.99/angrmanagement/resources/fonts/DejaVuSansMono.ttf`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/fonts/SourceCodePro-Regular.ttf` & `angr_management-9.2.99/angrmanagement/resources/fonts/SourceCodePro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/images/angr-ds.png` & `angr_management-9.2.99/angrmanagement/resources/images/angr-ds.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/images/angr-splash.png` & `angr_management-9.2.99/angrmanagement/resources/images/angr-splash.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/images/angr.ico` & `angr_management-9.2.99/angrmanagement/resources/images/angr.ico`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/images/angr.png` & `angr_management-9.2.99/angrmanagement/resources/images/angr.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/images/benchmark-icon.png` & `angr_management-9.2.99/angrmanagement/resources/images/benchmark-icon.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/images/error-icon.png` & `angr_management-9.2.99/angrmanagement/resources/images/error-icon.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/images/run-icon.svg` & `angr_management-9.2.99/angrmanagement/resources/images/run-icon.svg`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/images/toolbar-docker-open.png` & `angr_management-9.2.99/angrmanagement/resources/images/toolbar-docker-open.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/images/toolbar-file-open.ico` & `angr_management-9.2.99/angrmanagement/resources/images/toolbar-file-open.ico`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/images/toolbar-file-save.png` & `angr_management-9.2.99/angrmanagement/resources/images/toolbar-file-save.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/images/toolbar-forward.png` & `angr_management-9.2.99/angrmanagement/resources/images/toolbar-forward.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/images/toolbar-previous.png` & `angr_management-9.2.99/angrmanagement/resources/images/toolbar-previous.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/images/toolbar-show-alignment.png` & `angr_management-9.2.99/angrmanagement/resources/images/toolbar-show-alignment.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/images/warning-icon.png` & `angr_management-9.2.99/angrmanagement/resources/images/warning-icon.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/themes/Catppuccin Mocha/images/close.svg` & `angr_management-9.2.99/angrmanagement/resources/themes/Catppuccin Mocha/images/close.svg`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/themes/Catppuccin Mocha/images/drawing-pin.svg` & `angr_management-9.2.99/angrmanagement/resources/themes/Catppuccin Mocha/images/drawing-pin.svg`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/themes/Dark/images/close.svg` & `angr_management-9.2.99/angrmanagement/resources/themes/Dark/images/close.svg`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/themes/Dark/images/drawing-pin.svg` & `angr_management-9.2.99/angrmanagement/resources/themes/Dark/images/drawing-pin.svg`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/themes/Dracula/images/close.svg` & `angr_management-9.2.99/angrmanagement/resources/themes/Dracula/images/close.svg`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/themes/Dracula/images/drawing-pin.svg` & `angr_management-9.2.99/angrmanagement/resources/themes/Dracula/images/drawing-pin.svg`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/themes/Light/images/close.svg` & `angr_management-9.2.99/angrmanagement/resources/themes/Light/images/close.svg`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/themes/Light/images/drawing-pin-light.svg` & `angr_management-9.2.99/angrmanagement/resources/themes/Light/images/drawing-pin-light.svg`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/themes/Light/images/drawing-pin.svg` & `angr_management-9.2.99/angrmanagement/resources/themes/Light/images/drawing-pin.svg`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/resources/themes/base.css` & `angr_management-9.2.99/angrmanagement/resources/themes/base.css`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/awesome_tooltip_event_filter.py` & `angr_management-9.2.99/angrmanagement/ui/awesome_tooltip_event_filter.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/css/__init__.py` & `angr_management-9.2.99/angrmanagement/ui/css/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/__init__.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/about.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/about.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/analysis_options.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/analysis_options.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/assemble_patch.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/assemble_patch.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/breakpoint.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/breakpoint.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/command_palette.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/command_palette.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/data_dep_graph_search.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/data_dep_graph_search.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/dependson.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/dependson.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/env_config.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/env_config.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/fs_mount.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/fs_mount.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/func_doc.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/func_doc.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/function.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/function.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/hook.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/hook.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/input_prompt.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/input_prompt.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/jumpto.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/jumpto.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/load_binary.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/load_binary.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/load_docker_prompt.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/load_docker_prompt.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/load_plugins.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/load_plugins.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/new_state.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/new_state.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/preferences.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/preferences.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/rename.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/rename.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/rename_label.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/rename_label.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/rename_node.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/rename_node.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/retype_node.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/retype_node.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/set_comment.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/set_comment.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/socket_config.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/socket_config.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/type_editor.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/type_editor.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/welcome.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/welcome.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/dialogs/xref.py` & `angr_management-9.2.99/angrmanagement/ui/dialogs/xref.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/documents/qcodedocument.py` & `angr_management-9.2.99/angrmanagement/ui/documents/qcodedocument.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/icons.py` & `angr_management-9.2.99/angrmanagement/ui/icons.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/main_window.py` & `angr_management-9.2.99/angrmanagement/ui/main_window.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/menus/analyze_menu.py` & `angr_management-9.2.99/angrmanagement/ui/menus/analyze_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/menus/disasm_insn_context_menu.py` & `angr_management-9.2.99/angrmanagement/ui/menus/disasm_insn_context_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/menus/disasm_label_context_menu.py` & `angr_management-9.2.99/angrmanagement/ui/menus/disasm_label_context_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/menus/disasm_options_menu.py` & `angr_management-9.2.99/angrmanagement/ui/menus/disasm_options_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/menus/file_menu.py` & `angr_management-9.2.99/angrmanagement/ui/menus/file_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/menus/function_context_menu.py` & `angr_management-9.2.99/angrmanagement/ui/menus/function_context_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/menus/help_menu.py` & `angr_management-9.2.99/angrmanagement/ui/menus/help_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/menus/log_menu.py` & `angr_management-9.2.99/angrmanagement/ui/menus/log_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/menus/menu.py` & `angr_management-9.2.99/angrmanagement/ui/menus/menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/menus/view_menu.py` & `angr_management-9.2.99/angrmanagement/ui/menus/view_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/toolbar_manager.py` & `angr_management-9.2.99/angrmanagement/ui/toolbar_manager.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/toolbars/debug_toolbar.py` & `angr_management-9.2.99/angrmanagement/ui/toolbars/debug_toolbar.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/toolbars/feature_map_toolbar.py` & `angr_management-9.2.99/angrmanagement/ui/toolbars/feature_map_toolbar.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/toolbars/file_toolbar.py` & `angr_management-9.2.99/angrmanagement/ui/toolbars/file_toolbar.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/toolbars/function_table_toolbar.py` & `angr_management-9.2.99/angrmanagement/ui/toolbars/function_table_toolbar.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/toolbars/nav_toolbar.py` & `angr_management-9.2.99/angrmanagement/ui/toolbars/nav_toolbar.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/toolbars/toolbar.py` & `angr_management-9.2.99/angrmanagement/ui/toolbars/toolbar.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/toolbars/toolbar_action.py` & `angr_management-9.2.99/angrmanagement/ui/toolbars/toolbar_action.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/toolbars/toolbar_dock.py` & `angr_management-9.2.99/angrmanagement/ui/toolbars/toolbar_dock.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/view_manager.py` & `angr_management-9.2.99/angrmanagement/ui/view_manager.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/views/__init__.py` & `angr_management-9.2.99/angrmanagement/ui/views/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/views/breakpoints_view.py` & `angr_management-9.2.99/angrmanagement/ui/views/breakpoints_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/views/call_explorer_view.py` & `angr_management-9.2.99/angrmanagement/ui/views/call_explorer_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/views/code_view.py` & `angr_management-9.2.99/angrmanagement/ui/views/code_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/views/console_view.py` & `angr_management-9.2.99/angrmanagement/ui/views/console_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/views/data_dep_view.py` & `angr_management-9.2.99/angrmanagement/ui/views/data_dep_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/views/dep_view.py` & `angr_management-9.2.99/angrmanagement/ui/views/dep_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/views/disassembly_view.py` & `angr_management-9.2.99/angrmanagement/ui/views/disassembly_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/views/functions_view.py` & `angr_management-9.2.99/angrmanagement/ui/views/functions_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/views/hex_view.py` & `angr_management-9.2.99/angrmanagement/ui/views/hex_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/views/interaction_view.py` & `angr_management-9.2.99/angrmanagement/ui/views/interaction_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/views/log_view.py` & `angr_management-9.2.99/angrmanagement/ui/views/log_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/views/patches_view.py` & `angr_management-9.2.99/angrmanagement/ui/views/patches_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/views/proximity_view.py` & `angr_management-9.2.99/angrmanagement/ui/views/proximity_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/views/registers_view.py` & `angr_management-9.2.99/angrmanagement/ui/views/registers_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/views/stack_view.py` & `angr_management-9.2.99/angrmanagement/ui/views/stack_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/views/states_view.py` & `angr_management-9.2.99/angrmanagement/ui/views/states_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/views/strings_view.py` & `angr_management-9.2.99/angrmanagement/ui/views/strings_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/views/symexec_view.py` & `angr_management-9.2.99/angrmanagement/ui/views/symexec_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/views/trace_map_view.py` & `angr_management-9.2.99/angrmanagement/ui/views/trace_map_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/views/traces_view.py` & `angr_management-9.2.99/angrmanagement/ui/views/traces_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/views/types_view.py` & `angr_management-9.2.99/angrmanagement/ui/views/types_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/views/view.py` & `angr_management-9.2.99/angrmanagement/ui/views/view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/__init__.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/filesystem_table.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/filesystem_table.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qaddress_input.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qaddress_input.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qast_viewer.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qast_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qblock.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qblock.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qblock_code.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qblock_code.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qblock_label.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qblock_label.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qccode_edit.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qccode_edit.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qccode_highlighter.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qccode_highlighter.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qcolor_option.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qcolor_option.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qconstraint_viewer.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qconstraint_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qdatadep_graph.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qdatadep_graph.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qdatadepgraph_block.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qdatadepgraph_block.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qdecomp_options.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qdecomp_options.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qdep_graph.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qdep_graph.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qdepgraph_block.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qdepgraph_block.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qdisasm_base_control.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qdisasm_base_control.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qdisasm_graph.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qdisasm_graph.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qdisasm_statusbar.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qdisasm_statusbar.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qfeature_map.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qfeature_map.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qfiledesc_viewer.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qfiledesc_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qfont_option.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qfont_option.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qfunction_combobox.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qfunction_combobox.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qfunction_header.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qfunction_header.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qfunction_table.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qfunction_table.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qgraph.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qgraph.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qgraph_arrow.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qgraph_arrow.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qgraph_object.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qgraph_object.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qicon_label.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qicon_label.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qinst_annotation.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qinst_annotation.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qinstruction.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qinstruction.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qipython_widget.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qipython_widget.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qlinear_viewer.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qlinear_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qlog_widget.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qlog_widget.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qmemory_data_block.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qmemory_data_block.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qmemory_viewer.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qmemory_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qminimap.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qminimap.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qoperand.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qoperand.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qpatch_table.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qpatch_table.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qpathtree.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qpathtree.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qphivariable.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qphivariable.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qproximity_graph.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qproximity_graph.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qproximitygraph_block.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qproximitygraph_block.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qregister_viewer.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qregister_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qsimulation_manager_viewer.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qsimulation_manager_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qsimulation_managers.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qsimulation_managers.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qstate_block.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qstate_block.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qstate_combobox.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qstate_combobox.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qstate_table.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qstate_table.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qstring_table.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qstring_table.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qsymexec_graph.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qsymexec_graph.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qtrace_map.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qtrace_map.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qtypedef.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qtypedef.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qunknown_block.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qunknown_block.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qvariable.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qvariable.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qvextemps_viewer.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qvextemps_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/qxref_viewer.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/qxref_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/widgets/state_inspector.py` & `angr_management-9.2.99/angrmanagement/ui/widgets/state_inspector.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/ui/workspace.py` & `angr_management-9.2.99/angrmanagement/ui/workspace.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/utils/__init__.py` & `angr_management-9.2.99/angrmanagement/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/utils/block_objects.py` & `angr_management-9.2.99/angrmanagement/utils/block_objects.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/utils/cfg.py` & `angr_management-9.2.99/angrmanagement/utils/cfg.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/utils/edge.py` & `angr_management-9.2.99/angrmanagement/utils/edge.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/utils/env.py` & `angr_management-9.2.99/angrmanagement/utils/env.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/utils/func.py` & `angr_management-9.2.99/angrmanagement/utils/func.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/utils/graph.py` & `angr_management-9.2.99/angrmanagement/utils/graph.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/utils/graph_layouter.py` & `angr_management-9.2.99/angrmanagement/utils/graph_layouter.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/utils/io.py` & `angr_management-9.2.99/angrmanagement/utils/io.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/utils/monkeypatch_stdio.py` & `angr_management-9.2.99/angrmanagement/utils/monkeypatch_stdio.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/utils/namegen.py` & `angr_management-9.2.99/angrmanagement/utils/namegen.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/utils/tree_graph_layouter.py` & `angr_management-9.2.99/angrmanagement/utils/tree_graph_layouter.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/ansi_code_processor.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/ansi_code_processor.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/base_frontend_mixin.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/base_frontend_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/bracket_matcher.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/bracket_matcher.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/call_tip_widget.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/call_tip_widget.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/client.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/client.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/comms.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/comms.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/completion_html.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/completion_html.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/completion_plain.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/completion_plain.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/completion_widget.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/completion_widget.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/console_widget.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/console_widget.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/frontend_widget.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/frontend_widget.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/history_console_widget.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/history_console_widget.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/inprocess.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/inprocess.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/jupyter_widget.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/jupyter_widget.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/kernel_mixins.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/kernel_mixins.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/kill_ring.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/kill_ring.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/mainwindow.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/mainwindow.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/manager.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/manager.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/pygments_highlighter.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/pygments_highlighter.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/qstringhelpers.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/qstringhelpers.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/qtconsoleapp.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/qtconsoleapp.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/rich_jupyter_widget.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/rich_jupyter_widget.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/rich_text.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/rich_text.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/styles.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/styles.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/svg.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/svg.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/usage.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/usage.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/angrmanagement/vendor/qtconsole/util.py` & `angr_management-9.2.99/angrmanagement/vendor/qtconsole/util.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/pyproject.toml` & `angr_management-9.2.99/pyproject.toml`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/setup.cfg` & `angr_management-9.2.99/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [options]
 packages = find:
 install_requires = 
 	PySide6>=6.4.2
 	PySide6-QtAds>=4.2.1
 	QtAwesome
 	QtPy
-	angr[angrDB]==9.2.98
+	angr[angrDB]==9.2.99
 	bidict
 	ipython
 	pyqodeng>=0.0.10
 	requests[socks]
 	tomlkit
 	pyobjc-framework-Cocoa;platform_system == "Darwin"
 	thefuzz[speedup]
@@ -49,15 +49,15 @@
 	binharness~=0.1.0
 bintrace = 
 	bintrace
 pyinstaller = 
 	pyinstaller==6.5.0
 	pillow;platform_system == "Darwin"
 	keystone-engine
-	archr==9.2.98;platform_system == "Linux"
+	archr==9.2.99;platform_system == "Linux"
 testing = 
 	pytest
 	pytest-xdist
 
 [options.package_data]
 angrmanagement = 
 	plugins/**/plugin.toml
```

### Comparing `angr-management-9.2.98/tests/test_qaddress_input.py` & `angr_management-9.2.99/tests/test_qaddress_input.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/tests/test_rename_functions.py` & `angr_management-9.2.99/tests/test_rename_functions.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/tests/test_rename_variables.py` & `angr_management-9.2.99/tests/test_rename_variables.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/tests/test_tagged_interval_map.py` & `angr_management-9.2.99/tests/test_tagged_interval_map.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/tests/test_views_open.py` & `angr_management-9.2.99/tests/test_views_open.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.98/tests/test_workflow.py` & `angr_management-9.2.99/tests/test_workflow.py`

 * *Files identical despite different names*

