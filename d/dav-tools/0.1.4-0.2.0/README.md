# Comparing `tmp/dav_tools-0.1.4.tar.gz` & `tmp/dav_tools-0.2.0.tar.gz`

## Comparing `dav_tools-0.1.4.tar` & `dav_tools-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 dav_tools-0.1.4/.readthedocs.yaml
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 dav_tools-0.1.4/Makefile
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dav_tools-0.1.4/requirements.txt
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dav_tools-0.1.4/docs/Makefile
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 dav_tools-0.1.4/docs/conf.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 dav_tools-0.1.4/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 dav_tools-0.1.4/docs/make.bat
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dav_tools-0.1.4/docs/requirements.txt
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 dav_tools-0.1.4/src/dav_tools/__init__.py
--rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 dav_tools-0.1.4/src/dav_tools/_arg_parser.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dav_tools-0.1.4/src/dav_tools/_text_format.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 dav_tools-0.1.4/src/dav_tools/commands.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 dav_tools-0.1.4/src/dav_tools/devtools.py
--rw-r--r--   0        0        0     8079 2020-02-02 00:00:00.000000 dav_tools-0.1.4/src/dav_tools/messages.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 dav_tools-0.1.4/src/dav_tools/requirements.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 dav_tools-0.1.4/src/dav_tools/text_format.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dav_tools-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dav_tools-0.1.4/tests/test_messages.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 dav_tools-0.1.4/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 dav_tools-0.1.4/LICENSE
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 dav_tools-0.1.4/README.md
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 dav_tools-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 dav_tools-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 dav_tools-0.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 dav_tools-0.2.0/Makefile
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dav_tools-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 dav_tools-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 dav_tools-0.2.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 dav_tools-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dav_tools-0.2.0/docs/requirements.txt
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 dav_tools-0.2.0/src/dav_tools/__init__.py
+-rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 dav_tools-0.2.0/src/dav_tools/_arg_parser.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dav_tools-0.2.0/src/dav_tools/_text_format.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 dav_tools-0.2.0/src/dav_tools/commands.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 dav_tools-0.2.0/src/dav_tools/database.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 dav_tools-0.2.0/src/dav_tools/devtools.py
+-rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 dav_tools-0.2.0/src/dav_tools/messages.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 dav_tools-0.2.0/src/dav_tools/requirements.py
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 dav_tools-0.2.0/src/dav_tools/text_format.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dav_tools-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dav_tools-0.2.0/tests/test_messages.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 dav_tools-0.2.0/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 dav_tools-0.2.0/LICENSE
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 dav_tools-0.2.0/README.md
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 dav_tools-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 dav_tools-0.2.0/PKG-INFO
```

### Comparing `dav_tools-0.1.4/.readthedocs.yaml` & `dav_tools-0.2.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.4/Makefile` & `dav_tools-0.2.0/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Makefile by Davide Ponzini
 
 NAME=dav-tools
-PY=python3
+PY=python
 
 
 prepare: test documentation
 	:
 
 install: uninstall build
 	$(PY) -m pip install ./dist/*.whl
```

### Comparing `dav_tools-0.1.4/docs/Makefile` & `dav_tools-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.4/docs/conf.py` & `dav_tools-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.4/docs/index.rst` & `dav_tools-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.4/docs/make.bat` & `dav_tools-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.4/src/dav_tools/_arg_parser.py` & `dav_tools-0.2.0/src/dav_tools/_arg_parser.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.4/src/dav_tools/_text_format.py` & `dav_tools-0.2.0/src/dav_tools/_text_format.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.4/src/dav_tools/commands.py` & `dav_tools-0.2.0/src/dav_tools/commands.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 '''External command execution on local machine.'''
 
 import platform as _platform
 import subprocess as _subprocess
 from shlex import split as _split
 from subprocess import CalledProcessError
 from typing import Callable as _Callable
+import sys as _sys
 
 
-def execute(command: str) -> bool:
+def execute(command: str, stdin = _sys.stdin, stdout = _sys.stdout, stderr = _sys.stderr) -> bool:
     '''
     Run a command.
 
     :param command: the command to execute
 
+    :param stdin: input redirection
+    :param stdout: output redirection
+    :param stderr: error redirection
+
     :returns: `True` if the command exits with return code zero, `False` otherwise
     '''
-    exit_status = _subprocess.check_call(_split(command))
+    exit_status = _subprocess.check_call(_split(command), stdin=stdin, stdout=stdout, stderr=stderr)
     return exit_status == 0
 
-def get_output(command: str, on_success: _Callable[[bytes], any] = lambda x: x, on_error: _Callable[[], any] = None):
+def get_output(command: str, on_success: _Callable[[bytes], any] = lambda x: x, on_error: _Callable[[], any] = None,
+               stdin = _sys.stdin, stderr = _sys.stderr):
     '''
     Run a command and return its output.
     
     :param command: the command to execute
 
     :param on_success: call the specified function on the output before returning the data. Useful for casting the output from its original `bytes` format
     :param on_error: call the specified function if the command raised an exception. If this value is `None`, raises the exception.
-    '''
+
+    :param stdin: input redirection
+    :param stderr: error redirection
+            '''
     try:
-        return on_success(_subprocess.check_output(_split(command)))
+        return on_success(_subprocess.check_output(_split(command), stdin=stdin, stderr=stderr))
     except CalledProcessError as e:
         if on_error is None:
             raise e
         return on_success(on_error())
```

### Comparing `dav_tools-0.1.4/src/dav_tools/devtools.py` & `dav_tools-0.2.0/src/dav_tools/devtools.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.4/src/dav_tools/text_format.py` & `dav_tools-0.2.0/src/dav_tools/text_format.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,28 +14,30 @@
 
     :returns: The format string corresponding to the options.
     '''
 
     result = ''
 
     for option in options:
-        result += option.decode()
+        if option is not None:
+            result += option.decode()
 
     return result
 
 def _set_format(*options, file = _sys.stdout):
     '''
     Set text styling.
 
     :param option: Text styling options.
     :param file: Where to set text styling.
     '''
 
     for option in options:
-        print(option.decode(), end='', file=file)
+        if option is not None:
+            print(option.decode(), end='', file=file)
 
 def format_text(text: str, *format_options) -> str:
     '''
     Return a styled text.
 
     :param text: Text to print.
     :param format_options: Text styling options.
```

### Comparing `dav_tools-0.1.4/tests/test_messages.py` & `dav_tools-0.2.0/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.4/LICENSE` & `dav_tools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.4/pyproject.toml` & `dav_tools-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dav_tools"
-version = "0.1.4"
+version = "0.2.0"
 authors = [
   { name="Davide Ponzini", email="davide.ponzini95@gmail.com" },
 ]
 description = "Various utilies to aid in program development."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dav_tools-0.1.4/PKG-INFO` & `dav_tools-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dav_tools
-Version: 0.1.4
+Version: 0.2.0
 Summary: Various utilies to aid in program development.
 Project-URL: Repository, https://github.com/DavidePonzini/dav-utils
 Project-URL: Documentation, https://dav-tools.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/DavidePonzini/dav-utils/issues
 Author-email: Davide Ponzini <davide.ponzini95@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

