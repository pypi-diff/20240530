# Comparing `tmp/sphinxcontrib_typer-0.2.3.tar.gz` & `tmp/sphinxcontrib_typer-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib_typer-0.2.3.tar", max compression
+gzip compressed data, was "sphinxcontrib_typer-0.2.4.tar", max compression
```

## Comparing `sphinxcontrib_typer-0.2.3.tar` & `sphinxcontrib_typer-0.2.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1068 2023-12-14 00:10:27.893967 sphinxcontrib_typer-0.2.3/LICENSE
--rw-r--r--   0        0        0     5323 2024-05-18 14:56:08.366192 sphinxcontrib_typer-0.2.3/README.md
--rw-r--r--   0        0        0     2914 2024-05-22 16:54:07.852818 sphinxcontrib_typer-0.2.3/pyproject.toml
--rw-r--r--   0        0        0    34497 2024-05-22 17:06:43.503141 sphinxcontrib_typer-0.2.3/sphinxcontrib/typer/__init__.py
--rw-r--r--   0        0        0     6950 1970-01-01 00:00:00.000000 sphinxcontrib_typer-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-03 19:52:41.798588 sphinxcontrib_typer-0.2.4/LICENSE
+-rw-r--r--   0        0        0     5323 2024-05-29 23:45:18.623298 sphinxcontrib_typer-0.2.4/README.md
+-rw-r--r--   0        0        0     2914 2024-05-29 23:45:48.141309 sphinxcontrib_typer-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0    34769 2024-05-29 23:47:41.002365 sphinxcontrib_typer-0.2.4/sphinxcontrib/typer/__init__.py
+-rw-r--r--   0        0        0     6950 1970-01-01 00:00:00.000000 sphinxcontrib_typer-0.2.4/PKG-INFO
```

### Comparing `sphinxcontrib_typer-0.2.3/LICENSE` & `sphinxcontrib_typer-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_typer-0.2.3/README.md` & `sphinxcontrib_typer-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_typer-0.2.3/pyproject.toml` & `sphinxcontrib_typer-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinxcontrib-typer"
-version = "0.2.3"
+version = "0.2.4"
 description = "Auto generate docs for typer commands."
 authors = ["Brian Kohan <bckohan@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sphinx-contrib/typer"
 homepage = "https://sphinxcontrib-typer.readthedocs.io"
 classifiers = [
```

### Comparing `sphinxcontrib_typer-0.2.3/sphinxcontrib/typer/__init__.py` & `sphinxcontrib_typer-0.2.4/sphinxcontrib/typer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,19 +40,19 @@
 from rich import terminal_theme as rich_theme
 from rich.console import Console
 from rich.theme import Theme
 from sphinx import application
 from sphinx.util import logging
 
 from typer import rich_utils as typer_rich_utils
-from typer.main import Typer, TyperGroup
+from typer.main import Typer, TyperGroup, TyperInfo
 from typer.main import get_command as get_typer_command
 from typer.models import Context as TyperContext
 
-VERSION = (0, 2, 3)
+VERSION = (0, 2, 4)
 
 __title__ = "SphinxContrib Typer"
 __version__ = ".".join(str(i) for i in VERSION)
 __author__ = "Brian Kohan"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Brian Kohan"
 
@@ -291,20 +291,25 @@
         :param typer_path: The python path to the Typer app instance.
         """
 
         def resolve_root_command(obj):
             if isinstance(obj, (click.Command, click.Group)):
                 return obj
 
-            if isinstance(obj, Typer):
+            # use lenient duck typing check incase obj is a proxy for a Typer instance
+            if isinstance(obj, Typer) or isinstance(
+                getattr(obj, "info", None, TyperInfo)
+            ):
                 return get_typer_command(obj)
 
             if callable(obj):
                 ret = obj()
-                if isinstance(ret, Typer):
+                if isinstance(ret, Typer) or isinstance(
+                    getattr(obj, "info", None, TyperInfo)
+                ):
                     return get_typer_command(obj)
                 if isinstance(ret, (click.Command, click.Group)):
                     return ret
 
             raise self.error(
                 f'"{typer_path}" of type {type(obj)} is not Typer, click.Command or '
                 "click.Group."
```

### Comparing `sphinxcontrib_typer-0.2.3/PKG-INFO` & `sphinxcontrib_typer-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-typer
-Version: 0.2.3
+Version: 0.2.4
 Summary: Auto generate docs for typer commands.
 Home-page: https://sphinxcontrib-typer.readthedocs.io
 License: MIT
 Author: Brian Kohan
 Author-email: bckohan@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

