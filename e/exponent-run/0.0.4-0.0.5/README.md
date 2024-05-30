# Comparing `tmp/exponent_run-0.0.4.tar.gz` & `tmp/exponent_run-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exponent_run-0.0.4.tar", max compression
+gzip compressed data, was "exponent_run-0.0.5.tar", max compression
```

## Comparing `exponent_run-0.0.4.tar` & `exponent_run-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0       57 2024-05-03 23:47:20.021413 exponent_run-0.0.4/exponent/__init__.py
--rw-r--r--   0        0        0     7325 2024-05-18 22:21:15.560183 exponent_run-0.0.4/exponent/cli.py
--rw-r--r--   0        0        0     1727 2024-05-14 23:30:22.001306 exponent_run-0.0.4/exponent/core/config.py
--rw-r--r--   0        0        0     5548 2024-05-19 02:03:41.245790 exponent_run-0.0.4/exponent/core/remote_execution/client.py
--rw-r--r--   0        0        0     1508 2024-05-19 02:03:41.246067 exponent_run-0.0.4/exponent/core/remote_execution/code_execution.py
--rw-r--r--   0        0        0     3440 2024-05-17 09:30:56.979279 exponent_run-0.0.4/exponent/core/remote_execution/files.py
--rw-r--r--   0        0        0     1254 2024-05-17 07:50:43.085085 exponent_run-0.0.4/exponent/core/remote_execution/languages/diff.py
--rw-r--r--   0        0        0     4428 2024-05-15 21:47:37.236001 exponent_run-0.0.4/exponent/core/remote_execution/languages/python.py
--rw-r--r--   0        0        0      555 2024-05-18 00:30:25.944494 exponent_run-0.0.4/exponent/core/remote_execution/languages/shell.py
--rw-r--r--   0        0        0      578 2024-05-15 21:47:37.236935 exponent_run-0.0.4/exponent/core/remote_execution/session.py
--rw-r--r--   0        0        0      952 2024-05-15 21:47:37.238191 exponent_run-0.0.4/exponent/core/remote_execution/system_context.py
--rw-r--r--   0        0        0     4574 2024-05-19 02:03:41.246350 exponent_run-0.0.4/exponent/core/remote_execution/types.py
--rw-r--r--   0        0        0     8685 2024-05-19 02:03:41.246483 exponent_run-0.0.4/exponent/core/remote_execution/utils.py
--rw-r--r--   0        0        0        0 2024-05-03 23:47:19.960349 exponent_run-0.0.4/exponent/tests/__init__.py
--rw-r--r--   0        0        0     1719 2024-05-14 18:25:03.436018 exponent_run-0.0.4/exponent/tests/conftest.py
--rw-r--r--   0        0        0    11284 2024-05-17 09:35:45.870376 exponent_run-0.0.4/exponent/tests/test_cli.py
--rw-r--r--   0        0        0     1563 2024-05-20 23:52:54.688326 exponent_run-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      748 1970-01-01 00:00:00.000000 exponent_run-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       57 2024-05-03 23:47:20.021413 exponent_run-0.0.5/exponent/__init__.py
+-rw-r--r--   0        0        0     7496 2024-05-29 15:08:28.825877 exponent_run-0.0.5/exponent/cli.py
+-rw-r--r--   0        0        0     2062 2024-05-29 15:08:28.828783 exponent_run-0.0.5/exponent/core/config.py
+-rw-r--r--   0        0        0     6118 2024-05-29 15:08:28.833415 exponent_run-0.0.5/exponent/core/remote_execution/client.py
+-rw-r--r--   0        0        0     1508 2024-05-21 03:07:44.004550 exponent_run-0.0.5/exponent/core/remote_execution/code_execution.py
+-rw-r--r--   0        0        0     3440 2024-05-21 03:07:44.004699 exponent_run-0.0.5/exponent/core/remote_execution/files.py
+-rw-r--r--   0        0        0     1119 2024-05-29 15:08:28.833779 exponent_run-0.0.5/exponent/core/remote_execution/git.py
+-rw-r--r--   0        0        0     1254 2024-05-17 07:50:43.085085 exponent_run-0.0.5/exponent/core/remote_execution/languages/diff.py
+-rw-r--r--   0        0        0     5573 2024-05-29 15:08:28.838366 exponent_run-0.0.5/exponent/core/remote_execution/languages/python.py
+-rw-r--r--   0        0        0      555 2024-05-21 03:07:44.004852 exponent_run-0.0.5/exponent/core/remote_execution/languages/shell.py
+-rw-r--r--   0        0        0      578 2024-05-15 21:47:37.236935 exponent_run-0.0.5/exponent/core/remote_execution/session.py
+-rw-r--r--   0        0        0     1225 2024-05-29 15:08:28.838630 exponent_run-0.0.5/exponent/core/remote_execution/system_context.py
+-rw-r--r--   0        0        0     5532 2024-05-29 15:08:28.843112 exponent_run-0.0.5/exponent/core/remote_execution/types.py
+-rw-r--r--   0        0        0     9098 2024-05-29 15:08:28.848036 exponent_run-0.0.5/exponent/core/remote_execution/utils.py
+-rw-r--r--   0        0        0        0 2024-05-03 23:47:19.960349 exponent_run-0.0.5/exponent/tests/__init__.py
+-rw-r--r--   0        0        0     2644 2024-05-29 15:08:28.853461 exponent_run-0.0.5/exponent/tests/conftest.py
+-rw-r--r--   0        0        0    13100 2024-05-29 15:08:28.858182 exponent_run-0.0.5/exponent/tests/test_cli.py
+-rw-r--r--   0        0        0     1303 2024-05-29 15:08:28.860063 exponent_run-0.0.5/exponent/tests/utils.py
+-rw-r--r--   0        0        0     1576 2024-05-30 05:42:09.651678 exponent_run-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 exponent_run-0.0.5/PKG-INFO
```

### Comparing `exponent_run-0.0.4/exponent/cli.py` & `exponent_run-0.0.5/exponent/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,31 +60,38 @@
 @click.option(
     "--prod",
     is_flag=True,
     hidden=True,
     help="Use production URLs even if in editable mode",
 )
 @click.option(
+    "--staging",
+    is_flag=True,
+    hidden=True,
+    help="Use staging URLs even if in editable mode",
+)
+@click.option(
     "--prompt",
     help="Start a chat with a given prompt.",
 )
 @click.option(
     "--benchmark",
     is_flag=True,
     help="Enable benchmarking mode",
 )
 def run(
     chat_id: str | None = None,
     prod: bool = False,
+    staging: bool = False,
     prompt: str | None = None,
     benchmark: bool = False,
 ) -> None:
     chat_uuid = chat_id
 
-    settings = get_settings(use_prod=prod)
+    settings = get_settings(use_prod=prod, use_staging=staging)
     if is_editable_install() and not prod:
         click.secho(
             "Detected local editable install, using local URLs", fg="yellow", bold=True
         )
         click.secho("- base_url=", fg="yellow", bold=True, nl=False)
         click.secho(f"{settings.base_url}", fg=(100, 200, 255), bold=False)
         click.secho("- base_api_url=", fg="yellow", bold=True, nl=False)
```

### Comparing `exponent_run-0.0.4/exponent/core/config.py` & `exponent_run-0.0.5/exponent/core/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -49,14 +49,20 @@
         env_prefix="EXPONENT_",
         env_file=os.path.expanduser("~/.exponent"),
         case_sensitive=False,
     )
 
 
 @lru_cache(maxsize=1)
-def get_settings(use_prod: bool = False) -> Settings:
-    if is_editable_install() and not use_prod:
-        return Settings(
-            base_url="http://localhost:3000", base_api_url="http://localhost:8000"
-        )
+def get_settings(use_prod: bool = False, use_staging: bool = False) -> Settings:
+    if is_editable_install() and not (use_prod or use_staging):
+        base_url = "http://localhost:3000"
+        base_api_url = "http://localhost:8000"
+    elif use_staging:
+        # TODO: Change this to a real staging URL?
+        base_url = "https://exponent.run"
+        base_api_url = "https://staging-api.exponent.run"
+    else:
+        base_url = "https://exponent.run"
+        base_api_url = "https://api.exponent.run"
 
-    return Settings()
+    return Settings(base_url=base_url, base_api_url=base_api_url)
```

### Comparing `exponent_run-0.0.4/exponent/core/remote_execution/client.py` & `exponent_run-0.0.5/exponent/core/remote_execution/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 import json
 import logging
 from collections.abc import AsyncGenerator
 from contextlib import asynccontextmanager
 
-from httpx import AsyncClient
+from httpx import (
+    AsyncClient,
+    codes as http_status,
+)
 
-from exponent.core.remote_execution import files
+from exponent.core.remote_execution import files, git, system_context
 from exponent.core.remote_execution.code_execution import execute_code
 from exponent.core.remote_execution.session import (
     RemoteExecutionClientSession,
     get_session,
 )
-from exponent.core.remote_execution.system_context import get_system_context
 from exponent.core.remote_execution.types import (
     CLIConnectedState,
     CodeExecutionRequest,
     CreateChatResponse,
     ExecutionEndResponse,
+    GetAllTrackedFilesRequest,
     GetFileContentsRequest,
     GetMatchingFilesRequest,
+    HeartbeatInfo,
     ListFilesRequest,
     RemoteExecutionRequestType,
     RemoteExecutionResponse,
     StartChatRequest,
     StartChatResponse,
     SystemContextRequest,
     UseToolsConfig,
@@ -109,20 +113,28 @@
                 ).model_dump(),
                 timeout=60,
             )
         return StartChatResponse(**response.json())
 
     async def send_heartbeat(self, chat_uuid: str) -> CLIConnectedState:
         logger.info(f"Sending heartbeat for chat_uuid {chat_uuid}")
+        heartbeat_info = HeartbeatInfo(
+            system_info=system_context.get_system_info(self.working_directory),
+        )
         async with AsyncClient() as client:
             response = await client.post(
                 f"{self.base_url}/api/remote_execution/{chat_uuid}/heartbeat",
                 headers=self.headers,
+                content=heartbeat_info.model_dump_json(),
                 timeout=60,
             )
+        if response.status_code != http_status.OK:
+            raise Exception(
+                f"Heartbeat failed with status code {response.status_code} and response {response.text}"
+            )
         connected_state = CLIConnectedState(**response.json())
         logger.info(f"Heartbeat response: {connected_state}")
         return connected_state
 
     async def handle_request(
         self, request: RemoteExecutionRequestType
     ) -> RemoteExecutionResponse:
@@ -133,15 +145,17 @@
         elif isinstance(request, ListFilesRequest):
             return files.list_files(request)
         elif isinstance(request, GetFileContentsRequest):
             return files.get_file_contents(request, self.working_directory)
         elif isinstance(request, GetMatchingFilesRequest):
             return files.get_matching_files(request, self.file_cache)
         elif isinstance(request, SystemContextRequest):
-            return get_system_context(request, self.working_directory)
+            return system_context.get_system_context(request, self.working_directory)
+        elif isinstance(request, GetAllTrackedFilesRequest):
+            return git.get_all_tracked_files(request, self.working_directory)
 
     @staticmethod
     @asynccontextmanager
     async def session(
         api_key: str, base_url: str, working_directory: str
     ) -> AsyncGenerator["RemoteExecutionClient", None]:
         async with get_session(api_key, base_url, working_directory) as session:
```

### Comparing `exponent_run-0.0.4/exponent/core/remote_execution/code_execution.py` & `exponent_run-0.0.5/exponent/core/remote_execution/code_execution.py`

 * *Files identical despite different names*

### Comparing `exponent_run-0.0.4/exponent/core/remote_execution/files.py` & `exponent_run-0.0.5/exponent/core/remote_execution/files.py`

 * *Files identical despite different names*

### Comparing `exponent_run-0.0.4/exponent/core/remote_execution/languages/diff.py` & `exponent_run-0.0.5/exponent/core/remote_execution/languages/diff.py`

 * *Files identical despite different names*

### Comparing `exponent_run-0.0.4/exponent/core/remote_execution/languages/python.py` & `exponent_run-0.0.5/exponent/core/remote_execution/languages/python.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import asyncio
 import logging
 import queue
 import re
+import subprocess
 import threading
 import time
 from typing import Any
 
 from jupyter_client.client import KernelClient
 from jupyter_client.manager import KernelManager
 
+from exponent.core.remote_execution.types import PythonEnvInfo
+
 logger = logging.getLogger(__name__)
 
 
 class IOChannelHandler:
     ESCAPE_SEQUENCE = re.compile(r"\x1B\[[0-?]*[ -/]*[@-~]")
 
     def __init__(self) -> None:
@@ -124,7 +127,47 @@
         if self._manager:
             self._manager.shutdown_kernel()
             self._manager = None
 
 
 async def execute_python(code: str, kernel: Kernel) -> str:
     return await kernel.execute_code(code)
+
+
+### Environment Helpers
+
+
+def get_python_env_info() -> PythonEnvInfo:
+    return PythonEnvInfo(
+        interpreter_path=get_active_python_interpreter_path(),
+        interpreter_version=get_active_python_interpreter_version(),
+    )
+
+
+def get_active_python_interpreter_path() -> str | None:
+    # Run the command `which python`
+    result = subprocess.run(
+        ["which", "python"],
+        capture_output=True,
+        text=True,
+        check=False,
+    )
+    if result.returncode != 0:
+        return None
+    return result.stdout.strip()
+
+
+def get_active_python_interpreter_version() -> str | None:
+    try:
+        # Run the command `python -V`
+        result = subprocess.run(
+            ["python", "-V"], capture_output=True, text=True, check=False
+        )
+    except FileNotFoundError:
+        # Python is not installed?
+        return None
+    # Capture the standard output and standard error
+    stdout = result.stdout.strip()
+    match = re.search(r"Python (\d+\.\d+\.\d+)", stdout)
+    if match:
+        return match.group(1)
+    return None
```

### Comparing `exponent_run-0.0.4/exponent/core/remote_execution/languages/shell.py` & `exponent_run-0.0.5/exponent/core/remote_execution/languages/shell.py`

 * *Files identical despite different names*

### Comparing `exponent_run-0.0.4/exponent/core/remote_execution/session.py` & `exponent_run-0.0.5/exponent/core/remote_execution/session.py`

 * *Files identical despite different names*

### Comparing `exponent_run-0.0.4/exponent/core/remote_execution/types.py` & `exponent_run-0.0.5/exponent/core/remote_execution/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 from enum import Enum
 from typing import ClassVar, Generic, Literal, TypeGuard, TypeVar
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 
 class UseToolsMode(str, Enum):
     read_only = "read_only"
     read_write = "read_write"
     disabled = "disabled"
 
@@ -40,32 +40,54 @@
     chat_uuid: str
 
 
 class ExecutionEndResponse(BaseModel):
     execution_ended: bool
 
 
+class GitInfo(BaseModel):
+    branch: str
+    remote: str | None
+
+
+class PythonEnvInfo(BaseModel):
+    interpreter_path: str | None
+    interpreter_version: str | None
+    name: str | None = "exponent"
+    provider: Literal["venv", "pyenv", "pipenv", "conda"] | None = "pyenv"
+
+
 class SystemInfo(BaseModel):
     name: str
     cwd: str
-    shell: str
     os: str
+    shell: str
+    git: GitInfo | None
+    python_env: PythonEnvInfo | None
+
+
+class HeartbeatInfo(BaseModel):
+    system_info: SystemInfo | None
+    timestamp: datetime.datetime = Field(
+        default_factory=lambda: datetime.datetime.now(datetime.UTC)
+    )
 
 
 Direction = Literal[
     "request",
     "response",
 ]
 
 Namespace = Literal[
     "code_execution",
     "list_files",
     "get_file_contents",
     "get_matching_files",
     "system_context",
+    "get_all_tracked_files",
 ]
 
 SupportedLanguage = Literal[
     "python",
     "shell",
     "diff",
 ]
@@ -168,14 +190,24 @@
 
 class GetMatchingFilesRequest(RemoteExecutionRequest[GetMatchingFilesResponse]):
     namespace: ClassVar[Namespace] = "get_matching_files"
 
     search_term: str
 
 
+class GetAllTrackedFilesResponse(RemoteExecutionResponse):
+    namespace: ClassVar[Namespace] = "get_all_tracked_files"
+
+    file_paths: list[str]
+
+
+class GetAllTrackedFilesRequest(RemoteExecutionRequest[GetAllTrackedFilesResponse]):
+    namespace: ClassVar[Namespace] = "get_all_tracked_files"
+
+
 class SystemContextResponse(RemoteExecutionResponse):
     namespace: ClassVar[Namespace] = "system_context"
 
     exponent_txt: str | None
     system_info: SystemInfo | None
 
 
@@ -184,23 +216,26 @@
 
 
 RemoteExecutionRequestType = (
     CodeExecutionRequest
     | ListFilesRequest
     | GetFileContentsRequest
     | GetMatchingFilesRequest
+    | GetAllTrackedFilesRequest
     | SystemContextRequest
 )
 
 RemoteExecutionResponseType = (
     CodeExecutionResponse
     | ListFilesResponse
     | GetFileContentsResponse
     | GetMatchingFilesResponse
+    | GetAllTrackedFilesResponse
     | SystemContextResponse
 )
 
 
 class CLIConnectedState(BaseModel):
     chat_uuid: str
     connected: bool
     last_connected_at: datetime.datetime | None
+    system_info: SystemInfo | None
```

### Comparing `exponent_run-0.0.4/exponent/core/remote_execution/utils.py` & `exponent_run-0.0.5/exponent/core/remote_execution/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import NoReturn, TypeGuard, TypeVar, cast, overload
 
 from exponent.core.remote_execution.types import (
     CodeExecutionRequest,
     CodeExecutionResponse,
+    GetAllTrackedFilesRequest,
+    GetAllTrackedFilesResponse,
     GetFileContentsRequest,
     GetFileContentsResponse,
     GetMatchingFilesRequest,
     GetMatchingFilesResponse,
     ListFilesRequest,
     ListFilesResponse,
     RemoteExecutionMessage,
@@ -56,14 +58,18 @@
         request = ListFilesRequest.model_validate_json(request_data.message_data)
     elif request_data.namespace == "get_file_contents":
         request = GetFileContentsRequest.model_validate_json(request_data.message_data)
     elif request_data.namespace == "get_matching_files":
         request = GetMatchingFilesRequest.model_validate_json(request_data.message_data)
     elif request_data.namespace == "system_context":
         request = SystemContextRequest.model_validate_json(request_data.message_data)
+    elif request_data.namespace == "get_all_tracked_files":
+        request = GetAllTrackedFilesRequest.model_validate_json(
+            request_data.message_data
+        )
     else:
         # type checking trick, if you miss a namespace then
         # this won't typecheck due to the input parameter
         # having a potential type other than no-return
         request = assert_unreachable(request_data.namespace)
     return truncate_message(request)
 
@@ -86,14 +92,18 @@
         )
     elif response_data.namespace == "get_file_contents":
         response = GetFileContentsResponse.model_validate_json(
             response_data.message_data
         )
     elif response_data.namespace == "system_context":
         response = SystemContextResponse.model_validate_json(response_data.message_data)
+    elif response_data.namespace == "get_all_tracked_files":
+        response = GetAllTrackedFilesResponse.model_validate_json(
+            response_data.message_data
+        )
     else:
         # type checking trick, if you miss a namespace then
         # this won't typecheck due to the input parameter
         # having a potential type other than no-return
         response = assert_unreachable(response_data.namespace)
     return truncate_message(response)
```

### Comparing `exponent_run-0.0.4/exponent/tests/test_cli.py` & `exponent_run-0.0.5/exponent/tests/test_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,26 +5,30 @@
 from unittest import mock
 from unittest.mock import mock_open
 
 import pytest
 from click.testing import CliRunner
 
 from exponent.cli import login
-from exponent.core.remote_execution import files
+from exponent.core.remote_execution import files, git
 from exponent.core.remote_execution.client import RemoteExecutionClient
-from exponent.core.remote_execution.languages.python import Kernel
+from exponent.core.remote_execution.languages.python import Kernel, get_python_env_info
 from exponent.core.remote_execution.system_context import get_system_context
 from exponent.core.remote_execution.types import (
     CodeExecutionRequest,
     CodeExecutionResponse,
+    GetAllTrackedFilesRequest,
+    GetAllTrackedFilesResponse,
     GetFileContentsRequest,
     GetFileContentsResponse,
     GetMatchingFilesRequest,
     GetMatchingFilesResponse,
+    GitInfo,
     ListFilesRequest,
+    PythonEnvInfo,
     SystemContextRequest,
     SystemContextResponse,
     SystemInfo,
 )
 
 
 async def test_exponent_login(cli_runner: CliRunner) -> None:
@@ -59,23 +63,29 @@
         assert isinstance(request, ListFilesRequest)
         assert request == ListFilesRequest(
             correlation_id="123456", directory=default_temporary_directory
         )
 
         response = files.list_files(request)
         assert response.correlation_id == "123456"
-        assert sorted(response.filenames) == ["exponent.txt", "test1.py", "test2.py"]
+        assert sorted(response.filenames) == [
+            ".git",
+            "exponent.txt",
+            "test1.py",
+            "test2.py",
+        ]
 
 
 @mock.patch(
     "exponent.core.remote_execution.client.RemoteExecutionClient.get_execution_requests"
 )
 async def test_get_system_context(
     get_execution_requests: mock.Mock,
     default_temporary_directory: str,
+    python_env_info: PythonEnvInfo,
 ) -> None:
     get_execution_requests.return_value = [
         SystemContextRequest(correlation_id="123456")
     ]
 
     async with RemoteExecutionClient.session(
         api_key="123456",
@@ -96,14 +106,16 @@
             correlation_id="123456",
             exponent_txt="Hello, world!",
             system_info=SystemInfo(
                 name=getpass.getuser(),
                 cwd=default_temporary_directory,
                 shell=os.environ.get("SHELL", "bash"),
                 os=platform.system(),
+                git=GitInfo(branch="master", remote=None),
+                python_env=python_env_info,
             ),
         )
 
 
 @mock.patch(
     "exponent.core.remote_execution.client.RemoteExecutionClient.get_execution_requests"
 )
@@ -317,7 +329,51 @@
 
         with open("echo_server.py") as f:
             contents = f.read()
         assert (
             contents
             == 'from fastapi import FastAPI\nfrom pydantic import BaseModel\n\napp = FastAPI()\n\nclass Message(BaseModel):\n    content: str\n\n@app.get("/echo")\ndef echo(message: Message):\n    return {"Echo": message.content}\n\nif __name__ == "__main__":\n    import uvicorn\n    uvicorn.run(app, host="127.0.0.1", port=8000)\n'
         )
+
+
+@mock.patch(
+    "exponent.core.remote_execution.client.RemoteExecutionClient.get_execution_requests"
+)
+async def test_get_all_tracked_files(
+    get_execution_requests: mock.Mock,
+    default_temporary_directory: str,
+) -> None:
+    get_execution_requests.return_value = [
+        GetAllTrackedFilesRequest(correlation_id="123456"),
+    ]
+
+    async with RemoteExecutionClient.session(
+        api_key="123456",
+        base_url="https://example.com",
+        working_directory=default_temporary_directory,
+    ) as client:
+        EXPECTED_REQUESTS_COUNT = 1
+        requests = await client.get_execution_requests(chat_uuid="123456")
+        assert len(requests) == EXPECTED_REQUESTS_COUNT
+
+        request1 = requests[0]
+        assert isinstance(request1, GetAllTrackedFilesRequest)
+        assert request1 == GetAllTrackedFilesRequest(
+            correlation_id="123456",
+        )
+        response1 = git.get_all_tracked_files(request1, client.working_directory)
+        assert response1 == GetAllTrackedFilesResponse(
+            correlation_id="123456",
+            file_paths=[
+                "exponent.txt",
+                "test1.py",
+                "test2.py",
+            ],
+        )
+
+
+def test_get_python_env_info() -> None:
+    venv_info = get_python_env_info()
+    assert venv_info.interpreter_path
+    assert venv_info.interpreter_version
+    assert venv_info.interpreter_path.endswith("python")
+    assert venv_info.interpreter_version == platform.python_version()
```

### Comparing `exponent_run-0.0.4/pyproject.toml` & `exponent_run-0.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [tool.poetry]
 authors = ["Sashank Thupukari <sashank@exponent.run>"]
 description = "Exponent is an AI Pair Programmer"
 name = "exponent-run"
-version = "0.0.4"
+version = "0.0.5"
 packages = [{ include = "exponent" }]
 
 [tool.poetry.scripts]
 exponent = "exponent.cli:cli"
 
 [tool.poetry.dependencies]
-python = "^3.11,<3.13"
+python = "^3.10"
 
 
 pydantic = { extras = ["dotenv", "email"], version = "^2.6.4" }
 pydantic-settings = "^2.2.1"
 pytest-env = "^1.1.3"
 click = "^8.1.7"
 httpx = "^0.27.0"
 rapidfuzz = "^3.9.0"
 gitignore-parser = "^0.1.11"
 jupyter-client = "^8.6.1"
 ipykernel = "^6.29.4"
+pygit2 = "^1.15.0"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.4.4"
 freezegun = "^1.4.0"
 gevent = "^24.2.1"
 mypy = "^1.9.0"
 pre-commit = "^3.7.0"
```

### Comparing `exponent_run-0.0.4/PKG-INFO` & `exponent_run-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: exponent-run
-Version: 0.0.4
+Version: 0.0.5
 Summary: Exponent is an AI Pair Programmer
 Author: Sashank Thupukari
 Author-email: sashank@exponent.run
-Requires-Python: >=3.11,<3.13
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: gitignore-parser (>=0.1.11,<0.2.0)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: ipykernel (>=6.29.4,<7.0.0)
 Requires-Dist: jupyter-client (>=8.6.1,<9.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: pydantic[dotenv,email] (>=2.6.4,<3.0.0)
+Requires-Dist: pygit2 (>=1.15.0,<2.0.0)
 Requires-Dist: pytest-env (>=1.1.3,<2.0.0)
 Requires-Dist: rapidfuzz (>=3.9.0,<4.0.0)
```

