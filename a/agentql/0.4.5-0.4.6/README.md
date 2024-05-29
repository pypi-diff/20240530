# Comparing `tmp/agentql-0.4.5.tar.gz` & `tmp/agentql-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentql-0.4.5.tar", max compression
+gzip compressed data, was "agentql-0.4.6.tar", max compression
```

## Comparing `agentql-0.4.5.tar` & `agentql-0.4.6.tar`

### file list

```diff
@@ -1,61 +1,60 @@
--rw-r--r--   0        0        0     1066 2024-05-16 01:15:44.746817 agentql-0.4.5/LICENSE
--rw-r--r--   0        0        0      111 2024-05-16 01:15:44.746817 agentql-0.4.5/PACKAGE_README.md
--rw-r--r--   0        0        0      835 2024-05-16 01:15:44.834817 agentql-0.4.5/pyproject.toml
--rw-r--r--   0        0        0      591 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_cli/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_cli/_commands/__init__.py
--rw-r--r--   0        0        0      261 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_cli/_commands/doctor_command.py
--rw-r--r--   0        0        0     2681 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_cli/_commands/init_command.py
--rw-r--r--   0        0        0      228 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_cli/_main.py
--rw-r--r--   0        0        0        0 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/__init__.py
--rw-r--r--   0        0        0      177 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_api_constants.py
--rw-r--r--   0        0        0     5443 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_errors.py
--rw-r--r--   0        0        0        0 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_js_snippets/__init__.py
--rw-r--r--   0        0        0      322 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_js_snippets/add_dom_change_listener.js
--rw-r--r--   0        0        0     7249 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_js_snippets/generate_accessibility_tree.js
--rw-r--r--   0        0        0      147 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_js_snippets/get_last_dom_change.js
--rw-r--r--   0        0        0      119 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_js_snippets/iframe_contains_doc_or_body.js
--rw-r--r--   0        0        0      145 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_js_snippets/remove_dom_change_listener.js
--rw-r--r--   0        0        0      506 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_js_snippets/scroll_to_bottom.js
--rw-r--r--   0        0        0      503 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_js_snippets/scroll_to_top.js
--rw-r--r--   0        0        0      843 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_js_snippets/set_iframe_path.js
--rw-r--r--   0        0        0      436 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_js_snippets/snippet_loader.py
--rw-r--r--   0        0        0        0 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_syntax/__init__.py
--rw-r--r--   0        0        0     1098 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_syntax/character_utils.py
--rw-r--r--   0        0        0     4997 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_syntax/lexer.py
--rw-r--r--   0        0        0     2475 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_syntax/node.py
--rw-r--r--   0        0        0     4686 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_syntax/parser.py
--rw-r--r--   0        0        0     1196 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_syntax/source.py
--rw-r--r--   0        0        0     1602 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_syntax/token.py
--rw-r--r--   0        0        0      213 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_syntax/token_kind.py
--rw-r--r--   0        0        0      297 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_trail_logger/__init__.py
--rw-r--r--   0        0        0     5151 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/_core/_trail_logger/_trail_logger_impl.py
--rw-r--r--   0        0        0      535 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/_core/_typing.py
--rw-r--r--   0        0        0     1962 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/_core/_utils.py
--rw-r--r--   0        0        0      363 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/async_api/__init__.py
--rw-r--r--   0        0        0     3871 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/async_api/_agentql_service.py
--rw-r--r--   0        0        0     2893 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/async_api/_api.py
--rw-r--r--   0        0        0     2194 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/async_api/_popup.py
--rw-r--r--   0        0        0     6166 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/async_api/_response_proxy.py
--rw-r--r--   0        0        0     8409 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/async_api/_session.py
--rw-r--r--   0        0        0     6023 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/async_api/_web_driver.py
--rw-r--r--   0        0        0     1283 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/experimental/async_api/_protocol/_browser.py
--rw-r--r--   0        0        0     3981 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/experimental/async_api/_protocol/_page.py
--rw-r--r--   0        0        0     1269 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/experimental/sync_api/_protocol/_browser.py
--rw-r--r--   0        0        0     3919 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/experimental/sync_api/_protocol/_page.py
--rw-r--r--   0        0        0        0 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/ext/__init__.py
--rw-r--r--   0        0        0      440 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/ext/playwright/__init__.py
--rw-r--r--   0        0        0      193 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/ext/playwright/_driver_constants.py
--rw-r--r--   0        0        0      280 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/ext/playwright/_driver_settings.py
--rw-r--r--   0        0        0     1980 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/ext/playwright/_html_constants.py
--rw-r--r--   0        0        0     4554 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/ext/playwright/_network_monitor.py
--rw-r--r--   0        0        0    30022 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/ext/playwright/playwright_driver_async.py
--rw-r--r--   0        0        0    29657 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/ext/playwright/playwright_driver_sync.py
--rw-r--r--   0        0        0      363 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/sync_api/__init__.py
--rw-r--r--   0        0        0     3768 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/sync_api/_agentql_service.py
--rw-r--r--   0        0        0     2847 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/sync_api/_api.py
--rw-r--r--   0        0        0     1918 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/sync_api/_popup.py
--rw-r--r--   0        0        0     5478 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/sync_api/_response_proxy.py
--rw-r--r--   0        0        0     8199 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/sync_api/_session.py
--rw-r--r--   0        0        0     5433 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/sync_api/_web_driver.py
--rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 agentql-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-29 22:17:45.713739 agentql-0.4.6/LICENSE
+-rw-r--r--   0        0        0      111 2024-05-29 22:17:45.713739 agentql-0.4.6/PACKAGE_README.md
+-rw-r--r--   0        0        0      835 2024-05-29 22:17:45.801738 agentql-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0      591 2024-05-29 22:17:45.801738 agentql-0.4.6/src/agentql/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:17:45.801738 agentql-0.4.6/src/agentql/_cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:17:45.801738 agentql-0.4.6/src/agentql/_cli/_commands/__init__.py
+-rw-r--r--   0        0        0      261 2024-05-29 22:17:45.801738 agentql-0.4.6/src/agentql/_cli/_commands/doctor_command.py
+-rw-r--r--   0        0        0     2681 2024-05-29 22:17:45.801738 agentql-0.4.6/src/agentql/_cli/_commands/init_command.py
+-rw-r--r--   0        0        0      228 2024-05-29 22:17:45.801738 agentql-0.4.6/src/agentql/_cli/_main.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:17:45.801738 agentql-0.4.6/src/agentql/_core/__init__.py
+-rw-r--r--   0        0        0      177 2024-05-29 22:17:45.801738 agentql-0.4.6/src/agentql/_core/_api_constants.py
+-rw-r--r--   0        0        0     8073 2024-05-29 22:17:45.801738 agentql-0.4.6/src/agentql/_core/_errors.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:17:45.801738 agentql-0.4.6/src/agentql/_core/_js_snippets/__init__.py
+-rw-r--r--   0        0        0      322 2024-05-29 22:17:45.801738 agentql-0.4.6/src/agentql/_core/_js_snippets/add_dom_change_listener.js
+-rw-r--r--   0        0        0     7249 2024-05-29 22:17:45.801738 agentql-0.4.6/src/agentql/_core/_js_snippets/generate_accessibility_tree.js
+-rw-r--r--   0        0        0      147 2024-05-29 22:17:45.801738 agentql-0.4.6/src/agentql/_core/_js_snippets/get_last_dom_change.js
+-rw-r--r--   0        0        0      147 2024-05-29 22:17:45.801738 agentql-0.4.6/src/agentql/_core/_js_snippets/get_scroll_info.js
+-rw-r--r--   0        0        0      119 2024-05-29 22:17:45.801738 agentql-0.4.6/src/agentql/_core/_js_snippets/iframe_contains_doc_or_body.js
+-rw-r--r--   0        0        0      145 2024-05-29 22:17:45.801738 agentql-0.4.6/src/agentql/_core/_js_snippets/remove_dom_change_listener.js
+-rw-r--r--   0        0        0      843 2024-05-29 22:17:45.801738 agentql-0.4.6/src/agentql/_core/_js_snippets/set_iframe_path.js
+-rw-r--r--   0        0        0      436 2024-05-29 22:17:45.801738 agentql-0.4.6/src/agentql/_core/_js_snippets/snippet_loader.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:17:45.801738 agentql-0.4.6/src/agentql/_core/_syntax/__init__.py
+-rw-r--r--   0        0        0     2114 2024-05-29 22:17:45.801738 agentql-0.4.6/src/agentql/_core/_syntax/character_utils.py
+-rw-r--r--   0        0        0     7207 2024-05-29 22:17:45.801738 agentql-0.4.6/src/agentql/_core/_syntax/lexer.py
+-rw-r--r--   0        0        0     3060 2024-05-29 22:17:45.801738 agentql-0.4.6/src/agentql/_core/_syntax/node.py
+-rw-r--r--   0        0        0     5443 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/_core/_syntax/parser.py
+-rw-r--r--   0        0        0     1196 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/_core/_syntax/source.py
+-rw-r--r--   0        0        0     1602 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/_core/_syntax/token.py
+-rw-r--r--   0        0        0      245 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/_core/_syntax/token_kind.py
+-rw-r--r--   0        0        0      297 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/_core/_trail_logger/__init__.py
+-rw-r--r--   0        0        0     5151 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/_core/_trail_logger/_trail_logger_impl.py
+-rw-r--r--   0        0        0      535 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/_core/_typing.py
+-rw-r--r--   0        0        0     1962 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/_core/_utils.py
+-rw-r--r--   0        0        0      363 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/async_api/__init__.py
+-rw-r--r--   0        0        0     4343 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/async_api/_agentql_service.py
+-rw-r--r--   0        0        0     2893 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/async_api/_api.py
+-rw-r--r--   0        0        0     2194 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/async_api/_popup.py
+-rw-r--r--   0        0        0     6166 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/async_api/_response_proxy.py
+-rw-r--r--   0        0        0     8642 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/async_api/_session.py
+-rw-r--r--   0        0        0     6023 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/async_api/_web_driver.py
+-rw-r--r--   0        0        0     1283 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/experimental/async_api/_protocol/_browser.py
+-rw-r--r--   0        0        0     3981 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/experimental/async_api/_protocol/_page.py
+-rw-r--r--   0        0        0     1269 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/experimental/sync_api/_protocol/_browser.py
+-rw-r--r--   0        0        0     3919 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/experimental/sync_api/_protocol/_page.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/ext/__init__.py
+-rw-r--r--   0        0        0      440 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/ext/playwright/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/ext/playwright/_driver_constants.py
+-rw-r--r--   0        0        0      280 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/ext/playwright/_driver_settings.py
+-rw-r--r--   0        0        0     1980 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/ext/playwright/_html_constants.py
+-rw-r--r--   0        0        0     4591 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/ext/playwright/_network_monitor.py
+-rw-r--r--   0        0        0    30957 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/ext/playwright/playwright_driver_async.py
+-rw-r--r--   0        0        0    30543 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/ext/playwright/playwright_driver_sync.py
+-rw-r--r--   0        0        0      363 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/sync_api/__init__.py
+-rw-r--r--   0        0        0     4240 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/sync_api/_agentql_service.py
+-rw-r--r--   0        0        0     2847 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/sync_api/_api.py
+-rw-r--r--   0        0        0     1918 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/sync_api/_popup.py
+-rw-r--r--   0        0        0     5478 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/sync_api/_response_proxy.py
+-rw-r--r--   0        0        0     8427 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/sync_api/_session.py
+-rw-r--r--   0        0        0     5433 2024-05-29 22:17:45.805739 agentql-0.4.6/src/agentql/sync_api/_web_driver.py
+-rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 agentql-0.4.6/PKG-INFO
```

### Comparing `agentql-0.4.5/LICENSE` & `agentql-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `agentql-0.4.5/pyproject.toml` & `agentql-0.4.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agentql"
-version = "0.4.5"
+version = "0.4.6"
 description = "Tiny Fish AgentQL Python Client"
 authors = []
 license = "MIT"
 readme = "PACKAGE_README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `agentql-0.4.5/src/agentql/__init__.py` & `agentql-0.4.6/src/agentql/__init__.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.5/src/agentql/_cli/_commands/init_command.py` & `agentql-0.4.6/src/agentql/_cli/_commands/init_command.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.5/src/agentql/_core/_js_snippets/generate_accessibility_tree.js` & `agentql-0.4.6/src/agentql/_core/_js_snippets/generate_accessibility_tree.js`

 * *Files identical despite different names*

### Comparing `agentql-0.4.5/src/agentql/_core/_js_snippets/set_iframe_path.js` & `agentql-0.4.6/src/agentql/_core/_js_snippets/set_iframe_path.js`

 * *Files identical despite different names*

### Comparing `agentql-0.4.5/src/agentql/_core/_syntax/node.py` & `agentql-0.4.6/src/agentql/_core/_syntax/node.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,41 @@
-from typing import List
+from typing import List, Optional
 
 from pydantic import BaseModel, ConfigDict, Field, SerializeAsAny
-from typing_extensions import Annotated
+from typing_extensions import TYPE_CHECKING, Annotated
 
 DEFAULT_INDENT = 2
 
 
 class _NodeWithChildrenMixin:
-    children: Annotated[SerializeAsAny[List["Node"]], Field(default_factory=List)]
+    if TYPE_CHECKING:
+        children: List["Node"]
 
 
 class Node(BaseModel):
     name: str
+    description: Optional[str]
+
     # Freeze the model to make it immutable
     model_config = ConfigDict(frozen=True)
 
     @property
     def query_name(self) -> str:
         """
         Returns the query name of the node.
         """
-        return self.name
+        description = f"({self.query_description})" if self.query_description else ""
+        return f"{self.name}{description}"
+
+    @property
+    def query_description(self) -> Optional[str]:
+        """
+        Returns the query description of the node.
+        """
+        return self.description
 
     def _dump(self, level: int = 0, indent: int = DEFAULT_INDENT) -> str:
         indent_spaces = " " * indent * level
         res = self.query_name
         return f"{indent_spaces}{res}"
 
     def dump(self, indent: int = DEFAULT_INDENT) -> str:
@@ -61,27 +72,30 @@
     {
         search_btns[]
     }
     """
 
     @property
     def query_name(self) -> str:
-        return f"{self.name}[]"
+        description = f"({self.query_description})" if self.query_description else ""
+        return f"{self.name}{description}[]"
 
 
 class ContainerNode(Node, _NodeWithChildrenMixin):
     """
     {
         container {
             child1
             child2
         }
     }
     """
 
+    children: Annotated[SerializeAsAny[List["Node"]], Field(default_factory=List)]
+
     def _dump(self, level: int = 0, indent: int = DEFAULT_INDENT) -> str:
         indent_spaces = " " * indent * level
         node_name = f"{self.query_name} " if self.query_name else ""
         header = f"{indent_spaces}{node_name}{{\n"
         # pylint: disable=protected-access
         body = "\n".join([child._dump(indent=indent, level=level + 1) for child in self.children])
         footer = f"\n{indent_spaces}}}"
@@ -96,8 +110,9 @@
             child2
         }
     }
     """
 
     @property
     def query_name(self) -> str:
-        return f"{self.name}[]"
+        description = f"({self.query_description})" if self.query_description else ""
+        return f"{self.name}{description}[]"
```

### Comparing `agentql-0.4.5/src/agentql/_core/_syntax/parser.py` & `agentql-0.4.6/src/agentql/_core/_syntax/parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union
+from typing import List, Optional, Union
 
 from agentql import QuerySyntaxError
 
 from .lexer import Lexer
 from .node import ContainerListNode, ContainerNode, IdListNode, IdNode, Node
 from .source import Source
 from .token import Token
@@ -25,88 +25,100 @@
     def parse(self) -> ContainerNode:
         """Parses the source and check for syntax. It is the entry point of the parser."""
         self._expect_token(TokenKind.SOF)
         node = self._parse_container()
         self._expect_token(TokenKind.EOF)
         return node
 
-    def _parse_container(self, name: str = "") -> ContainerNode:
+    def _parse_container(self, name: str = "", description: Optional[str] = None) -> ContainerNode:
         """Parses a container, which is enclosed by curly braces."""
 
-        nodes = self._many(TokenKind.BRACE_L, self._parse_identifier, TokenKind.BRACE_R)
-        return ContainerNode(name=name, children=nodes)
+        nodes = self._many(TokenKind.BRACE_L, self._parse_node, TokenKind.BRACE_R)
+        return ContainerNode(name=name, description=description, children=nodes)
 
-    def _parse_identifier(self) -> Node:
-        """Parses an identifier."""
+    def _parse_node(self) -> Node:
+        """Parses a node."""
         name = self._expect_token(TokenKind.IDENTIFIER).value
 
+        description = None
+        if self._peek(TokenKind.DESCRIPTION):  # Description is SOMETIMES present
+            description = self._expect_token(TokenKind.DESCRIPTION).value
+
         if self._peek(TokenKind.BRACE_L):
-            node = self._parse_container(name)
+            node = self._parse_container(name=name, description=description)
         elif self._peek(TokenKind.BRACKET_L):
-            node = self._parse_list(name)
+            node = self._parse_list(name=name, description=description)
         else:
-            node = IdNode(name=name)
+            node = IdNode(name=name, description=description)
         return node
 
-    def _parse_list(self, name: str) -> Union[ContainerListNode, IdListNode]:
+    def _parse_list(
+        self, name: str, description: Optional[str]
+    ) -> Union[ContainerListNode, IdListNode]:
         """Parses a list, represented by two brackets."""
         prev_token = self.lexer.token.prev
-        # make sure list token is following an identifier
-        if prev_token.kind != TokenKind.IDENTIFIER:
-            error_message = f"Expected Identifier, found {prev_token.kind.value} on row {prev_token.line}. List token ([]) must follow an identifier."
+        # make sure list token is following an identifier or description
+        if prev_token.kind != TokenKind.IDENTIFIER and prev_token.kind != TokenKind.DESCRIPTION:
+            error_message = f"Expected Identifier or Description, found {prev_token.kind.value} on row {prev_token.line}. List token ([]) must follow an identifier or description."
             raise QuerySyntaxError(
                 message=error_message,
                 unexpected_token=prev_token.kind.value,
                 row=prev_token.line,
                 column=prev_token.column,
             )
 
         self._expect_token(TokenKind.BRACKET_L)
         self._expect_token(TokenKind.BRACKET_R)
 
         if self._peek(TokenKind.BRACE_L):
-            container = self._parse_container(name)
-            node = ContainerListNode(name=container.name, children=container.children)
+            container = self._parse_container(name=name, description=description)
+            node = ContainerListNode(
+                name=container.name, description=description, children=container.children
+            )
         else:
-            node = IdListNode(name=name)
+            node = IdListNode(name=name, description=description)
         return node
 
     def _many(
         self, open_kind: TokenKind, parse_fn: callable, close_kind: TokenKind, **kwargs
     ) -> List[Node]:
         """Parses zero or more tokens of the given kind by repeatedly calling the given
         parse function. Check whether the syntax is valid."""
         self._expect_token(open_kind)
         identifier_name_list = set()
         nodes = []
 
         while True:
-            # make sure there is no duplicate identifier in the same container
+            # Make sure there is no duplicate identifier in the same container
             if self._peek(TokenKind.IDENTIFIER):
                 identifier = self.lexer.token.value
                 if identifier in identifier_name_list:
                     error_message = f"Duplicate identifier '{identifier}' on row {self.lexer.token.line}. Identifier must be unique in the same container."
                     raise QuerySyntaxError(
                         error_message,
                         unexpected_token=identifier,
                         row=self.lexer.token.line,
                         column=self.lexer.token.column,
                     )
                 identifier_name_list.add(identifier)
 
+            # We do not enforce description to be unique, but we need to advance the lexer
+            if self._peek(TokenKind.DESCRIPTION):
+                self._expect_token(TokenKind.DESCRIPTION)
+
             nodes.append(parse_fn(**kwargs))
 
             if self._peek(close_kind):
                 self.lexer.advance()
                 break
 
         return nodes
 
     def _expect_token(self, kind: TokenKind) -> Token:
-        """Consumes the next token if it matches the given kind, otherwise throws an
+        """Consumes the next token if it matches the given kind. Else, throw an
         error.
         """
         token = self.lexer.token
         if token.kind == kind:
             self.lexer.advance()
             return token
```

### Comparing `agentql-0.4.5/src/agentql/_core/_syntax/source.py` & `agentql-0.4.6/src/agentql/_core/_syntax/source.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.5/src/agentql/_core/_syntax/token.py` & `agentql-0.4.6/src/agentql/_core/_syntax/token.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.5/src/agentql/_core/_trail_logger/_trail_logger_impl.py` & `agentql-0.4.6/src/agentql/_core/_trail_logger/_trail_logger_impl.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.5/src/agentql/_core/_typing.py` & `agentql-0.4.6/src/agentql/_core/_typing.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.5/src/agentql/_core/_utils.py` & `agentql-0.4.6/src/agentql/_core/_utils.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.5/src/agentql/async_api/_agentql_service.py` & `agentql-0.4.6/src/agentql/sync_api/_agentql_service.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,114 +1,116 @@
+import json
 import os
 
-import httpx
+import requests
 
 from agentql import AgentQLServerError, AgentQLServerTimeoutError, APIKeyError
 from agentql._core._api_constants import (
     CHECK_SERVER_STATUS_ENDPOINT,
     GET_AGENTQL_ENDPOINT,
     SERVICE_URL,
     VALIDATE_API_KEY_ENDPOINT,
 )
-from agentql._core._utils import get_api_key_async
+from agentql._core._utils import get_api_key
 
 RESPONSE_ERROR_KEY = "detail"
 
 
-async def query_agentql_server(
-    query: str, accessibility_tree: dict, timeout: int, page_url: str
-) -> dict:
+def query_agentql_server(query: str, accessibility_tree: dict, timeout: int, page_url: str) -> dict:
     """Make Request to AgentQL Server's query endpoint.
 
     Parameters:
     ----------
     query (str): The query string.
     accessibility_tree (dict): The accessibility tree.
     timeout (int): The timeout value for the connection with backend api service
     page_url (str): The URL of the active page.
 
     Returns:
     -------
     dict: AgentQL response in json format.
     """
-    api_key = await get_api_key_async()
+    api_key = get_api_key()
     if not api_key:
         raise APIKeyError(
-            "API key not provided. Please set the environment variable 'AGENTQL_API_KEY' with your API key."
+            """
+            AgentQL API key not found.
+            Please set the AgentQL API key by invoking `agentql init` command or by setting the environment variable 'AGENTQL_API_KEY'.
+            You could refer to the documentation for more information: https://docs.agentql.com/docs/installation/sdk-installation.
+            """
         )
 
     try:
         request_data = {
             "query": f"{query}",
             "accessibility_tree": accessibility_tree,
             "metadata": {"url": page_url},
         }
         url = os.getenv("AGENTQL_API_HOST", SERVICE_URL) + GET_AGENTQL_ENDPOINT
         headers = {"X-API-Key": api_key}
-        async with httpx.AsyncClient() as client:
-            response = await client.post(
-                url, json=request_data, headers=headers, timeout=timeout, follow_redirects=True
-            )
-            response.raise_for_status()
-            return response.json()
-    except httpx.TimeoutException as e:
-        raise AgentQLServerTimeoutError() from e
-    except httpx.HTTPStatusError as e:
-        if e.response.status_code == 401:
+        response = requests.post(
+            url, json=request_data, headers=headers, timeout=timeout, allow_redirects=True
+        )
+        response.raise_for_status()
+        return response.json()
+    except requests.exceptions.RequestException as e:
+        if isinstance(e, requests.exceptions.ReadTimeout):
+            raise AgentQLServerTimeoutError() from e
+        if isinstance(e, requests.exceptions.HTTPError) and e.response.status_code == 401:
             raise APIKeyError(
-                "Invalid or expired API key provided. Please set the environment variable 'AGENTQL_API_KEY' with a valid API key."
+                """
+                Invalid or expired API key provided.
+                Please set a valid AgentQL API key by invoking `agentql init` command or by setting the environment variable 'AGENTQL_API_KEY'.
+                You could refer to the documentation for more information: https://docs.agentql.com/docs/installation/sdk-installation.
+                """
             ) from e
-        error_code = e.response.status_code
-        server_error = e.response.text
+        error_code = e.response.status_code if e.response is not None else None
+        server_error = e.response.content.decode("utf-8") if e.response is not None else None
         if server_error:
             try:
-                server_error_json = e.response.json()
+                server_error_json = json.loads(server_error)
                 if isinstance(server_error_json, dict):
                     server_error = server_error_json.get(RESPONSE_ERROR_KEY)
             except ValueError:
                 raise AgentQLServerError(server_error, error_code) from e
         raise AgentQLServerError(server_error, error_code) from e
-    except httpx.RequestError as e:
-        raise AgentQLServerError(str(e)) from e
 
 
-async def validate_api_key(api_key: str, timeout: int = 30):
+def validate_api_key(api_key: str, timeout: int = 30):
     """Validate the API key through the AgentQL service.
 
     Parameters:
     ----------
     api_key (str): The AGENTQL API key to validate.
 
     Returns:
     -------
     bool: True if the API key is valid, False otherwise.
     """
     try:
         url = os.getenv("AGENTQL_API_HOST", SERVICE_URL) + VALIDATE_API_KEY_ENDPOINT
         headers = {"X-API-Key": api_key}
-        async with httpx.AsyncClient() as client:
-            response = await client.get(url, headers=headers, timeout=timeout)
-            response.raise_for_status()
-            return True
-    except httpx.HTTPStatusError:
+        response = requests.get(url, headers=headers, timeout=timeout)
+        response.raise_for_status()
+        return True
+    except requests.exceptions.RequestException:
         return False
 
 
-async def check_agentql_server_status(timeout: int = 15) -> bool:
+def check_agentql_server_status(timeout: int = 15) -> bool:
     """Check the status of the AgentQL server.
 
     Parameters:
     ----------
-    timeout (int): The timeout value for the connection with backend API service.
+    timeout (int): The timeout value for the connection with backend api service.
 
     Returns:
     -------
     bool: True if the server is up and running, False otherwise.
     """
     try:
         url = os.getenv("AGENTQL_API_HOST", SERVICE_URL) + CHECK_SERVER_STATUS_ENDPOINT
-        async with httpx.AsyncClient() as client:
-            response = await client.get(url, timeout=timeout)
-            response.raise_for_status()
-            return True
-    except httpx.HTTPStatusError:
+        response = requests.get(url, timeout=timeout)
+        response.raise_for_status()
+        return True
+    except requests.exceptions.RequestException:
         return False
```

### Comparing `agentql-0.4.5/src/agentql/async_api/_api.py` & `agentql-0.4.6/src/agentql/async_api/_api.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.5/src/agentql/async_api/_popup.py` & `agentql-0.4.6/src/agentql/async_api/_popup.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.5/src/agentql/async_api/_response_proxy.py` & `agentql-0.4.6/src/agentql/async_api/_response_proxy.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.5/src/agentql/async_api/_session.py` & `agentql-0.4.6/src/agentql/async_api/_session.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,22 +109,26 @@
             wait_for_network_idle=wait_for_network_idle
         )
 
         accessibility_tree = await self._web_driver._prepare_accessibility_tree(
             lazy_load_pages_count=lazy_load_pages_count, include_aria_hidden=include_aria_hidden
         )
 
-        self._last_accessibility_tree = accessibility_tree
-
         # Check if there is a popup in the page before sending the agentql query
         popup_list = []
         if self._check_popup:
             popup_list = self._detect_popup(accessibility_tree, [])
             if popup_list:
                 await self._handle_popup(popup_list)
+                accessibility_tree = await self._web_driver._prepare_accessibility_tree(
+                    lazy_load_pages_count=lazy_load_pages_count,
+                    include_aria_hidden=include_aria_hidden,
+                )
+
+        self._last_accessibility_tree = accessibility_tree
 
         response = await query_agentql_server(
             query, accessibility_tree, timeout, self._web_driver.current_url
         )
         self._last_response = response
 
         # Check if there is a popup in the page after receiving the agentql response
```

### Comparing `agentql-0.4.5/src/agentql/async_api/_web_driver.py` & `agentql-0.4.6/src/agentql/async_api/_web_driver.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.5/src/agentql/experimental/async_api/_protocol/_browser.py` & `agentql-0.4.6/src/agentql/experimental/async_api/_protocol/_browser.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.5/src/agentql/experimental/async_api/_protocol/_page.py` & `agentql-0.4.6/src/agentql/experimental/async_api/_protocol/_page.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.5/src/agentql/experimental/sync_api/_protocol/_browser.py` & `agentql-0.4.6/src/agentql/experimental/sync_api/_protocol/_browser.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.5/src/agentql/experimental/sync_api/_protocol/_page.py` & `agentql-0.4.6/src/agentql/experimental/sync_api/_protocol/_page.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.5/src/agentql/ext/playwright/_html_constants.py` & `agentql-0.4.6/src/agentql/ext/playwright/_html_constants.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.5/src/agentql/ext/playwright/_network_monitor.py` & `agentql-0.4.6/src/agentql/ext/playwright/_network_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,9 +109,10 @@
 
     def reset(self):
         """Reset the network monitor."""
         self._request_log = {}
         self._response_log = set()
         self._last_network_active_time = time.time()
         self._multi_request_found = False
+        self._multi_request_url = ""
         self._start_time = time.time()
         self._page_loaded = False
```

### Comparing `agentql-0.4.5/src/agentql/ext/playwright/playwright_driver_async.py` & `agentql-0.4.6/src/agentql/ext/playwright/playwright_driver_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import random
 import time
 from typing import Optional, Union
 
 from playwright.async_api import (
     ElementHandle,
     Error,
     Frame,
@@ -19,14 +20,15 @@
     AccessibilityTreeError,
     AgentQLServerError,
     AttributeNotFoundError,
     ElementNotFoundError,
     NoOpenBrowserError,
     NoOpenPageError,
     OpenUrlError,
+    PageMonitorNotInitializedError,
     UnableToClosePopupError,
 )
 from agentql._core._js_snippets.snippet_loader import load_js
 from agentql._core._utils import ensure_url_scheme
 from agentql.async_api import ScrollDirection, WebDriver
 from agentql.async_api._agentql_service import query_agentql_server
 from agentql.async_api._response_proxy import AQLResponseProxy
@@ -239,51 +241,64 @@
         if not self._page_monitor:
             self._page_monitor = PageActivityMonitor()
         else:
             # Reset the network monitor to clear the logs
             self._page_monitor.reset()
 
         # Add event listeners to track DOM changes and network activities
-        await self._add_page_event_listeners()
+        await self._add_event_listeners_for_page_monitor()
 
         # Wait for the page to reach the "Page Ready" state
         await self._determine_load_state(
             self._page_monitor, wait_for_network_idle=wait_for_network_idle
         )
 
         # Remove the event listeners to prevent overwhelming the async event loop
-        await self._remove_page_event_listeners()
+        await self._remove_event_listeners_for_page_monitor()
 
     async def scroll_page(self, scroll_direction: ScrollDirection, pixels: int = 720):
         """Scrolls the page up or down by given pixels. By default, it will scroll 720 pixels.
 
         Parameters:
         -----------
         scroll_direction (ScrollDirection): An enumeration class that represents the direction in which a scroll action can occur. Currently, it has `UP` and `DOWN` member.
         pixels (int) (optional): The number of pixels to scroll. 720 by default.
         """
         if not self._current_page:
             raise NoOpenPageError()
 
+        await self.wait_for_page_ready_state()
         delta_y = pixels if scroll_direction == ScrollDirection.DOWN else -pixels
         await self._current_page.mouse.wheel(delta_x=0, delta_y=delta_y)
 
     async def scroll_to_bottom(self):
         """Scrolls to the bottom of the current page."""
         if not self._current_page:
             raise NoOpenPageError()
 
-        await self._current_page.evaluate(load_js("scroll_to_bottom"))
+        await self.wait_for_page_ready_state()
+        height_information = await self._current_page.evaluate(load_js("get_scroll_info"))
+        viewport_height, total_height, scroll_height = height_information
+        while scroll_height < total_height:
+            scroll_height = scroll_height + viewport_height
+            await self._current_page.mouse.wheel(delta_x=0, delta_y=viewport_height)
+            await asyncio.sleep(random.uniform(0.05, 0.1))
 
     async def scroll_to_top(self):
         """Scrolls to the top of the current page."""
         if not self._current_page:
             raise NoOpenPageError()
 
-        await self._current_page.evaluate(load_js("scroll_to_top"))
+        await self.wait_for_page_ready_state()
+        height_information = await self._current_page.evaluate(load_js("get_scroll_info"))
+        viewport_height, scroll_height = height_information[0], height_information[2]
+        while scroll_height > 0:
+            scroll_height = scroll_height - viewport_height
+            await self._current_page.mouse.wheel(delta_x=0, delta_y=-viewport_height)
+            await asyncio.sleep(random.uniform(0.05, 0.1))
 
     async def _close_popup(self, popup_tree: dict, page_url: str, timeout: int = 500):
         """Close the popup by querying AgentQL server for the close button and perform a click action with web driver.
 
         Parameters:
         -----------
         popup_tree (dict): The accessibility tree that has the popup node as the parent.
@@ -517,15 +532,15 @@
         Returns:
         --------
 
         [Playwright Locator](https://playwright.dev/python/docs/api/class-locator): The web element represented by Playwright's Locator object.
         """
         tf623_id = response_data.get("tf623_id")
         if not tf623_id:
-            raise ElementNotFoundError("tf623_id")
+            raise ElementNotFoundError(self.current_page.url, "tf623_id")
         iframe_path = response_data.get("attributes", {}).get("iframe_path")
         interactive_element = self._find_element_by_id(tf623_id, iframe_path)
         trail_logger.spy_on_object(interactive_element)
         return interactive_element
 
     async def _apply_stealth_mode_to_page(self, page: Page):
         """Applies stealth mode to the given page.
@@ -567,15 +582,15 @@
         try:
             page = await self._context.new_page()
             if self._stealth_mode_config is not None:
                 await self._apply_stealth_mode_to_page(page)
             self._current_tf_id = 0
             await page.goto(url, wait_until="domcontentloaded")
         except Exception as e:
-            raise OpenUrlError() from e
+            raise OpenUrlError(url) from e
 
         self._current_page = page
 
     async def _set_iframe_path(self, context: Union[Page, Frame], iframe_path=None):
         """
         Sets the iframe path in the given context.
 
@@ -710,27 +725,27 @@
         ------
         ElementNotFoundError: If the element with the specified TF ID is not found.
         """
         try:
             element_frame_context = self._get_frame_context(iframe_path)
             return element_frame_context.locator(f"[tf623_id='{tf623_id}']")
         except Exception as e:
-            raise ElementNotFoundError(tf623_id) from e
+            raise ElementNotFoundError(self.current_page.url, tf623_id) from e
 
     async def _determine_load_state(
         self,
         monitor: PageActivityMonitor,
         timeout_seconds: int = 14,
         wait_for_network_idle: bool = True,
     ):
         if not self._current_page:
             raise NoOpenPageError()
 
         if not self._page_monitor:
-            raise ValueError("Page monitor is not initialized.")
+            raise PageMonitorNotInitializedError()
 
         start_time = time.time()
 
         while True:
             if wait_for_network_idle:
                 try:
                     last_updated_timestamp = await self._current_page.evaluate(
@@ -753,20 +768,20 @@
                     break
 
             if time.time() - start_time > timeout_seconds:
                 trail_logger.add_event("Page ready: Timeout while waiting for page to settle.")
                 break
             await asyncio.sleep(0.1)
 
-    async def _add_page_event_listeners(self):
+    async def _add_event_listeners_for_page_monitor(self):
         if not self._current_page:
             raise NoOpenPageError()
 
         if not self._page_monitor:
-            raise ValueError("Page monitor is not initialized.")
+            raise PageMonitorNotInitializedError()
 
         self._current_page.on("request", self._page_monitor.track_network_request)
         self._current_page.on("requestfinished", self._page_monitor.track_network_response)
         self._current_page.on("requestfailed", self._page_monitor.track_network_response)
         self._current_page.on("load", self._page_monitor.track_load)
 
         try:
@@ -775,20 +790,20 @@
         except Error:
             start_time = time.time()
             while True:
                 if self._page_monitor.get_load_status() or time.time() - start_time > 6:
                     break
                 await asyncio.sleep(0.2)
 
-    async def _remove_page_event_listeners(self):
+    async def _remove_event_listeners_for_page_monitor(self):
         if not self._current_page:
             raise NoOpenPageError()
 
         if not self._page_monitor:
-            raise ValueError("Page monitor is not initialized.")
+            raise PageMonitorNotInitializedError()
 
         self._current_page.remove_listener("request", self._page_monitor.track_network_request)
         self._current_page.remove_listener(
             "requestfinished", self._page_monitor.track_network_response
         )
         self._current_page.remove_listener(
             "requestfailed", self._page_monitor.track_network_response
```

### Comparing `agentql-0.4.5/src/agentql/ext/playwright/playwright_driver_sync.py` & `agentql-0.4.6/src/agentql/ext/playwright/playwright_driver_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import random
 import time
 from typing import Optional, Union
 
 from playwright.sync_api import (
     ElementHandle,
     Error,
     Frame,
@@ -18,14 +19,15 @@
     AccessibilityTreeError,
     AgentQLServerError,
     AttributeNotFoundError,
     ElementNotFoundError,
     NoOpenBrowserError,
     NoOpenPageError,
     OpenUrlError,
+    PageMonitorNotInitializedError,
     UnableToClosePopupError,
 )
 from agentql._core._js_snippets.snippet_loader import load_js
 from agentql._core._utils import ensure_url_scheme
 from agentql.sync_api import ScrollDirection, WebDriver
 from agentql.sync_api._agentql_service import query_agentql_server
 from agentql.sync_api._response_proxy import AQLResponseProxy
@@ -256,21 +258,21 @@
         if not self._page_monitor:
             self._page_monitor = PageActivityMonitor()
         else:
             # Reset the network monitor to clear the logs
             self._page_monitor.reset()
 
         # Add event listeners to track DOM changes and network activities
-        self._add_page_event_listeners()
+        self._add_event_listeners_for_page_monitor()
 
         # Wait for the page to reach the "Page Ready" state
         self._determine_load_state(self._page_monitor, wait_for_network_idle=wait_for_network_idle)
 
         # Remove the event listeners to prevent overwhelming the async event loop
-        self._remove_page_event_listeners()
+        self._remove_event_listeners_for_page_monitor()
 
         trail_logger.add_event(
             f"Finished waiting for {self._current_page} to reach 'Page Ready' state"
         )
 
     def scroll_page(self, scroll_direction: ScrollDirection, pixels: int = 720):
         """Scrolls the page up or down by given pixels. By default, it will scroll 720 pixels.
@@ -279,30 +281,43 @@
         -----------
         scroll_direction (ScrollDirection): An enumeration class that represents the direction in which a scroll action can occur. Currently, it has `UP` and `DOWN` member.
         pixels (int) (optional): The number of pixels to scroll. 720 by default.
         """
         if not self._current_page:
             raise NoOpenPageError()
 
+        self.wait_for_page_ready_state()
         delta_y = pixels if scroll_direction == ScrollDirection.DOWN else -pixels
         self._current_page.mouse.wheel(delta_x=0, delta_y=delta_y)
 
     def scroll_to_bottom(self):
         """Scrolls to the bottom of the current page."""
         if not self._current_page:
             raise NoOpenPageError()
 
-        self._current_page.evaluate(load_js("scroll_to_bottom"))
+        self.wait_for_page_ready_state()
+        height_information = self._current_page.evaluate(load_js("get_scroll_info"))
+        viewport_height, total_height, scroll_height = height_information
+        while scroll_height < total_height:
+            scroll_height = scroll_height + viewport_height
+            self._current_page.mouse.wheel(delta_x=0, delta_y=viewport_height)
+            time.sleep(random.uniform(0.05, 0.1))
 
     def scroll_to_top(self):
         """Scrolls to the top of the current page."""
         if not self._current_page:
             raise NoOpenPageError()
 
-        self._current_page.evaluate(load_js("scroll_to_top"))
+        self.wait_for_page_ready_state()
+        height_information = self._current_page.evaluate(load_js("get_scroll_info"))
+        viewport_height, scroll_height = height_information[0], height_information[2]
+        while scroll_height > 0:
+            scroll_height = scroll_height - viewport_height
+            self._current_page.mouse.wheel(delta_x=0, delta_y=-viewport_height)
+            time.sleep(random.uniform(0.05, 0.1))
 
     def _close_popup(self, popup_tree: dict, page_url: str, timeout: int = 500):
         """Close the popup by querying AgentQL server for the close button and perform a click action with web driver.
 
         Parameters:
         -----------
         popup_tree (dict): The accessibility tree that has the popup node as the parent.
@@ -349,15 +364,15 @@
         Returns:
         --------
 
         [Playwright Locator](https://playwright.dev/python/docs/api/class-locator): The web element represented by Playwright's Locator object.
         """
         tf623_id = response_data.get("tf623_id")
         if not tf623_id:
-            raise ElementNotFoundError("tf623_id")
+            raise ElementNotFoundError(self.current_page.url, "tf623_id")
         iframe_path = response_data.get("attributes", {}).get("iframe_path")
         interactive_element = self._find_element_by_id(tf623_id, iframe_path)
         trail_logger.spy_on_object(interactive_element)
         return interactive_element
 
     def _prepare_accessibility_tree(
         self, lazy_load_pages_count: int = 3, include_aria_hidden: bool = False
@@ -382,15 +397,14 @@
         try:
             accessibility_tree = self._get_page_accessibility_tree(
                 self._current_page, include_aria_hidden=include_aria_hidden
             )
             self._process_iframes(accessibility_tree)
             self._post_process_accessibility_tree(accessibility_tree)
             return accessibility_tree
-
         except Exception as e:
             raise AccessibilityTreeError() from e
 
     def _post_process_accessibility_tree(self, accessibility_tree: dict):
         """Post-process the accessibility tree by removing node's attributes that are Null."""
         if "children" in accessibility_tree and accessibility_tree.get("children") is None:
             del accessibility_tree["children"]
@@ -593,15 +607,15 @@
         try:
             page = self._context.new_page()
             if self._stealth_mode_config is not None:
                 self._apply_stealth_mode_to_page(page)
             self._current_tf_id = 0
             page.goto(url, wait_until="domcontentloaded")
         except Exception as e:
-            raise OpenUrlError() from e
+            raise OpenUrlError(url) from e
 
         self._current_page = page
 
     def _set_iframe_path(self, context: Union[Page, Frame], iframe_path=None):
         """
         Sets the iframe path in the given context.
 
@@ -716,27 +730,27 @@
         ------
         ElementNotFoundError: If the element with the specified TF ID is not found.
         """
         try:
             element_frame_context = self._get_frame_context(iframe_path)
             return element_frame_context.locator(f"[tf623_id='{tf623_id}']")
         except Exception as e:
-            raise ElementNotFoundError(tf623_id) from e
+            raise ElementNotFoundError(self.current_page.url, tf623_id) from e
 
     def _determine_load_state(
         self,
         monitor: PageActivityMonitor,
         timeout_seconds: int = 14,
         wait_for_network_idle: bool = True,
     ):
         if not self._current_page:
             raise NoOpenPageError()
 
         if not self._page_monitor:
-            raise ValueError("Page monitor is not initialized.")
+            raise PageMonitorNotInitializedError()
 
         start_time = time.time()
 
         while True:
             if wait_for_network_idle:
                 try:
                     last_updated_timestamp = self._current_page.evaluate(
@@ -758,20 +772,20 @@
                     trail_logger.add_event("Page ready: Page emitted 'load' event.")
                     break
             if time.time() - start_time > timeout_seconds:
                 trail_logger.add_event("Page ready: Timeout while waiting for page to settle.")
                 break
             time.sleep(0.1)
 
-    def _add_page_event_listeners(self):
+    def _add_event_listeners_for_page_monitor(self):
         if not self._current_page:
             raise NoOpenPageError()
 
         if not self._page_monitor:
-            raise ValueError("Page monitor is not initialized.")
+            raise PageMonitorNotInitializedError()
 
         self._current_page.on("request", self._page_monitor.track_network_request)
         self._current_page.on("requestfinished", self._page_monitor.track_network_response)
         self._current_page.on("requestfailed", self._page_monitor.track_network_response)
         self._current_page.on("load", self._page_monitor.track_load)
 
         try:
@@ -780,20 +794,20 @@
         except Error:
             start_time = time.time()
             while True:
                 if self._page_monitor.get_load_status() or time.time() - start_time > 6:
                     break
                 time.sleep(0.2)
 
-    def _remove_page_event_listeners(self):
+    def _remove_event_listeners_for_page_monitor(self):
         if not self._current_page:
             raise NoOpenPageError()
 
         if not self._page_monitor:
-            raise ValueError("Page monitor is not initialized.")
+            raise PageMonitorNotInitializedError()
 
         self._current_page.remove_listener("request", self._page_monitor.track_network_request)
         self._current_page.remove_listener(
             "requestfinished", self._page_monitor.track_network_response
         )
         self._current_page.remove_listener(
             "requestfailed", self._page_monitor.track_network_response
```

### Comparing `agentql-0.4.5/src/agentql/sync_api/_api.py` & `agentql-0.4.6/src/agentql/sync_api/_api.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.5/src/agentql/sync_api/_popup.py` & `agentql-0.4.6/src/agentql/sync_api/_popup.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.5/src/agentql/sync_api/_response_proxy.py` & `agentql-0.4.6/src/agentql/sync_api/_response_proxy.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.5/src/agentql/sync_api/_session.py` & `agentql-0.4.6/src/agentql/sync_api/_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,22 +116,27 @@
         query_tree = parser.parse()
 
         self._web_driver.wait_for_page_ready_state(wait_for_network_idle)
 
         accessibility_tree = self._web_driver._prepare_accessibility_tree(
             lazy_load_pages_count=lazy_load_pages_count, include_aria_hidden=include_aria_hidden
         )
-        self._last_accessibility_tree = accessibility_tree
 
         popup_list = []
         # Check if there is a popup in the page before sending the agentql query
         if self._check_popup:
             popup_list = self._detect_popup(accessibility_tree, [])
             if popup_list:
                 self._handle_popup(popup_list)
+                accessibility_tree = self._web_driver._prepare_accessibility_tree(
+                    lazy_load_pages_count=lazy_load_pages_count,
+                    include_aria_hidden=include_aria_hidden,
+                )
+
+        self._last_accessibility_tree = accessibility_tree
 
         response = query_agentql_server(
             query, accessibility_tree, timeout, self._web_driver.current_url
         )
         self._last_response = response
 
         # Check if there is a popup in the page after receiving the agentql response
```

### Comparing `agentql-0.4.5/src/agentql/sync_api/_web_driver.py` & `agentql-0.4.6/src/agentql/sync_api/_web_driver.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.5/PKG-INFO` & `agentql-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentql
-Version: 0.4.5
+Version: 0.4.6
 Summary: Tiny Fish AgentQL Python Client
 License: MIT
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

