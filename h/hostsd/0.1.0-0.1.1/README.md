# Comparing `tmp/hostsd-0.1.0.tar.gz` & `tmp/hostsd-0.1.1.tar.gz`

## Comparing `hostsd-0.1.0.tar` & `hostsd-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 hostsd-0.1.0/.forgejo/workflows/pypi.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hostsd-0.1.0/src/hostsd/__init__.py
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 hostsd-0.1.0/src/hostsd/__main__.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 hostsd-0.1.0/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 hostsd-0.1.0/LICENSE
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 hostsd-0.1.0/README.md
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 hostsd-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 hostsd-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 hostsd-0.1.1/.forgejo/workflows/pypi.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hostsd-0.1.1/src/hostsd/__init__.py
+-rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 hostsd-0.1.1/src/hostsd/__main__.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 hostsd-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 hostsd-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 hostsd-0.1.1/README.md
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 hostsd-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 hostsd-0.1.1/PKG-INFO
```

### Comparing `hostsd-0.1.0/.forgejo/workflows/pypi.yml` & `hostsd-0.1.1/.forgejo/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `hostsd-0.1.0/src/hostsd/__main__.py` & `hostsd-0.1.1/src/hostsd/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,107 @@
 from pathlib import Path
-from os import PathLike
-from typing import Union
+from os import PathLike, sep
+from typing import Union, Optional, List
 from argparse import ArgumentParser
-from pathlib import Path
 
 import sys
 
 HOSTS_DIR = "/etc/hosts.d/"
 HOSTS_FILE = "/etc/hosts"
 
 HOSTS_DIR_WINDOWS = "C:\\Windows\\System32\\drivers\\etc\\hosts.d\\"
 HOSTS_FILE_WINDOWS = "C:\\Windows\\System32\\drivers\\etc\\hosts"
 
 
-def get_new_content(dirpath: Union[str, PathLike] = HOSTS_DIR) -> str:
-    """Read all files from a directory and join their contents in a string
+def read_directory(
+    dirpath: Optional[Union[str, PathLike]] = HOSTS_DIR, prefix: Optional[str] = None
+) -> List[Path]:
+    """Read all files from a directory
 
     This will not read files with names that begin with a period ("."), or binary files.
 
     Args:
         dir (str, optional): The directory from which to read files. Defaults to "/etc/hosts.d/".
+        prefix (str, optional): Prefix to add to the file path in the output. Defaults to None.
 
     Raises:
         IOError: Raised if the provided source path does not exist or is not a directory.
 
     Returns:
-        str: Joined content of read files
+        list[Path]: List of Path objects representing files in the directory
     """
-    content: str = ""
-
     directory = Path(dirpath)
 
     if not (directory.exists() and directory.is_dir()):
         raise IOError(f"Directory {dirpath} does not exist or is not a directory.")
 
-    for infile in sorted(list(directory.iterdir()), key=lambda f: f.name):
+    for infile in sorted(list(directory.glob("**/*")), key=lambda f: f.name):
+        full_path = f"{prefix if prefix else ''}{sep if prefix and prefix[-1] != sep else ''}{infile.name}"
+
         if (
             infile.is_file()
             and not infile.name.startswith(".")
             and not infile.name.endswith(".disabled")
         ):
-            with infile.open('r') as openfile:
-                try:
-                    filecontent = openfile.read()
-                except UnicodeDecodeError:
-                    print(f"File {infile.name} is not a text file - skipping")
+            try:
+                filecontent = infile.read_text()
+                if "HOSTSD_IGNORE" in filecontent:
+                    print(f"File {infile.name} is marked as ignored - skipping")
+                    continue
+            except UnicodeDecodeError:
+                print(f"File {infile.name} is not a text file - skipping")
+                return
+
+            yield f"# {full_path}\n\n{filecontent}"
+
+        elif infile.is_dir():
+            yield from read_directory(infile, full_path)
+
+
+def get_new_content(dirpath: Union[str, PathLike] = HOSTS_DIR) -> str:
+    """Read all files from a directory and join their contents in a string
+
+    This will not read files with names that begin with a period ("."), or binary files.
+
+    Args:
+        dir (str, optional): The directory from which to read files. Defaults to "/etc/hosts.d/".
+
+    Raises:
+        IOError: Raised if the provided source path does not exist or is not a directory.
+
+    Returns:
+        str: Joined content of read files
+    """
+    content: str = ""
+
+    directory = Path(dirpath)
+
+    if not (directory.exists() and directory.is_dir()):
+        raise IOError(f"Directory {dirpath} does not exist or is not a directory.")
 
-                if content:
-                    content += "\n\n"
+    for infile in read_directory(dirpath):
+        if content:
+            content += "\n\n"
 
-                content += f"# {infile.name}\n\n{filecontent}"
+        content += infile
 
     return content
 
 
 def write_hosts_file(content: str, path: Union[str, PathLike] = HOSTS_FILE):
     """Simple function writing text content to a file given by path
 
     Args:
         content (str): Text content to be written.
         path (Union[str, PathLike], optional): Path of the file to write to. Defaults to "/etc/hosts".
 
     Raises:
         IOError: Raised if the provided file path could not be written to.
     """
-    with Path(path).open('w') as hostsfile:
+    with Path(path).open("w") as hostsfile:
         try:
             hostsfile.write(content)
         except Exception as e:
             raise IOError(f"Unable to write file {path} – {e}")
 
 
 def main():
```

### Comparing `hostsd-0.1.0/LICENSE` & `hostsd-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hostsd-0.1.0/README.md` & `hostsd-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # hostsd - A simple hosts file manager
 
 [![Support Private.coffee!](https://shields.private.coffee/badge/private.coffee-support%20us!-pink?logo=coffeescript)](https://private.coffee)
 [![PyPI](https://shields.private.coffee/pypi/v/hostsd)](https://pypi.org/project/hostsd/)
 [![PyPI - Python Version](https://shields.private.coffee/pypi/pyversions/hostsd)](https://pypi.org/project/hostsd/)
 [![PyPI - License](https://shields.private.coffee/pypi/l/hostsd)](https://pypi.org/project/hostsd/)
-[![Git Workflow Status](https://shields.private.coffee/gitea/last-commit/kumi/hostsd?gitea-url=https://git.private.coffee)](https://git.private.coffee/kumi/hostsd)
+[![Latest Git Commit](https://shields.private.coffee/gitea/last-commit/kumi/hostsd?gitea_url=https://git.private.coffee)](https://git.private.coffee/kumi/hostsd)
 
 `hostsd` is a simple hosts file manager that allows you to separate your hosts file into multiple files and easily enable or disable them. It's useful for development environments where you need to manage lots of hosts entries, or for managing ad-blocking hosts files.
 
 ## Dependencies
 
 - Python 3.8 or later (earlier versions may work but are untested)
 - Linux or macOS (should work on Windows too but is untested)
```

### Comparing `hostsd-0.1.0/pyproject.toml` & `hostsd-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hostsd"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Kumi Mitterer", email="hostsd@kumi.email" },
 ]
 description = "A simple hosts file manager"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `hostsd-0.1.0/PKG-INFO` & `hostsd-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hostsd
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple hosts file manager
 Project-URL: Homepage, https://git.private.coffee/kumi/hostsd
 Project-URL: Bug Tracker, https://git.private.coffee/kumi/hostsd/issues
 Project-URL: Source Code, https://git.private.coffee/kumi/hostsd
 Author-email: Kumi Mitterer <hostsd@kumi.email>
 License: Copyright (c) 2023 Kumi Mitterer <hostsd@kumi.email>
         
@@ -34,15 +34,15 @@
 
 # hostsd - A simple hosts file manager
 
 [![Support Private.coffee!](https://shields.private.coffee/badge/private.coffee-support%20us!-pink?logo=coffeescript)](https://private.coffee)
 [![PyPI](https://shields.private.coffee/pypi/v/hostsd)](https://pypi.org/project/hostsd/)
 [![PyPI - Python Version](https://shields.private.coffee/pypi/pyversions/hostsd)](https://pypi.org/project/hostsd/)
 [![PyPI - License](https://shields.private.coffee/pypi/l/hostsd)](https://pypi.org/project/hostsd/)
-[![Git Workflow Status](https://shields.private.coffee/gitea/last-commit/kumi/hostsd?gitea-url=https://git.private.coffee)](https://git.private.coffee/kumi/hostsd)
+[![Latest Git Commit](https://shields.private.coffee/gitea/last-commit/kumi/hostsd?gitea_url=https://git.private.coffee)](https://git.private.coffee/kumi/hostsd)
 
 `hostsd` is a simple hosts file manager that allows you to separate your hosts file into multiple files and easily enable or disable them. It's useful for development environments where you need to manage lots of hosts entries, or for managing ad-blocking hosts files.
 
 ## Dependencies
 
 - Python 3.8 or later (earlier versions may work but are untested)
 - Linux or macOS (should work on Windows too but is untested)
```

