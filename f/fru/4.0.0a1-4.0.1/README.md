# Comparing `tmp/fru-4.0.0a1.tar.gz` & `tmp/fru-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fru-4.0.0a1.tar", max compression
+gzip compressed data, was "fru-4.0.1.tar", max compression
```

## Comparing `fru-4.0.0a1.tar` & `fru-4.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2021-05-10 12:27:59.681306 fru-4.0.0a1/LICENSE.txt
--rw-r--r--   0        0        0     1636 2021-05-22 19:41:44.407087 fru-4.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     5696 2021-05-10 12:27:59.681306 fru-4.0.0a1/README.md
--rw-r--r--   0        0        0      319 2021-05-22 19:41:44.407087 fru-4.0.0a1/src/fru/__init__.py
--rw-r--r--   0        0        0      311 2021-05-22 19:41:44.407087 fru-4.0.0a1/src/fru/__main__.py
--rw-r--r--   0        0        0     3108 2021-05-22 19:41:44.407087 fru-4.0.0a1/src/fru/console.py
--rw-r--r--   0        0        0      787 2021-05-22 19:41:44.407087 fru-4.0.0a1/src/fru/exceptions.py
--rw-r--r--   0        0        0    10636 2021-05-22 19:41:44.422711 fru-4.0.0a1/src/fru/fru_format.py
--rw-r--r--   0        0        0     2644 2021-05-22 19:41:44.422711 fru-4.0.0a1/src/fru/shared.py
--rw-r--r--   0        0        0    11856 2021-05-22 19:41:44.422711 fru-4.0.0a1/src/fru/toml_format.py
--rw-r--r--   0        0        0     6707 2021-05-22 19:44:05.153646 fru-4.0.0a1/setup.py
--rw-r--r--   0        0        0     6865 2021-05-22 19:44:05.153646 fru-4.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-05-30 15:49:37.030626 fru-4.0.1/CHANGELOG.rst
+-rw-r--r--   0        0        0     1074 2024-05-29 15:01:43.920237 fru-4.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     5462 2024-05-29 15:01:43.920237 fru-4.0.1/README.rst
+-rw-r--r--   0        0        0     1842 2024-05-30 15:49:37.030626 fru-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0      334 2024-05-29 15:01:43.920237 fru-4.0.1/src/fru/__init__.py
+-rw-r--r--   0        0        0      307 2024-05-29 15:01:43.920237 fru-4.0.1/src/fru/__main__.py
+-rw-r--r--   0        0        0     3224 2024-05-29 15:01:43.920237 fru-4.0.1/src/fru/console.py
+-rw-r--r--   0        0        0      787 2024-05-29 15:01:43.920237 fru-4.0.1/src/fru/exceptions.py
+-rw-r--r--   0        0        0    10934 2024-05-29 15:01:43.920237 fru-4.0.1/src/fru/fru_format.py
+-rw-r--r--   0        0        0     2645 2024-05-29 15:01:43.920237 fru-4.0.1/src/fru/shared.py
+-rw-r--r--   0        0        0    11257 2024-05-30 15:49:37.030626 fru-4.0.1/src/fru/toml_format.py
+-rw-r--r--   0        0        0     6624 1970-01-01 00:00:00.000000 fru-4.0.1/PKG-INFO
```

### Comparing `fru-4.0.0a1/LICENSE.txt` & `fru-4.0.1/LICENSE.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `fru-4.0.0a1/pyproject.toml` & `fru-4.0.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 [tool.poetry]
 name = "fru"
-version = "4.0.0a1"
+version = "4.0.1"
 description = "Read and write binary FRU files"
 authors = [
     "Kurt McKee <contactme@kurtmckee.org>",
     "Ganesh Viswanathan <dev@genotrance.com>",
 ]
 license = "MIT"
-readme = "README.md"
+readme = "README.rst"
+include = [
+    "CHANGELOG.rst",
+]
 repository = "https://github.com/kurtmckee/fru-tool/"
 keywords = ["fru", "ipmi"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Customer Service",
     "Intended Audience :: Developers",
     "Intended Audience :: Manufacturing",
@@ -19,67 +22,87 @@
     "Operating System :: OS Independent",
     "Topic :: System :: Hardware",
     "Topic :: Utilities",
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = ">=3.8"
 click = "^8.0.0"
-importlib-metadata = { version = "^4.0.1", python = "<3.8" }
-toml = "^0.10.2"
-
-
-[tool.poetry.dev-dependencies]
-tox = "^3.23.1"
+tomli = { version = "^2.0.1", python = "<3.11" }
 
 
 [tool.poetry.scripts]
 frutool = 'fru.console:run'
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
-[tool.tox]
-legacy_tox_ini = """
-
-[tox]
-envlist =
-    coverage_erase
-    py{39, 38, 37, 36}
-    coverage_report
-skip_missing_interpreters = True
-isolated_build = True
-
-[testenv]
-deps =
-    pytest
-    pytest-cov
-commands =
-    {envpython} -m pytest --cov=fru --cov=tests --cov-append --cov-report=term
-
-[testenv:coverage_erase]
-skipsdist = true
-skip_install = true
-deps = coverage[toml]
-commands = coverage erase
-
-[testenv:coverage_report]
-skipsdist = true
-skip_install = true
-deps = coverage[toml]
-commands = coverage html -d htmlcov
-"""
-
+# coverage
+# --------
 
 [tool.coverage.run]
 branch = true
-
+parallel = true
+source = [
+    "fru",
+    "tests",
+]
 
 [tool.coverage.paths]
 source = [
     "src",
-    ".tox/*/site-packages",
+    "*/site-packages",
+]
+
+[tool.coverage.report]
+fail_under = 82
+
+
+# mypy
+# ----
+#
+#[tool.mypy]
+#packages = "src.fru"
+#strict = true
+#sqlite_cache = true
+
+
+# isort
+# -----
+
+[tool.isort]
+profile = "black"
+
+
+# pytest
+# ------
+[tool.pytest.ini_options]
+addopts = "--color=yes"
+filterwarnings = [
+    "error",
+]
+
+
+# scriv
+# -----
+
+[tool.scriv]
+version = "literal: pyproject.toml: tool.poetry.version"
+categories = [
+    "Python support",
+    "Added",
+    "Fixed",
+    "Removed",
+    "Changed",
+    "Deprecated",
+    "Security",
+    "Documentation",
 ]
+entry_title_template = "{{ version }} - {{ date.strftime('%Y-%m-%d') }}"
+format = "rst"
+fragment_directory = "changelog.d"
+insert_marker = "scriv-insert-here"
+main_branches = ["main", "releases"]
```

### Comparing `fru-4.0.0a1/src/fru/console.py` & `fru-4.0.1/src/fru/console.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,94 +1,124 @@
 # fru - Read and write binary IPMI FRU files
-# Copyright 2018-2021 Kurt McKee <contactme@kurtmckee.org>
+# Copyright 2018-2024 Kurt McKee <contactme@kurtmckee.org>
 # Copyright 2017 Dell Technologies
 #
 # https://github.com/kurtmckee/fru-tool/
 #
 # Licensed under the terms of the MIT License:
 # https://opensource.org/licenses/MIT
 
 
-import json
-import os
 import pathlib
 import sys
 
 import click
 
-from . import fru_format
-from . import toml_format
+from . import fru_format, toml_format
 
 
 @click.group()
 @click.version_option()
 def run():
     pass
 
 
-@click.command('generate', no_args_is_help=True)
-@click.argument('toml_file', type=click.Path(exists=True, dir_okay=False, resolve_path=True, path_type=pathlib.Path))
-@click.argument('fru_file', type=click.Path(exists=False, dir_okay=False, resolve_path=True, path_type=pathlib.Path))
-@click.option('--force', is_flag=True, help='Overwrite an existing file if it already exists.')
+@click.command("generate", no_args_is_help=True)
+@click.argument(
+    "toml_file",
+    type=click.Path(
+        exists=True, dir_okay=False, resolve_path=True, path_type=pathlib.Path
+    ),
+)
+@click.argument(
+    "fru_file",
+    type=click.Path(
+        exists=False, dir_okay=False, resolve_path=True, path_type=pathlib.Path
+    ),
+)
+@click.option(
+    "--force", is_flag=True, help="Overwrite an existing file if it already exists."
+)
 def run_generate(toml_file: pathlib.Path, fru_file: pathlib.Path, force: bool):
     """Generate a binary FRU file using data in a TOML file."""
 
     if fru_file.exists() and not force:
-        click.echo(f'{fru_file} exists and will not be overwritten.')
+        click.echo(f"{fru_file} exists and will not be overwritten.")
         sys.exit(1)
 
     try:
         data = toml_format.load(toml_file)
         blob = fru_format.dump(data)
     except ValueError as error:
         click.echo(error.args[0])
         sys.exit(1)
 
-    with open(fru_file, 'wb') as file:
+    with open(fru_file, "wb") as file:
         file.write(blob)
 
 
-@click.command('dump', no_args_is_help=True)
-@click.argument('fru_file', type=click.Path(exists=True, dir_okay=False, resolve_path=True, path_type=pathlib.Path))
-@click.argument('toml_file', type=click.Path(exists=False, dir_okay=False, resolve_path=True, path_type=pathlib.Path), required=False)
-@click.option('--force', is_flag=True, help='Overwrite an existing file if it already exists.')
+@click.command("dump", no_args_is_help=True)
+@click.argument(
+    "fru_file",
+    type=click.Path(
+        exists=True, dir_okay=False, resolve_path=True, path_type=pathlib.Path
+    ),
+)
+@click.argument(
+    "toml_file",
+    type=click.Path(
+        exists=False, dir_okay=False, resolve_path=True, path_type=pathlib.Path
+    ),
+    required=False,
+)
+@click.option(
+    "--force", is_flag=True, help="Overwrite an existing file if it already exists."
+)
 def run_dump(fru_file: pathlib.Path, toml_file: pathlib.Path, force: bool):
     """Dump data from a binary FRU file to the TOML file format."""
 
     if toml_file and toml_file.exists() and not force:
-        click.echo(f'{toml_file} exists and will not be overwritten.')
+        click.echo(f"{toml_file} exists and will not be overwritten.")
         sys.exit(1)
 
     try:
         data = fru_format.load(path=fru_file)
     except ValueError as error:
         click.echo(error.args[0])
         sys.exit(1)
 
     output = toml_format.dump(data)
     if toml_file:
-        with toml_file.open('wt', encoding='utf8') as file:
+        with toml_file.open("wt", encoding="utf8") as file:
             file.write(output)
     else:
         click.echo(output)
 
 
-@click.command('sample')
-@click.argument('toml_file', type=click.Path(exists=False, dir_okay=False, resolve_path=True, path_type=pathlib.Path), required=False)
-@click.option('--force', is_flag=True, help='Overwrite an existing file if it already exists.')
+@click.command("sample")
+@click.argument(
+    "toml_file",
+    type=click.Path(
+        exists=False, dir_okay=False, resolve_path=True, path_type=pathlib.Path
+    ),
+    required=False,
+)
+@click.option(
+    "--force", is_flag=True, help="Overwrite an existing file if it already exists."
+)
 def run_sample(toml_file, force: bool):
     """Generate a blank TOML document."""
 
     if toml_file and toml_file.exists() and not force:
-        click.echo(f'{toml_file} exists and will not be overwritten.')
+        click.echo(f"{toml_file} exists and will not be overwritten.")
         sys.exit(1)
 
     output = toml_format.dump()
     if toml_file:
-        with toml_file.open('wt', encoding='utf8') as file:
+        with toml_file.open("wt", encoding="utf8") as file:
             file.write(output)
     else:
         click.echo(output)
 
 
 run.add_command(run_generate)
 run.add_command(run_dump)
```

### Comparing `fru-4.0.0a1/src/fru/exceptions.py` & `fru-4.0.1/src/fru/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # fru - Read and write binary IPMI FRU files
-# Copyright 2018-2021 Kurt McKee <contactme@kurtmckee.org>
+# Copyright 2018-2024 Kurt McKee <contactme@kurtmckee.org>
 # Copyright 2017 Dell Technologies
 #
 # https://github.com/kurtmckee/fru-tool/
 #
 # Licensed under the terms of the MIT License:
 # https://opensource.org/licenses/MIT
```

### Comparing `fru-4.0.0a1/src/fru/fru_format.py` & `fru-4.0.1/src/fru/fru_format.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,189 +1,197 @@
 # fru - Read and write binary IPMI FRU files
-# Copyright 2018-2021 Kurt McKee <contactme@kurtmckee.org>
+# Copyright 2018-2024 Kurt McKee <contactme@kurtmckee.org>
 # Copyright 2017 Dell Technologies
 #
 # https://github.com/kurtmckee/fru-tool/
 #
 # Licensed under the terms of the MIT License:
 # https://opensource.org/licenses/MIT
 
 
-import itertools
-import os
 import pathlib
 import struct
 from typing import Dict, List, Union
 
 from . import shared
 
 
 def validate_checksum(blob: bytes, offset: int, length: int):
     """Validate a chassis, board, or product checksum.
 
     *blob* is the binary data blob, and *offset* is the integer offset that
     the chassis, board, or product info area starts at.
     """
 
-    checksum = ord(blob[offset + length - 1:offset + length])
+    checksum = ord(blob[offset + length - 1 : offset + length])
     data_sum = sum(
-        struct.unpack('%dB' % (length - 1), blob[offset:offset + length - 1])
+        struct.unpack("%dB" % (length - 1), blob[offset : offset + length - 1])
     )
-    if 0xff & (data_sum + checksum) != 0:
-        raise ValueError('The data do not match the checksum')
+    if 0xFF & (data_sum + checksum) != 0:
+        raise ValueError("The data do not match the checksum")
 
 
 def extract_values(blob: bytes, offset: int, names: List[str]):
     """Extract values that are delimited by type/length bytes.
 
     The values will be extracted into a dictionary. They'll be saved to keys
     in the same order that keys are provided in *names*.
 
     If there are more values than key names then the values will be stored
     in the key *custom_fields*.
     """
 
     data = {
-        'custom_fields': [],
+        "custom_fields": [],
     }
 
     for name in names:
-        type_length = ord(blob[offset:offset + 1])
-        if type_length == 0xc1:
+        type_length = ord(blob[offset : offset + 1])
+        if type_length == 0xC1:
             return data
-        length = type_length & 0x3f
+        length = type_length & 0x3F
         # encoding = (ord(blob[offset:offset + 1]) & 0xc0) >> 6
-        data[name] = blob[offset + 1:offset + length + 1].decode('ascii')
+        data[name] = blob[offset + 1 : offset + length + 1].decode("ascii")
         offset += length + 1
 
     while True:
-        type_length = ord(blob[offset:offset + 1])
-        if type_length == 0xc1:
+        type_length = ord(blob[offset : offset + 1])
+        if type_length == 0xC1:
             return data
-        length = type_length & 0x3f
+        length = type_length & 0x3F
         # encoding = (ord(blob[offset:offset + 1]) & 0xc0) >> 6
-        data['custom_fields'].append(blob[offset + 1:offset + length + 1].decode('ascii'))
+        data["custom_fields"].append(
+            blob[offset + 1 : offset + length + 1].decode("ascii")
+        )
         offset += length + 1
 
 
 def load(
-        path: Union[pathlib.Path, str] = None,
-        blob: bytes = None,
+    path: Union[pathlib.Path, str] = None,
+    blob: bytes = None,
 ) -> Dict[str, Dict[str, Union[bool, int, str, List]]]:
     """Load binary FRU information from a file or binary data blob.
 
     If *path* is provided, it will be read into memory.
     If *blob* is provided it will be used as-is.
     """
 
     if not path and not blob:
-        raise ValueError('You must specify *path* or *blob*.')
+        raise ValueError("You must specify *path* or *blob*.")
     if path and blob:
-        raise ValueError('You must specify *path* or *blob*, but not both.')
+        raise ValueError("You must specify *path* or *blob*, but not both.")
 
     if path:
-        with open(path, 'rb') as f:
+        with open(path, "rb") as f:
             blob = f.read()
 
     validate_checksum(blob, 0, 8)
 
-    format_version = ord(blob[0:1]) & 0x0f
+    format_version = ord(blob[0:1]) & 0x0F
     internal_offset = ord(blob[1:2]) * 8
     chassis_offset = ord(blob[2:3]) * 8
     board_offset = ord(blob[3:4]) * 8
     product_offset = ord(blob[4:5]) * 8
     # multirecord_offset = ord(blob[5:6]) * 8
 
     data = {
-        'common': {
-            'format_version': format_version,
-            'size': len(blob),
+        "common": {
+            "format_version": format_version,
+            "size": len(blob),
         },
     }
 
     if internal_offset:
         next_offset = chassis_offset or board_offset or product_offset
-        internal_blob = blob[internal_offset + 1:next_offset or len(blob)]
-        data['internal'] = {
-            'format_version': ord(blob[internal_offset:internal_offset + 1]) & 0x0f,
-            'data': internal_blob,
+        internal_blob = blob[internal_offset + 1 : next_offset or len(blob)]
+        data["internal"] = {
+            "format_version": ord(blob[internal_offset : internal_offset + 1]) & 0x0F,
+            "data": internal_blob,
         }
 
     if chassis_offset:
-        length = ord(blob[chassis_offset + 1:chassis_offset + 2]) * 8
+        length = ord(blob[chassis_offset + 1 : chassis_offset + 2]) * 8
         validate_checksum(blob, chassis_offset, length)
 
-        data['chassis'] = shared.get_default_chassis_section()
-        data['chassis'].update({
-            'format_version': ord(blob[chassis_offset:chassis_offset + 1]) & 0x0f,
-            'type': ord(blob[chassis_offset + 2:chassis_offset + 3]),
-        })
+        data["chassis"] = shared.get_default_chassis_section()
+        data["chassis"].update(
+            {
+                "format_version": ord(blob[chassis_offset : chassis_offset + 1]) & 0x0F,
+                "type": ord(blob[chassis_offset + 2 : chassis_offset + 3]),
+            }
+        )
         names = shared.get_chassis_section_names()
-        data['chassis'].update(extract_values(blob, chassis_offset + 3, names))
+        data["chassis"].update(extract_values(blob, chassis_offset + 3, names))
 
     if board_offset:
-        length = ord(blob[board_offset + 1:board_offset + 2]) * 8
+        length = ord(blob[board_offset + 1 : board_offset + 2]) * 8
         validate_checksum(blob, board_offset, length)
 
-        data['board'] = shared.get_default_board_section()
-        data['board'].update({
-            'format_version': ord(blob[board_offset:board_offset + 1]) & 0x0f,
-            'language_code': ord(blob[board_offset + 2:board_offset + 3]),
-            'mfg_date_time': sum([
-                ord(blob[board_offset + 3:board_offset + 4]),
-                ord(blob[board_offset + 4:board_offset + 5]) << 8,
-                ord(blob[board_offset + 5:board_offset + 6]) << 16,
-            ]),
-        })
+        data["board"] = shared.get_default_board_section()
+        data["board"].update(
+            {
+                "format_version": ord(blob[board_offset : board_offset + 1]) & 0x0F,
+                "language_code": ord(blob[board_offset + 2 : board_offset + 3]),
+                "mfg_date_time": sum(
+                    [
+                        ord(blob[board_offset + 3 : board_offset + 4]),
+                        ord(blob[board_offset + 4 : board_offset + 5]) << 8,
+                        ord(blob[board_offset + 5 : board_offset + 6]) << 16,
+                    ]
+                ),
+            }
+        )
         names = shared.get_board_section_names()
-        data['board'].update(extract_values(blob, board_offset + 6, names))
+        data["board"].update(extract_values(blob, board_offset + 6, names))
 
     if product_offset:
-        length = ord(blob[product_offset + 1:product_offset + 2]) * 8
+        length = ord(blob[product_offset + 1 : product_offset + 2]) * 8
         validate_checksum(blob, product_offset, length)
 
-        data['product'] = shared.get_default_product_section()
-        data['product'].update({
-            'format_version': ord(blob[product_offset:product_offset + 1]) & 0x0f,
-            'language_code': ord(blob[product_offset + 2:product_offset + 3]),
-        })
+        data["product"] = shared.get_default_product_section()
+        data["product"].update(
+            {
+                "format_version": ord(blob[product_offset : product_offset + 1]) & 0x0F,
+                "language_code": ord(blob[product_offset + 2 : product_offset + 3]),
+            }
+        )
         names = shared.get_product_section_names()
-        data['product'].update(extract_values(blob, product_offset + 3, names))
+        data["product"].update(extract_values(blob, product_offset + 3, names))
 
     return data
 
 
 def dump(data):
-    if 'common' not in data:
-        raise ValueError('[common] section missing in data')
+    if "common" not in data:
+        raise ValueError("[common] section missing in data")
 
-    if 'format_version' not in data['common']:
+    if "format_version" not in data["common"]:
         raise ValueError('"format_version" key missing in [common]')
 
-    if 'size' not in data['common']:
+    if "size" not in data["common"]:
         raise ValueError('"size" key missing in [common]')
 
     internal_offset = 0
     chassis_offset = 0
     board_offset = 0
     product_offset = 0
     multirecord_offset = 0
 
-    internal = bytes()
-    chassis = bytes()
-    board = bytes()
-    product = bytes()
+    internal = b""
+    chassis = b""
+    board = b""
+    product = b""
 
-    if data.get('internal', {}).get('data'):
+    if data.get("internal", {}).get("data"):
         internal = make_internal(data)
-    if 'chassis' in data:
+    if "chassis" in data:
         chassis = make_chassis(data)
-    if 'board' in data:
+    if "board" in data:
         board = make_board(data)
-    if 'product' in data:
+    if "product" in data:
         product = make_product(data)
 
     pos = 1
     if len(internal):
         internal_offset = pos
         pos += len(internal) // 8
     if len(chassis):
@@ -193,177 +201,186 @@
         board_offset = pos
         pos += len(board) // 8
     if len(product):
         product_offset = pos
 
     # Header
     out = struct.pack(
-        'BBBBBBB',
-        data['common']['format_version'],
+        "BBBBBBB",
+        data["common"]["format_version"],
         internal_offset,
         chassis_offset,
         board_offset,
         product_offset,
         multirecord_offset,
-        0x00
+        0x00,
     )
 
     # Checksum
-    out += struct.pack('B', (0 - sum(bytearray(out))) & 0xff)
+    out += struct.pack("B", (0 - sum(bytearray(out))) & 0xFF)
 
     blob = out + internal + chassis + board + product
-    difference = data['common']['size'] - len(blob)
-    pad = struct.pack('B' * difference, *[0] * difference)
+    difference = data["common"]["size"] - len(blob)
+    pad = struct.pack("B" * difference, *[0] * difference)
 
-    if len(blob + pad) > data['common']['size']:
-        raise ValueError('Too much content, does not fit')
+    if len(blob + pad) > data["common"]["size"]:
+        raise ValueError("Too much content, does not fit")
 
     return blob + pad
 
 
 def make_internal(data):
     return struct.pack(
-        'B%ds' % len(data['internal']['data']),
-        data['internal'].get('format_version', 1),
-        data['internal']['data'],
+        "B%ds" % len(data["internal"]["data"]),
+        data["internal"].get("format_version", 1),
+        data["internal"]["data"],
     )
 
 
 def make_chassis(config):
     chassis = shared.get_default_chassis_section()
-    chassis.update(config['chassis'])
+    chassis.update(config["chassis"])
 
-    out = bytes()
+    out = b""
 
     # Type
-    out += struct.pack('B', chassis['type'])
+    out += struct.pack("B", chassis["type"])
 
     # Strings
     fields = shared.get_chassis_section_names()
 
     for key in fields:
         if chassis[key]:
-            value = chassis[key].encode('ascii')
-            out += struct.pack('B%ds' % len(value), len(value) | 0xC0, value)
+            value = chassis[key].encode("ascii")
+            out += struct.pack("B%ds" % len(value), len(value) | 0xC0, value)
         else:
-            out += struct.pack('B', 0)
+            out += struct.pack("B", 0)
 
-    if isinstance(chassis['custom_fields'], (list, tuple)):
-        for record in chassis['custom_fields']:
-            value = record.encode('ascii')
-            out += struct.pack('B%ds' % len(value), len(value) | 0xC0, value)
+    if isinstance(chassis["custom_fields"], (list, tuple)):
+        for record in chassis["custom_fields"]:
+            value = record.encode("ascii")
+            out += struct.pack("B%ds" % len(value), len(value) | 0xC0, value)
 
     # No more fields
-    out += struct.pack('B', 0xC1)
+    out += struct.pack("B", 0xC1)
 
     # Padding
     while len(out) % 8 != 5:
-        out += struct.pack('B', 0)
+        out += struct.pack("B", 0)
 
     # Header version and length in bytes
-    out = struct.pack(
-        'BB',
-        chassis['format_version'],
-        (len(out) + 3) // 8,
-    ) + out
+    out = (
+        struct.pack(
+            "BB",
+            chassis["format_version"],
+            (len(out) + 3) // 8,
+        )
+        + out
+    )
 
     # Checksum
-    out += struct.pack('B', (0 - sum(bytearray(out))) & 0xff)
+    out += struct.pack("B", (0 - sum(bytearray(out))) & 0xFF)
 
     return out
 
 
 def make_board(config):
     board = shared.get_default_board_section()
-    board.update(config['board'])
+    board.update(config["board"])
 
-    out = bytes()
+    out = b""
 
     # Language
-    out += struct.pack('B', board['language_code'])
+    out += struct.pack("B", board["language_code"])
 
     # Date
-    date = board['mfg_date_time']
+    date = board["mfg_date_time"]
     out += struct.pack(
-        'BBB',
+        "BBB",
         (date & 0xFF),
         (date & 0xFF00) >> 8,
         (date & 0xFF0000) >> 16,
     )
 
     # String values
     fields = shared.get_board_section_names()
 
     for key in fields:
         if board[key]:
-            value = board[key].encode('ascii')
-            out += struct.pack('B%ds' % len(value), len(value) | 0xC0, value)
+            value = board[key].encode("ascii")
+            out += struct.pack("B%ds" % len(value), len(value) | 0xC0, value)
         else:
-            out += struct.pack('B', 0)
+            out += struct.pack("B", 0)
 
-    if isinstance(board['custom_fields'], (list, tuple)):
-        for record in board['custom_fields']:
-            value = record.encode('ascii')
-            out += struct.pack('B%ds' % len(value), len(value) | 0xC0, value)
+    if isinstance(board["custom_fields"], (list, tuple)):
+        for record in board["custom_fields"]:
+            value = record.encode("ascii")
+            out += struct.pack("B%ds" % len(value), len(value) | 0xC0, value)
 
     # No more fields
-    out += struct.pack('B', 0xC1)
+    out += struct.pack("B", 0xC1)
 
     # Padding
     while len(out) % 8 != 5:
-        out += struct.pack('B', 0)
+        out += struct.pack("B", 0)
 
     # Header version and length in bytes
-    out = struct.pack(
-        'BB',
-        board['format_version'],
-        (len(out)+3) // 8,
-    ) + out
+    out = (
+        struct.pack(
+            "BB",
+            board["format_version"],
+            (len(out) + 3) // 8,
+        )
+        + out
+    )
 
     # Checksum
-    out += struct.pack('B', (0 - sum(bytearray(out))) & 0xff)
+    out += struct.pack("B", (0 - sum(bytearray(out))) & 0xFF)
 
     return out
 
 
 def make_product(config):
     product = shared.get_default_product_section()
-    product.update(config['product'])
+    product.update(config["product"])
 
-    out = bytes()
+    out = b""
 
     # Language
-    out += struct.pack('B', product['language_code'])
+    out += struct.pack("B", product["language_code"])
 
     # Strings
     fields = shared.get_product_section_names()
 
     for key in fields:
         if product[key]:
-            value = product[key].encode('ascii')
-            out += struct.pack('B%ds' % len(value), len(value) | 0xC0, value)
+            value = product[key].encode("ascii")
+            out += struct.pack("B%ds" % len(value), len(value) | 0xC0, value)
         else:
-            out += struct.pack('B', 0)
+            out += struct.pack("B", 0)
 
-    if isinstance(product['custom_fields'], (list, tuple)):
-        for record in product['custom_fields']:
-            value = record.encode('ascii')
-            out += struct.pack('B%ds' % len(value), len(value) | 0xC0, value)
+    if isinstance(product["custom_fields"], (list, tuple)):
+        for record in product["custom_fields"]:
+            value = record.encode("ascii")
+            out += struct.pack("B%ds" % len(value), len(value) | 0xC0, value)
 
     # No more fields
-    out += struct.pack('B', 0xC1)
+    out += struct.pack("B", 0xC1)
 
     # Padding
     while len(out) % 8 != 5:
-        out += struct.pack('B', 0)
+        out += struct.pack("B", 0)
 
     # Header version and length in bytes
-    out = struct.pack(
-        'BB',
-        product['format_version'],
-        (len(out) + 3) // 8,
-    ) + out
+    out = (
+        struct.pack(
+            "BB",
+            product["format_version"],
+            (len(out) + 3) // 8,
+        )
+        + out
+    )
 
     # Checksum
-    out += struct.pack('B', (0 - sum(bytearray(out))) & 0xff)
+    out += struct.pack("B", (0 - sum(bytearray(out))) & 0xFF)
 
     return out
```

### Comparing `fru-4.0.0a1/src/fru/shared.py` & `fru-4.0.1/src/fru/shared.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # fru - Read and write binary IPMI FRU files
-# Copyright 2018-2021 Kurt McKee <contactme@kurtmckee.org>
+# Copyright 2018-2024 Kurt McKee <contactme@kurtmckee.org>
 # Copyright 2017 Dell Technologies
 #
 # https://github.com/kurtmckee/fru-tool/
 #
 # Licensed under the terms of the MIT License:
 # https://opensource.org/licenses/MIT
 
@@ -11,98 +11,99 @@
 from typing import Dict, Tuple, Union
 
 
 def get_default_common_section() -> Dict[str, int]:
     """Create an empty common section with default values."""
 
     return {
-        'format_version': 1,
-        'size': 0,  # Guarantee an error if this is not updated.
+        "format_version": 1,
+        "size": 0,  # Guarantee an error if this is not updated.
     }
 
 
 def get_default_board_section() -> Dict[str, Union[int, str, list]]:
     """Create an empty board section with default values."""
 
     return {
-        'format_version': 1,
-        'language_code': 0,
-        'mfg_date_time': 0,
-        'manufacturer': '',
-        'product_name': '',
-        'serial_number': '',
-        'part_number': '',
-        'fru_file_id': '',
-        'custom_fields': [],
+        "format_version": 1,
+        "language_code": 0,
+        "mfg_date_time": 0,
+        "manufacturer": "",
+        "product_name": "",
+        "serial_number": "",
+        "part_number": "",
+        "fru_file_id": "",
+        "custom_fields": [],
     }
 
 
 def get_board_section_names() -> Tuple[str, ...]:
     """Get the list of board section names, in their correct order."""
 
     return (
-        'manufacturer',
-        'product_name',
-        'serial_number',
-        'part_number',
-        'fru_file_id',
+        "manufacturer",
+        "product_name",
+        "serial_number",
+        "part_number",
+        "fru_file_id",
     )
 
+
 def get_default_chassis_section() -> Dict[str, Union[int, str, list]]:
     """Create an empty chassis section with default values."""
 
     return {
-        'format_version': 1,
-        'type': 0,
-        'part_number': '',
-        'serial_number': '',
-        'custom_fields': [],
+        "format_version": 1,
+        "type": 0,
+        "part_number": "",
+        "serial_number": "",
+        "custom_fields": [],
     }
 
 
 def get_chassis_section_names() -> Tuple[str, ...]:
     """Get the list of chassis section names, in their correct order."""
 
     return (
-        'part_number',
-        'serial_number',
+        "part_number",
+        "serial_number",
     )
 
 
 def get_default_product_section() -> Dict[str, Union[int, str, list]]:
     """Create an empty product section with default values."""
 
     return {
-        'format_version': 1,
-        'language_code': 0,
-        'manufacturer': '',
-        'product_name': '',
-        'part_number': '',
-        'product_version': '',
-        'serial_number': '',
-        'asset_tag': '',
-        'fru_file_id': '',
-        'custom_fields': [],
+        "format_version": 1,
+        "language_code": 0,
+        "manufacturer": "",
+        "product_name": "",
+        "part_number": "",
+        "product_version": "",
+        "serial_number": "",
+        "asset_tag": "",
+        "fru_file_id": "",
+        "custom_fields": [],
     }
 
 
 def get_product_section_names() -> Tuple[str, ...]:
     """Get the list of product section names, in their correct order."""
 
     return (
-        'manufacturer',
-        'product_name',
-        'part_number',
-        'product_version',
-        'serial_number',
-        'asset_tag',
-        'fru_file_id',
+        "manufacturer",
+        "product_name",
+        "part_number",
+        "product_version",
+        "serial_number",
+        "asset_tag",
+        "fru_file_id",
     )
 
 
 def get_default_internal_section() -> Dict[str, Union[int, bytes]]:
     """Create an empty internal section with default values."""
 
     return {
-        'format_version': 1,
-        'data': b'',
+        "format_version": 1,
+        "data": b"",
     }
```

### Comparing `fru-4.0.0a1/src/fru/toml_format.py` & `fru-4.0.1/src/fru/toml_format.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 # fru - Read and write binary IPMI FRU files
-# Copyright 2018-2021 Kurt McKee <contactme@kurtmckee.org>
+# Copyright 2018-2024 Kurt McKee <contactme@kurtmckee.org>
 # Copyright 2017 Dell Technologies
 #
 # https://github.com/kurtmckee/fru-tool/
 #
 # Licensed under the terms of the MIT License:
 # https://opensource.org/licenses/MIT
 
 
 import datetime
 import os
 import pathlib
+import sys
+import textwrap
+from importlib.metadata import version
 from typing import Dict, List, Tuple, Union
 
-try:
-    from importlib.metadata import version
-except ImportError:
-    # Python <3.8
-    from importlib_metadata import version
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    # Compatibility
+    import tomli as tomllib
 
-import toml
+from . import exceptions, shared
 
-from . import exceptions
-from . import shared
-
-
-min_date =  datetime.datetime(1996, 1, 1, 0, 0)  # 0x000000
+min_date = datetime.datetime(1996, 1, 1, 0, 0)  # 0x000000
 max_date = datetime.datetime(2027, 11, 24, 20, 15)  # 0xffffff
 
 
 def convert_str_to_minutes(stamp: str) -> int:
     """Convert a str to the number of minutes since 1996-01-01 00:00."""
 
     try:
-        date = datetime.datetime.strptime(stamp, '%Y-%m-%d %H:%M')
+        date = datetime.datetime.strptime(stamp, "%Y-%m-%d %H:%M")
     except ValueError:
         msg = f'The date "{stamp}" must follow the format "YYYY-MM-DD HH:MM"'
         raise exceptions.DateTimeException(msg)
 
     if date < min_date:
         msg = f'The date/time "{stamp}" must be at least 1996-01-01 00:00'
         raise exceptions.DateTimeException(msg)
@@ -53,269 +52,255 @@
     """Format minutes as a human-friendly date/time string.
 
     The return string will be formatted as YYYY-MM-DD HH:MM.
     For example, "2021-02-01 19:28".
     """
 
     if minutes < 0:
-        msg = f'*minutes* must be >= 0 (got {minutes})'
-        raise exceptions.DateTimeException(minutes)
+        msg = f"*minutes* must be >= 0 (got {minutes})"
+        raise exceptions.DateTimeException(msg)
 
-    if minutes > 0xff_ff_ff:
-        msg = f'*minutes* must be <= 0xffffff (got 0x{minutes:x})'
-        raise exceptions.DateTimeException(minutes)
+    if minutes > 0xFF_FF_FF:
+        msg = f"*minutes* must be <= 0xffffff (got 0x{minutes:x})"
+        raise exceptions.DateTimeException(msg)
 
     date = min_date + datetime.timedelta(minutes=minutes)
-    return date.strftime('%Y-%m-%d %H:%M')
+    return date.strftime("%Y-%m-%d %H:%M")
 
 
 def repr_(value: Union[bool, int, str, List]) -> str:
     if isinstance(value, bool):
         return str(bool(value)).lower()
     elif isinstance(value, int):
         return str(value)
     elif isinstance(value, str):
-        value = value.replace('\\', '\\\\')
+        value = value.replace("\\", "\\\\")
         value = value.replace('"', '\\"')
         return f'"{value}"'
     elif isinstance(value, list):
-        output = ' '.join(f'{repr_(v)},' for v in value).rstrip(',')
-        return f'[{output}]'
+        output = " ".join(f"{repr_(v)}," for v in value).rstrip(",")
+        return f"[{output}]"
 
-    msg = f'Unable to represent {repr(value)} (type={type(value)}) in the TOML format'
+    msg = f"Unable to represent {repr(value)} (type={type(value)}) in the TOML format"
     raise exceptions.TOMLException(msg)
 
 
 def repr_internal(value: bytes) -> str:
     """Represent the internal section as a sequence of bytes."""
 
     if not value:
-        return '[]'
+        return "[]"
 
-    output = ['[']
+    output = ["["]
     for block in range(0, len(value), 16):
         pieces = []
-        for i in value[block:block + 16]:
-            pieces.append(f'0x{i:02x}')
-        output.append('    ' + ', '.join(pieces) + ',')
-    output.append(']')
-    return '\n'.join(output)
+        for i in value[block : block + 16]:
+            pieces.append(f"0x{i:02x}")
+        output.append("    " + ", ".join(pieces) + ",")
+    output.append("]")
+    return "\n".join(output)
 
 
-def load(path: Union[pathlib.Path, str] = None, text: str = None) -> Dict[str, Dict[str, Union[bytes, int, str]]]:
+def load(
+    path: Union[pathlib.Path, str] = None, text: str = None
+) -> Dict[str, Dict[str, Union[bytes, int, str]]]:
     """Load a TOML file and return its data as a dictionary.
 
     If *path* is specified it must be a TOML-formatted file.
     If *text* is specified it must be a TOML-formatted string.
     """
 
     if not path and not text:
-        raise exceptions.FRUException('*path* or *text* must be specified')
+        raise exceptions.FRUException("*path* or *text* must be specified")
 
     data = {
-        'common': shared.get_default_common_section(),
-        'board': shared.get_default_board_section(),
-        'chassis': shared.get_default_chassis_section(),
-        'product': shared.get_default_product_section(),
-        'internal': shared.get_default_internal_section(),
+        "common": shared.get_default_common_section(),
+        "board": shared.get_default_board_section(),
+        "chassis": shared.get_default_chassis_section(),
+        "product": shared.get_default_product_section(),
+        "internal": shared.get_default_internal_section(),
     }
 
     if path:
-        toml_data = toml.load(path)
+        with open(path, encoding="utf-8") as file:
+            toml_data = tomllib.loads(file.read())
     else:
-        toml_data = toml.loads(text)
+        toml_data = tomllib.loads(text)
 
     for section in data:
         if section in toml_data:
             data[section].update(toml_data[section])
 
     # These values must be integers.
     integers: Tuple[Tuple[str, str], ...] = (
-        ('common', 'size'),
-        ('common', 'format_version'),
-        ('board', 'language_code'),
-        ('chassis', 'type'),
-        ('product', 'language_code'),
+        ("common", "size"),
+        ("common", "format_version"),
+        ("board", "language_code"),
+        ("chassis", "type"),
+        ("product", "language_code"),
     )
 
-    dates = (
-        ('board', 'mfg_date_time'),
-    )
+    dates = (("board", "mfg_date_time"),)
 
     # Remove sections that are explicitly excluded.
-    for section in ['internal', 'chassis', 'board', 'product', 'multirecord']:
-        include_section = f'include_{section}'
-        if not data['common'].get(include_section, True) and section in data:
-            del(data[section])
-        if include_section in data['common']:
-            del(data['common'][include_section])
+    for section in ["internal", "chassis", "board", "product", "multirecord"]:
+        include_section = f"include_{section}"
+        if not data["common"].get(include_section, True) and section in data:
+            del data[section]
+        if include_section in data["common"]:
+            del data["common"][include_section]
 
     # Standardize integer values.
     for section, key in integers:
         if not isinstance(data.get(section, {}).get(key, 0), int):
             msg = f'Section [{section}] key "{key}" must be a number'
             raise exceptions.TOMLException(msg)
 
     # Standardize date/time values.
     for section, key in dates:
         if section in data and key in data[section]:
             # Convert a default value of 0 to a corresponding string.
             if not data[section][key]:
-                data[section][key] = '1996-01-01 00:00'
+                data[section][key] = "1996-01-01 00:00"
             if not isinstance(data[section][key], str):
                 msg = f'Section [{section}] key "{key}" must be a string'
                 raise exceptions.TOMLException(msg)
             data[section][key] = convert_str_to_minutes(data[section][key])
 
     # Normalize the internal info area data.
-    if data.get('internal', {}).get('data'):
-        msg = f'Section [internal] key "data" must be a list of numbers or a string'
+    if data.get("internal", {}).get("data"):
+        msg = 'Section [internal] key "data" must be a list of numbers or a string'
         try:
-            data['internal']['data'] = bytes(data['internal']['data'])
+            data["internal"]["data"] = bytes(data["internal"]["data"])
         except TypeError:
             try:
-                data['internal']['data'] = data['internal']['data'].encode('utf8')
+                data["internal"]["data"] = data["internal"]["data"].encode("utf8")
             except AttributeError:
                 raise exceptions.TOMLException(msg)
-    elif data.get('internal', {}).get('file'):
-        internal_file = os.path.join(
-            os.path.dirname(path), data['internal']['file']
-        )
+    elif data.get("internal", {}).get("file"):
+        internal_file = os.path.join(os.path.dirname(path), data["internal"]["file"])
         try:
-            with open(internal_file, 'rb') as f:
-                data['internal']['data'] = f.read()
+            with open(internal_file, "rb") as f:
+                data["internal"]["data"] = f.read()
         except FileNotFoundError:
-            msg = f'Internal info area file {internal_file} not found'
+            msg = f"Internal info area file {internal_file} not found"
             raise exceptions.TOMLException(msg)
-    if 'file' in data.get('internal', {}):
-        del(data['internal']['file'])
+    if "file" in data.get("internal", {}):
+        del data["internal"]["file"]
 
     return data
 
 
 def dump(data: Dict[str, Dict[str, Union[bytes, int, str]]] = None) -> str:
     """Dump data to the TOML format.
 
     This function can also generate a blank TOML file.
     """
 
     data = data or {}
     info = {
-        'common': shared.get_default_common_section(),
-        'board': shared.get_default_board_section(),
-        'chassis': shared.get_default_chassis_section(),
-        'product': shared.get_default_product_section(),
+        "common": shared.get_default_common_section(),
+        "board": shared.get_default_board_section(),
+        "chassis": shared.get_default_chassis_section(),
+        "product": shared.get_default_product_section(),
     }
-    for section in ('common', 'board', 'chassis', 'product'):
+    for section in ("common", "board", "chassis", "product"):
         info[section].update(data.get(section, {}))
 
-    output = [
-        # Header
-        f'# -------------------------------------------------------------------',
-        f'# Generated by frutool {version("fru")}',
-        f'# https://github.com/kurtmckee/fru-tool/',
-        f'#',
-        f'# Notes regarding the TOML format, which is like an INI file:',
-        f'#',
-        f'# * Values surrounded by quotation marks are strings: "Vendor"',
-        f'#   Literal quotation marks must be escaped using a backslash: "\\""',
-        f'#   Literal backslashes must also be escaped using a backslash: "\\\\"',
-        f'# * Boolean values use the words "true" and "false" without quotes.',
-        f'# * Numbers that begin with 0x are interpreted as hexadecimal: 0x30',
-        f'#',
-        f'# -------------------------------------------------------------------',
-        f'',
-        f'',
-
-        # Common
-        f'[common]',
-        f'# Warning: It may be harmful to modify *format_version*.',
-        f'format_version = {repr_(info["common"]["format_version"])}',
-        f'',
-        f'# Warning: It may be harmful to modify *size*.',
-        f'size = {repr_(info["common"]["size"])}',
-        f'',
-        f'# These options control which sections are included in the FRU file.',
-        f'include_board = {repr_(bool(data.get("board", False)))}',
-        f'include_chassis = {repr_(bool(data.get("chassis", False)))}',
-        f'include_product = {repr_(bool(data.get("product", False)))}',
-        f'include_internal = {repr_(bool(data.get("internal", False)))}',
-        f'include_multirecord = {repr_(bool(data.get("multirecord", False)))}',
-        f'',
-        f'',
-
-        # Board
-        f'[board]',
-        f'# Warning: It may be harmful to modify *format_version*.',
-        f'format_version = {repr_(info["board"]["format_version"])}',
-        f'',
-        f'language_code = {repr_(info["board"]["language_code"])}',
-        f'',
-        f'mfg_date_time = "{convert_minutes_to_str(info["board"]["mfg_date_time"])}"',
-        f'#                │    │  │  │  │',
-        f'#         year ──┘    │  │  │  ╰── minutes',
-        f'#             month ──╯  │  ╰── hours',
-        f'#                  day ──╯',
-        f'',
-        f'manufacturer = {repr_(info["board"]["manufacturer"])}',
-        f'product_name = {repr_(info["board"]["product_name"])}',
-        f'serial_number = {repr_(info["board"]["serial_number"])}',
-        f'part_number = {repr_(info["board"]["part_number"])}',
-        f'fru_file_id = {repr_(info["board"]["fru_file_id"])}',
-        f'custom_fields = {repr_(info["board"]["custom_fields"])}',
-        f'',
-        f'',
-
-        # Chassis
-        f'[chassis]',
-        f'# Warning: It may be harmful to modify *format_version*.',
-        f'format_version = {repr_(info["chassis"]["format_version"])}',
-        f'',
-        f'type = {repr_(info["chassis"]["type"])}',
-        f'part_number = {repr_(info["chassis"]["part_number"])}',
-        f'serial_number = {repr_(info["chassis"]["serial_number"])}',
-        f'custom_fields = {repr_(info["chassis"]["custom_fields"])}',
-        f'',
-        f'',
-
-        # Product
-        f'[product]',
-        f'# Warning: It may be harmful to modify *format_version*.',
-        f'format_version = {repr_(info["product"]["format_version"])}',
-        f'',
-        f'language_code = {repr_(info["product"]["language_code"])}',
-        f'manufacturer = {repr_(info["product"]["manufacturer"])}',
-        f'product_name = {repr_(info["product"]["product_name"])}',
-        f'part_number = {repr_(info["product"]["part_number"])}',
-        f'product_version = {repr_(info["product"]["product_version"])}',
-        f'serial_number = {repr_(info["product"]["serial_number"])}',
-        f'asset_tag = {repr_(info["product"]["asset_tag"])}',
-        f'fru_file_id = {repr_(info["product"]["fru_file_id"])}',
-        f'custom_fields = {repr_(info["product"]["custom_fields"])}',
-        f'',
-        f'',
-
-        # Internal
-        f'[internal]',
-        f'# Warning: It may be harmful to modify *format_version*.',
-        f'format_version = {repr_(data.get("internal", {}).get("format_version", 1))}',
-        f'',
-        f'# The *data* key can be used to encode a sequence of bytes serialized',
-        f'# as a list of numbers. For small amounts of internal data this might',
-        f'# be sufficient.',
-        f'#',
-        f'# Alternatively, if the *file* key is specified then the file will be',
-        f'# opened and read in binary mode.',
-        f'#',
-        f'# Examples:',
-        f'#',
-        f'#     data = [0x01, 0x02, 0x03]',
-        f'#     file = "path/to/file"',
-        f'#',
-        f'# Do not use the *data* and *file* keys at the same time.',
-        f'',
-        f'data = {repr_internal(data.get("internal", {}).get("data", b""))}',
-        f'',
-        f'',
-    ]
-    
-    return '\n'.join(output)
+    output = f"""
+        # -------------------------------------------------------------------
+        # Generated by frutool {version("fru")}
+        # https://github.com/kurtmckee/fru-tool/
+        #
+        # Notes regarding the TOML format, which is like an INI file:
+        #
+        # * Values surrounded by quotation marks are strings: "Vendor"
+        #   Literal quotation marks must be escaped using a backslash: "\\""
+        #   Literal backslashes must also be escaped using a backslash: "\\\\"
+        # * Boolean values use the words "true" and "false" without quotes.
+        # * Numbers that begin with 0x are interpreted as hexadecimal: 0x30
+        #
+        # -------------------------------------------------------------------
+
+
+        [common]
+        # Warning: It may be harmful to modify *format_version*.
+        format_version = {repr_(info["common"]["format_version"])}
+
+        # Warning: It may be harmful to modify *size*.
+        size = {repr_(info["common"]["size"])}
+
+        # These options control which sections are included in the FRU file.
+        include_board = {repr_(bool(data.get("board", False)))}
+        include_chassis = {repr_(bool(data.get("chassis", False)))}
+        include_product = {repr_(bool(data.get("product", False)))}
+        include_internal = {repr_(bool(data.get("internal", False)))}
+        include_multirecord = {repr_(bool(data.get("multirecord", False)))}
+
+
+        [board]
+        # Warning: It may be harmful to modify *format_version*.
+        format_version = {repr_(info["board"]["format_version"])}
+
+        language_code = {repr_(info["board"]["language_code"])}
+
+        mfg_date_time = "{convert_minutes_to_str(info["board"]["mfg_date_time"])}"
+        #                │    │  │  │  │
+        #         year ──┘    │  │  │  ╰── minutes
+        #             month ──╯  │  ╰── hours
+        #                  day ──╯
+
+        manufacturer = {repr_(info["board"]["manufacturer"])}
+        product_name = {repr_(info["board"]["product_name"])}
+        serial_number = {repr_(info["board"]["serial_number"])}
+        part_number = {repr_(info["board"]["part_number"])}
+        fru_file_id = {repr_(info["board"]["fru_file_id"])}
+        custom_fields = {repr_(info["board"]["custom_fields"])}
+
+
+        [chassis]
+        # Warning: It may be harmful to modify *format_version*.
+        format_version = {repr_(info["chassis"]["format_version"])}
+
+        type = {repr_(info["chassis"]["type"])}
+        part_number = {repr_(info["chassis"]["part_number"])}
+        serial_number = {repr_(info["chassis"]["serial_number"])}
+        custom_fields = {repr_(info["chassis"]["custom_fields"])}
+
+
+        [product]
+        # Warning: It may be harmful to modify *format_version*.
+        format_version = {repr_(info["product"]["format_version"])}
+
+        language_code = {repr_(info["product"]["language_code"])}
+        manufacturer = {repr_(info["product"]["manufacturer"])}
+        product_name = {repr_(info["product"]["product_name"])}
+        part_number = {repr_(info["product"]["part_number"])}
+        product_version = {repr_(info["product"]["product_version"])}
+        serial_number = {repr_(info["product"]["serial_number"])}
+        asset_tag = {repr_(info["product"]["asset_tag"])}
+        fru_file_id = {repr_(info["product"]["fru_file_id"])}
+        custom_fields = {repr_(info["product"]["custom_fields"])}
+
+
+        [internal]
+        # Warning: It may be harmful to modify *format_version*.
+        format_version = {repr_(data.get("internal", {}).get("format_version", 1))}
+
+        # The *data* key can be used to encode a sequence of bytes serialized
+        # as a list of numbers. For small amounts of internal data this might
+        # be sufficient.
+        #
+        # Alternatively, if the *file* key is specified then the file will be
+        # opened and read in binary mode.
+        #
+        # Examples:
+        #
+        #     data = [0x01, 0x02, 0x03]
+        #     file = "path/to/file"
+        #
+        # Do not use the *data* and *file* keys at the same time.
+
+        data = {repr_internal(data.get("internal", {}).get("data", b""))}
+    """
+
+    return textwrap.dedent(output).strip() + "\n"
```

