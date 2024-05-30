# Comparing `tmp/codeflash-0.6.3.tar.gz` & `tmp/codeflash-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeflash-0.6.3.tar", max compression
+gzip compressed data, was "codeflash-0.6.4.tar", max compression
```

## Comparing `codeflash-0.6.3.tar` & `codeflash-0.6.4.tar`

### file list

```diff
@@ -1,59 +1,63 @@
--rw-r--r--   0        0        0       11 2024-01-05 04:36:50.272525 codeflash-0.6.3/README.md
--rw-r--r--   0        0        0     4405 2024-05-15 20:37:10.891716 codeflash-0.6.3/codeflash/LICENSE
--rw-r--r--   0        0        0        0 2024-02-13 02:11:11.085505 codeflash-0.6.3/codeflash/__init__.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.274581 codeflash-0.6.3/codeflash/api/__init__.py
--rw-r--r--   0        0        0     8992 2024-05-20 22:02:25.658457 codeflash-0.6.3/codeflash/api/aiservice.py
--rw-r--r--   0        0        0     4699 2024-05-11 03:50:31.229426 codeflash-0.6.3/codeflash/api/cfapi.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.274847 codeflash-0.6.3/codeflash/cli_cmds/__init__.py
--rw-r--r--   0        0        0     8319 2024-05-11 03:50:31.229647 codeflash-0.6.3/codeflash/cli_cmds/cli.py
--rw-r--r--   0        0        0    22865 2024-04-18 20:02:37.017426 codeflash-0.6.3/codeflash/cli_cmds/cmd_init.py
--rw-r--r--   0        0        0      440 2024-04-16 22:27:44.247326 codeflash-0.6.3/codeflash/cli_cmds/logging_config.py
--rw-r--r--   0        0        0     1827 2024-03-24 21:57:44.196107 codeflash-0.6.3/codeflash/cli_cmds/workflows/codeflash-optimize.yaml
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.275400 codeflash-0.6.3/codeflash/code_utils/__init__.py
--rw-r--r--   0        0        0     9536 2024-05-13 05:06:56.603708 codeflash-0.6.3/codeflash/code_utils/code_extractor.py
--rw-r--r--   0        0        0     8556 2024-05-13 05:06:56.603994 codeflash-0.6.3/codeflash/code_utils/code_replacer.py
--rw-r--r--   0        0        0     2956 2024-05-11 03:50:31.230947 codeflash-0.6.3/codeflash/code_utils/code_utils.py
--rw-r--r--   0        0        0      273 2024-04-15 22:14:14.315668 codeflash-0.6.3/codeflash/code_utils/compat.py
--rw-r--r--   0        0        0      224 2024-02-10 04:17:44.568348 codeflash-0.6.3/codeflash/code_utils/config_consts.py
--rw-r--r--   0        0        0     3908 2024-04-18 23:42:01.686181 codeflash-0.6.3/codeflash/code_utils/config_parser.py
--rw-r--r--   0        0        0     2880 2024-04-18 22:25:22.392531 codeflash-0.6.3/codeflash/code_utils/env_utils.py
--rw-r--r--   0        0        0     2056 2024-05-11 03:50:31.232101 codeflash-0.6.3/codeflash/code_utils/formatter.py
--rw-r--r--   0        0        0     3345 2024-05-19 03:53:17.610537 codeflash-0.6.3/codeflash/code_utils/git_utils.py
--rw-r--r--   0        0        0    23837 2024-05-19 03:53:17.611076 codeflash-0.6.3/codeflash/code_utils/instrument_existing_tests.py
--rw-r--r--   0        0        0     3497 2024-04-18 23:24:18.257591 codeflash-0.6.3/codeflash/code_utils/shell_utils.py
--rw-r--r--   0        0        0     1007 2024-01-05 04:36:50.277228 codeflash-0.6.3/codeflash/code_utils/sqlalchemy_utils.py
--rw-r--r--   0        0        0     1898 2024-05-13 05:06:56.605285 codeflash-0.6.3/codeflash/code_utils/time_utils.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.277391 codeflash-0.6.3/codeflash/discovery/__init__.py
--rw-r--r--   0        0        0    18567 2024-05-11 03:50:31.233149 codeflash-0.6.3/codeflash/discovery/discover_unit_tests.py
--rw-r--r--   0        0        0    20032 2024-05-14 17:53:59.915027 codeflash-0.6.3/codeflash/discovery/functions_to_optimize.py
--rw-r--r--   0        0        0     1291 2024-05-20 22:02:25.659212 codeflash-0.6.3/codeflash/github/PrComment.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.277833 codeflash-0.6.3/codeflash/github/__init__.py
--rw-r--r--   0        0        0      725 2024-05-07 21:23:45.633992 codeflash-0.6.3/codeflash/main.py
--rw-r--r--   0        0        0      133 2024-05-11 03:50:31.233935 codeflash-0.6.3/codeflash/models/ExperimentMetadata.py
--rw-r--r--   0        0        0        0 2024-05-11 03:50:31.233961 codeflash-0.6.3/codeflash/models/__init__.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.278392 codeflash-0.6.3/codeflash/optimization/__init__.py
--rw-r--r--   0        0        0    11999 2024-05-20 22:02:25.659613 codeflash-0.6.3/codeflash/optimization/function_context.py
--rw-r--r--   0        0        0    54363 2024-05-20 22:02:25.660170 codeflash-0.6.3/codeflash/optimization/optimizer.py
--rw-r--r--   0        0        0        0 2024-01-29 22:33:50.970495 codeflash-0.6.3/codeflash/result/__init__.py
--rw-r--r--   0        0        0     4539 2024-05-13 05:06:56.606567 codeflash-0.6.3/codeflash/result/create_pr.py
--rw-r--r--   0        0        0     1992 2024-05-13 05:06:56.607228 codeflash-0.6.3/codeflash/result/explanation.py
--rw-r--r--   0        0        0        0 2024-03-19 02:04:16.181069 codeflash-0.6.3/codeflash/telemetry/__init__.py
--rw-r--r--   0        0        0     1247 2024-04-19 00:07:03.195469 codeflash-0.6.3/codeflash/telemetry/posthog.py
--rw-r--r--   0        0        0      579 2024-03-19 02:04:16.181306 codeflash-0.6.3/codeflash/telemetry/sentry.py
--rw-r--r--   0        0        0    20467 2024-05-11 03:50:31.235086 codeflash-0.6.3/codeflash/tracer.py
--rw-r--r--   0        0        0        1 2024-05-11 03:50:31.235685 codeflash-0.6.3/codeflash/tracing/__init__.py
--rw-r--r--   0        0        0     2644 2024-05-11 03:50:31.235798 codeflash-0.6.3/codeflash/tracing/profile_stats.py
--rw-r--r--   0        0        0     5942 2024-05-11 03:50:31.235999 codeflash-0.6.3/codeflash/tracing/replay_test.py
--rw-r--r--   0        0        0      210 2024-05-09 02:05:53.366617 codeflash-0.6.3/codeflash/tracing/tracing_utils.py
--rw-r--r--   0        0        0     1905 2024-04-18 03:01:28.781529 codeflash-0.6.3/codeflash/update_license_version.py
--rw-r--r--   0        0        0        0 2024-01-20 20:41:44.799451 codeflash-0.6.3/codeflash/verification/__init__.py
--rw-r--r--   0        0        0     4977 2024-05-11 03:50:31.236508 codeflash-0.6.3/codeflash/verification/comparator.py
--rw-r--r--   0        0        0     1241 2024-05-14 17:53:59.915887 codeflash-0.6.3/codeflash/verification/equivalence.py
--rw-r--r--   0        0        0    14621 2024-05-11 03:50:31.236755 codeflash-0.6.3/codeflash/verification/parse_test_output.py
--rw-r--r--   0        0        0     6839 2024-05-19 03:53:17.612310 codeflash-0.6.3/codeflash/verification/test_results.py
--rw-r--r--   0        0        0     1852 2024-05-11 03:50:31.237506 codeflash-0.6.3/codeflash/verification/test_runner.py
--rw-r--r--   0        0        0     2338 2024-05-09 02:05:53.368797 codeflash-0.6.3/codeflash/verification/verification_utils.py
--rw-r--r--   0        0        0     4191 2024-05-20 22:02:25.660439 codeflash-0.6.3/codeflash/verification/verifier.py
--rw-r--r--   0        0        0      150 2024-05-20 22:09:46.506693 codeflash-0.6.3/codeflash/version.py
--rw-r--r--   0        0        0     2963 2024-05-20 22:09:46.505324 codeflash-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     1447 1970-01-01 00:00:00.000000 codeflash-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-01-05 03:52:06.661399 codeflash-0.6.4/README.md
+-rw-r--r--   0        0        0     4405 2024-05-30 02:49:44.753622 codeflash-0.6.4/codeflash/LICENSE
+-rw-r--r--   0        0        0        0 2024-02-12 23:19:32.441827 codeflash-0.6.4/codeflash/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-05 03:52:06.664022 codeflash-0.6.4/codeflash/api/__init__.py
+-rw-r--r--   0        0        0     8936 2024-05-23 20:37:01.092407 codeflash-0.6.4/codeflash/api/aiservice.py
+-rw-r--r--   0        0        0     4833 2024-05-29 02:22:36.999360 codeflash-0.6.4/codeflash/api/cfapi.py
+-rw-r--r--   0        0        0        0 2024-01-05 03:52:20.903968 codeflash-0.6.4/codeflash/cli_cmds/__init__.py
+-rw-r--r--   0        0        0     8062 2024-05-29 02:22:36.999766 codeflash-0.6.4/codeflash/cli_cmds/cli.py
+-rw-r--r--   0        0        0      305 2024-05-29 02:22:37.000004 codeflash-0.6.4/codeflash/cli_cmds/cli_common.py
+-rw-r--r--   0        0        0    22576 2024-05-29 02:22:37.000347 codeflash-0.6.4/codeflash/cli_cmds/cmd_init.py
+-rw-r--r--   0        0        0      475 2024-05-29 02:22:37.000790 codeflash-0.6.4/codeflash/cli_cmds/logging_config.py
+-rw-r--r--   0        0        0     1835 2024-05-29 02:22:37.000925 codeflash-0.6.4/codeflash/cli_cmds/workflows/codeflash-optimize.yaml
+-rw-r--r--   0        0        0        0 2024-01-05 03:52:06.665124 codeflash-0.6.4/codeflash/code_utils/__init__.py
+-rw-r--r--   0        0        0     9586 2024-05-30 02:48:32.417243 codeflash-0.6.4/codeflash/code_utils/code_extractor.py
+-rw-r--r--   0        0        0     8556 2024-05-23 20:36:49.437532 codeflash-0.6.4/codeflash/code_utils/code_replacer.py
+-rw-r--r--   0        0        0     2956 2024-05-23 20:36:49.437828 codeflash-0.6.4/codeflash/code_utils/code_utils.py
+-rw-r--r--   0        0        0      273 2024-03-09 01:29:18.207924 codeflash-0.6.4/codeflash/code_utils/compat.py
+-rw-r--r--   0        0        0      224 2024-02-12 23:19:32.443100 codeflash-0.6.4/codeflash/code_utils/config_consts.py
+-rw-r--r--   0        0        0     3908 2024-04-26 00:11:25.877810 codeflash-0.6.4/codeflash/code_utils/config_parser.py
+-rw-r--r--   0        0        0     2979 2024-05-23 20:36:49.438085 codeflash-0.6.4/codeflash/code_utils/env_utils.py
+-rw-r--r--   0        0        0     2056 2024-05-23 20:36:49.438180 codeflash-0.6.4/codeflash/code_utils/formatter.py
+-rw-r--r--   0        0        0     3143 2024-05-29 02:22:37.001222 codeflash-0.6.4/codeflash/code_utils/git_utils.py
+-rw-r--r--   0        0        0     1083 2024-05-29 02:22:37.001407 codeflash-0.6.4/codeflash/code_utils/github_utils.py
+-rw-r--r--   0        0        0    24003 2024-05-23 20:36:49.438744 codeflash-0.6.4/codeflash/code_utils/instrument_existing_tests.py
+-rw-r--r--   0        0        0      293 2024-05-09 02:00:12.294226 codeflash-0.6.4/codeflash/code_utils/main_calls_bubblesort.py
+-rw-r--r--   0        0        0     3497 2024-04-26 00:11:25.878498 codeflash-0.6.4/codeflash/code_utils/shell_utils.py
+-rw-r--r--   0        0        0        0 2024-05-23 20:36:49.438788 codeflash-0.6.4/codeflash/code_utils/sqlalchemy_experiment.py
+-rw-r--r--   0        0        0     1007 2024-01-05 03:52:06.666361 codeflash-0.6.4/codeflash/code_utils/sqlalchemy_utils.py
+-rw-r--r--   0        0        0     1898 2024-05-23 20:36:49.439035 codeflash-0.6.4/codeflash/code_utils/time_utils.py
+-rw-r--r--   0        0        0        0 2024-01-05 03:52:06.666515 codeflash-0.6.4/codeflash/discovery/__init__.py
+-rw-r--r--   0        0        0    18481 2024-05-23 20:36:49.439328 codeflash-0.6.4/codeflash/discovery/discover_unit_tests.py
+-rw-r--r--   0        0        0    20032 2024-05-23 20:36:49.439635 codeflash-0.6.4/codeflash/discovery/functions_to_optimize.py
+-rw-r--r--   0        0        0     1291 2024-05-23 20:36:49.439889 codeflash-0.6.4/codeflash/github/PrComment.py
+-rw-r--r--   0        0        0        0 2024-01-05 03:52:06.667045 codeflash-0.6.4/codeflash/github/__init__.py
+-rw-r--r--   0        0        0      725 2024-05-29 01:00:54.268195 codeflash-0.6.4/codeflash/main.py
+-rw-r--r--   0        0        0      133 2024-05-09 01:04:19.209290 codeflash-0.6.4/codeflash/models/ExperimentMetadata.py
+-rw-r--r--   0        0        0        0 2024-05-09 01:04:19.209321 codeflash-0.6.4/codeflash/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-05 03:52:06.667651 codeflash-0.6.4/codeflash/optimization/__init__.py
+-rw-r--r--   0        0        0    12006 2024-05-23 20:36:49.440092 codeflash-0.6.4/codeflash/optimization/function_context.py
+-rw-r--r--   0        0        0    54363 2024-05-23 20:36:49.440453 codeflash-0.6.4/codeflash/optimization/optimizer.py
+-rw-r--r--   0        0        0        0 2024-01-29 22:42:06.720542 codeflash-0.6.4/codeflash/result/__init__.py
+-rw-r--r--   0        0        0     4539 2024-05-23 20:36:49.440782 codeflash-0.6.4/codeflash/result/create_pr.py
+-rw-r--r--   0        0        0     1992 2024-05-23 20:36:49.441057 codeflash-0.6.4/codeflash/result/explanation.py
+-rw-r--r--   0        0        0        0 2024-03-19 03:48:11.207605 codeflash-0.6.4/codeflash/telemetry/__init__.py
+-rw-r--r--   0        0        0     1247 2024-04-26 00:11:25.880328 codeflash-0.6.4/codeflash/telemetry/posthog.py
+-rw-r--r--   0        0        0      579 2024-03-19 03:48:11.207884 codeflash-0.6.4/codeflash/telemetry/sentry.py
+-rw-r--r--   0        0        0    20467 2024-05-23 20:36:49.441169 codeflash-0.6.4/codeflash/tracer.py
+-rw-r--r--   0        0        0        1 2024-05-23 20:36:49.441293 codeflash-0.6.4/codeflash/tracing/__init__.py
+-rw-r--r--   0        0        0     2644 2024-05-23 20:36:49.441383 codeflash-0.6.4/codeflash/tracing/profile_stats.py
+-rw-r--r--   0        0        0     5942 2024-05-23 20:36:49.441614 codeflash-0.6.4/codeflash/tracing/replay_test.py
+-rw-r--r--   0        0        0      210 2024-04-26 00:11:25.881219 codeflash-0.6.4/codeflash/tracing/tracing_utils.py
+-rw-r--r--   0        0        0     1905 2024-04-26 00:11:25.881455 codeflash-0.6.4/codeflash/update_license_version.py
+-rw-r--r--   0        0        0        0 2024-01-19 22:35:16.406336 codeflash-0.6.4/codeflash/verification/__init__.py
+-rw-r--r--   0        0        0     4977 2024-05-09 01:04:19.210115 codeflash-0.6.4/codeflash/verification/comparator.py
+-rw-r--r--   0        0        0     1241 2024-05-23 20:36:49.441868 codeflash-0.6.4/codeflash/verification/equivalence.py
+-rw-r--r--   0        0        0    14621 2024-05-23 20:36:49.442151 codeflash-0.6.4/codeflash/verification/parse_test_output.py
+-rw-r--r--   0        0        0     6830 2024-05-23 20:36:49.442405 codeflash-0.6.4/codeflash/verification/test_results.py
+-rw-r--r--   0        0        0     1759 2024-05-23 20:36:49.442652 codeflash-0.6.4/codeflash/verification/test_runner.py
+-rw-r--r--   0        0        0     2338 2024-04-26 00:11:25.882465 codeflash-0.6.4/codeflash/verification/verification_utils.py
+-rw-r--r--   0        0        0     4189 2024-05-23 20:36:49.442883 codeflash-0.6.4/codeflash/verification/verifier.py
+-rw-r--r--   0        0        0      150 2024-05-30 02:49:52.922329 codeflash-0.6.4/codeflash/version.py
+-rw-r--r--   0        0        0     2963 2024-05-30 02:49:52.917532 codeflash-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 codeflash-0.6.4/PKG-INFO
```

### Comparing `codeflash-0.6.3/codeflash/LICENSE` & `codeflash-0.6.4/codeflash/LICENSE`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.3/codeflash/api/aiservice.py` & `codeflash-0.6.4/codeflash/api/aiservice.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,51 +1,49 @@
 from __future__ import annotations
 
 import json
 import logging
 import os
 import platform
-from typing import TYPE_CHECKING, Any, Dict, Optional, Tuple
+from typing import Any
 
 import requests
 from pydantic.dataclasses import dataclass
 from pydantic.json import pydantic_encoder
 
 from codeflash.code_utils.env_utils import get_codeflash_api_key
+from codeflash.discovery.functions_to_optimize import FunctionToOptimize
+from codeflash.models.ExperimentMetadata import ExperimentMetadata
 from codeflash.telemetry.posthog import ph
 
-if TYPE_CHECKING:
-    from codeflash.discovery.functions_to_optimize import FunctionToOptimize
-    from codeflash.models.ExperimentMetadata import ExperimentMetadata
-
 
 @dataclass(frozen=True)
 class OptimizedCandidate:
     source_code: str
     explanation: str
     optimization_id: str
 
 
 class AiServiceClient:
-    def __init__(self):
+    def __init__(self) -> None:
         self.base_url = self.get_aiservice_base_url()
         self.headers = {"Authorization": f"Bearer {get_codeflash_api_key()}"}
 
     def get_aiservice_base_url(self) -> str:
         if os.environ.get("CODEFLASH_AIS_SERVER", default="prod").lower() == "local":
             logging.info("Using local AI Service at http://localhost:8000")
             return "http://localhost:8000"
         return "https://app.codeflash.ai"
 
     def make_ai_service_request(
         self,
         endpoint: str,
         method: str = "POST",
-        payload: Optional[Dict[str, Any]] = None,
-        timeout: float = None,
+        payload: dict[str, Any] | None = None,
+        timeout: float | None = None,
     ) -> requests.Response:
         """Make an API request to the given endpoint on the AI service.
 
         :param endpoint: The endpoint to call, e.g., "/optimize".
         :param method: The HTTP method to use ('GET' or 'POST').
         :param payload: Optional JSON payload to include in the POST request body.
         :param timeout: The timeout for the request.
@@ -158,15 +156,15 @@
         function_to_optimize: FunctionToOptimize,
         helper_function_names: list[str],
         module_path: str,
         test_module_path: str,
         test_framework: str,
         test_timeout: int,
         trace_id: str,
-    ) -> Optional[Tuple[str, str]]:
+    ) -> tuple[str, str] | None:
         """Generate regression tests for the given function by making a request to the Django endpoint.
 
         Parameters
         ----------
         - source_code_being_tested (str): The source code of the function being tested.
         - function_to_optimize (FunctionToOptimize): The function to optimize.
         - helper_function_names (list[Source]): List of helper function names.
```

### Comparing `codeflash-0.6.3/codeflash/api/cfapi.py` & `codeflash-0.6.4/codeflash/api/cfapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,17 +115,21 @@
         "existingTests": existing_tests,
         "generatedTests": generated_tests,
     }
     response = make_cfapi_request(endpoint="/create-pr", method="POST", payload=payload)
     return response
 
 
-def check_github_app_installed_on_repo(owner: str, repo: str) -> Response:
+def is_github_app_installed_on_repo(owner: str, repo: str) -> bool:
     """Check if the Codeflash GitHub App is installed on the specified repository.
     :param owner: The owner of the repository.
     :param repo: The name of the repository.
     :return: The response object.
     """
-    return make_cfapi_request(
+    response = make_cfapi_request(
         endpoint=f"/is-github-app-installed?repo={repo}&owner={owner}",
         method="GET",
     )
+    if not response.ok or response.text != "true":
+        logging.error(f"Error: {response.text}")
+        return False
+    return True
```

### Comparing `codeflash-0.6.3/codeflash/cli_cmds/cli.py` & `codeflash-0.6.4/codeflash/cli_cmds/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import logging
 import os
+import sys
 from argparse import SUPPRESS, ArgumentParser, Namespace
 
 import git
 
-from codeflash.api.cfapi import check_github_app_installed_on_repo
 from codeflash.cli_cmds import logging_config
-from codeflash.cli_cmds.cmd_init import apologize_and_exit, init_codeflash
+from codeflash.cli_cmds.cli_common import apologize_and_exit
+from codeflash.cli_cmds.cmd_init import init_codeflash, install_github_actions
 from codeflash.code_utils import env_utils
-from codeflash.code_utils.compat import LF
 from codeflash.code_utils.config_parser import parse_config_file
 from codeflash.code_utils.git_utils import (
-    get_github_secrets_page_url,
     get_repo_owner_and_name,
 )
+from codeflash.code_utils.github_utils import get_github_secrets_page_url, require_github_app_or_exit
 from codeflash.version import __version__ as version
 
 
 def parse_args() -> Namespace:
     parser = ArgumentParser()
-    parser.add_argument("command", nargs="?", help="The command to run (e.g., 'init')")
+    parser.add_argument("command", nargs="*", help="The command to run (e.g., 'init' or 'init actions')")
     parser.add_argument("--file", help="Try to optimize only this file")
     parser.add_argument(
         "--function",
         help="Try to optimize only this function within the given file path",
     )
     parser.add_argument(
         "--all",
@@ -73,40 +73,53 @@
     parser.add_argument("-v", "--verbose", action="store_true", help="Print verbose debug logs")
     parser.add_argument("--version", action="store_true", help="Print the version of codeflash")
     args: Namespace = parser.parse_args()
     return process_cmd_args(args)
 
 
 def process_cmd_args(args: Namespace) -> Namespace:
+    is_init: bool = "command" in args and args.command and args.command[0] == "init"
     if args.verbose:
-        logging_config.set(logging.DEBUG)
+        logging_config.set_level(logging.DEBUG, echo_setting=not is_init)
     else:
-        logging_config.set(logging.INFO)
+        logging_config.set_level(logging.INFO, echo_setting=not is_init)
     if args.version:
         logging.info(f"Codeflash version {version}")
-        exit()
-    if "command" in args and args.command == "init":
-        init_codeflash()
-        exit()
+        sys.exit()
+
+    if is_init:
+        if args.command == ["init"]:
+            init_codeflash()
+            sys.exit()
+        if args.command == ["init", "actions"]:
+            install_github_actions()
+            sys.exit()
+        else:
+            logging.error(f"Command `{' '.join(args.command)}` not recognized")
+            sys.exit(1)
+
     if args.function and not args.file:
-        raise ValueError("If you specify a --function, you must specify the --file it is in")
+        logging.error("If you specify a --function, you must specify the --file it is in")
+        sys.exit(1)
     if args.file:
         if not os.path.exists(args.file):
-            raise ValueError(f"File {args.file} does not exist")
+            logging.error(f"File {args.file} does not exist")
+            exit(1)
         args.file = os.path.realpath(args.file)
     if args.replay_test:
         if not os.path.isfile(args.replay_test):
-            raise ValueError(f"Replay test file {args.replay_test} does not exist")
+            logging.error(f"Replay test file {args.replay_test} does not exist")
+            sys.exit(1)
         args.replay_test = os.path.realpath(args.replay_test)
 
     try:
         pyproject_config, pyproject_file_path = parse_config_file(args.config_file)
     except ValueError as e:
         logging.exception(e.args[0])
-        exit(1)
+        sys.exit(1)
     supported_keys = [
         "module_root",
         "tests_root",
         "test_framework",
         "ignore_paths",
         "minimum_performance_gain",
         "pytest_cmd",
@@ -169,27 +182,15 @@
             logging.exception(
                 "I couldn't find a git repository in the current directory. "
                 "I need a git repository to run --all and open PRs for optimizations. Exiting...",
             )
             apologize_and_exit()
         owner, repo = get_repo_owner_and_name(git_repo)
         if not args.no_pr:
-            try:
-                response = check_github_app_installed_on_repo(owner, repo)
-                if not response.ok or response.text != "true":
-                    logging.error(f"Error: {response.text}")
-                    raise Exception
-            except Exception:
-                logging.exception(
-                    f"Could not find the Codeflash GitHub App installed on the repository {owner}/{repo} or the GitHub"
-                    f" account linked to your CODEFLASH_API_KEY does not have access to the repository {owner}/{repo}.{LF}"
-                    "Please install the Codeflash GitHub App on your repository to use --all. You can install it by going to "
-                    f"https://github.com/settings/installations/{LF}",
-                )
-                apologize_and_exit()
+            require_github_app_or_exit(owner, repo)
     if not hasattr(args, "all"):
         args.all = None
     elif args.all == "":
         # The default behavior of --all is to optimize everything in args.module_root
         args.all = args.module_root
     else:
         args.all = os.path.realpath(args.all)
```

### Comparing `codeflash-0.6.3/codeflash/cli_cmds/cmd_init.py` & `codeflash-0.6.4/codeflash/cli_cmds/cmd_init.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 import ast
+import logging
 import os
 import re
 import subprocess
 import sys
 import time
-from typing import NoReturn, Optional
+from typing import Optional
 
 import click
 import inquirer
 import inquirer.themes
 import tomlkit
 from git import Repo
 from pydantic.dataclasses import dataclass
 from returns.pipeline import is_successful
 
+from codeflash.cli_cmds.cli_common import apologize_and_exit
 from codeflash.code_utils.compat import LF
+from codeflash.code_utils.config_parser import parse_config_file
 from codeflash.code_utils.env_utils import (
     get_codeflash_api_key,
 )
-from codeflash.code_utils.git_utils import get_github_secrets_page_url
+from codeflash.code_utils.git_utils import get_repo_owner_and_name
+from codeflash.code_utils.github_utils import get_github_secrets_page_url, require_github_app_or_exit
 from codeflash.code_utils.shell_utils import (
     get_shell_rc_path,
     save_api_key_to_rc,
 )
 from codeflash.telemetry.posthog import ph
 from codeflash.version import __version__ as version
 
@@ -44,27 +48,22 @@
     tests_root: str
     test_framework: str
     ignore_paths: list[str]
 
 
 def init_codeflash() -> None:
     try:
-        click.echo(CODEFLASH_LOGO)
         click.echo(f"⚡️ Welcome to Codeflash! Let's get you set up.{LF}")
 
         did_add_new_key = prompt_api_key()
 
         setup_info: SetupInfo = collect_setup_info()
 
         configure_pyproject_toml(setup_info)
 
-        prompt_github_action(setup_info)
-
-        ask_run_end_to_end_test(setup_info)  # mebbe run this after the following help text?
-
         click.echo(
             f"{LF}"
             f"⚡️ Codeflash is now set up! You can now run:{LF}"
             f"    codeflash --file <path-to-file> --function <function-name> to optimize a function within a file{LF}"
             f"    codeflash --file <path-to-file> to optimize all functions in a file{LF}"
             f"    codeflash --all to optimize all functions in all files in the module you selected ({setup_info.module_root}){LF}"
             # f"    codeflash --pr <pr-number> to optimize a PR{LF}"
@@ -130,17 +129,15 @@
 
     curdir_option = "current directory (" + curdir + ")"
     module_subdir_options = valid_module_subdirs + [curdir_option]
 
     module_root_answer = inquirer.list_input(
         message="Which Python module do you want me to optimize going forward? (Usually the top-most directory with all of your Python source code)",
         choices=module_subdir_options,
-        default=(
-            project_name if project_name in module_subdir_options else module_subdir_options[0]
-        ),
+        default=(project_name if project_name in module_subdir_options else module_subdir_options[0]),
     )
     module_root = "." if module_root_answer == curdir_option else module_root_answer
     ph("cli-project-root-provided")
 
     # Discover test directory
     default_tests_subdir = "tests"
     create_for_me_option = f"okay, create a tests{os.pathsep} directory for me!"
@@ -148,17 +145,15 @@
     custom_dir_option = "enter a custom directory..."
     test_subdir_options.append(custom_dir_option)
     tests_root_answer = inquirer.list_input(
         message="Where are your tests located? "
         f"(If you don't have any tests yet, I can create an empty tests{os.pathsep} directory for you)",
         choices=test_subdir_options,
         default=(
-            default_tests_subdir
-            if default_tests_subdir in test_subdir_options
-            else test_subdir_options[0]
+            default_tests_subdir if default_tests_subdir in test_subdir_options else test_subdir_options[0]
         ),
     )
 
     if tests_root_answer == create_for_me_option:
         tests_root = os.path.join(curdir, default_tests_subdir)
         os.mkdir(tests_root)
         click.echo(f"✅ Created directory {tests_root}{os.pathsep}{LF}")
@@ -170,28 +165,24 @@
                     message=f"Enter the path to your tests directory inside {os.path.abspath(module_root) + os.pathsep} ",
                     path_type=inquirer.Path.DIRECTORY,
                     exists=True,
                     normalize_to_absolute_path=True,
                 ),
             ],
         )
-        tests_root = (
-            custom_tests_root_answer["path"] if custom_tests_root_answer else apologize_and_exit()
-        )
+        tests_root = custom_tests_root_answer["path"] if custom_tests_root_answer else apologize_and_exit()
     else:
         tests_root = tests_root_answer
     tests_root = os.path.relpath(tests_root, curdir)
     ph("cli-tests-root-provided")
 
     # Autodiscover test framework
     autodetected_test_framework = detect_test_framework(curdir, tests_root)
     autodetected_suffix = (
-        f" (seems to me you're using {autodetected_test_framework})"
-        if autodetected_test_framework
-        else ""
+        f" (seems to me you're using {autodetected_test_framework})" if autodetected_test_framework else ""
     )
     test_framework = inquirer.list_input(
         message="Which test framework do you use?" + autodetected_suffix,
         choices=["pytest", "unittest"],
         default=autodetected_test_framework or "pytest",
         carousel=True,
     )
@@ -274,15 +265,17 @@
             click.echo("✅ I found a pyproject.toml for your project.")
             ph("cli-pyproject-toml-found")
     else:
         if os.path.exists(setup_py_path):
             with open(setup_py_path, encoding="utf8") as f:
                 setup_py_content = f.read()
             project_name_match = re.search(
-                r"setup\s*\([^)]*?name\s*=\s*['\"](.*?)['\"]", setup_py_content, re.DOTALL,
+                r"setup\s*\([^)]*?name\s*=\s*['\"](.*?)['\"]",
+                setup_py_content,
+                re.DOTALL,
             )
             if project_name_match:
                 project_name = project_name_match.group(1)
                 click.echo(f"✅ Found setup.py for your project {project_name}")
                 ph("cli-setup-py-found-name")
             else:
                 click.echo("✅ Found setup.py.")
@@ -322,99 +315,99 @@
         else:
             click.echo("⏩️ Skipping pyproject.toml creation.")
             apologize_and_exit()
     click.echo()
     return project_name
 
 
-def apologize_and_exit() -> NoReturn:
-    click.echo(
-        "💡 If you're having trouble, see https://app.codeflash.ai/app/getting-started for further help getting started with Codeflash!",
-    )
-    click.echo("👋 Exiting...")
-    sys.exit(1)
+def install_github_actions() -> None:
+    try:
+        click.echo(
+            "⚡️ Codeflash can automatically optimize new Github PRs for you when they're opened. Let's get that set up!",
+        )
+        config, config_file_path = parse_config_file()
 
+        ph("cli-github-optimization-choice", {"optimize_prs": True})
+        repo = Repo(config["module_root"], search_parent_directories=True)
+
+        owner, repo_name = get_repo_owner_and_name(repo)
+        require_github_app_or_exit(owner, repo_name)
 
-# Ask if the user wants Codeflash to optimize new GitHub PRs
-def prompt_github_action(setup_info: SetupInfo) -> None:
-    optimize_yes = inquirer.confirm(
-        message="Do you want Codeflash to automatically optimize new Github PRs when they're opened (recommended)?",
-        default=True,
-    )
-    ph("cli-github-optimization-choice", {"optimize_prs": optimize_yes})
-    if optimize_yes:
-        repo = Repo(setup_info.module_root, search_parent_directories=True)
         git_root = repo.git.rev_parse("--show-toplevel")
         workflows_path = os.path.join(git_root, ".github", "workflows")
         optimize_yaml_path = os.path.join(workflows_path, "codeflash-optimize.yaml")
 
         confirm_creation_yes = inquirer.confirm(
-            message=f"Great! I'll create a new workflow file at {optimize_yaml_path} ... is this OK?",
+            message=f"I'm going to create a new GitHub actions workflow file at {optimize_yaml_path} ... is this OK?",
             default=True,
         )
         ph(
             "cli-github-optimization-confirm-workflow-creation",
             {"confirm_creation": confirm_creation_yes},
         )
-        if confirm_creation_yes:
-            os.makedirs(workflows_path, exist_ok=True)
-            from importlib.resources import read_text
+        if not confirm_creation_yes:
+            click.echo("⏩️ Exiting workflow creation.")
+            ph("cli-github-workflow-skipped")
+            apologize_and_exit()
+        os.makedirs(workflows_path, exist_ok=True)
+        from importlib.resources import read_text
 
-            py_version = sys.version_info
-            python_version_string = f" {py_version.major}.{py_version.minor}"
+        py_version = sys.version_info
+        python_version_string = f" {py_version.major}.{py_version.minor}"
 
-            optimize_yml_content = read_text(
-                "codeflash.cli_cmds.workflows", "codeflash-optimize.yaml",
-            )
-            optimize_yml_content = optimize_yml_content.replace(
-                " {{ python_version }}", python_version_string,
-            )
-            with open(optimize_yaml_path, "w", encoding="utf8") as optimize_yml_file:
-                optimize_yml_file.write(optimize_yml_content)
-            click.echo(f"✅ Created {optimize_yaml_path}{LF}")
-            click.prompt(
-                f"Next, you'll need to add your CODEFLASH_API_KEY as a secret to your GitHub repo.{LF}"
-                + f"Press Enter to open your repo's secrets page at {get_github_secrets_page_url(repo)} ...{LF}"
-                + f"Then, click 'New repository secret' to add your api key with the variable name CODEFLASH_API_KEY.{LF}",
-                default="",
-                type=click.STRING,
-                prompt_suffix="",
-                show_default=False,
-            )
-            click.launch(get_github_secrets_page_url(repo))
-            click.echo(
-                "🐙 I opened your Github secrets page! Note: if you see a 404, you probably don't have access to this "
-                + "repo's secrets; ask a repo admin to add it for you, or (not super recommended) you can temporarily "
-                f"hard-code your api key into the workflow file.{LF}",
-            )
-            click.pause()
-            click.echo()
-            click.prompt(
-                f"Finally, for the workflow to work, you'll need to edit the workflow file to install the right "
-                f"Python version and any project dependencies.{LF}"
-                + f"Press Enter to open {optimize_yaml_path} in your editor.{LF}",
-                default="",
-                type=click.STRING,
-                prompt_suffix="",
-                show_default=False,
-            )
-            click.launch(optimize_yaml_path)
-            click.echo(
-                "📝 I opened the workflow file in your editor! You'll need to edit the steps that install the right Python "
-                + f"version and any project dependencies. See the comments in the file for more details.{LF}",
-            )
-            click.pause()
-            click.echo()
-            click.echo(
-                f"🚀 Codeflash is now configured to automatically optimize new Github PRs!{LF}",
-            )
-            ph("cli-github-workflow-created")
-        else:
-            click.echo("⏩️ Skipping GitHub workflow creation.")
-            ph("cli-github-workflow-skipped")
+        optimize_yml_content = read_text(
+            "codeflash.cli_cmds.workflows",
+            "codeflash-optimize.yaml",
+        )
+        optimize_yml_content = optimize_yml_content.replace(
+            " {{ python_version }}",
+            python_version_string,
+        )
+        with open(optimize_yaml_path, "w", encoding="utf8") as optimize_yml_file:
+            optimize_yml_file.write(optimize_yml_content)
+        click.echo(f"✅ Created {optimize_yaml_path}{LF}")
+        click.prompt(
+            f"Next, you'll need to add your CODEFLASH_API_KEY as a secret to your GitHub repo.{LF}"
+            + f"Press Enter to open your repo's secrets page at {get_github_secrets_page_url(repo)} ...{LF}"
+            + f"Then, click 'New repository secret' to add your api key with the variable name CODEFLASH_API_KEY.{LF}",
+            default="",
+            type=click.STRING,
+            prompt_suffix="",
+            show_default=False,
+        )
+        click.launch(get_github_secrets_page_url(repo))
+        click.echo(
+            "🐙 I opened your Github secrets page! Note: if you see a 404, you probably don't have access to this "
+            + "repo's secrets; ask a repo admin to add it for you, or (not super recommended) you can temporarily "
+            f"hard-code your api key into the workflow file.{LF}",
+        )
+        click.pause()
+        click.echo()
+        click.prompt(
+            f"Finally, for the workflow to work, you'll need to edit the workflow file to install the right "
+            f"Python version and any project dependencies.{LF}"
+            + f"Press Enter to open {optimize_yaml_path} in your editor.{LF}",
+            default="",
+            type=click.STRING,
+            prompt_suffix="",
+            show_default=False,
+        )
+        click.launch(optimize_yaml_path)
+        click.echo(
+            "📝 I opened the workflow file in your editor! You'll need to edit the steps that install the right Python "
+            + f"version and any project dependencies. See the comments in the file for more details.{LF}",
+        )
+        click.pause()
+        click.echo()
+        click.echo(
+            f"🚀 Codeflash is now configured to automatically optimize new Github PRs!{LF}",
+        )
+        ph("cli-github-workflow-created")
+    except KeyboardInterrupt:
+        apologize_and_exit()
 
 
 # Create or update the pyproject.toml file with the Codeflash dependency & configuration
 def configure_pyproject_toml(setup_info: SetupInfo) -> None:
     toml_path = os.path.join(os.getcwd(), "pyproject.toml")
     try:
         with open(toml_path, encoding="utf8") as pyproject_file:
```

### Comparing `codeflash-0.6.3/codeflash/cli_cmds/workflows/codeflash-optimize.yaml` & `codeflash-0.6.4/codeflash/cli_cmds/workflows/codeflash-optimize.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         with:
           python-version: {{ python_version }}
       # TODO: Replace this with your project's dependency installation method
       - name: Install Project Dependencies
         if: steps.bot_check.outputs.skip_remaining_steps == 'no'
         run: |
           python -m pip install --upgrade pip
-          pip install -r requirements.txt # TODO: Replace this with your project setup method
+        # TODO: Replace this with your project setup method
+          pip install -r requirements.txt
           pip install codeflash
       - name: Run Codeflash to optimize code
         if: steps.bot_check.outputs.skip_remaining_steps == 'no'
         id: optimize_code
         run: |
           codeflash
```

### Comparing `codeflash-0.6.3/codeflash/code_utils/code_extractor.py` & `codeflash-0.6.4/codeflash/code_utils/code_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,15 +200,18 @@
 
     name_parts = target_name.split(".")
     target_node = None
     stack: deque[ast.AST] = deque([module_node])
 
     while stack:
         node = stack.pop()
-        if isinstance(node, (ast.FunctionDef, ast.AsyncFunctionDef)) and node.name == name_parts[-1]:
+        if (
+            isinstance(node, (ast.FunctionDef, ast.AsyncFunctionDef, ast.ClassDef))
+            and node.name == name_parts[-1]
+        ):
             target_node = node
             break
         stack.extend(list(ast.iter_child_nodes(node)))
 
     if target_node is None:
         return None
```

### Comparing `codeflash-0.6.3/codeflash/code_utils/code_replacer.py` & `codeflash-0.6.4/codeflash/code_utils/code_replacer.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.3/codeflash/code_utils/code_utils.py` & `codeflash-0.6.4/codeflash/code_utils/code_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.3/codeflash/code_utils/config_parser.py` & `codeflash-0.6.4/codeflash/code_utils/config_parser.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.3/codeflash/code_utils/env_utils.py` & `codeflash-0.6.4/codeflash/code_utils/env_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,27 +60,28 @@
     if not get_pr_number():
         raise OSError(
             "CODEFLASH_PR_NUMBER not found in environment variables; make sure the Github Action is setting this so Codeflash can comment on the right PR",
         )
     return True
 
 
-def ensure_git_repo(module_root: str) -> bool:
+def ensure_git_repo(module_root: str) -> tuple[bool, bool]:
+    # return type is (should_continue, disable_PR_creation)
     try:
         _ = git.Repo(module_root, search_parent_directories=True).git_dir
-        return True
+        return True, False
     except git.exc.InvalidGitRepositoryError:
         # Only ask for the prompt if running in non-interactive mode
         if sys.__stdin__.isatty():
             response = click.prompt(
                 "I did not find a git repository for the code. If you run codeflash, it might overwrite the"
                 " code and you might irreversibly lose your current code. Proceed?",
                 type=click.Choice(["yes", "no"], case_sensitive=False),
                 show_choices=True,
             )
             if response == "no":
-                return False
+                return False, True
             if response == "yes":
-                return True
+                return True, True
         else:
             # continue running, important for GitHub actions
-            return True
+            return True, False
```

### Comparing `codeflash-0.6.3/codeflash/code_utils/formatter.py` & `codeflash-0.6.4/codeflash/code_utils/formatter.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.3/codeflash/code_utils/git_utils.py` & `codeflash-0.6.4/codeflash/code_utils/git_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,15 +80,10 @@
     repo_owner_with_github, repo_name = split_url[-2], split_url[-1]
     repo_owner = (
         repo_owner_with_github.split(":")[1] if ":" in repo_owner_with_github else repo_owner_with_github
     )
     return repo_owner, repo_name
 
 
-def get_github_secrets_page_url(repo: Optional[Repo] = None) -> str:
-    owner, repo_name = get_repo_owner_and_name(repo)
-    return f"https://github.com/{owner}/{repo_name}/settings/secrets/actions"
-
-
 def git_root_dir(repo: Optional[Repo] = None) -> str:
     repository: Repo = repo if repo else git.Repo(search_parent_directories=True)
     return repository.working_dir
```

### Comparing `codeflash-0.6.3/codeflash/code_utils/instrument_existing_tests.py` & `codeflash-0.6.4/codeflash/code_utils/instrument_existing_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from __future__ import annotations
 
 import ast
 import logging
 from typing import Iterable
 
+import isort
+
 from codeflash.code_utils.code_utils import get_run_tmp_file, module_name_from_file_path
 
 
 class ReplaceCallNodeWithName(ast.NodeTransformer):
     def __init__(self, only_function_name: str, new_variable_name: str = "codeflash_return_value") -> None:
         self.only_function_name = only_function_name
         self.new_variable_name = new_variable_name
 
     def visit_Call(self, node: ast.Call) -> ast.Name | ast.Call:
         if isinstance(node, ast.Call):
+            function_name: str = ""
             if hasattr(node.func, "id"):
                 function_name = node.func.id
 
             if hasattr(node.func, "attr"):
                 function_name = node.func.attr
 
             if hasattr(node.func, "value") and hasattr(node.func.value, "id"):
@@ -33,21 +36,21 @@
 class InjectPerfOnly(ast.NodeTransformer):
     def __init__(self, function_name: str, module_path: str) -> None:
         self.only_function_name = function_name
         self.module_path = module_path
 
     def update_line_node(
         self,
-        test_node: ast.AST,
+            test_node: ast.stmt,
         node_name: str,
         index: str,
         test_class_name: str | None = None,
     ) -> Iterable[ast.stmt]:
         call_node = None
-        function_name = ""
+        function_name: str = ""
         for node in ast.walk(test_node):
             if isinstance(node, ast.Call):
                 if hasattr(node.func, "id"):
                     function_name = node.func.id
 
                 if hasattr(node.func, "attr"):
                     function_name = node.func.attr
@@ -94,30 +97,31 @@
         updated_nodes.append(subbed_node)
         return updated_nodes
 
     def is_target_function_line(self, line_node: ast.AST) -> bool:
         node: ast.AST
         for node in ast.walk(line_node):
             if isinstance(node, ast.Call):
+                function_name: str = ""
                 if hasattr(node.func, "id"):
-                    function_name: str = node.func.id
+                    function_name = node.func.id
 
                 if hasattr(node.func, "attr"):
                     function_name = node.func.attr
 
                 if hasattr(node.func, "value") and hasattr(node.func.value, "id"):
                     function_name = node.func.value.id + "." + function_name
 
                 if function_name == self.only_function_name:
                     return True
 
         return False
 
     def visit_ClassDef(self, node: ast.ClassDef) -> ast.ClassDef:
-        # TODO: Ensure that this class inherits from unittest.TestCase. Don't modify non unittest.TestCase classes
+        # TODO: Ensure that this class inherits from unittest.TestCase. Don't modify non unittest.TestCase classes.
         for inner_node in ast.walk(node):
             if isinstance(inner_node, ast.FunctionDef):
                 self.visit_FunctionDef(inner_node, node.name)
 
         return node
 
     def visit_FunctionDef(self, node: ast.FunctionDef, test_class_name: str | None = None) -> ast.FunctionDef:
@@ -224,15 +228,15 @@
 
                 if isinstance(line_node, (ast.With, ast.For, ast.While)):
                     j = len(line_node.body) - 1
                     while j >= 0:
                         compound_line_node: ast.stmt = line_node.body[j]
                         internal_node: ast.AST
                         for internal_node in ast.walk(compound_line_node):
-                            if self.is_target_function_line(internal_node):
+                            if isinstance(internal_node, ast.stmt) and self.is_target_function_line(internal_node):
                                 line_node.body[j : j + 1] = self.update_line_node(
                                     internal_node,
                                     node.name,
                                     str(i) + "_" + str(j),
                                     test_class_name,
                                 )
                                 break
@@ -296,16 +300,15 @@
         ast.Import(names=[ast.alias(name="time")]),
         ast.Import(names=[ast.alias(name="gc")]),
         ast.Import(names=[ast.alias(name="os")]),
         ast.Import(names=[ast.alias(name="sqlite3")]),
         ast.Import(names=[ast.alias(name="dill", asname="pickle")]),
     ]
     tree.body = [*new_imports, create_wrapper_function(), *tree.body]
-
-    return True, ast.unparse(tree)
+    return True, isort.code(ast.unparse(tree), float_to_top=True)
 
 
 def create_wrapper_function() -> ast.FunctionDef:
     lineno = 1
     return ast.FunctionDef(
         name="codeflash_wrap",
         args=ast.arguments(
```

### Comparing `codeflash-0.6.3/codeflash/code_utils/shell_utils.py` & `codeflash-0.6.4/codeflash/code_utils/shell_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.3/codeflash/code_utils/sqlalchemy_utils.py` & `codeflash-0.6.4/codeflash/code_utils/sqlalchemy_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.3/codeflash/code_utils/time_utils.py` & `codeflash-0.6.4/codeflash/code_utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.3/codeflash/discovery/discover_unit_tests.py` & `codeflash-0.6.4/codeflash/discovery/discover_unit_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,17 +311,15 @@
             indices = [i for i, x in enumerate(test_functions_raw) if x == scope]
             for index in indices:
                 scope_test_function = test_functions_list[index].function_name
                 scope_test_suite = test_functions_list[index].test_suite_name
                 scope_parameters = test_functions_list[index].parameters
                 test_type = test_functions_list[index].test_type
                 try:
-                    definition = script.goto(
-                        line=name.line,
-                        column=name.column,
+                    definition = name.goto(
                         follow_imports=True,
                         follow_builtin_imports=False,
                     )
                 except Exception as e:
                     logging.exception(str(e))
                     continue
                 if definition and definition[0].type == "function":
```

### Comparing `codeflash-0.6.3/codeflash/discovery/functions_to_optimize.py` & `codeflash-0.6.4/codeflash/discovery/functions_to_optimize.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.3/codeflash/github/PrComment.py` & `codeflash-0.6.4/codeflash/github/PrComment.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.3/codeflash/main.py` & `codeflash-0.6.4/codeflash/main.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.3/codeflash/optimization/function_context.py` & `codeflash-0.6.4/codeflash/optimization/function_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
                         ),
                     ],
                 )[0]
                 if source_code:
                     sources.append(
                         (
                             Source(
-                                definition[0].name,
+                                definition[0].full_name,
                                 definition[0],
                                 source_code,
                             ),
                             definition_path,
                             definition[0].full_name.removeprefix(
                                 definition[0].module_name + ".",
                             ),
@@ -273,10 +273,10 @@
     logging.debug(f"ALL DEPENDENCIES TOKENS LENGTH: {sum(helper_functions_tokens)}")
     for function_source, source_len in zip(helper_functions_sources, helper_functions_tokens):
         if context_len + source_len <= max_tokens:
             context_list.append(function_source)
             context_len += source_len
         else:
             break
-    logging.debug("FINAL OPTIMIZATION CONTEXT TOKENS LENGTH:", context_len)
+    logging.debug(f"FINAL OPTIMIZATION CONTEXT TOKENS LENGTH: {context_len}")
     helper_code: str = "\n".join(context_list)
     return helper_code, helper_functions
```

### Comparing `codeflash-0.6.3/codeflash/optimization/optimizer.py` & `codeflash-0.6.4/codeflash/optimization/optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 import os
 import pathlib
 import sys
 import uuid
 from argparse import Namespace
 from collections import defaultdict
-from typing import List, Optional, Tuple, Union
+from typing import Optional
 
 import isort
 import libcst as cst
 from pydantic import BaseModel
 from returns.pipeline import is_successful
 from returns.result import Failure, Result, Success
 
@@ -127,17 +127,20 @@
         self.instrumented_unittests_created: set[str] = set()
 
     def run(self) -> None:
         ph("cli-optimize-run-start")
         logging.info("Running optimizer.")
         if not env_utils.ensure_codeflash_api_key():
             return
-        if not env_utils.ensure_git_repo(module_root=self.args.module_root):
+        continue_execution, disable_pr = env_utils.ensure_git_repo(module_root=self.args.module_root)
+        if not continue_execution:
             logging.error("No git repository detected and user aborted run. Exiting...")
             sys.exit(1)
+        if disable_pr:
+            self.args.no_pr = True
 
         file_to_funcs_to_optimize: dict[str, list[FunctionToOptimize]]
         num_optimizable_functions: int
 
         (
             file_to_funcs_to_optimize,
             num_optimizable_functions,
@@ -761,16 +764,14 @@
         code_to_optimize_with_helpers: str,
         function_to_optimize: FunctionToOptimize,
         helper_functions: list[tuple[Source, str, str]],
         module_path: str,
         function_trace_id: str,
         run_experiment: bool = False,
     ) -> Result[tuple[GeneratedTests, OptimizationSet], str]:
-        generated_original_test_source = None
-        instrumented_test_source = None
         max_workers = 2 if not run_experiment else 3
         with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
             future_tests = executor.submit(
                 self.generate_and_instrument_tests,
                 code_to_optimize_with_helpers,
                 function_to_optimize,
                 [definition[0].full_name for definition in helper_functions],
@@ -975,15 +976,15 @@
         optimization_index: int,
         instrumented_unittests_created_for_function: set[str],
         overall_original_test_results: TestResults,
         original_existing_test_results: TestResults,
         original_generated_test_results: TestResults,
         generated_tests_path: str,
         best_runtime_until_now: int,
-        tests_in_file: Optional[List[TestsInFile]],
+        tests_in_file: list[TestsInFile] | None,
         run_generated_tests: bool,
     ) -> Result[OptimizedCandidateResult, str]:
         success = True
         best_test_runtime = None
         best_test_results = None
         equal_results = True
         generated_tests_elapsed_time = 0.0
@@ -1145,15 +1146,15 @@
 
     def run_and_parse_tests(
         self,
         test_env: dict[str, str],
         test_file: str,
         test_type: TestType,
         optimization_iteration: int,
-        test_function: Optional[str] = None,
+        test_function: str | None = None,
     ) -> TestResults:
         result_file_path, run_result = run_tests(
             test_file,
             test_framework=self.args.test_framework,
             cwd=self.args.project_root,
             pytest_timeout=INDIVIDUAL_TEST_TIMEOUT,
             pytest_cmd=self.test_cfg.pytest_cmd,
@@ -1180,15 +1181,15 @@
     def generate_and_instrument_tests(
         self,
         source_code_being_tested: str,
         function_to_optimize: FunctionToOptimize,
         helper_function_names: list[str],
         module_path: str,
         function_trace_id: str,
-    ) -> Union[Tuple[str, str], None]:
+    ) -> tuple[str, str] | None:
         tests = generate_tests(
             self.aiservice_client,
             source_code_being_tested=source_code_being_tested,
             function_to_optimize=function_to_optimize,
             helper_function_names=helper_function_names,
             module_path=module_path,
             test_cfg=self.test_cfg,
```

### Comparing `codeflash-0.6.3/codeflash/result/create_pr.py` & `codeflash-0.6.4/codeflash/result/create_pr.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.3/codeflash/result/explanation.py` & `codeflash-0.6.4/codeflash/result/explanation.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.3/codeflash/telemetry/posthog.py` & `codeflash-0.6.4/codeflash/telemetry/posthog.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.3/codeflash/telemetry/sentry.py` & `codeflash-0.6.4/codeflash/telemetry/sentry.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.3/codeflash/tracer.py` & `codeflash-0.6.4/codeflash/tracer.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.3/codeflash/tracing/profile_stats.py` & `codeflash-0.6.4/codeflash/tracing/profile_stats.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.3/codeflash/tracing/replay_test.py` & `codeflash-0.6.4/codeflash/tracing/replay_test.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.3/codeflash/update_license_version.py` & `codeflash-0.6.4/codeflash/update_license_version.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.3/codeflash/verification/comparator.py` & `codeflash-0.6.4/codeflash/verification/comparator.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.3/codeflash/verification/equivalence.py` & `codeflash-0.6.4/codeflash/verification/equivalence.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.3/codeflash/verification/parse_test_output.py` & `codeflash-0.6.4/codeflash/verification/parse_test_output.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.3/codeflash/verification/test_results.py` & `codeflash-0.6.4/codeflash/verification/test_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import logging
 import sys
 from enum import Enum
-from typing import Iterator, List, Optional
+from typing import Iterator, Optional
 
 from pydantic import BaseModel
 from pydantic.dataclasses import dataclass
 
 from codeflash.verification.comparator import comparator
 
 
@@ -67,29 +67,29 @@
     runtime: Optional[int]  # Time in nanoseconds
     test_framework: str  # unittest or pytest
     test_type: TestType
     return_value: Optional[object]  # The return value of the function invocation
 
 
 class TestResults(BaseModel):
-    test_results: List[FunctionTestInvocation] = []
+    test_results: list[FunctionTestInvocation] = []
 
     def add(self, function_test_invocation: FunctionTestInvocation) -> None:
         self.test_results.append(function_test_invocation)
 
     def merge(self, other: TestResults) -> None:
         self.test_results.extend(other.test_results)
 
     def get_by_id(
         self,
         invocation_id: InvocationId,
-    ) -> Optional[FunctionTestInvocation]:
+    ) -> FunctionTestInvocation | None:
         return next((r for r in self.test_results if r.id == invocation_id), None)
 
-    def get_all_ids(self) -> List[InvocationId]:
+    def get_all_ids(self) -> list[InvocationId]:
         return [test_result.id for test_result in self.test_results]
 
     def get_test_pass_fail_report(self) -> str:
         passed = 0
         failed = 0
         for test_result in self.test_results:
             if test_result.did_pass:
```

### Comparing `codeflash-0.6.3/codeflash/verification/test_runner.py` & `codeflash-0.6.4/codeflash/verification/test_runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
+from __future__ import annotations
+
 import subprocess
-from typing import Optional, Tuple
 
 from codeflash.code_utils.code_utils import get_run_tmp_file
 
 
 def run_tests(
     test_path: str,
     test_framework: str,
-    cwd: Optional[str] = None,
-    test_env: Optional[dict[str, str]] = None,
-    pytest_timeout: Optional[int] = None,
+    cwd: str | None = None,
+    test_env: dict[str, str] | None = None,
+    pytest_timeout: int | None = None,
     pytest_cmd: str = "pytest",
     verbose: bool = False,
-    only_run_this_test_function: Optional[str] = None,
-) -> Tuple[str, subprocess.CompletedProcess]:
+    only_run_this_test_function: str | None = None,
+) -> tuple[str, subprocess.CompletedProcess]:
     assert test_framework in ["pytest", "unittest"]
     if only_run_this_test_function and "__replay_test" in test_path:
         test_path = test_path + "::" + only_run_this_test_function
 
     if test_framework == "pytest":
         result_file_path = get_run_tmp_file("pytest_results.xml")
         pytest_cmd_list = [chunk for chunk in pytest_cmd.split(" ") if chunk != ""]
@@ -25,30 +26,28 @@
             pytest_cmd_list
             + [
                 test_path,
                 "-q",
                 f"--timeout={pytest_timeout}",
                 f"--junitxml={result_file_path}",
             ],
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
+            capture_output=True,
             cwd=cwd,
             env=test_env,
-            check=False,
+            text=True,
             timeout=600,
         )
     elif test_framework == "unittest":
         result_file_path = get_run_tmp_file("unittest_results.xml")
         results = subprocess.run(
             ["python", "-m", "xmlrunner"]
             + (["-v"] if verbose else [])
             + [test_path]
             + ["--output-file", result_file_path],
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
+            capture_output=True,
             cwd=cwd,
             env=test_env,
-            check=False,
+            text=True,
         )
     else:
         raise ValueError("Invalid test framework -- I only support Pytest and Unittest currently.")
     return result_file_path, results
```

### Comparing `codeflash-0.6.3/codeflash/verification/verification_utils.py` & `codeflash-0.6.4/codeflash/verification/verification_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.3/codeflash/verification/verifier.py` & `codeflash-0.6.4/codeflash/verification/verifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from __future__ import annotations
+
 import ast
 import logging
-from typing import Optional, Tuple
 
 from codeflash.api.aiservice import AiServiceClient
 from codeflash.code_utils.code_utils import get_run_tmp_file, module_name_from_file_path
 from codeflash.discovery.functions_to_optimize import FunctionToOptimize
 from codeflash.verification.verification_utils import (
     ModifyInspiredTests,
     TestConfig,
@@ -19,15 +20,15 @@
     function_to_optimize: FunctionToOptimize,
     helper_function_names: list[str],
     module_path: str,
     test_cfg: TestConfig,
     test_timeout: int,
     use_cached_tests: bool,
     function_trace_id: str,
-) -> Optional[Tuple[str, str]]:
+) -> tuple[str, str] | None:
     # TODO: Sometimes this recreates the original Class definition. This overrides and messes up the original
     #  class import. Remove the recreation of the class definition
     logging.info(f"Generating new tests for function {function_to_optimize.function_name} ...")
     if use_cached_tests:
         import importlib
 
         module = importlib.import_module(module_path)
```

### Comparing `codeflash-0.6.3/pyproject.toml` & `codeflash-0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "codeflash"
-version = "0.6.3" # Determined by poetry-dynamic-versioning during `poetry build`
+version = "0.6.4" # Determined by poetry-dynamic-versioning during `poetry build`
 description = "Client for codeflash.ai - automatic code performance optimization, powered by AI"
 license = "BSL-1.1"
 authors = ["CodeFlash Inc. <contact@codeflash.ai>"]
 homepage = "https://codeflash.ai"
 readme = "README.md"
 packages = [
     { include = "codeflash" },
```

### Comparing `codeflash-0.6.3/PKG-INFO` & `codeflash-0.6.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: codeflash
-Version: 0.6.3
+Version: 0.6.4
 Summary: Client for codeflash.ai - automatic code performance optimization, powered by AI
 Home-page: https://codeflash.ai
 License: BSL-1.1
 Keywords: codeflash,performance,optimization,ai,code,machine learning,LLM
 Author: CodeFlash Inc.
 Author-email: contact@codeflash.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: black (>=22.3.0)
 Requires-Dist: click (>=8.1.0)
 Requires-Dist: dill (>=0.3.8,<0.4.0)
 Requires-Dist: gitpython (>=3.1.31)
 Requires-Dist: humanize (>=4.0.0)
 Requires-Dist: inquirer (>=3.0.0)
 Requires-Dist: isort (>=5.11.0)
```

