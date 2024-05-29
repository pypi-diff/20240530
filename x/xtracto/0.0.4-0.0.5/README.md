# Comparing `tmp/xtracto-0.0.4.tar.gz` & `tmp/xtracto-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtracto-0.0.4.tar", last modified: Wed Jan 17 18:28:22 2024, max compression
+gzip compressed data, was "xtracto-0.0.5.tar", last modified: Wed May 29 23:13:23 2024, max compression
```

## Comparing `xtracto-0.0.4.tar` & `xtracto-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-01-17 18:28:22.651660 xtracto-0.0.4/
--rw-rw-rw-   0        0        0     1071 2023-10-28 05:28:47.000000 xtracto-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     3317 2024-01-17 18:28:22.648122 xtracto-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-01-17 18:28:22.611625 xtracto-0.0.4/dev/
--rw-rw-rw-   0        0        0    34131 2024-01-17 18:21:57.000000 xtracto-0.0.4/dev/__init__.py
--rw-rw-rw-   0        0        0     4729 2024-01-15 17:55:34.000000 xtracto-0.0.4/dev/tests.py
--rw-rw-rw-   0        0        0       74 2024-01-15 17:36:16.000000 xtracto-0.0.4/dev/xtracto.config.py
--rw-rw-rw-   0        0        0       42 2024-01-17 18:28:22.651660 xtracto-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1161 2024-01-17 18:27:17.000000 xtracto-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-17 18:28:22.617623 xtracto-0.0.4/xtracto/
--rw-rw-rw-   0        0        0    34069 2024-01-17 18:27:05.000000 xtracto-0.0.4/xtracto/__init__.py
--rw-rw-rw-   0        0        0  1604430 2024-01-02 13:13:39.000000 xtracto-0.0.4/xtracto/_images.py
-drwxrwxrwx   0        0        0        0 2024-01-17 18:28:22.644117 xtracto-0.0.4/xtracto.egg-info/
--rw-rw-rw-   0        0        0     3317 2024-01-17 18:28:22.000000 xtracto-0.0.4/xtracto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2024-01-17 18:28:22.000000 xtracto-0.0.4/xtracto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-17 18:28:22.000000 xtracto-0.0.4/xtracto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-01-17 18:28:22.000000 xtracto-0.0.4/xtracto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-01-17 18:28:22.000000 xtracto-0.0.4/xtracto.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 23:13:23.044713 xtracto-0.0.5/
+-rw-rw-rw-   0        0        0     1071 2023-10-28 05:28:47.000000 xtracto-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     3344 2024-05-29 23:13:23.043202 xtracto-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-29 23:13:23.044713 xtracto-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1157 2024-05-29 23:12:46.000000 xtracto-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 23:13:23.022821 xtracto-0.0.5/xtracto/
+-rw-rw-rw-   0        0        0    41235 2024-05-29 23:08:55.000000 xtracto-0.0.5/xtracto/__init__.py
+-rw-rw-rw-   0        0        0  1604430 2024-01-02 13:13:39.000000 xtracto-0.0.5/xtracto/_images.py
+drwxrwxrwx   0        0        0        0 2024-05-29 23:13:23.040266 xtracto-0.0.5/xtracto.egg-info/
+-rw-rw-rw-   0        0        0     3344 2024-05-29 23:13:22.000000 xtracto-0.0.5/xtracto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2024-05-29 23:13:23.000000 xtracto-0.0.5/xtracto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 23:13:22.000000 xtracto-0.0.5/xtracto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-29 23:13:22.000000 xtracto-0.0.5/xtracto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-29 23:13:22.000000 xtracto-0.0.5/xtracto.egg-info/top_level.txt
```

### Comparing `xtracto-0.0.4/LICENSE.txt` & `xtracto-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xtracto-0.0.4/PKG-INFO` & `xtracto-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtracto
-Version: 0.0.4
+Version: 0.0.5
 Summary: Xtracto is a lightweight web development framework designed to simplify the process of creating dynamic web pages using Python and pypx. 
 Author: shashstormer
 Project-URL: GitHub, https://github.com/shashstormer/xtracto
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,15 @@
 Classifier: Topic :: Database
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
 Requires-Dist: beautifulsoup4
 Requires-Dist: requestez
+Requires-Dist: pytailwind
 
 
 # Xtracto Web Development Framework
 eXtensible, Configurable, and Reusable Automation Component Tool and Organizer <sub>for html through pypx</sub>
 
 
 Xtracto is a lightweight web development framework designed to simplify the process of creating dynamic web pages using Python.
```

### Comparing `xtracto-0.0.4/dev/__init__.py` & `xtracto-0.0.5/xtracto/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 """
 A web framework for integration with pypx
 """
-__version__ = "0.0.2"
+__version__ = "0.0.4"
 __author__ = "shashstormer"
 __description__ = "A web framework for integration with pypx"
 
 import os
 import re
+from fastapi import FastAPI, HTTPException, status, Response, Request
+from fastapi.responses import FileResponse
+from pytailwind import Tailwind
 
 MAXIMUM_DEPTH_PROJECT_ROOT = 100
 
+validated_files = {}
+
 
 class Utils:
     @staticmethod
     def import_module_by_path(module_path):
         """
         Imports python module from the speficied module path
 
@@ -27,22 +32,26 @@
         spec.loader.exec_module(module)
         return module
 
     @staticmethod
     def get_project_root():
         current_script = os.getcwd()
         ic = 0
-        while not os.path.isfile(os.path.join(current_script, 'xtracto.config.py')):
+        while current_script:
+            if os.path.exists(os.path.join(current_script, 'xtracto.config.py')):
+                break
             ic += 1
             current_script = os.path.dirname(current_script)
             if ic > MAXIMUM_DEPTH_PROJECT_ROOT:
-                Log.critical(Error.ProjectConfig.message)
-                if Config().debug:
+                Log.critical(Error.ProjectConfig.message, "")
+                if Config("").debug:
                     Log.debug(Error.ProjectConfig.resolution)
-                raise Error.ProjectConfig.error
+                current_script = False
+        else:
+            raise Error.ProjectConfig.error
         return current_script
 
     @staticmethod
     def get_config_file():
         return os.path.join(Utils.get_project_root(), "xtracto.config.py")
 
     @staticmethod
@@ -134,62 +143,102 @@
 
         Returns:
         - str: The absolute path to the user's home directory.
         """
         home_directory = os.path.expanduser("~")
         return home_directory
 
+    @staticmethod
+    def layout_exists():
+        """
+        This method returns if the layout file exists.
+        If it exists it is used and the page is rendered in that layout.
+        """
+        return os.path.exists(os.path.join(Config().project_root, "_layout.pypx"))
+
 
 class Parser:
-    def __init__(self, path=None, content=None, module=False, layout=False):
+    def __init__(self, path=None, content=None, module=False, layout=False, _additional_contexts=None):
         """
         Wrapper for parsing a pypx to a deliverable html file.
         """
         self.raw_type = "path" if path is not None else "content"
         self.raw_origin = path if path is not None else content
         if path:
             if module:
                 _fpath = os.path.join(str(Config().module_root), path)
+                layout = True
             else:
                 _fpath = os.path.join(str(Config().pages_root), path)
             with open(_fpath) as f:
                 self.content = f.read()
         else:
             self.content = content
         self.raw_content = self.content
-        self.pypx_parser = Pypx(self.content, self.raw_origin)
         self.html_content = ""
         self.layout = layout
+        self.static_requirements = {}
+        self.module = module
+        if _additional_contexts is None:
+            _additional_contexts = []
+        self.pypx_parser = Pypx(self.content, self.raw_origin, _additional_contexts=_additional_contexts)
+        self.contexts = _additional_contexts
         del path, content, module, layout
         if self.content:
             if self.layout:
-                self.pypx_parser.load_variables()
+                _ = [self.pypx_parser.parsed]
+                _.extend(self.contexts)
+                self.pypx_parser.load_variables(_addnl_var_contexts=_)
             self.parse()
 
     def parse(self):
         self.pypx_parser.parse(self.layout)
-        self.html_content = self.pypx_parser.parsed
+        if not self.module:
+            self.static_requirements.update(self.pypx_parser.parse_static_import())
+            self.static_requirements.update(self.pypx_parser.static_requirements)
+
+        self.html_content = self.pypx_parser.normalize(self.pypx_parser.parsed)
 
     def render(self):
-        self.pypx_parser.load_variables()
+        _loaders_match = re.compile("\+\$(.*?)\$\+")
+        _load_list = []
+        _ = [self.pypx_parser.parsed]
+        _.extend(self.contexts)
+        for _load in _loaders_match.findall("\n".join(_)):
+            _load_list.append(_load.split("=", 1))
+        for var, val in _load_list:
+            locals()[var] = val
+        self.pypx_parser.load_variables(_addnl_var_contexts=_)
         self.pypx_parser.do_imports()
-        self.pypx_parser.load_variables()
-        self.pypx_parser.normalize()
-        self.html_content = self.pypx_parser.parsed
+        self.pypx_parser.load_variables(_addnl_var_contexts=_)
+        self.html_content = self.pypx_parser.normalize(self.pypx_parser.parsed)
+
+    def clear_variables(self):
+        _loaders_match = re.compile("(\+\$.*?\$\+)")
+        _matches = _loaders_match.findall(self.html_content)
+        for _match in _matches:
+            self.html_content = self.html_content.replace(_match, '')
 
 
 class Config:
-    def __init__(self):
+    def __init__(self, project_root=None):
         """
         load xtracto.config.py
         """
-        config = Utils.import_module_by_path(Utils.get_config_file())
-        self.project_root = Utils.get_project_root()
-        self.module_root = Utils.root_path(getattr(config, "modules_dir", "xtractocomponents"))
-        self.pages_root = Utils.root_path(getattr(config, "pages_dir", "xtractopages"))
+        if project_root is None:
+            config = Utils.import_module_by_path(Utils.get_config_file())
+            self.project_root = Utils.get_project_root()
+            self.module_root = Utils.root_path(getattr(config, "modules_dir", "xtractocomponents"))
+            self.pages_root = Utils.root_path(getattr(config, "pages_dir", "xtractopages"))
+        else:
+            config = Config
+            self.project_root = project_root
+            self.module_root = os.getcwd()
+            self.pages_root = os.getcwd()
+        self.production = getattr(config, 'production', os.getenv("env", "prod").startswith("dev"))
         self.strip_imports = getattr(config, 'strip_imports', True)
         self.debug = getattr(config, 'debug', os.getenv("env", "prod").startswith("dev"))
         self.log_level = "debug" if self.debug else getattr(config, 'log_level', "info")
         self.raise_value_errors_while_importing = getattr(config, 'raise_value_errors_while_importing', True)
         del config
 
 
@@ -201,24 +250,27 @@
         pass
 
     @staticmethod
     def xtracto_initiated():
         pass
 
     @staticmethod
-    def get_logger():
+    def get_logger(config_path=None):
         import requestez.helpers as ez_helper
-        config = Config()
+        if config_path is None:
+            config = Config()
+        else:
+            config = Config(config_path)
         ez_helper.set_log_level(config.log_level)
         logger = ez_helper.get_logger()
         return logger
 
     @staticmethod
-    def critical(message):
-        Log.get_logger().log("c", msg=message, color="red")
+    def critical(message, config=None):
+        Log.get_logger(config).log("c", msg=message, color="red")
 
     @staticmethod
     def error(message, *args):
         Log.get_logger().stack("e", *args, msg=message, color="red")
 
     @staticmethod
     def warn(message):
@@ -260,22 +312,28 @@
         Manages api request origins,
         Manages asset delivery allowance.
         """
         pass
 
     @staticmethod
     def get_file_if_valid(path):
+        path = os.path.join(str(Config().module_root), path)
         valid = FileManager.Valid(path).valid()
         if valid[0]:
             if valid[1]:
                 return valid[1]
-            with open(os.path.join(str(Config().module_root), path)) as f:
-                return f.read()
+            if os.path.exists(path):
+                with open(path) as f:
+                    return f.read()
+            else:
+                log.critical(path, "NOT FOUND")
+                return ""
         else:
             log.critical(path + " not used")
+            log.debug(valid[1])
             return ""
 
     @staticmethod
     def get_file_type(path):
         """
             Returns the file type (extension) of the given file path.
 
@@ -307,14 +365,17 @@
 
         def valid(self) -> list[[bool, str]]:
             """
             Detects the file content type and Checks if it is valid
             """
             if self.file_type in self.invalid_types:
                 raise ValueError("invalid file type")
+            if Config().production:
+                if self.file_type != "pypx":
+                    return [True, ""]
             func = getattr(self, self.file_type, self.unknown)
             return func(self.path)
 
         def error(self):
             if self.file_type in self.invalid_types:
                 raise ValueError("invalid file type")
             func = getattr(self, self.file_type, self.unknown)
@@ -384,41 +445,62 @@
         @staticmethod
         def unknown(path):
             log.info(f"Unknown file type: {path}")
             return [True, ""]
 
         @staticmethod
         def pypx(path):
+            _contexts = []
+            nearest_self = Utils.get_variable_value_from_nearest_frame('self', _default_value="", _raise_error=False, _skip_after_current=0)
+            if nearest_self:
+                if hasattr(nearest_self, 'pypx_parser'):
+                    _contexts.append(nearest_self.pypx_parser.parsed)
+                if hasattr(nearest_self, 'parsed'):
+                    _contexts.append(nearest_self.parsed)
             try:
-                _parser = Parser(path=path, module=True)
+                _parser = Parser(path=path, module=True, _additional_contexts=_contexts)
                 _parser.parse()
-                return [True, _parser.html_content]
+                return [True, _parser]
             except Exception as e:
                 return [False, e]
 
+        @staticmethod
+        def html(path):
+            try:
+                f = open(path)
+                f.close()
+                return [True, ""]
+            except Exception as e:
+                Log.debug(e)
+                return [False, e]
+
 
 class Pypx:
-    def __init__(self, content=None, fname=None):
+    def __init__(self, content=None, fname=None, _additional_contexts=None):
         """
         Parses pypx
         """
         if content is None:
             content = ""
+        if _additional_contexts is None:
+            _additional_contexts = []
         content = content.replace("\t", " " * 4)
         self.content = content.split("\n")
+        self.contexts = _additional_contexts
         self.fname = fname
         self.parsing = self.content.copy()
         self.groups = [
             ["::", "::"],  # Removed comment
-            ["?:", ":?"],  # Comment to be inserted in html
+            ["?:", "?:"],  # File to be included as static asset
             ["{{", "}}"],  # Variable Field
             [";;", ";;"],  # HTML Attribute
-            ["[[", "]]"],  # Import Files
+            ["[[", "]]"],  # Import Files and embed them into the generated html
             ["(-(", ")-)"],  # Markdown Content
             ["{[", "]}"],  # Bundling groups
+            ["+-", "-+"],  # Set Python variable values in pypx
         ]
         self.void_elements = [
             "area",
             "base",
             "br",
             "col",
             "embed",
@@ -443,14 +525,15 @@
             "noscript", "object", "optgroup", "option", "output", "paragraphs", "phrase", "pre", "progress",
             "q", "rp", "rt", "ruby", "s", "samp", "section", "small", "spacer", "span", "strike", "strong",
             "style", "sub", "sup", "summary", "svg", "table", "tbody", "td", "template", "tfoot", "th", "thead",
             "time", "title", "tr", "tt", "underline", "var", "video", "xmp"
         ]
         self.parsed = ""
         self.blocks = []
+        self.static_requirements = {}
         del content, fname
 
     def parse(self, layout=False):
         """
         imports files, parses other stuff, does not replace variables (this is because it is required to create build files)
         """
         self.make_groups_valid()
@@ -461,25 +544,27 @@
         self.normalize()
         if not layout:
             self.use_layout()
 
     def use_layout(self):
         _layout_file = os.path.join(str(Config().pages_root), "_layout.pypx")
         if not os.path.exists(_layout_file):
-            print("NO LAYOUT FILE")
+            log.warn("NO LAYOUT FILE")
             return
         children = self.parsed
         head = re.compile("<head>(.*)</head>").findall(self.parsed)
         head = head[0] if head else ""
         children = children.replace(f"<head>{head}</head>", "")
         if not children:
             log.warn("no children")
-        _ = Parser(path="_layout.pypx", layout=True)
-        log.info(_.html_content)
+        _contexts = [self.parsed]
+        _contexts.extend(self.contexts)
+        _ = Parser(path="_layout.pypx", layout=True, _additional_contexts=_contexts)
         _.render()
+        self.static_requirements.update(_.static_requirements)
         if self.parsed not in _.html_content:
             log.critical("please put {{children}} in the layout file where the page content must appear")
         self.parsed = _.html_content
 
     def make_groups_valid(self):
         num = 0
         while num < len(self.parsing):
@@ -492,32 +577,45 @@
                                (line.count(value1) % 2 != 0) and (value1 == value2)
                        )):
                     try:
                         self.parsing[num] += "#&N#" + self.parsing[num + 1]
                         self.parsing.pop(num + 1)
                         line = self.parsing[num]
                     except IndexError:
-                        log.error("Syntax error in file being parsed", "FILE CONTENT:\n" + "\n".join(self.parsing))
+                        # log.error("Syntax error in file being parsed", "FILE CONTENT:\n" + "\n".join(self.parsing))
                         self.parsed = []
                         return
             num += 1
 
     def parse_comments(self):
         self.parsing = [
-            i.replace("?:", "<!--").replace(":?", "-->")
+            i
             for i in
-            re.sub("(::.*::)", "", "\n".join(self.parsing)).split("\n")
+            re.sub("(::.*?::)", "", "\n".join(self.parsing)).split("\n")
             if i
         ]
 
+    def parse_static_import(self):
+        static_regex = re.compile("\?:(.*?)\?:")
+        found = static_regex.findall(self.parsed)
+        static_requirements = {}
+        for i in found:
+            sanitized_i = i.replace("./", "")
+            static_requirements[sanitized_i] = i
+            self.parsed = self.parsed.replace("?:" + i + "?:", f"/__static/{sanitized_i}")
+        self.static_requirements.update(static_requirements)
+        return static_requirements
+
     def normalize(self, content=None):
+        ori_content = content
         if content is None:
             content = self.parsed
+        _loaders_match = re.compile("\+\$(.*?)\$\+")
         content = content.replace("#&N#", "\n")
-        if content is None:
+        if ori_content is None:
             self.parsed = content
         return content
 
     def parse_blocks(self):
         stack = []  # [[indent, element, children...]...]
         parent_indent = []
         for line in self.parsing:
@@ -624,59 +722,77 @@
                                 curendtx_indent = len(self.content[num]) - len(self.content[num].lstrip(" "))
                                 if nextx_indent <= curendtx_indent:
                                     pred_line = num + forward
                     log.warn(f"\n{self.fname}:{pred_line} -> element \"" + block[
                         1] + "\" must have children elements/content as this does not have any children it will be considered as plain text")
                 # SECTION FOR WARNING WHEN ELEMENT DOES NOT HAVE CHILDREN ENDS HERE
                 loaded_block += block[1]
+                loaded_block += "\n"
         if blocks == self.blocks:
             self.parsed = loaded_block
         return loaded_block
 
-    def load_variables(self, _content=None, _load_list: list or None = None):
+    def load_variables(self, _content=None, _load_list: list or None = None, _addnl_var_contexts: list or None = None):
         _original_content = _content
         if _content is None:
             _content = self.parsed
         if _load_list is None:
             _load_list = []
+        _loaders_match = re.compile("\+\$(.*?)\$\+")
+        if _addnl_var_contexts is None:
+            _addnl_var_contexts = []
+        _addnl_var_contexts.append(_content)
+        for _load in _loaders_match.findall("\n".join(_addnl_var_contexts)):
+            _load_list.append(_load.split("=", 1))
         for var, val in _load_list:
-            locals()[val] = val
+            locals()[var] = val
+        if _load_list:
+            print(locals()[_load_list[0][0]])
         if _load_list:
             del var, val
         _vars_reg = re.compile(r'\{\{(.*?)}}')
         _vars = _vars_reg.findall(_content)
         for _var in _vars:
-            _ori_var = "{{"+_var+"}}"
+            _ori_var = "{{" + _var + "}}"
             _var = _var.strip(" ")
-            log.info(_var)
             _var = _var.split("=", 1)
             if len(_var) == 2:
                 _default = _var[1]
                 _raise_error = False
             else:
                 _default = False
                 _raise_error = True
             _var = _var[0]
-            _value = Utils.get_variable_value_from_nearest_frame(_variable_name=_var, _default_value=_default,
-                                                                 _raise_error=_raise_error)
+            if _var == "tailwind_css_content":
+                _tailwind = Tailwind()
+                _value = _tailwind.generate(_content)
+            else:
+                try:
+                    print(locals()[_var])
+                except KeyError:
+                    print("NOT FOUND:", _var)
+                _value = Utils.get_variable_value_from_nearest_frame(_variable_name=_var, _default_value=_default,
+                                                                     _raise_error=_raise_error)
             _content = _content.replace(_ori_var, _value)
         if _original_content is None:
             self.parsed = _content
         return _content
 
     def do_imports(self, content=None):
         ori_cont = content
         if content is None:
             content = self.parsed
-        fixed = Pypx(content=content)
+        _contexts = [content]
+        _contexts.extend(self.contexts)
+        fixed = Pypx(content=content, _additional_contexts=_contexts)
         fixed.make_groups_valid()
         fixed = "\n".join(fixed.parsing)
-        file_groups = re.compile("(\[\[.*]])")
-        files = re.compile(r"\[\[([a-zA-Z0-9. /\\]+)(?:.*)?]]")
-        parameters = re.compile("\[\[[a-zA-Z0-9.]+\|\|(.*)\|\|.*")
+        file_groups = re.compile("(\[\[.*?]])")
+        files = re.compile(r"\[\[([a-zA-Z0-9. /\\]+)(?:.*?)?]]")
+        parameters = re.compile("\[\[[a-zA-Z0-9.]+\|\|(.*?)\|\|.*?")
         for group in file_groups.findall(fixed):
             file = files.findall(group)
             file = file[0]
             parms = parameters.findall(group)
             final_parms = []
             while parms:
                 param = parms.pop()
@@ -685,15 +801,18 @@
                     continue
                 final_parms.append(param)
             parms = [i.replace("#|#", "|") for i in final_parms]
             for num, param in enumerate(parms.copy()):
                 parms[num] = param.strip("#&N#").strip(" ").strip("#&N#").strip(" ")
             parms = [i.split("=") for i in parms]  # [[key, value]...]
             cont = FileManager.get_file_if_valid(file)
-            cont = self.load_variables(_content=cont, _load_list=parms)
+            if isinstance(cont, Parser):
+                self.static_requirements.update(cont.static_requirements)
+                cont = cont.html_content
+            cont = self.load_variables(_content=cont, _load_list=parms, _addnl_var_contexts=[content, fixed])
             fixed = fixed.replace(group, cont)
         if ori_cont is None:
             self.parsed = fixed
         return fixed
 
     def generate_bundle(self, content="", path_name=""):
         import datetime
@@ -712,20 +831,20 @@
             path_name = ".".join(path_name.split(".")[:-1])
         if path_name.startswith(".\\"):
             pass
         elif path_name.startswith("\\"):
             path_name = "." + path_name
         else:
             path_name = ".\\" + path_name
-        fixed = Pypx(content=content)
+        fixed = Pypx(content=content, _additional_contexts=self.contexts)
         fixed.make_groups_valid()
         fixed = "\n".join(fixed.parsing)
-        file_groups = re.compile("(\[\{.*}])")
-        files = re.compile(r"\[\{([a-zA-Z0-9. /\\]+)(?:.*)?}]")
-        parameters = re.compile("\[\{[a-zA-Z0-9.]+\|\|(.*)\|\|.*")
+        file_groups = re.compile("(\[\{.*?}])")
+        files = re.compile(r"\[\{([a-zA-Z0-9. /\\]+)(?:.*?)?}]")
+        parameters = re.compile("\[\{[a-zA-Z0-9.]+\|\|(.*?)\|\|.*?")
         bundles = {}
         for group in file_groups.findall(fixed):
             file = files.findall(group)
             file = file[0]
             bgroup = file.split(".")[-1]
             if bgroup in bundles:
                 bundles[bgroup]["files"].append(group)
@@ -776,15 +895,15 @@
                         continue
                     final_parms.append(param)
                 parms = [i.replace("#|#", "|") for i in final_parms]
                 for num, param in enumerate(parms.copy()):
                     parms[num] = param.strip("#&N#").strip(" ").strip("#&N#").strip(" ")
                 parms = [i.split("=") for i in parms]  # [[key, value]...]
                 cont = FileManager.get_file_if_valid(file)
-                cont = self.load_variables(_content=cont, _load_list=parms)
+                cont = self.load_variables(_content=cont, _load_list=parms, _addnl_var_contexts=[self.parsed, content, fixed, ])
                 bundles[bgroup]["content"] += cont
         for bgroup in bundles:
             with open(os.path.join(str(Config().module_root), path_name + "." + bundles[bgroup]["hash"] + "." + bgroup),
                       "wt") as f:
                 f.write(bundles[bgroup]["content"])
             while len(bundles[bgroup]["files"]) > 1:
                 popped = bundles[bgroup]["files"].pop(0)
@@ -807,25 +926,60 @@
         """
         import markdown2
         self.content = content
         self.parsed = markdown2.markdown(content)
 
 
 class App:
-    def __init__(self):
-        for _ in range(10):
-            log.critical("THIS FEATURE IS NOT IMPLEMENTED DO NOT USE THIS")
-        from fastapi import FastAPI, HTTPException, status
-        import uvicorn
-        self.app = FastAPI()
+    def __init__(self, app: FastAPI, auto_run=True, uvicorn_kwargs=None):
+        for _ in range(1):
+            log.warn("THIS FEATURE IS NOT IMPLEMENTED COMPLETELY")
+        self.app = app
         self.add_routes()
         self.not_authorized = HTTPException(status_code=status.HTTP_403_FORBIDDEN,
                                             detail="You are not authorized to access this file")
-        uvicorn.run(self.app, )
+        self.static_assets = {}
+        if uvicorn_kwargs is None:
+            uvicorn_kwargs = {}
+        if auto_run:
+            import uvicorn
+            uvicorn.run(self.app, **uvicorn_kwargs)
 
     def add_routes(self):
+        @self.app.middleware("*")
+        async def set_assisted_by_header(request: Request, next_process):
+            resp = await next_process(request)
+            resp.headers['X-Assisted-By'] = 'eXTRACTO by shashstormer'
+            return resp
+
+        @self.app.get("/__static/{path:path}")
+        async def serve_static_files(path: str):
+            file_path = self.static_assets.get(path, False)
+            if not file_path:
+                raise self.not_authorized
+            with open(file_path, "rb") as f:
+                file_content = f.read()
+            return Response(file_content)
+
         @self.app.get("/{path:path}")
         async def serve_pages(path: str = ""):
             if path == "":
                 path += "index"
-            if path.startswith("_"):
+            _pypx_c1 = "../" in path
+            _pypx_c2 = path.startswith("_")
+            _pypx_c3 = "..\\/" in path
+            _pypx_overall = _pypx_c1 or _pypx_c2 or _pypx_c3
+            if _pypx_overall:
                 raise self.not_authorized
+            if len(path.split("/")[-1].split(".")) == 1:
+                path += ".pypx"
+            if path == "favicon.ico":
+                if os.path.exists(Utils.get_project_root() + "/favicon.ico"):
+                    return FileResponse(Utils.get_project_root() + "/favicon.ico")
+                else:
+                    import xtracto._images
+                    return xtracto._images.favicon
+            _pypx_parsed = Parser(path=path, layout=Utils.layout_exists())
+            _pypx_parsed.render()
+            _pypx_parsed.clear_variables()
+            self.static_assets.update(_pypx_parsed.static_requirements)
+            return Response(_pypx_parsed.html_content, media_type="text/html")
```

### Comparing `xtracto-0.0.4/setup.py` & `xtracto-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='xtracto',
-    version='0.0.4',
+    version='0.0.5',
     author='shashstormer',
     description='Xtracto is a lightweight web development framework designed to simplify the process of creating dynamic web pages using Python and pypx. ',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    packages=find_packages(),
+    packages=['xtracto'],
     install_requires=[
-        "fastapi", "uvicorn", "beautifulsoup4", "requestez"
+        "fastapi", "uvicorn", "beautifulsoup4", "requestez", "pytailwind",
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

### Comparing `xtracto-0.0.4/xtracto/_images.py` & `xtracto-0.0.5/xtracto/_images.py`

 * *Files identical despite different names*

### Comparing `xtracto-0.0.4/xtracto.egg-info/PKG-INFO` & `xtracto-0.0.5/xtracto.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtracto
-Version: 0.0.4
+Version: 0.0.5
 Summary: Xtracto is a lightweight web development framework designed to simplify the process of creating dynamic web pages using Python and pypx. 
 Author: shashstormer
 Project-URL: GitHub, https://github.com/shashstormer/xtracto
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,15 @@
 Classifier: Topic :: Database
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
 Requires-Dist: beautifulsoup4
 Requires-Dist: requestez
+Requires-Dist: pytailwind
 
 
 # Xtracto Web Development Framework
 eXtensible, Configurable, and Reusable Automation Component Tool and Organizer <sub>for html through pypx</sub>
 
 
 Xtracto is a lightweight web development framework designed to simplify the process of creating dynamic web pages using Python.
```

