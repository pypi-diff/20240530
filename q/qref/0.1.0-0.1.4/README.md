# Comparing `tmp/qref-0.1.0.tar.gz` & `tmp/qref-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qref-0.1.0.tar", max compression
+gzip compressed data, was "qref-0.1.4.tar", max compression
```

## Comparing `qref-0.1.0.tar` & `qref-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    11356 2024-04-24 19:32:15.940256 qref-0.1.0/LICENSE
--rw-r--r--   0        0        0     3649 2024-04-24 19:32:15.941392 qref-0.1.0/README.md
--rw-r--r--   0        0        0      931 2024-04-24 19:32:15.954882 qref-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1342 2024-04-24 19:32:15.956820 qref-0.1.0/src/qref/__init__.py
--rw-r--r--   0        0        0     3684 2024-04-24 19:32:15.957759 qref-0.1.0/src/qref/_schema_v1.py
--rw-r--r--   0        0        0      582 2024-04-24 19:32:15.959657 qref-0.1.0/src/qref/experimental/__init__.py
--rw-r--r--   0        0        0     6805 2024-04-24 19:32:15.960637 qref-0.1.0/src/qref/experimental/rendering.py
--rw-r--r--   0        0        0     4237 1970-01-01 00:00:00.000000 qref-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-30 16:57:36.142609 qref-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4039 2024-05-30 16:57:36.142609 qref-0.1.4/README.md
+-rw-r--r--   0        0        0     1070 2024-05-30 16:57:36.146609 qref-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1342 2024-05-30 16:57:36.146609 qref-0.1.4/src/qref/__init__.py
+-rw-r--r--   0        0        0     4031 2024-05-30 16:57:36.146609 qref-0.1.4/src/qref/_schema_v1.py
+-rw-r--r--   0        0        0      581 2024-05-30 16:57:36.146609 qref-0.1.4/src/qref/experimental/__init__.py
+-rw-r--r--   0        0        0     6805 2024-05-30 16:57:36.146609 qref-0.1.4/src/qref/experimental/rendering.py
+-rw-r--r--   0        0        0        0 2024-05-30 16:57:36.146609 qref-0.1.4/src/qref/py.typed
+-rw-r--r--   0        0        0     4627 1970-01-01 00:00:00.000000 qref-0.1.4/PKG-INFO
```

### Comparing `qref-0.1.0/LICENSE` & `qref-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qref-0.1.0/README.md` & `qref-0.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 - Rudimentary visualization tool `qref-render`.
 
 ## Installation
 
 Using QREF data format does not require installation - you can easily write quantum
 programs in YAML or JSON.
 
-To install QREF Python package, clone this repository and install it as usual with `pip`:
+To install QREF Python package, run `pip install qref`.
+
+Alternatively, you can clone this repository and build it from source:
 
 ```bash
 # Clone QREF repo (you can use HTTP link as well)
 git clone git@github.com:PsiQ/qref.git
 cd qref
 pip install .
 ```
@@ -30,15 +32,15 @@
 - *hierarchical*: each node can contain subgraphs, i.e. routines can be nested inside
   larger routines.
 - *directed*: information flow is unidirectional, and the direction is unambiguous.
 - *acyclic*: meaning there are no loops.
 
 Consider the following hierarchical DAG of a hypothetical quantum program:
 
-![program example](example_routine.svg)
+![program example](https://raw.githubusercontent.com/PsiQ/qref/main/example_routine.svg)
 
 It can be succinctly written in QREF format as:
 
 
 ```yaml
 version: v1
 program:
@@ -99,15 +101,15 @@
   - source: subroutine_2.out_1
     target: merge.in_1
   - source: merge.out_0
     target: out_0
 ```
 
 
-For full description of QREF format, check our [docs](https://example.com).
+For full description of QREF format, check our [docs](https://psiq.github.io/qref/latest/).
 
 ## Using QREF package
 
 ### Using JSON schema for validating data in QREF format
 
 JSON schema for QREF format can be obtained by calling `generate_program_schema` function.
 Such schema can be then used for validating user's input, e.g. using `jsonschema` package:
@@ -137,8 +139,15 @@
 
 # This will raise if data is not valid
 program = SchemaV1.model_validate(data)
 ```
 
 ## Development
 
-In order to install development environment or build documentation locally, please refer to [Development Guide](TODO).
+In order to install development environment or build documentation locally, please refer to [Development Guide](https://psiq.github.io/qref/latest/development/).
+
+
+## Documentation
+
+Documentation for `qref` can be found [here](https://psiq.github.io/qref/latest/).
+
+To run docs locally install it with `docs` option: `pip install ".[docs]"` (or `poetry install --with docs`) and then run `mkdocs serve`.
```

### Comparing `qref-0.1.0/pyproject.toml` & `qref-0.1.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qref"
-version = "0.1.0"
+version = "0.1.4"
 description = "Quantum Resource Estimation Format"
 authors = ["PsiQuantum, Corp."]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -29,18 +29,22 @@
 mkdocs-open-in-new-tab = "^1.0.3"
 mkdocstrings = {version = "^0.24.2", extras = ["python"]}
 mike = "^2.0.0"
 
 [tool.poetry.scripts]
 qref-render = "qref.experimental.rendering:render_entry_point"
 
+[tool.poetry-dynamic-versioning]
+enable = true
+pattern = "default-unprefixed"
+
 
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
+build-backend = "poetry_dynamic_versioning.backend"
 
 
 [tool.black]
 line-length = 100
 target-version = ['py39']
```

### Comparing `qref-0.1.0/src/qref/__init__.py` & `qref-0.1.4/src/qref/__init__.py`

 * *Files identical despite different names*

### Comparing `qref-0.1.0/src/qref/_schema_v1.py` & `qref-0.1.4/src/qref/_schema_v1.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,28 +14,39 @@
 
 """Pydantic models used for defining V1 schema of Routine."""
 
 from __future__ import annotations
 
 from typing import Annotated, Any, Literal, Optional, Union
 
-from pydantic import BaseModel, ConfigDict, Field, StringConstraints
+from pydantic import AfterValidator, BaseModel, ConfigDict, Field, StringConstraints
 from pydantic.json_schema import GenerateJsonSchema
 
 NAME_PATTERN = "[A-Za-z_][A-Za-z0-9_]*"
 NAMESPACED_NAME_PATTERN = rf"{NAME_PATTERN}\.{NAME_PATTERN}"
 
 Name = Annotated[str, StringConstraints(pattern=rf"^{NAME_PATTERN}$")]
 NamespacedName = Annotated[str, StringConstraints(pattern=rf"^{NAMESPACED_NAME_PATTERN}")]
 OptionallyNamespacedName = Annotated[
     str, StringConstraints(pattern=rf"^(({NAME_PATTERN})|({NAMESPACED_NAME_PATTERN}))$")
 ]
 _Value = Union[int, float, str]
 
 
+def sorter(key):
+    def _inner(v):
+        return sorted(v, key=key)
+
+    return _inner
+
+
+name_sorter = AfterValidator(sorter(lambda p: p.name))
+source_sorter = AfterValidator(sorter(lambda c: c.source))
+
+
 class _PortV1(BaseModel):
     name: Name
     direction: Literal["input", "output", "through"]
     size: Optional[_Value]
     model_config = ConfigDict(title="Port")
 
 
@@ -66,22 +77,22 @@
 
     Note:
         This is NOT a top-level object in the schema. Instead, RoutineV1 is wrapped in
         SchemaV1.
     """
 
     name: Name
-    children: list[RoutineV1] = Field(default_factory=list)
+    children: Annotated[list[RoutineV1], name_sorter] = Field(default_factory=list)
     type: Optional[str] = None
-    ports: list[_PortV1] = Field(default_factory=list)
-    resources: list[_ResourceV1] = Field(default_factory=list)
-    connections: list[_ConnectionV1] = Field(default_factory=list)
+    ports: Annotated[list[_PortV1], name_sorter] = Field(default_factory=list)
+    resources: Annotated[list[_ResourceV1], name_sorter] = Field(default_factory=list)
+    connections: Annotated[list[_ConnectionV1], source_sorter] = Field(default_factory=list)
     input_params: list[Name] = Field(default_factory=list)
     local_variables: list[str] = Field(default_factory=list)
-    linked_params: list[_ParamLinkV1] = Field(default_factory=list)
+    linked_params: Annotated[list[_ParamLinkV1], source_sorter] = Field(default_factory=list)
     meta: dict[str, Any] = Field(default_factory=dict)
 
     model_config = ConfigDict(title="Routine")
 
     def __init__(self, **data: Any):
         super().__init__(**{k: v for k, v in data.items() if v != [] and v != {}})
```

### Comparing `qref-0.1.0/src/qref/experimental/__init__.py` & `qref-0.1.4/src/qref/experimental/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `qref-0.1.0/src/qref/experimental/rendering.py` & `qref-0.1.4/src/qref/experimental/rendering.py`

 * *Files identical despite different names*

### Comparing `qref-0.1.0/PKG-INFO` & `qref-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qref
-Version: 0.1.0
+Version: 0.1.4
 Summary: Quantum Resource Estimation Format
 License: Apache 2.0
 Author: PsiQuantum, Corp.
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -26,15 +26,17 @@
 - Rudimentary visualization tool `qref-render`.
 
 ## Installation
 
 Using QREF data format does not require installation - you can easily write quantum
 programs in YAML or JSON.
 
-To install QREF Python package, clone this repository and install it as usual with `pip`:
+To install QREF Python package, run `pip install qref`.
+
+Alternatively, you can clone this repository and build it from source:
 
 ```bash
 # Clone QREF repo (you can use HTTP link as well)
 git clone git@github.com:PsiQ/qref.git
 cd qref
 pip install .
 ```
@@ -47,15 +49,15 @@
 - *hierarchical*: each node can contain subgraphs, i.e. routines can be nested inside
   larger routines.
 - *directed*: information flow is unidirectional, and the direction is unambiguous.
 - *acyclic*: meaning there are no loops.
 
 Consider the following hierarchical DAG of a hypothetical quantum program:
 
-![program example](example_routine.svg)
+![program example](https://raw.githubusercontent.com/PsiQ/qref/main/example_routine.svg)
 
 It can be succinctly written in QREF format as:
 
 
 ```yaml
 version: v1
 program:
@@ -116,15 +118,15 @@
   - source: subroutine_2.out_1
     target: merge.in_1
   - source: merge.out_0
     target: out_0
 ```
 
 
-For full description of QREF format, check our [docs](https://example.com).
+For full description of QREF format, check our [docs](https://psiq.github.io/qref/latest/).
 
 ## Using QREF package
 
 ### Using JSON schema for validating data in QREF format
 
 JSON schema for QREF format can be obtained by calling `generate_program_schema` function.
 Such schema can be then used for validating user's input, e.g. using `jsonschema` package:
@@ -154,8 +156,16 @@
 
 # This will raise if data is not valid
 program = SchemaV1.model_validate(data)
 ```
 
 ## Development
 
-In order to install development environment or build documentation locally, please refer to [Development Guide](TODO).
+In order to install development environment or build documentation locally, please refer to [Development Guide](https://psiq.github.io/qref/latest/development/).
+
+
+## Documentation
+
+Documentation for `qref` can be found [here](https://psiq.github.io/qref/latest/).
+
+To run docs locally install it with `docs` option: `pip install ".[docs]"` (or `poetry install --with docs`) and then run `mkdocs serve`. 
+
```

