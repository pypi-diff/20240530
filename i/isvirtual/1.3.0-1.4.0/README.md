# Comparing `tmp/isvirtual-1.3.0.tar.gz` & `tmp/isvirtual-1.4.0.tar.gz`

## Comparing `isvirtual-1.3.0.tar` & `isvirtual-1.4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 isvirtual-1.3.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 isvirtual-1.3.0/.github/workflows/release.yml
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 isvirtual-1.3.0/isvirtual/VERSION.md
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 isvirtual-1.3.0/isvirtual/__init__.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 isvirtual-1.3.0/isvirtual/cli.py
--rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 isvirtual-1.3.0/isvirtual/main.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 isvirtual-1.3.0/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 isvirtual-1.3.0/LICENSE
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 isvirtual-1.3.0/README.md
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 isvirtual-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 isvirtual-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 isvirtual-1.4.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 isvirtual-1.4.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 isvirtual-1.4.0/isvirtual/VERSION.md
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 isvirtual-1.4.0/isvirtual/__init__.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 isvirtual-1.4.0/isvirtual/cli.py
+-rw-r--r--   0        0        0     7281 2020-02-02 00:00:00.000000 isvirtual-1.4.0/isvirtual/main.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 isvirtual-1.4.0/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 isvirtual-1.4.0/LICENSE
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 isvirtual-1.4.0/README.md
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 isvirtual-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7764 2020-02-02 00:00:00.000000 isvirtual-1.4.0/PKG-INFO
```

### Comparing `isvirtual-1.3.0/.github/workflows/publish.yml` & `isvirtual-1.4.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `isvirtual-1.3.0/.github/workflows/release.yml` & `isvirtual-1.4.0/.github/workflows/release.yml`

 * *Files 11% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         run: pip install build
 
       - name: Build
         run: python -m build
 
       - name: Read VERSION file
         id: getversion
-        run: echo "version=$(cat src/VERSION.md)" >> $GITHUB_OUTPUT
+        run: echo "version=$(cat isvirtual/VERSION.md)" >> $GITHUB_OUTPUT
 
       - name: Changelog
         run: git log $(git describe --tags --abbrev=0)..HEAD --format="%s %h" > LATEST-CHANGES.md
 
       - name: Release
         uses: softprops/action-gh-release@v2
         with:
```

### Comparing `isvirtual-1.3.0/isvirtual/main.py` & `isvirtual-1.4.0/isvirtual/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import hashlib
 import json
 import os
 import re
 import sys
 from contextlib import suppress
 from pathlib import Path
+import subprocess
 
 from platformdirs import user_cache_path
 
 config = None
 
 
 def is_virtual() -> bool:
@@ -124,61 +125,95 @@
     if config is None:
         conf = configparser.ConfigParser()
         with open(path) as stream:
             # Add fake section name to make pyvenv.cfg compatible with ConfigParser
             conf.read_string("[root]\n" + stream.read())
         config = conf
 
+def _read_config_static(path: str) -> dict:
+    config = {}
+    conf = configparser.ConfigParser()
+    with open(path) as stream:
+        # Add fake section name to make pyvenv.cfg compatible with ConfigParser
+        conf.read_string("[root]\n" + stream.read())
+    config = dict(conf["root"])
+    return config
 
-def check_dir(path: str | Path):
+
+def check_dir(path: str | Path) -> dict:
     if isinstance(path, str) is True:
         path = Path(path)
 
     if path == Path("."):
         path = Path(os.getcwd())
 
+    config = {}
     # Check classic virtual env in a given directory
     for file in path.iterdir():
         if file.is_dir() is True:
             if (
                 (file / "bin").exists() is True
                 and (file / "bin" / "activate").exists() is True
                 and (file / "include").exists() is True
                 and (file / "lib").exists() is True
                 and (file / "pyvenv.cfg").exists() is True
             ):
-                # config = _read_config(str(file / "pyvenv.cfg"))
-                # return config
-                print(f"Found venv/virtualenv: {file}")
-                return True
+                config = _read_config_static(str(file / "pyvenv.cfg"))
+                config["path"] = str(file)
+                if "virtualenv" in config:
+                    config["source"] = "virtualenv"
+                else:
+                    config["source"] = "venv"
 
     # Check for poetry
     poetry_hash = generate_env_name(path.name, str(path))
     # From https://github.com/python-poetry/poetry/blob/108d7323280889b277751807fb7d564674fe6896/src/poetry/locations.py
     poetry_root = Path(user_cache_path("pypoetry", appauthor=False))
 
     poetry_venvs = poetry_root / "virtualenvs"
+    poetry_envs = list(Path(poetry_venvs).glob(f"{poetry_hash}-*"))
     if (
         poetry_venvs.exists() is True
-        and len(list(Path(poetry_venvs).glob(f"{poetry_hash}-*"))) > 0
+        and len(poetry_envs) > 0
     ):
-        print(f"Found Poetry env: {poetry_venvs}")
-        return True
+        config = _read_config_static(str(poetry_envs[0] / "pyvenv.cfg"))
+        config["path"] = str(poetry_envs[0])
+        config["source"] = "poetry"
 
     # Check for pipenv
     pipenv_hash = generate_env_name(path.name, str(path / "Pipfile"))
     pipenv_root = Path("~/.local/share").expanduser() / "virtualenvs"
 
     if pipenv_root.exists() is True and (pipenv_files := Path(pipenv_root).glob("*")):
         for pipenv_file in pipenv_files:
             if pipenv_file.name == pipenv_hash:
-                print(f"Found Pipenv env: {pipenv_file}")
-                return True
+                config = _read_config_static(str(pipenv_file / "pyvenv.cfg"))
+                config["path"] = str(pipenv_file)
+                config["source"] = "pipenv"
+
+    return config
+
 
-    return False
+def scan_dir(path: str) -> list[str]:
+    output = subprocess.check_output(
+        f"find {path} -name activate -type f 2>/dev/null", shell=True
+    )
+    envs = output.decode("utf-8")
+    validated_envs = []
+    for line in envs.split("\n"):
+        if len(line) > 0:
+            cpath = Path(line)
+            if (
+                (cpath.parent.parent / "bin").exists() is True
+                and (cpath.parent.parent / "include").exists() is True
+                and (cpath.parent.parent / "lib").exists() is True
+                and (cpath.parent.parent / "pyvenv.cfg").exists() is True
+            ):
+                validated_envs.append(cpath.parent.parent)
+    return validated_envs
 
 
 def _encode(string: str, encodings: list[str] | None = None) -> bytes:
     if isinstance(string, bytes):
         return string
     encodings = encodings or ["utf-8", "latin1", "ascii"]
     for encoding in encodings:
```

### Comparing `isvirtual-1.3.0/LICENSE` & `isvirtual-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isvirtual-1.3.0/pyproject.toml` & `isvirtual-1.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "isvirtual"
-description = "Detect if your script is running inside a virtual environment"
+description = "Tool to detect if the current directory is linked to a virtual environment, get the config of this env and more. Work with venv, virtualenv, pipenv, poetry and soon hatch and pdm."
 dynamic = ["version"]
 readme = "README.md"
 authors = [{ name = "Alex Mili" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.3"
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -22,16 +22,16 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.13",
 ]
-keywords = ["virtual", "env", "venv", "virtualenv", "environment", "poetry", "pipenv", "pdm"]
-dependencies = ["platformdirs", "typer"]
+keywords = ["virtual", "env", "venv", "virtualenv", "environment", "poetry", "pipenv", "pdm", "hatch"]
+dependencies = ["platformdirs", "typer", "sty"]
 
 [project.urls]
 Homepage = "https://github.com/AlexMili/isVirtual"
 Issues = "https://github.com/AlexMili/isVirtual/issues"
 Repository = "https://github.com/AlexMili/isVirtual"
 Documentation = "https://github.com/AlexMili/isVirtual"
```

