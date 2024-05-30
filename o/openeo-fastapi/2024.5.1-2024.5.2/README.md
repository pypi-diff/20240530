# Comparing `tmp/openeo_fastapi-2024.5.1.tar.gz` & `tmp/openeo_fastapi-2024.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openeo_fastapi-2024.5.1.tar", max compression
+gzip compressed data, was "openeo_fastapi-2024.5.2.tar", max compression
```

## Comparing `openeo_fastapi-2024.5.1.tar` & `openeo_fastapi-2024.5.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11358 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/LICENSE
--rw-r--r--   0        0        0     2191 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/README.md
--rw-r--r--   0        0        0        0 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/api/__init__.py
--rw-r--r--   0        0        0    19273 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/api/app.py
--rw-r--r--   0        0        0    21803 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/api/models.py
--rw-r--r--   0        0        0    18134 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/api/types.py
--rw-r--r--   0        0        0     1778 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/cli.py
--rw-r--r--   0        0        0        0 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/client/__init__.py
--rw-r--r--   0        0        0     7848 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/client/auth.py
--rw-r--r--   0        0        0     6469 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/client/collections.py
--rw-r--r--   0        0        0     6260 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/client/core.py
--rw-r--r--   0        0        0     3408 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/client/files.py
--rw-r--r--   0        0        0    13680 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/client/jobs.py
--rw-r--r--   0        0        0    11239 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/client/processes.py
--rw-r--r--   0        0        0        0 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/client/psql/__init__.py
--rw-r--r--   0        0        0     5077 2024-05-28 09:57:54.469145 openeo_fastapi-2024.5.1/openeo_fastapi/client/psql/engine.py
--rw-r--r--   0        0        0     2493 2024-05-28 09:57:54.469145 openeo_fastapi-2024.5.1/openeo_fastapi/client/psql/models.py
--rw-r--r--   0        0        0      828 2024-05-28 09:57:54.469145 openeo_fastapi-2024.5.1/openeo_fastapi/client/psql/settings.py
--rw-r--r--   0        0        0      737 2024-05-28 09:57:54.469145 openeo_fastapi-2024.5.1/openeo_fastapi/client/register.py
--rw-r--r--   0        0        0     2257 2024-05-28 09:57:54.469145 openeo_fastapi-2024.5.1/openeo_fastapi/client/settings.py
--rw-r--r--   0        0        0     1426 2024-05-28 09:57:54.469145 openeo_fastapi-2024.5.1/openeo_fastapi/templates.py
--rw-r--r--   0        0        0     1388 2024-05-28 09:57:54.469145 openeo_fastapi-2024.5.1/pyproject.toml
--rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 openeo_fastapi-2024.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-30 08:56:01.395262 openeo_fastapi-2024.5.2/LICENSE
+-rw-r--r--   0        0        0     2191 2024-05-30 08:56:01.395262 openeo_fastapi-2024.5.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-30 08:56:01.399262 openeo_fastapi-2024.5.2/openeo_fastapi/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 08:56:01.399262 openeo_fastapi-2024.5.2/openeo_fastapi/api/__init__.py
+-rw-r--r--   0        0        0    19273 2024-05-30 08:56:01.399262 openeo_fastapi-2024.5.2/openeo_fastapi/api/app.py
+-rw-r--r--   0        0        0    21803 2024-05-30 08:56:01.399262 openeo_fastapi-2024.5.2/openeo_fastapi/api/models.py
+-rw-r--r--   0        0        0    18134 2024-05-30 08:56:01.399262 openeo_fastapi-2024.5.2/openeo_fastapi/api/types.py
+-rw-r--r--   0        0        0     1634 2024-05-30 08:56:01.399262 openeo_fastapi-2024.5.2/openeo_fastapi/cli.py
+-rw-r--r--   0        0        0        0 2024-05-30 08:56:01.399262 openeo_fastapi-2024.5.2/openeo_fastapi/client/__init__.py
+-rw-r--r--   0        0        0     7848 2024-05-30 08:56:01.399262 openeo_fastapi-2024.5.2/openeo_fastapi/client/auth.py
+-rw-r--r--   0        0        0     6469 2024-05-30 08:56:01.399262 openeo_fastapi-2024.5.2/openeo_fastapi/client/collections.py
+-rw-r--r--   0        0        0     6260 2024-05-30 08:56:01.399262 openeo_fastapi-2024.5.2/openeo_fastapi/client/core.py
+-rw-r--r--   0        0        0     3408 2024-05-30 08:56:01.399262 openeo_fastapi-2024.5.2/openeo_fastapi/client/files.py
+-rw-r--r--   0        0        0    13680 2024-05-30 08:56:01.399262 openeo_fastapi-2024.5.2/openeo_fastapi/client/jobs.py
+-rw-r--r--   0        0        0    11239 2024-05-30 08:56:01.399262 openeo_fastapi-2024.5.2/openeo_fastapi/client/processes.py
+-rw-r--r--   0        0        0        0 2024-05-30 08:56:01.399262 openeo_fastapi-2024.5.2/openeo_fastapi/client/psql/__init__.py
+-rw-r--r--   0        0        0     5077 2024-05-30 08:56:01.399262 openeo_fastapi-2024.5.2/openeo_fastapi/client/psql/engine.py
+-rw-r--r--   0        0        0     2493 2024-05-30 08:56:01.399262 openeo_fastapi-2024.5.2/openeo_fastapi/client/psql/models.py
+-rw-r--r--   0        0        0      828 2024-05-30 08:56:01.399262 openeo_fastapi-2024.5.2/openeo_fastapi/client/psql/settings.py
+-rw-r--r--   0        0        0      737 2024-05-30 08:56:01.399262 openeo_fastapi-2024.5.2/openeo_fastapi/client/register.py
+-rw-r--r--   0        0        0     2257 2024-05-30 08:56:01.399262 openeo_fastapi-2024.5.2/openeo_fastapi/client/settings.py
+-rw-r--r--   0        0        0     1426 2024-05-30 08:56:01.399262 openeo_fastapi-2024.5.2/openeo_fastapi/templates.py
+-rw-r--r--   0        0        0     1388 2024-05-30 08:56:01.399262 openeo_fastapi-2024.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 openeo_fastapi-2024.5.2/PKG-INFO
```

### Comparing `openeo_fastapi-2024.5.1/LICENSE` & `openeo_fastapi-2024.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.5.1/README.md` & `openeo_fastapi-2024.5.2/README.md`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.5.1/openeo_fastapi/api/app.py` & `openeo_fastapi-2024.5.2/openeo_fastapi/api/app.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.5.1/openeo_fastapi/api/models.py` & `openeo_fastapi-2024.5.2/openeo_fastapi/api/models.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.5.1/openeo_fastapi/api/types.py` & `openeo_fastapi-2024.5.2/openeo_fastapi/api/types.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.5.1/openeo_fastapi/cli.py` & `openeo_fastapi-2024.5.2/openeo_fastapi/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,74 @@
 """CLI to support quick initialisation of the project source directory."""
+from pathlib import Path
+
 import click
 import fsspec
-
 from alembic import command
 from alembic.config import Config
-from pathlib import Path
 
 from openeo_fastapi.templates import (
     get_app_template,
     get_models_template,
-    get_revision_template
+    get_revision_template,
 )
 
 
 @click.group()
 def cli():
     """Defining group for executor CLI."""
     pass
 
+
 @click.command()
-@click.option('--path', default=None, type=str)
+@click.option("--path", default=None, type=str)
 def new(path):
     """Initialize a source directory for an openeo_fastapi api project at the specified location."""
     fs = fsspec.filesystem(protocol="file")
-        
+
     if path:
         path = Path(path)
-        if not path.exists():
-            raise ValueError("Provided path does not exist.")
     else:
         path = Path(fs.get_mapper("").root)
-    
+
     openeo_dir = path
     db_dir = openeo_dir / "psql"
     init_file = openeo_dir / "__init__.py"
     app_file = openeo_dir / "app.py"
     revise_file = openeo_dir / "revise.py"
 
-
     alembic_dir = db_dir / "alembic"
     alembic_models = db_dir / "models.py"
     alembic_ini = db_dir / "alembic.ini"
 
     fs.mkdir(openeo_dir)
 
     fs.mkdir(db_dir)
-    
+
     fs.mkdir(alembic_dir)
 
     fs.touch(alembic_models)
-    with fs.open(alembic_models, 'w') as f:
+    with fs.open(alembic_models, "w") as f:
         f.write(get_models_template())
-    
+
     alembic_cfg = Config(alembic_ini)
-    
-    command.init(
-        alembic_cfg,
-        directory=alembic_dir
-    )
-    
+
+    command.init(alembic_cfg, directory=alembic_dir)
+
     fs.touch(init_file)
-    
+
     fs.touch(app_file)
-    with fs.open(app_file, 'w') as f:
+    with fs.open(app_file, "w") as f:
         f.write(get_app_template())
 
     revise_file = openeo_dir / "revise.py"
     fs.touch(revise_file)
-    with fs.open(revise_file, 'w') as f:
+    with fs.open(revise_file, "w") as f:
         f.write(get_revision_template())
 
     pass
 
+
 cli.add_command(new)
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     cli()
```

### Comparing `openeo_fastapi-2024.5.1/openeo_fastapi/client/auth.py` & `openeo_fastapi-2024.5.2/openeo_fastapi/client/auth.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.5.1/openeo_fastapi/client/collections.py` & `openeo_fastapi-2024.5.2/openeo_fastapi/client/collections.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.5.1/openeo_fastapi/client/core.py` & `openeo_fastapi-2024.5.2/openeo_fastapi/client/core.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.5.1/openeo_fastapi/client/files.py` & `openeo_fastapi-2024.5.2/openeo_fastapi/client/files.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.5.1/openeo_fastapi/client/jobs.py` & `openeo_fastapi-2024.5.2/openeo_fastapi/client/jobs.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.5.1/openeo_fastapi/client/processes.py` & `openeo_fastapi-2024.5.2/openeo_fastapi/client/processes.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.5.1/openeo_fastapi/client/psql/engine.py` & `openeo_fastapi-2024.5.2/openeo_fastapi/client/psql/engine.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.5.1/openeo_fastapi/client/psql/models.py` & `openeo_fastapi-2024.5.2/openeo_fastapi/client/psql/models.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.5.1/openeo_fastapi/client/psql/settings.py` & `openeo_fastapi-2024.5.2/openeo_fastapi/client/psql/settings.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.5.1/openeo_fastapi/client/register.py` & `openeo_fastapi-2024.5.2/openeo_fastapi/client/register.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.5.1/openeo_fastapi/client/settings.py` & `openeo_fastapi-2024.5.2/openeo_fastapi/client/settings.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.5.1/openeo_fastapi/templates.py` & `openeo_fastapi-2024.5.2/openeo_fastapi/templates.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.5.1/pyproject.toml` & `openeo_fastapi-2024.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openeo-fastapi"
-version = "2024.5.1"
+version = "2024.5.2"
 description = "FastApi implementation conforming to the OpenEO Api specification."
 authors = ["Sean Hoyal <sean.hoyal@external.eodc.eu>"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
```

### Comparing `openeo_fastapi-2024.5.1/PKG-INFO` & `openeo_fastapi-2024.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openeo-fastapi
-Version: 2024.5.1
+Version: 2024.5.2
 Summary: FastApi implementation conforming to the OpenEO Api specification.
 Author: Sean Hoyal
 Author-email: sean.hoyal@external.eodc.eu
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

