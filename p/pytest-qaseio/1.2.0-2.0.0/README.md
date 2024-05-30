# Comparing `tmp/pytest_qaseio-1.2.0.tar.gz` & `tmp/pytest_qaseio-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_qaseio-1.2.0.tar", max compression
+gzip compressed data, was "pytest_qaseio-2.0.0.tar", max compression
```

## Comparing `pytest_qaseio-1.2.0.tar` & `pytest_qaseio-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1092 2023-04-06 07:25:14.690639 pytest_qaseio-1.2.0/LICENSE
--rw-r--r--   0        0        0     5785 2023-05-11 09:07:18.681663 pytest_qaseio-1.2.0/README.md
--rw-r--r--   0        0        0     2828 2024-05-22 08:01:02.025745 pytest_qaseio-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-05 13:30:54.606605 pytest_qaseio-1.2.0/pytest_qaseio/__init__.py
--rw-r--r--   0        0        0     2387 2024-05-22 07:49:13.893891 pytest_qaseio-1.2.0/pytest_qaseio/api_client.py
--rw-r--r--   0        0        0      402 2023-04-05 13:30:52.095153 pytest_qaseio-1.2.0/pytest_qaseio/constants.py
--rw-r--r--   0        0        0     8055 2024-05-22 07:49:13.894504 pytest_qaseio-1.2.0/pytest_qaseio/converter.py
--rw-r--r--   0        0        0     3128 2024-05-22 07:49:19.391090 pytest_qaseio-1.2.0/pytest_qaseio/debug_info.py
--rw-r--r--   0        0        0      295 2024-04-22 09:59:50.443803 pytest_qaseio-1.2.0/pytest_qaseio/hooks.py
--rw-r--r--   0        0        0     8936 2024-05-22 07:49:19.391628 pytest_qaseio-1.2.0/pytest_qaseio/plugin.py
--rw-r--r--   0        0        0     1386 2024-05-22 07:49:19.391889 pytest_qaseio-1.2.0/pytest_qaseio/plugin_exceptions.py
--rw-r--r--   0        0        0        0 2023-04-05 13:31:00.616603 pytest_qaseio-1.2.0/pytest_qaseio/py.typed
--rw-r--r--   0        0        0     1156 2024-05-22 07:49:13.896526 pytest_qaseio-1.2.0/pytest_qaseio/storage.py
--rw-r--r--   0        0        0     6995 1970-01-01 00:00:00.000000 pytest_qaseio-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-06 07:25:14.690639 pytest_qaseio-2.0.0/LICENSE
+-rw-r--r--   0        0        0     6008 2024-05-30 04:43:23.010101 pytest_qaseio-2.0.0/README.md
+-rw-r--r--   0        0        0     6569 2024-05-30 04:43:23.011491 pytest_qaseio-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-05 13:30:54.606605 pytest_qaseio-2.0.0/pytest_qaseio/__init__.py
+-rw-r--r--   0        0        0     2734 2024-05-30 04:43:23.011967 pytest_qaseio-2.0.0/pytest_qaseio/api_client.py
+-rw-r--r--   0        0        0      402 2023-04-05 13:30:52.095153 pytest_qaseio-2.0.0/pytest_qaseio/constants.py
+-rw-r--r--   0        0        0     8035 2024-05-30 04:43:23.012437 pytest_qaseio-2.0.0/pytest_qaseio/converter.py
+-rw-r--r--   0        0        0     3237 2024-05-30 04:43:23.012811 pytest_qaseio-2.0.0/pytest_qaseio/debug_info.py
+-rw-r--r--   0        0        0      487 2024-05-30 04:43:23.013177 pytest_qaseio-2.0.0/pytest_qaseio/hooks.py
+-rw-r--r--   0        0        0     8617 2024-05-30 04:43:23.013515 pytest_qaseio-2.0.0/pytest_qaseio/plugin.py
+-rw-r--r--   0        0        0     1386 2024-05-23 06:15:21.577934 pytest_qaseio-2.0.0/pytest_qaseio/plugin_exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-05 13:31:00.616603 pytest_qaseio-2.0.0/pytest_qaseio/py.typed
+-rw-r--r--   0        0        0     1839 2024-05-30 04:43:23.013874 pytest_qaseio-2.0.0/pytest_qaseio/storage.py
+-rw-r--r--   0        0        0     7167 1970-01-01 00:00:00.000000 pytest_qaseio-2.0.0/PKG-INFO
```

### Comparing `pytest_qaseio-1.2.0/LICENSE` & `pytest_qaseio-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_qaseio-1.2.0/README.md` & `pytest_qaseio-2.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -50,19 +50,27 @@
 import pytest
 
 @pytest.mark.qase("https://app.qase.io/case/DEMO-1")
 def test_demo():
     """Check qaseio plugin works as expected."""
 ```
 
-Since this package is mostly used for selenium tests, you need to provide a
-value for `--webdriver` flag. If you set `--webdriver=remote` and want to specify
-name of remote browser (not just Remote), use `--remote-browser`
-flag or set capabilities via `variables`. This will be used in test run name and
-in attachments path.
+Since this package is mostly used for selenium tests, it expects to get browser
+name to use in Qase.io test run name and in attachments path. By default you can
+ provide it using `--webdriver` flag. But you can also override
+ `pytest_qase_browser_name` hook to implement some custom logic.
+ Here's default implementation of hook:
+
+ ```python
+@pytest.hookimpl(trylast=True)
+def pytest_qase_browser_name(config: pytest.Config) -> str:
+    """Try to get browser name from `webdriver` pytest option."""
+    return config.getoption("--webdriver")
+
+ ```
 
 To enable plugin use flag `--qase-enabled`.
 
 ```bash
 pytest tests/ --qase-enabled --webdriver=chrome
 ```
```

### Comparing `pytest_qaseio-1.2.0/pytest_qaseio/api_client.py` & `pytest_qaseio-2.0.0/pytest_qaseio/api_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import sys
+from typing import cast
 
 import qaseio
-import qaseio.apis
+from qaseio import configuration as qaseio_config
 from qaseio import models
 
 
 class QaseClient:
     """Class for interacting with tests runs in Qase API."""
 
     def __init__(
@@ -17,69 +18,79 @@
         """Init client."""
         super().__init__()
         self._logger = logging.getLogger("qase")
         self._logger.addHandler(
             logging.StreamHandler(sys.stderr),
         )
         self._client = qaseio.ApiClient(
-            configuration=qaseio.Configuration(
+            configuration=qaseio_config.Configuration(
                 api_key={
                     "TokenAuth": token,
                 },
             ),
         )
         self._project_code: str = project_code
 
     def get_run(
         self,
         run_id: int,
     ) -> models.Run:
-        return qaseio.apis.RunsApi(self._client).get_run(
-            code=self._project_code, id=run_id,
-        ).result
+        run_response = qaseio.RunsApi(self._client).get_run(
+            code=self._project_code,
+            id=run_id,
+        )
+        return cast(models.Run, run_response.result)
 
     def create_run(
         self,
         run_data: models.RunCreate,
     ) -> models.Run:
         """Create test run in Qase."""
-        response = qaseio.apis.RunsApi(self._client).create_run(
+        response = qaseio.RunsApi(self._client).create_run(
             code=self._project_code,
             run_create=run_data,
         )
-        return self.get_run(response.result.id)
+        created_run = cast(models.IdResponseAllOfResult, response.result)
+
+        return self.get_run(cast(int, created_run.id))
 
     def load_cases_ids(
         self,
     ) -> list[int]:
         """Load all cases ids of project."""
         limit = 100
         cases: list[int] = []
-        response: models.TestCaseListResponse = qaseio.apis.CasesApi(self._client).get_cases(
+        response = qaseio.CasesApi(self._client).get_cases(
             code=self._project_code,
             limit=limit,
             offset=len(cases),
         )
         while True:
-            response = qaseio.apis.CasesApi(self._client).get_cases(
+            response = qaseio.CasesApi(self._client).get_cases(
                 code=self._project_code,
                 limit=limit,
                 offset=len(cases),
             )
-            new_cases = [case.id for case in response.result.entities]
+            response_cases = getattr(response.result, "entities", [])
+            new_cases = [case.id for case in response_cases]
             cases += new_cases
             if not new_cases:
                 break
         return cases
 
     def report_test_results(
         self,
-        run: models.RunCreate,
+        run: models.Run,
         report_data: models.ResultCreate,
     ) -> tuple[str, models.ResultCreate]:
         """Report test results back to Qase."""
-        result = qaseio.apis.ResultsApi(self._client).create_result(
-            code=self._project_code,
-            id=run.id,
-            result_create=report_data,
-        ).result
-        return result.hash, report_data.status
+        result = (
+            qaseio.ResultsApi(self._client)
+            .create_result(
+                code=self._project_code,
+                id=cast(int, run.id),
+                result_create=report_data,
+            )
+            .result
+        )
+        assert result
+        return cast(str, result.hash), cast(models.ResultCreate, report_data.status)
```

### Comparing `pytest_qaseio-1.2.0/pytest_qaseio/converter.py` & `pytest_qaseio-2.0.0/pytest_qaseio/converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         cases, tests = self._prepare_cases_for_run(
             cases_ids_from_api=cases_ids_from_api,
             items=items,
         )
         title = constants.RUN_NAME_TEMPLATE.format(
             env=self._env.capitalize(),
             browser=self._browser.capitalize(),
-            date=datetime.datetime.utcnow().strftime("%m/%d/%Y %H:%M:%S"),
+            date=datetime.datetime.now(tz=datetime.UTC).strftime("%m/%d/%Y %H:%M:%S"),
         )
         run_data = models.RunCreate(
             title=title,
             cases=cases,
         )
 
         return run_data, tests
@@ -196,33 +196,29 @@
                     f"Please check case id for {item.location[0]}",
                 )
                 case_id_invalid = True
                 continue
             cases_ids.append(case_id)
 
         duplicating_ids = [
-            case_id for case_id, counter in collections.Counter(cases_ids).items()
-            if counter > 1
+            case_id for case_id, counter in collections.Counter(cases_ids).items() if counter > 1
         ]
         if duplicating_ids:
             raise plugin_exceptions.DuplicatingCaseId(duplicating_ids)
 
         if case_id_invalid:
             raise plugin_exceptions.InvalidCaseId()
         return cases_ids, tests
 
     def _extract_qase_marker(
         self,
         item: pytest.Function,
     ) -> pytest.Mark | None:
         """Extract qase's `Mark` object from test item."""
-        qase_markers = [
-            marker for marker in item.own_markers
-            if marker.name == "qase"
-        ]
+        qase_markers = [marker for marker in item.own_markers if marker.name == "qase"]
         if not qase_markers:
             return None
 
         if len(qase_markers) == 1:
             return qase_markers[0]
 
         self._logger.error(
@@ -230,15 +226,15 @@
         )
         raise plugin_exceptions.MultipleIDsForTest()
 
     def _extract_case_id_from_marker(
         self,
         project_code: str,
         marker: pytest.Mark,
-    ):
+    ) -> None | int:
         """Shortcut to extract qase case ID from marker."""
         if len(marker.args) != 1:
             return None
         url = marker.args[0]
         return int(url.split(f"{project_code}-")[-1])
 
     def _extract_case_id_from_test(
```

### Comparing `pytest_qaseio-1.2.0/pytest_qaseio/debug_info.py` & `pytest_qaseio-2.0.0/pytest_qaseio/debug_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import base64
 import logging
+import typing
+from collections.abc import Iterable
 
 import arrow
 from _pytest.python import Function
 from selenium.common.exceptions import WebDriverException
 from selenium.webdriver.remote.webdriver import WebDriver
 
 from . import constants, storage
@@ -38,44 +40,45 @@
                 logs.append(self._format_log(self.webdriver.get_log(name)))  # type: ignore
         except WebDriverException:
             # https://github.com/mozilla/geckodriver/issues/284
             return ""
         return "\n".join(logs)
 
     @staticmethod
-    def _format_log(log) -> str:
+    def _format_log(log: Iterable[dict[str, typing.Any]]) -> str:
         """Format logs.
 
         Copied from pytest-selenium.
 
         """
         timestamp_format = "%Y-%m-%d %H:%M:%S.%f"
-        entries = []
+        entries: list[str] = []
         for entry in log:
             timestamp = arrow.get(entry["timestamp"] / 1000.0).strftime(timestamp_format)
             entries.append(f"{timestamp} {entry['level']} - {entry['message']}")
-        log = "\n".join(entries)
-        return log
+        return "\n".join(entries)
 
     def generate_debug_comment(
         self,
         file_storage: storage.FileStorage,
         folder: str,
     ) -> str:
         try:
             screenshot_url = file_storage.save_file_obj(
-                content=self.screenshot, filename=f"{folder}/screenshot.png",
+                content=self.screenshot,
+                filename=f"{folder}/screenshot.png",
             )
         except Exception:
             self.logger.error(msg="Can't save screenshot to storage", exc_info=True)
             screenshot_url = ""
 
         try:
             html_url = file_storage.save_file_obj(
-                content=self.html, filename=f"{folder}/html.html",
+                content=self.html,
+                filename=f"{folder}/html.html",
             )
         except Exception:
             self.logger.error(msg="Can't save HTML to storage", exc_info=True)
             html_url = ""
 
         try:
             browser_log_url = file_storage.save_file_obj(
```

### Comparing `pytest_qaseio-1.2.0/pytest_qaseio/plugin.py` & `pytest_qaseio-2.0.0/pytest_qaseio/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 import logging
 import os
 import pathlib
+from typing import cast
 
 import filelock
 import pytest
 from _pytest.terminal import TerminalReporter
 from qaseio import models
 from qaseio.exceptions import ApiException
 
 from . import api_client, converter, plugin_exceptions, storage
 
 
-def pytest_addoption(parser: pytest.Parser):
+def pytest_addoption(parser: pytest.Parser) -> None:
     """Add custom args to command line."""
     parser.addoption(
         "--qase-enabled",
         action="store_true",
         default=False,
         help="Store run result in qase",
     )
     parser.addoption(
         "--qase-file-storage",
         default="qase",
         help="Choose file storage to upload debug files",
     )
 
 
-def pytest_addhooks(pluginmanager):
+def pytest_addhooks(pluginmanager: pytest.PytestPluginManager) -> None:
     """Add hooks for plugin."""
     from . import hooks
 
     pluginmanager.add_hookspecs(hooks)
 
 
 def _get_file_storage(config: pytest.Config) -> storage.FileStorage | None:
     """Provide file storage via pytest config."""
-    file_storage_name = config.getoption("--qase-file-storage")
+    file_storage_name: str = config.getoption("--qase-file-storage")
     if file_storage_name.lower() == "none":
         return None
 
     file_storages: dict[str, storage.FileStorage] = config.hook.pytest_qase_file_storages()
 
     if file_storage_name not in file_storages:
         logging.getLogger("qase").error(
@@ -58,51 +59,42 @@
         "qase": storage.QaseFileStorage(
             qase_token=os.environ["QASE_TOKEN"],
             qase_project_code=os.environ["QASE_PROJECT_CODE"],
         ),
     }
 
 
-def _get_browser_name(config: pytest.Config, default: str = "remote"):
-    """Try to get browser name from options and variables.
-
-    Since `pytest-selenium` uses `pytest-variables` and recommends to put
-    capabilities there. So we try to get `browserName` from `config.stash` (and
-    `config._variables` for older version of `pytest-variables`).
-
-    """
-    stash = getattr(config, "stash", getattr(config, "_variables", {}))
-    browser_name = stash.get("capabilities", {}).get("browserName", None)
-
-    return browser_name or config.getoption("--remote-browser", default=default)
+@pytest.hookimpl(trylast=True)
+def pytest_qase_browser_name(config: pytest.Config) -> str:
+    """Try to get browser name from `webdriver` pytest option."""
+    return config.getoption("--webdriver")
 
 
 @pytest.hookimpl(trylast=True)
-def pytest_configure(config: pytest.Config):
+def pytest_configure(config: pytest.Config) -> None:
     """Configure pytest-qaseio plugin.
 
     Add `qase` marker for pytest.
     If qase enabled, register qase plugin.
     Get file storage for qase plugin.
 
     """
     config.addinivalue_line(
         "markers",
         "qase(test_case_url): Mark test for qase",
     )
     qase_enabled = config.getoption("--qase-enabled")
     if not qase_enabled:
         return
-    browser = config.getoption("--webdriver")
-    if browser == "remote":
-        browser = _get_browser_name(config, default=browser)
+
+    browser_name: str = config.hook.pytest_qase_browser_name(config=config)
 
     config.pluginmanager.register(
         plugin=QasePlugin(
-            browser=browser,
+            browser=browser_name,
             file_storage=_get_file_storage(config),
         ),
         name="qase_plugin",
     )
 
 
 class QasePlugin:
@@ -134,27 +126,27 @@
         )
 
         # Mapping of pytest items ids and case id
         self._tests: dict[str, int | None] = dict()
         # Mapping of case ids and result hash from qase with status
         self._qase_results: dict[str, tuple[str, models.ResultCreate]] = dict()
 
-    def pytest_sessionstart(self, session: pytest.Session):
+    def pytest_sessionstart(self, session: pytest.Session) -> None:
         """Clear previously saved run, prepare lock file."""
         if hasattr(session.config, "workerinput"):
             # Do nothing if it is not master thread
             return
         self.__run_file.unlink(missing_ok=True)
         self.__run_file_lock.touch(exist_ok=True)
 
     @pytest.hookimpl(trylast=True)
     def pytest_collection_modifyitems(
         self,
         items: list[pytest.Function],
-    ):
+    ) -> None:
         """Create test run in qase."""
         with filelock.FileLock(self.__run_file_lock):
             try:
                 run_data, self._tests = self._converter.prepare_run_data(
                     cases_ids_from_api=self._cases_ids_from_api,
                     items=items,
                 )
@@ -185,40 +177,40 @@
                 )
                 with pathlib.Path(self.__run_file).open(mode="w") as lock_file:
                     lock_file.write(str(self._current_run.id))
             except plugin_exceptions.BaseQasePluginException as e:
                 pytest.exit(e.message)
 
     @pytest.hookimpl(tryfirst=True, hookwrapper=True)
-    def pytest_runtest_makereport(self, item: pytest.Function):
+    def pytest_runtest_makereport(self, item: pytest.Function):  # noqa: ANN201
         """Represent standard pytest hook on test completion.
 
         At this hook we will report passed, skipped and failed tests.
 
         """
         provided_report = yield
         report: pytest.TestReport = provided_report.get_result()
         should_report = not (
             # Passed tests should be reported only on call
-            (report.passed and report.when in ("setup", "teardown"))
+            report.passed and report.when in ("setup", "teardown")
         )
         if not should_report:
             return
         case_id = self._tests[item.nodeid]
         # No need to report same passed status,
         # while skipped and failed should be always reported
         if not case_id or item.nodeid in self._qase_results and report.passed:
             return
         if not self._current_run:
             raise plugin_exceptions.RunNotConfigured()
         try:
             self._qase_results[item.nodeid] = self._client.report_test_results(
                 run=self._current_run,
                 report_data=self._converter.prepare_report_data(
-                    run_id=self._current_run.id,
+                    run_id=cast(int, self._current_run.id),
                     case_id=case_id,
                     item=item,
                     report=report,
                 ),
             )
 
         except ApiException as error:
```

### Comparing `pytest_qaseio-1.2.0/pytest_qaseio/plugin_exceptions.py` & `pytest_qaseio-2.0.0/pytest_qaseio/plugin_exceptions.py`

 * *Files identical despite different names*

### Comparing `pytest_qaseio-1.2.0/PKG-INFO` & `pytest_qaseio-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: pytest-qaseio
-Version: 1.2.0
+Version: 2.0.0
 Summary: Pytest plugin for Qase.io integration
 Home-page: https://pypi.org/project/pytest-qaseio/
 License: MIT
 Keywords: pytest,qase,qaseio,selenium,autotests
 Author: Saritasa
 Author-email: pypi@saritasa.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Bug Tracking
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Requires-Dist: arrow (>=1.3.0,<2.0.0)
 Requires-Dist: filelock (>=3.14.0,<4.0.0)
 Requires-Dist: pytest (>=7.2.2,<9.0.0)
-Requires-Dist: qaseio (>=3.4.1,<4.0.0)
+Requires-Dist: qaseio (>=4.0.0,<5.0.0)
 Requires-Dist: selenium (>=4.21.0,<5.0.0)
 Project-URL: Repository, https://github.com/saritasa-nest/pytest-qaseio
 Description-Content-Type: text/markdown
 
 # pytest-qaseio
 
 [![Build Status](https://github.com/saritasa-nest/pytest-qaseio/workflows/checks/badge.svg?branch=main&event=push)](https://github.com/saritasa-nest/pytest-qaseio/actions?query=workflow%3Achecks)
@@ -80,19 +79,27 @@
 import pytest
 
 @pytest.mark.qase("https://app.qase.io/case/DEMO-1")
 def test_demo():
     """Check qaseio plugin works as expected."""
 ```
 
-Since this package is mostly used for selenium tests, you need to provide a
-value for `--webdriver` flag. If you set `--webdriver=remote` and want to specify
-name of remote browser (not just Remote), use `--remote-browser`
-flag or set capabilities via `variables`. This will be used in test run name and
-in attachments path.
+Since this package is mostly used for selenium tests, it expects to get browser
+name to use in Qase.io test run name and in attachments path. By default you can
+ provide it using `--webdriver` flag. But you can also override
+ `pytest_qase_browser_name` hook to implement some custom logic.
+ Here's default implementation of hook:
+
+ ```python
+@pytest.hookimpl(trylast=True)
+def pytest_qase_browser_name(config: pytest.Config) -> str:
+    """Try to get browser name from `webdriver` pytest option."""
+    return config.getoption("--webdriver")
+
+ ```
 
 To enable plugin use flag `--qase-enabled`.
 
 ```bash
 pytest tests/ --qase-enabled --webdriver=chrome
 ```
```

