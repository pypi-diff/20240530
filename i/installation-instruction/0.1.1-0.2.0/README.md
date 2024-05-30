# Comparing `tmp/installation_instruction-0.1.1.tar.gz` & `tmp/installation_instruction-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "installation_instruction-0.1.1.tar", last modified: Tue May 21 09:29:42 2024, max compression
+gzip compressed data, was "installation_instruction-0.2.0.tar", last modified: Thu May 30 13:49:48 2024, max compression
```

## Comparing `installation_instruction-0.1.1.tar` & `installation_instruction-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:29:42.600176 installation_instruction-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-05-21 09:29:39.000000 installation_instruction-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-21 09:29:42.600176 installation_instruction-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-05-21 09:29:39.000000 installation_instruction-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:29:42.596176 installation_instruction-0.1.1/installation_instruction/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-21 09:29:39.000000 installation_instruction-0.1.1/installation_instruction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-21 09:29:39.000000 installation_instruction-0.1.1/installation_instruction/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-21 09:29:39.000000 installation_instruction-0.1.1/installation_instruction/get_flags_and_options_from_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-21 09:29:39.000000 installation_instruction-0.1.1/installation_instruction/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-21 09:29:39.000000 installation_instruction-0.1.1/installation_instruction/installation_instruction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:29:42.596176 installation_instruction-0.1.1/installation_instruction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-21 09:29:42.000000 installation_instruction-0.1.1/installation_instruction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-21 09:29:42.000000 installation_instruction-0.1.1/installation_instruction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:29:42.000000 installation_instruction-0.1.1/installation_instruction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 09:29:42.000000 installation_instruction-0.1.1/installation_instruction.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-21 09:29:42.000000 installation_instruction-0.1.1/installation_instruction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 09:29:42.000000 installation_instruction-0.1.1/installation_instruction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-21 09:29:39.000000 installation_instruction-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:29:42.600176 installation_instruction-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-21 09:29:39.000000 installation_instruction-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:29:42.596176 installation_instruction-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-21 09:29:39.000000 installation_instruction-0.1.1/tests/test_get_flags_and_options_from_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-21 09:29:39.000000 installation_instruction-0.1.1/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-21 09:29:39.000000 installation_instruction-0.1.1/tests/test_installation_instruction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:49:48.534595 installation_instruction-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-05-30 13:49:41.000000 installation_instruction-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-05-30 13:49:48.534595 installation_instruction-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-30 13:49:41.000000 installation_instruction-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:49:48.530595 installation_instruction-0.2.0/installation_instruction/
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-30 13:49:41.000000 installation_instruction-0.2.0/installation_instruction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-30 13:49:41.000000 installation_instruction-0.2.0/installation_instruction/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-30 13:49:41.000000 installation_instruction-0.2.0/installation_instruction/get_flags_and_options_from_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-30 13:49:41.000000 installation_instruction-0.2.0/installation_instruction/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-30 13:49:41.000000 installation_instruction-0.2.0/installation_instruction/installation_instruction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:49:48.530595 installation_instruction-0.2.0/installation_instruction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-05-30 13:49:48.000000 installation_instruction-0.2.0/installation_instruction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-30 13:49:48.000000 installation_instruction-0.2.0/installation_instruction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:49:48.000000 installation_instruction-0.2.0/installation_instruction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-30 13:49:48.000000 installation_instruction-0.2.0/installation_instruction.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-30 13:49:48.000000 installation_instruction-0.2.0/installation_instruction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-30 13:49:48.000000 installation_instruction-0.2.0/installation_instruction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-30 13:49:41.000000 installation_instruction-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 13:49:48.534595 installation_instruction-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 13:49:41.000000 installation_instruction-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:49:48.530595 installation_instruction-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-30 13:49:41.000000 installation_instruction-0.2.0/tests/test_get_flags_and_options_from_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-30 13:49:41.000000 installation_instruction-0.2.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-30 13:49:41.000000 installation_instruction-0.2.0/tests/test_installation_instruction.py
```

### Comparing `installation_instruction-0.1.1/LICENSE` & `installation_instruction-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `installation_instruction-0.1.1/PKG-INFO` & `installation_instruction-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 Metadata-Version: 2.1
-Name: installation_instruction
-Version: 0.1.1
+Name: installation-instruction
+Version: 0.2.0
 Summary: Library and CLI for generating installation instructions from json schema and jinja templates.
+Author: Kanushka Gupta
+Author-email: Adam McKellar <dev@mckellar.eu>, Timo Ege <timoege@online.de>
 Maintainer: Kanushka Gupta
-Maintainer-email: Adam McKellar <dev@mckellar.eu>, Timo Ege <Timoege@online.de>
+Maintainer-email: Adam McKellar <dev@mckellar.eu>, Timo Ege <timoege@online.de>
 License: Apache-2.0
+Project-URL: Repository, https://github.com/instructions-d-installation/installation-instruction
+Project-URL: Documentation, https://installation-instruction.readthedocs.io/en/latest/
+Project-URL: Issues, https://github.com/instructions-d-installation/installation-instruction/issues
+Project-URL: Changelog, https://github.com/instructions-d-installation/installation-instruction/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jinja2
@@ -24,92 +30,110 @@
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Requires-Dist: sphinx-autoapi; extra == "docs"
 
 <div align="center">
 
 # `installation-instruction`
 
-**Library for checking and parsing installation instruction schemas.**
+**Library and CLI for generating installation instructions from json schema and jinja templates.**
 
-![GitHub License](https://img.shields.io/github/license/instructions-d-installation/installation-instruction)
+[![GitHub License](https://img.shields.io/github/license/instructions-d-installation/installation-instruction)](./LICENSE)
+[![PyPI - Version](https://img.shields.io/pypi/v/installation-instruction)](https://pypi.org/project/installation-instruction/)
 [![Documentation Status](https://readthedocs.org/projects/installation-instruction/badge/?version=latest)](https://installation-instruction.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/instructions-d-installation/installation-instruction/graph/badge.svg?token=5AIH36HYG3)](https://codecov.io/gh/instructions-d-installation/installation-instruction)
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Finstructions-d-installation%2Finstallation-instruction.svg?type=small)](https://app.fossa.com/projects/git%2Bgithub.com%2Finstructions-d-installation%2Finstallation-instruction?ref=badge_small)
 
 </div>
 
 ## Installation
 
 ### [pipx](https://github.com/pypa/pipx)
 
 ```
-pipx install installation_instruction
+pipx install installation-instruction
 ```
 
 
 ### pip
 
 ```
-python -m pip install installation_instruction
+python -m pip install installation-instruction
 ```
 
 
-### installation_instruction
+### installation-instruction
 
 *(Don't try at home.)*
 ```yaml
-name: installation_instruction
+name: installation-instruction
 type: object
 properties:
   method:
     enum:
       - pipx
       - pip
 ----------------------------------
 {% if method == "pip" %}
   python -m pip
 {% else %}
   pipx
 {% endif %}
-  install installation_instruction
+  install installation-instruction
 ```
 
 
 ## CLI Usage
 
 ```
 Usage: ibi [OPTIONS] COMMAND [ARGS]...
 
+  Library and CLI for generating installation instructions from json schema
+  and jinja templates.
+
 Options:
-  --help  Show this message and exit.
+  --version   Show the version and exit.
+  -h, --help  Show this message and exit.
 
 Commands:
-  show  Shows installation instructions for your specified config file...
+  install  Installs with config and parameters given.
+  show     Shows installation instructions for your specified config file...
 ```
 
 Options are dynamically created with the schema part of the config file.   
 
 > [!TIP]
 > Show help for a config file with: `ibi show CONFIG_FILE --help`.
 
 
 ## Config
 
-The config is comprised of a single file. (Currently there is no fixed filename.) 
-For ease of use you should use the file extension `.yml.jinja` and develope said config file as two seperate files at first.
-The config file has two parts delimited by `------` (6 or more `-`).   
-The first part is the schema (*What is valid user input?*). The second part is the template (*What is the actual command for said user input?*).
-The first part must be a valid [JSON Schema](https://json-schema.org/) in [JSON](https://www.json.org/json-en.html) or to JSON capabilites restricted [YAML](https://yaml.org/) and the second part must be a valid [jinja2 template](https://jinja.palletsprojects.com/en/3.0.x/templates/).
-The exception to this is that `anyOf` and `oneOf` are only usable for enum like behaviour on the schema side.
-Instead of an `enum` you might want to use `anyOf` with `const` and `tile` properties.
-The `title` of a property is used for the pretty print name, while the `description` is used for the help message.
-There exists a jinja2 macro called `raise`, which is usefull if there is actually no installation instruction for said user input.
-All lineends in the template are removed after render, which means that commands can be splitted within the template (`conda install {{ "xyz" if myvar else "abc" }}` ).
-This also means that multiple commands need to be chained via `&&`.
-For examples please look at the [examples folder](./examples/).
+* The config is comprised of a single file `install.cfg`.
+* The config has two parts delimited by `------` (6 or more `-`).
+* Both parts should be developed in different files for language server support.
+
+
+### Schema
+
+* The first section of the config is a [json-schema](https://json-schema.org/).
+* It can be written in [JSON](https://www.json.org/json-en.html) or to JSON capabilites restricted [YAML](https://yaml.org/).
+* `title` are used for pretty print option names.
+* `description` is used for the options help message.
+* `anyOf` with nested `const` and `title` are a special case as a replacement for `enum` but with pretty print name.
+
+
+### Template
+
+* You can have as much whitespace and line breaks as you wish in and inbetween your commands.
+* Commands must be seperated by `&&`! (`pip install installation-instruction && pip uninstall installation-instruction`.)
+* If you wish to stop the render from within the template you can use the macro `raise`. (`{{ raise("no support!") }}`.) 
+
+
+### MISC
+
+Please have a look at the [examples](./examples/).
 
 
 ## Development installation
 
 If you want to contribute to the development of `installation_instruction`, we recommend
 the following editable installation from this repository:
 
@@ -121,17 +145,17 @@
 
 ```
 python -m pytest
 ```
 
 ## Contributors
 
-* [Adam McKellar](https://github.com/WyvernIXTL) [dev@mckellar.eu](mailto:dev@mckellar.eu)
+* [Adam McKellar](https://github.com/WyvernIXTL) ([dev@mckellar.eu](mailto:dev@mckellar.eu))
 * [Kanushka Gupta](https://github.com/KanushkaGupta)
-* [Timo Ege](https://github.com/TimoEg) [Timoege@online.de](mailto:Timoege@online.de)
+* [Timo Ege](https://github.com/TimoEg) ([timoege@online.de](mailto:timoege@online.de))
 
 
 ## Acknowledgments
 
 This repository was set up using the [SSC Cookiecutter for Python Packages](https://github.com/ssciwr/cookiecutter-python-package).
```

### Comparing `installation_instruction-0.1.1/README.md` & `installation_instruction-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,89 +1,107 @@
 <div align="center">
 
 # `installation-instruction`
 
-**Library for checking and parsing installation instruction schemas.**
+**Library and CLI for generating installation instructions from json schema and jinja templates.**
 
-![GitHub License](https://img.shields.io/github/license/instructions-d-installation/installation-instruction)
+[![GitHub License](https://img.shields.io/github/license/instructions-d-installation/installation-instruction)](./LICENSE)
+[![PyPI - Version](https://img.shields.io/pypi/v/installation-instruction)](https://pypi.org/project/installation-instruction/)
 [![Documentation Status](https://readthedocs.org/projects/installation-instruction/badge/?version=latest)](https://installation-instruction.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/instructions-d-installation/installation-instruction/graph/badge.svg?token=5AIH36HYG3)](https://codecov.io/gh/instructions-d-installation/installation-instruction)
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Finstructions-d-installation%2Finstallation-instruction.svg?type=small)](https://app.fossa.com/projects/git%2Bgithub.com%2Finstructions-d-installation%2Finstallation-instruction?ref=badge_small)
 
 </div>
 
 ## Installation
 
 ### [pipx](https://github.com/pypa/pipx)
 
 ```
-pipx install installation_instruction
+pipx install installation-instruction
 ```
 
 
 ### pip
 
 ```
-python -m pip install installation_instruction
+python -m pip install installation-instruction
 ```
 
 
-### installation_instruction
+### installation-instruction
 
 *(Don't try at home.)*
 ```yaml
-name: installation_instruction
+name: installation-instruction
 type: object
 properties:
   method:
     enum:
       - pipx
       - pip
 ----------------------------------
 {% if method == "pip" %}
   python -m pip
 {% else %}
   pipx
 {% endif %}
-  install installation_instruction
+  install installation-instruction
 ```
 
 
 ## CLI Usage
 
 ```
 Usage: ibi [OPTIONS] COMMAND [ARGS]...
 
+  Library and CLI for generating installation instructions from json schema
+  and jinja templates.
+
 Options:
-  --help  Show this message and exit.
+  --version   Show the version and exit.
+  -h, --help  Show this message and exit.
 
 Commands:
-  show  Shows installation instructions for your specified config file...
+  install  Installs with config and parameters given.
+  show     Shows installation instructions for your specified config file...
 ```
 
 Options are dynamically created with the schema part of the config file.   
 
 > [!TIP]
 > Show help for a config file with: `ibi show CONFIG_FILE --help`.
 
 
 ## Config
 
-The config is comprised of a single file. (Currently there is no fixed filename.) 
-For ease of use you should use the file extension `.yml.jinja` and develope said config file as two seperate files at first.
-The config file has two parts delimited by `------` (6 or more `-`).   
-The first part is the schema (*What is valid user input?*). The second part is the template (*What is the actual command for said user input?*).
-The first part must be a valid [JSON Schema](https://json-schema.org/) in [JSON](https://www.json.org/json-en.html) or to JSON capabilites restricted [YAML](https://yaml.org/) and the second part must be a valid [jinja2 template](https://jinja.palletsprojects.com/en/3.0.x/templates/).
-The exception to this is that `anyOf` and `oneOf` are only usable for enum like behaviour on the schema side.
-Instead of an `enum` you might want to use `anyOf` with `const` and `tile` properties.
-The `title` of a property is used for the pretty print name, while the `description` is used for the help message.
-There exists a jinja2 macro called `raise`, which is usefull if there is actually no installation instruction for said user input.
-All lineends in the template are removed after render, which means that commands can be splitted within the template (`conda install {{ "xyz" if myvar else "abc" }}` ).
-This also means that multiple commands need to be chained via `&&`.
-For examples please look at the [examples folder](./examples/).
+* The config is comprised of a single file `install.cfg`.
+* The config has two parts delimited by `------` (6 or more `-`).
+* Both parts should be developed in different files for language server support.
+
+
+### Schema
+
+* The first section of the config is a [json-schema](https://json-schema.org/).
+* It can be written in [JSON](https://www.json.org/json-en.html) or to JSON capabilites restricted [YAML](https://yaml.org/).
+* `title` are used for pretty print option names.
+* `description` is used for the options help message.
+* `anyOf` with nested `const` and `title` are a special case as a replacement for `enum` but with pretty print name.
+
+
+### Template
+
+* You can have as much whitespace and line breaks as you wish in and inbetween your commands.
+* Commands must be seperated by `&&`! (`pip install installation-instruction && pip uninstall installation-instruction`.)
+* If you wish to stop the render from within the template you can use the macro `raise`. (`{{ raise("no support!") }}`.) 
+
+
+### MISC
+
+Please have a look at the [examples](./examples/).
 
 
 ## Development installation
 
 If you want to contribute to the development of `installation_instruction`, we recommend
 the following editable installation from this repository:
 
@@ -95,17 +113,17 @@
 
 ```
 python -m pytest
 ```
 
 ## Contributors
 
-* [Adam McKellar](https://github.com/WyvernIXTL) [dev@mckellar.eu](mailto:dev@mckellar.eu)
+* [Adam McKellar](https://github.com/WyvernIXTL) ([dev@mckellar.eu](mailto:dev@mckellar.eu))
 * [Kanushka Gupta](https://github.com/KanushkaGupta)
-* [Timo Ege](https://github.com/TimoEg) [Timoege@online.de](mailto:Timoege@online.de)
+* [Timo Ege](https://github.com/TimoEg) ([timoege@online.de](mailto:timoege@online.de))
 
 
 ## Acknowledgments
 
 This repository was set up using the [SSC Cookiecutter for Python Packages](https://github.com/ssciwr/cookiecutter-python-package).
```

### Comparing `installation_instruction-0.1.1/installation_instruction/get_flags_and_options_from_schema.py` & `installation_instruction-0.2.0/installation_instruction/get_flags_and_options_from_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,33 +31,38 @@
     :return: List of all the clickoptions from the schema.
     :rtype: list[Option]
     """
     options = []
     required_args = set(schema.get('required', []))
 
     for key, value in schema.get('properties', {}).items():
+        orig_key = key
         key = key.replace('_', '-').replace(' ', '-')
         option_name = '--{}'.format(key)
         option_type = value.get('type', 'string')
         option_description = value.get('description', '')
         option_default = value.get('default', None)
 
         if 'anyOf' in value:
             option_type = Choice( [c['const'] for c in value['anyOf'] if 'const' in c] )
         elif "enum" in value:
             option_type = Choice( value["enum"] )
         else:
             option_type = SCHEMA_TO_CLICK_TYPE_MAPPING.get(option_type, click.STRING)
 
-        required = key in required_args
+        required = (orig_key in required_args) and option_default is None
+        is_flag=(option_type == click.BOOL)
+        if is_flag and required:
+            option_name = option_name + "/--no-{}".format(key)
 
         options.append(Option(
             param_decls=[option_name],
             type=option_type,
             help=option_description,
             required=required,
             default=option_default,
             show_default=True,
-            show_choices=True
+            show_choices=True,
+            is_flag=is_flag,
         ))
 
     return options
```

### Comparing `installation_instruction-0.1.1/installation_instruction/helpers.py` & `installation_instruction-0.2.0/installation_instruction/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,25 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import re
 from jinja2 import Environment, Template
 
 
+def _make_pretty_print_line_breaks(string: str) -> str:
+    """
+    Replaces `&& ` with a newline character.
+
+    :param string: String to be processed.
+    :type string: str
+    :return: String with `&& ` replaced with newline character.
+    :rtype: str
+    """
+    return re.sub(r"\s?&&\s?", "\n", string, 0, re.S)
+
 def _get_error_message_from_string(string: str) -> str | None:
     """
     Parses error message of error given by using jinja macro `RAISE_JINJA_MACRO_STRING`. If no error message is found returns `None`.
 
     :param string: This is the raw error string where an error message might be.
     :type string: str
     :return: Error message if found else None.
```

### Comparing `installation_instruction-0.1.1/installation_instruction/installation_instruction.py` & `installation_instruction-0.2.0/installation_instruction/installation_instruction.py`

 * *Files identical despite different names*

### Comparing `installation_instruction-0.1.1/installation_instruction.egg-info/PKG-INFO` & `installation_instruction-0.2.0/installation_instruction.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 Metadata-Version: 2.1
-Name: installation_instruction
-Version: 0.1.1
+Name: installation-instruction
+Version: 0.2.0
 Summary: Library and CLI for generating installation instructions from json schema and jinja templates.
+Author: Kanushka Gupta
+Author-email: Adam McKellar <dev@mckellar.eu>, Timo Ege <timoege@online.de>
 Maintainer: Kanushka Gupta
-Maintainer-email: Adam McKellar <dev@mckellar.eu>, Timo Ege <Timoege@online.de>
+Maintainer-email: Adam McKellar <dev@mckellar.eu>, Timo Ege <timoege@online.de>
 License: Apache-2.0
+Project-URL: Repository, https://github.com/instructions-d-installation/installation-instruction
+Project-URL: Documentation, https://installation-instruction.readthedocs.io/en/latest/
+Project-URL: Issues, https://github.com/instructions-d-installation/installation-instruction/issues
+Project-URL: Changelog, https://github.com/instructions-d-installation/installation-instruction/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jinja2
@@ -24,92 +30,110 @@
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Requires-Dist: sphinx-autoapi; extra == "docs"
 
 <div align="center">
 
 # `installation-instruction`
 
-**Library for checking and parsing installation instruction schemas.**
+**Library and CLI for generating installation instructions from json schema and jinja templates.**
 
-![GitHub License](https://img.shields.io/github/license/instructions-d-installation/installation-instruction)
+[![GitHub License](https://img.shields.io/github/license/instructions-d-installation/installation-instruction)](./LICENSE)
+[![PyPI - Version](https://img.shields.io/pypi/v/installation-instruction)](https://pypi.org/project/installation-instruction/)
 [![Documentation Status](https://readthedocs.org/projects/installation-instruction/badge/?version=latest)](https://installation-instruction.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/instructions-d-installation/installation-instruction/graph/badge.svg?token=5AIH36HYG3)](https://codecov.io/gh/instructions-d-installation/installation-instruction)
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Finstructions-d-installation%2Finstallation-instruction.svg?type=small)](https://app.fossa.com/projects/git%2Bgithub.com%2Finstructions-d-installation%2Finstallation-instruction?ref=badge_small)
 
 </div>
 
 ## Installation
 
 ### [pipx](https://github.com/pypa/pipx)
 
 ```
-pipx install installation_instruction
+pipx install installation-instruction
 ```
 
 
 ### pip
 
 ```
-python -m pip install installation_instruction
+python -m pip install installation-instruction
 ```
 
 
-### installation_instruction
+### installation-instruction
 
 *(Don't try at home.)*
 ```yaml
-name: installation_instruction
+name: installation-instruction
 type: object
 properties:
   method:
     enum:
       - pipx
       - pip
 ----------------------------------
 {% if method == "pip" %}
   python -m pip
 {% else %}
   pipx
 {% endif %}
-  install installation_instruction
+  install installation-instruction
 ```
 
 
 ## CLI Usage
 
 ```
 Usage: ibi [OPTIONS] COMMAND [ARGS]...
 
+  Library and CLI for generating installation instructions from json schema
+  and jinja templates.
+
 Options:
-  --help  Show this message and exit.
+  --version   Show the version and exit.
+  -h, --help  Show this message and exit.
 
 Commands:
-  show  Shows installation instructions for your specified config file...
+  install  Installs with config and parameters given.
+  show     Shows installation instructions for your specified config file...
 ```
 
 Options are dynamically created with the schema part of the config file.   
 
 > [!TIP]
 > Show help for a config file with: `ibi show CONFIG_FILE --help`.
 
 
 ## Config
 
-The config is comprised of a single file. (Currently there is no fixed filename.) 
-For ease of use you should use the file extension `.yml.jinja` and develope said config file as two seperate files at first.
-The config file has two parts delimited by `------` (6 or more `-`).   
-The first part is the schema (*What is valid user input?*). The second part is the template (*What is the actual command for said user input?*).
-The first part must be a valid [JSON Schema](https://json-schema.org/) in [JSON](https://www.json.org/json-en.html) or to JSON capabilites restricted [YAML](https://yaml.org/) and the second part must be a valid [jinja2 template](https://jinja.palletsprojects.com/en/3.0.x/templates/).
-The exception to this is that `anyOf` and `oneOf` are only usable for enum like behaviour on the schema side.
-Instead of an `enum` you might want to use `anyOf` with `const` and `tile` properties.
-The `title` of a property is used for the pretty print name, while the `description` is used for the help message.
-There exists a jinja2 macro called `raise`, which is usefull if there is actually no installation instruction for said user input.
-All lineends in the template are removed after render, which means that commands can be splitted within the template (`conda install {{ "xyz" if myvar else "abc" }}` ).
-This also means that multiple commands need to be chained via `&&`.
-For examples please look at the [examples folder](./examples/).
+* The config is comprised of a single file `install.cfg`.
+* The config has two parts delimited by `------` (6 or more `-`).
+* Both parts should be developed in different files for language server support.
+
+
+### Schema
+
+* The first section of the config is a [json-schema](https://json-schema.org/).
+* It can be written in [JSON](https://www.json.org/json-en.html) or to JSON capabilites restricted [YAML](https://yaml.org/).
+* `title` are used for pretty print option names.
+* `description` is used for the options help message.
+* `anyOf` with nested `const` and `title` are a special case as a replacement for `enum` but with pretty print name.
+
+
+### Template
+
+* You can have as much whitespace and line breaks as you wish in and inbetween your commands.
+* Commands must be seperated by `&&`! (`pip install installation-instruction && pip uninstall installation-instruction`.)
+* If you wish to stop the render from within the template you can use the macro `raise`. (`{{ raise("no support!") }}`.) 
+
+
+### MISC
+
+Please have a look at the [examples](./examples/).
 
 
 ## Development installation
 
 If you want to contribute to the development of `installation_instruction`, we recommend
 the following editable installation from this repository:
 
@@ -121,17 +145,17 @@
 
 ```
 python -m pytest
 ```
 
 ## Contributors
 
-* [Adam McKellar](https://github.com/WyvernIXTL) [dev@mckellar.eu](mailto:dev@mckellar.eu)
+* [Adam McKellar](https://github.com/WyvernIXTL) ([dev@mckellar.eu](mailto:dev@mckellar.eu))
 * [Kanushka Gupta](https://github.com/KanushkaGupta)
-* [Timo Ege](https://github.com/TimoEg) [Timoege@online.de](mailto:Timoege@online.de)
+* [Timo Ege](https://github.com/TimoEg) ([timoege@online.de](mailto:timoege@online.de))
 
 
 ## Acknowledgments
 
 This repository was set up using the [SSC Cookiecutter for Python Packages](https://github.com/ssciwr/cookiecutter-python-package).
```

### Comparing `installation_instruction-0.1.1/installation_instruction.egg-info/SOURCES.txt` & `installation_instruction-0.2.0/installation_instruction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `installation_instruction-0.1.1/pyproject.toml` & `installation_instruction-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -5,25 +5,30 @@
 requires = [
     "setuptools >=61",
 ]
 build-backend = "setuptools.build_meta"
 
 # This section provides general project metadata that is used across
 # a variety of build tools. Notably, the version specified here is the
-# single source of truth for installation_instruction's version
+# single source of truth for installation-instruction's version
 [project]
-name = "installation_instruction"
+name = "installation-instruction"
 description = "Library and CLI for generating installation instructions from json schema and jinja templates."
 readme = "README.md"
 maintainers = [
     { name = "Adam McKellar", email = "dev@mckellar.eu" },
     { name = "Kanushka Gupta" },
-    { name = "Timo Ege", email = "Timoege@online.de" },
+    { name = "Timo Ege", email = "timoege@online.de" },
 ]
-version = "0.1.1"
+authors = [
+    { name = "Adam McKellar", email = "dev@mckellar.eu" },
+    { name = "Kanushka Gupta" },
+    { name = "Timo Ege", email = "timoege@online.de" },
+]
+version = "0.2.0"
 requires-python = ">=3.10"
 license = { text = "Apache-2.0" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: Apache Software License",
 ]
@@ -46,14 +51,20 @@
     "sphinx-autoapi",
 ]
 
 # Here you can list scripts. (Listed is a shim to the cli.)
 [project.scripts]
 ibi = "installation_instruction.__main__:main"
 
+[project.urls]
+Repository = "https://github.com/instructions-d-installation/installation-instruction"
+Documentation = "https://installation-instruction.readthedocs.io/en/latest/"
+Issues = "https://github.com/instructions-d-installation/installation-instruction/issues"
+Changelog = "https://github.com/instructions-d-installation/installation-instruction/blob/main/CHANGELOG.md"
+
 # The following section contains setuptools-specific configuration
 # options. For a full reference of available options, check the overview
 # at https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [tool.setuptools]
 packages = [
     "installation_instruction",
 ]
```

### Comparing `installation_instruction-0.1.1/tests/test_helpers.py` & `installation_instruction-0.2.0/tests/test_helpers.py`

 * *Files identical despite different names*

