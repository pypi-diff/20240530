# Comparing `tmp/sqlalchemy-helpers-0.9.0.tar.gz` & `tmp/sqlalchemy_helpers-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-helpers-0.9.0.tar", max compression
+gzip compressed data, was "sqlalchemy_helpers-1.0.0.tar", max compression
```

## Comparing `sqlalchemy-helpers-0.9.0.tar` & `sqlalchemy_helpers-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0     7652 2017-09-30 07:16:26.000000 sqlalchemy-helpers-0.9.0/LICENSE
--rw-r--r--   0        0        0     3554 2021-12-17 13:11:40.744889 sqlalchemy-helpers-0.9.0/README.md
--rw-r--r--   0        0        0      176 2021-12-17 12:30:08.517115 sqlalchemy-helpers-0.9.0/docs/_source/sqlalchemy_helpers.flask_ext.rst
--rw-r--r--   0        0        0      168 2021-12-17 12:30:08.519115 sqlalchemy-helpers-0.9.0/docs/_source/sqlalchemy_helpers.manager.rst
--rw-r--r--   0        0        0      262 2021-12-17 12:30:08.514115 sqlalchemy-helpers-0.9.0/docs/_source/sqlalchemy_helpers.rst
--rw-r--r--   0        0        0     3795 2021-12-17 12:59:27.224601 sqlalchemy-helpers-0.9.0/docs/conf.py
--rw-r--r--   0        0        0     6549 2021-12-14 16:10:51.103905 sqlalchemy-helpers-0.9.0/docs/contributing.rst
--rw-r--r--   0        0        0      428 2021-12-17 12:59:27.224601 sqlalchemy-helpers-0.9.0/docs/index.rst
--rw-r--r--   0        0        0       78 2021-12-06 22:17:52.731702 sqlalchemy-helpers-0.9.0/docs/release_notes.rst
--rw-r--r--   0        0        0       61 2021-12-06 22:17:52.731702 sqlalchemy-helpers-0.9.0/docs/user.rst
--rw-r--r--   0        0        0     4069 2021-12-17 13:07:47.247161 sqlalchemy-helpers-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      712 2021-12-17 10:59:40.713185 sqlalchemy-helpers-0.9.0/sqlalchemy_helpers/__init__.py
--rw-r--r--   0        0        0     5199 2021-12-17 11:27:59.719485 sqlalchemy-helpers-0.9.0/sqlalchemy_helpers/flask_ext.py
--rw-r--r--   0        0        0     6542 2021-12-17 11:27:51.856460 sqlalchemy-helpers-0.9.0/sqlalchemy_helpers/manager.py
--rw-r--r--   0        0        0        0 2021-12-06 22:17:22.082613 sqlalchemy-helpers-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0     1334 2021-12-17 08:44:57.990975 sqlalchemy-helpers-0.9.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2021-12-17 07:10:20.616267 sqlalchemy-helpers-0.9.0/tests/integration/__init__.py
--rw-r--r--   0        0        0        0 2021-12-17 08:10:52.236594 sqlalchemy-helpers-0.9.0/tests/integration/app_fixture/__init__.py
--rw-r--r--   0        0        0      639 2021-12-17 08:55:45.743995 sqlalchemy-helpers-0.9.0/tests/integration/app_fixture/app.py
--rw-r--r--   0        0        0       34 2021-12-17 11:27:36.594413 sqlalchemy-helpers-0.9.0/tests/integration/app_fixture/models/__init__.py
--rw-r--r--   0        0        0      225 2021-12-17 11:27:21.915367 sqlalchemy-helpers-0.9.0/tests/integration/app_fixture/models/user.py
--rw-r--r--   0        0        0     1472 2021-12-17 08:21:12.662529 sqlalchemy-helpers-0.9.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     1548 2021-12-17 11:29:27.162757 sqlalchemy-helpers-0.9.0/tests/integration/test_integration.py
--rw-r--r--   0        0        0        0 2021-12-17 07:10:41.279331 sqlalchemy-helpers-0.9.0/tests/unit/__init__.py
--rw-r--r--   0        0        0      311 2021-12-17 07:11:40.034000 sqlalchemy-helpers-0.9.0/tests/unit/models.py
--rw-r--r--   0        0        0     3602 2021-12-17 08:54:57.382844 sqlalchemy-helpers-0.9.0/tests/unit/test_flask_ext.py
--rw-r--r--   0        0        0     2465 2021-12-17 07:13:02.229771 sqlalchemy-helpers-0.9.0/tests/unit/test_manager.py
--rw-r--r--   0        0        0      984 2021-12-17 09:40:08.033299 sqlalchemy-helpers-0.9.0/tox.ini
--rw-r--r--   0        0        0     4536 2021-12-17 13:15:10.576756 sqlalchemy-helpers-0.9.0/setup.py
--rw-r--r--   0        0        0     4838 2021-12-17 13:15:10.577104 sqlalchemy-helpers-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2322 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/README.md
+-rw-r--r--   0        0        0     2410 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/docs/aio-env.py.example
+-rw-r--r--   0        0        0     6739 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/docs/async.rst
+-rw-r--r--   0        0        0     3793 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/docs/conf.py
+-rw-r--r--   0        0        0     6549 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/docs/contributing.rst
+-rw-r--r--   0        0        0      439 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/docs/index.rst
+-rw-r--r--   0        0        0     3715 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/docs/release_notes.md
+-rw-r--r--   0        0        0     9614 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/docs/user.rst
+-rw-r--r--   0        0        0     3863 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      770 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/sqlalchemy_helpers/__init__.py
+-rw-r--r--   0        0        0     8199 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/sqlalchemy_helpers/aio.py
+-rw-r--r--   0        0        0     2131 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/sqlalchemy_helpers/fastapi.py
+-rw-r--r--   0        0        0     5895 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/sqlalchemy_helpers/flask_ext.py
+-rw-r--r--   0        0        0    10831 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/sqlalchemy_helpers/manager.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     2094 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/tests/integration/app_fixture/__init__.py
+-rw-r--r--   0        0        0      639 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/tests/integration/app_fixture/app.py
+-rw-r--r--   0        0        0       34 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/tests/integration/app_fixture/models/__init__.py
+-rw-r--r--   0        0        0      225 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/tests/integration/app_fixture/models/user.py
+-rw-r--r--   0        0        0     1796 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/tests/integration/conftest.py
+-rw-r--r--   0        0        0     1564 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/tests/integration/test_integration.py
+-rw-r--r--   0        0        0      539 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0      310 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/tests/unit/models.py
+-rw-r--r--   0        0        0     6768 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/tests/unit/test_aio.py
+-rw-r--r--   0        0        0     5089 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/tests/unit/test_fastapi.py
+-rw-r--r--   0        0        0     3600 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/tests/unit/test_flask_ext.py
+-rw-r--r--   0        0        0     4766 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/tests/unit/test_manager.py
+-rw-r--r--   0        0        0      923 2024-05-30 12:51:05.011534 sqlalchemy_helpers-1.0.0/tox.ini
+-rw-r--r--   0        0        0     3662 1970-01-01 00:00:00.000000 sqlalchemy_helpers-1.0.0/PKG-INFO
```

### Comparing `sqlalchemy-helpers-0.9.0/LICENSE` & `sqlalchemy_helpers-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-helpers-0.9.0/docs/conf.py` & `sqlalchemy_helpers-1.0.0/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,21 +93,23 @@
     ".rst": "restructuredtext",
     ".md": "markdown",
 }
 
 
 # -- Options for intersphinx extension ---------------------------------------
 
-# Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {"python": ("https://docs.python.org/3", None)}
+intersphinx_mapping = {
+    "python": ("https://docs.python.org/3", None),
+    "sqlalchemy": ("https://docs.sqlalchemy.org/en/20/", None),
+}
 
 extlinks = {
-    "commit": ("https://github.com/fedora-infra/sqlalchemy-helpers/commit/%s", ""),
-    "issue": ("https://github.com/fedora-infra/sqlalchemy-helpers/issues/%s", "#"),
-    "pr": ("https://github.com/fedora-infra/sqlalchemy-helpers/pull/%s", "PR#"),
+    "commit": ("https://github.com/fedora-infra/sqlalchemy-helpers/commit/%s", "%s"),
+    "issue": ("https://github.com/fedora-infra/sqlalchemy-helpers/issues/%s", "#%s"),
+    "pr": ("https://github.com/fedora-infra/sqlalchemy-helpers/pull/%s", "PR#%s"),
 }
 
 # -- Misc -----
 
 
 def run_apidoc(_):
     from sphinx.ext import apidoc
```

### Comparing `sqlalchemy-helpers-0.9.0/docs/contributing.rst` & `sqlalchemy_helpers-1.0.0/docs/contributing.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 Guidelines
 ==========
 
 Python Support
 --------------
-SQLAlchemy Helpers supports Python 3.6 or greater. This is automatically enforced by the
+SQLAlchemy Helpers supports Python 3.8 or greater. This is automatically enforced by the
 continuous integration (CI) suite.
 
 
 Code Style
 ----------
 We follow the `PEP8 <https://www.python.org/dev/peps/pep-0008/>`_ style guide
 for Python. This is automatically enforced by the CI suite.
```

### Comparing `sqlalchemy-helpers-0.9.0/pyproject.toml` & `sqlalchemy_helpers-1.0.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlalchemy-helpers"
-version = "0.9.0"
+version = "1.0.0"
 description = "SQLAlchemy Helpers"
 
 license = "LGPL-3.0-or-later"
 
 authors = [
   "Fedora Infrastructure <admin@fedoraproject.org>"
 ]
@@ -23,64 +23,85 @@
 ]
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Database",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6.2"
+python = "^3.8.0"
 SQLAlchemy = ">=1.3.0"
 alembic = ">=1.6.5"
-Flask = { version = "^2.0", optional = true }
-sphinx = {version = "^4", optional = true}
-myst-parser = {version = "^0.16.1", optional = true}
+Flask = { version = "^2.0.0 || ^3.0.0", optional = true }
+sphinx = {version = "*", optional = true}
+myst-parser = {version = "*", optional = true}
+sphinxcontrib-napoleon = {version = "*", optional = true}
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 pytest-cov = "*"
 pytest-mock = "*"
+pytest-asyncio = "*"
 bandit = "*"
 black = "*"
 flake8 = "*"
 isort = "*"
 coverage = {extras = ["toml"], version = "*"}
 liccheck = "*"
-sphinx = "^4"
+sphinx = "*"
 pre-commit = "*"
-myst-parser = "^0.16.1"
+myst-parser = "*"
+towncrier = "*"
+aiosqlite = "*"
+psycopg2 = "*"
+asyncpg = "*"
+pydantic = "*"
+pydantic-settings = "*"
 
 [tool.poetry.extras]
 flask = ["Flask"]
-docs = ["sphinx", "myst-parser"]
+docs = ["sphinx", "myst-parser", "Flask", "sphinxcontrib-napoleon"]
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
-[tool.isort]
-profile = "black"
-lines_after_imports = 2
-force_alphabetical_sort_within_sections = true
-
 [tool.black]
-target-version = ["py36"]
+target-version = ["py38"]
+
+[tool.ruff]
+select = ["E", "F", "W", "I", "UP", "S", "B", "RUF"]
+line-length = 100
+target-version = "py38"
+ignore = ["RUF010", "UP038"]
+
+[tool.ruff.per-file-ignores]
+"tests/*" = ["S101"]
+"tests/integration/*" = ["S603"]
+"news/get-authors.py" = ["S602", "S603", "S607"]
+"docs/conf.py" = ["I001"]
+"sqlalchemy_helpers/__init__.py" = ["F401"]
+
+[tool.ruff.isort]
+lines-after-imports = 2
+order-by-type = false
 
 [tool.pytest.ini_options]
+asyncio_mode = "auto"
 testpaths = [
     "tests",
 ]
 
 [tool.coverage.run]
 branch = true
 source = ["sqlalchemy_helpers"]
@@ -97,35 +118,30 @@
 omit = [
     "sqlalchemy_helpers/__init__.py",
     "sqlalchemy_helpers/migrations/env.py",
 ]
 
 
 [tool.towncrier]
-package = "sqlalchemy-helpers"
-filename = "docs/release_notes.rst"
+package = "sqlalchemy_helpers"
+filename = "docs/release_notes.md"
 directory = "news/"
-title_format = "v{version}"
 issue_format = "{issue}"
-template = "news/_template.rst"
-underlines = "=^-"
-wrap = true
+template = "news/_template.md"
+title_format = "## Version [{version}](https://github.com/fedora-infra/sqlalchemy-helpers/tree/v{version})"
+underlines = ["", "", ""]
+wrap = false
 all_bullets = true
 
   [[tool.towncrier.type]]
   directory = "bic"
   name = "Backwards Incompatible Changes"
   showcontent = true
 
   [[tool.towncrier.type]]
-  directory = "dependency"
-  name = "Dependency Changes"
-  showcontent = true
-
-  [[tool.towncrier.type]]
   directory = "feature"
   name = "Features"
   showcontent = true
 
   [[tool.towncrier.type]]
   directory = "bug"
   name = "Bug Fixes"
@@ -138,51 +154,20 @@
 
   [[tool.towncrier.type]]
   directory = "docs"
   name = "Documentation Improvements"
   showcontent = true
 
   [[tool.towncrier.type]]
+  directory = "dependency"
+  name = "Dependency Changes"
+  showcontent = true
+
+  [[tool.towncrier.type]]
   directory = "other"
   name = "Other Changes"
   showcontent = true
 
   [[tool.towncrier.type]]
   directory = "author"
   name = "Contributors"
   showcontent = true
-
-
-[tool.liccheck]
-authorized_licenses = [
-  "bsd",
-  "new bsd",
-  "simplified bsd",
-  "apache",
-  "apache 2.0",
-  "apache software",
-  "gnu lgpl",
-  "gpl v2",
-  "GNU General Public License v2 or later (GPLv2+)",
-  "GNU General Public License v3 (GPLv3)",
-  "GNU General Public License v3 or later (GPLv3+)",
-  "GNU Library or Lesser General Public License (LGPL)",
-  "GNU Lesser General Public License v2 or later (LGPLv2+)",
-  "GNU Lesser General Public License v3 or later (LGPLv3+)",
-  "GPLv3+",
-  "LGPLv2+",
-  "gpl v3",
-  "lgpl with exceptions or zpl",
-  "isc",
-  "isc license (iscl)",
-  "mit",
-  "python software foundation",
-  "zpl 2.1",
-  "mpl-2.0",
-  "MPL 2.0",
-  "Mozilla Public License 2.0 (MPL 2.0)",
-  "lgpl",
-  "CC0 (copyright waived)",
-  "Public Domain",
-  "Public Domain <http://unlicense.org>",
-  "Zope Public",
-]
```

### Comparing `sqlalchemy-helpers-0.9.0/sqlalchemy_helpers/__init__.py` & `sqlalchemy_helpers-1.0.0/sqlalchemy_helpers/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,20 +2,24 @@
 
 A set of tools to integrate SQLAlchemy and Alembic in your project, with sane defauts.
 
 Attributes:
     __version__ (str): this package's version.
 """
 
-from .manager import (  # noqa: F401
+from .manager import (
     Base,
     DatabaseManager,
+    DatabaseStatus,
     exists_in_db,
+    get_base,
     get_or_create,
     is_sqlite,
+    SyncResult,
+    update_or_create,
 )
 
 
 # Set the version
 try:
     import importlib.metadata
```

### Comparing `sqlalchemy-helpers-0.9.0/sqlalchemy_helpers/flask_ext.py` & `sqlalchemy_helpers-1.0.0/sqlalchemy_helpers/flask_ext.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 """
 Flask integration of database management.
 """
 
 import os
 
 import click
-from flask import _app_ctx_stack, abort, current_app, has_app_context
+from flask import abort, current_app, has_app_context
 from flask.cli import AppGroup
 from werkzeug.utils import find_modules, import_string
 
 from .manager import DatabaseManager, SyncResult
 
 
-def _get_manager():
+def _get_manager(engine_args=None, app=None):
     """Get the database manager using the Flask app's configuration."""
-    uri = current_app.config["SQLALCHEMY_DATABASE_URI"]
-    alembic_location = current_app.config["DB_ALEMBIC_LOCATION"]
-    manager = DatabaseManager(uri, alembic_location)
+    app = app or current_app
+    uri = app.config["SQLALCHEMY_DATABASE_URI"]
+    alembic_location = app.config["DB_ALEMBIC_LOCATION"]
+    base_model = app.extensions[DatabaseExtension._app_base_model_name]
+    manager = DatabaseManager(
+        uri, alembic_location, engine_args=engine_args, base_model=base_model
+    )
     return manager
 
 
 def _syncdb():
     """Run :meth:`DatabaseManager.sync` on the command-line."""
     manager = _get_manager()
     result = manager.sync()
@@ -38,41 +42,49 @@
 class DatabaseExtension:
     """A Flask extension to configure the database manager according the the app's configuration.
 
     It cleans up database connections at the end of the requests, and creates the CLI endpoint to
     sync the database schema.
     """
 
-    def __init__(self, app=None):
+    _app_manager_name = "_sqlah_database_manager"
+    _app_base_model_name = "_sqlah_base_model"
+
+    def __init__(self, app=None, base_model=None):
         self.app = app
+        self._base_model = base_model
         if app is not None:
-            self.init_app(app)
+            self.init_app(app, base_model=self._base_model)
 
-    def init_app(self, app):
+    def init_app(self, app, base_model=None):
         """Initialize the extention on the provided Flask app
 
         Args:
             app (flask.Flask): the Flask application.
         """
+        base_model = base_model or self._base_model
         # Set config defaults
         app.config.setdefault("SQLALCHEMY_DATABASE_URI", "sqlite:///:memory:")
         app.config.setdefault(
             "DB_ALEMBIC_LOCATION", os.path.join(app.root_path, "migrations")
         )
         main_module = app.import_name
         if main_module.endswith(".app"):
             main_module = main_module[:-4]
         app.config.setdefault("DB_MODELS_LOCATION", f"{main_module}.models")
         # Connect hook
         app.before_request(self.before_request)
         # Disconnect hook
         app.teardown_appcontext(self.teardown)
+        # Store the base_model
+        app.extensions[self._app_base_model_name] = base_model
+
         # CLI
         db_cli = AppGroup("db", help="Database operations.")
-        db_cli.command("syncdb", help="Create or migrate the database.")(_syncdb)
+        db_cli.command("sync", help="Create or migrate the database.")(_syncdb)
         app.cli.add_command(db_cli)
         # Import all modules here that might define models so that
         # they will be registered properly on the metadata.
         models_location = app.config["DB_MODELS_LOCATION"]
         try:
             for module in find_modules(
                 models_location, include_packages=True, recursive=True
@@ -80,53 +92,55 @@
                 import_string(module)
         except ValueError:
             # It's just a module, importing it is enough
             import_string(models_location)
 
     def teardown(self, exception):
         """Close the database connection at the end of each requests."""
-        ctx = _app_ctx_stack.top
-        if hasattr(ctx, "database_manager"):
-            ctx.database_manager.Session.remove()
+        if self._app_manager_name in current_app.extensions:
+            current_app.extensions[self._app_manager_name].Session.remove()
 
     def before_request(self):
         """Prepare the database manager at the start of each request.
 
-        This is necessary to allow access to the ``Model.query`` property.
+        This is necessary to allow access to the ``Model.get_*`` methods.
         """
         # Just create the manager
-        self.manager
+        self.manager  # noqa: B018
 
     @property
     def session(self):
         """sqlalchemy.session.Session: the database Session instance to use."""
         return self.manager.Session()
 
     @property
     def manager(self):
         """DatabaseManager: the instance of the database manager."""
-        ctx = _app_ctx_stack.top
-        if ctx is not None:
-            if not hasattr(ctx, "database_manager"):
-                ctx.database_manager = _get_manager()
-            return ctx.database_manager
+        try:
+            if self._app_manager_name not in current_app.extensions:
+                current_app.extensions[self._app_manager_name] = _get_manager()
+
+            return current_app.extensions[self._app_manager_name]
+        except RuntimeError:
+            # RuntimeError: Working outside of application context.
+            return None
 
 
 # View helpers
 
 
-def get_or_404(Model, ident, description=None):
+def get_or_404(Model, pk, description=None):
     """Like ``query.get`` but aborts with 404 if not found.
 
     Args:
         Model (manager.Base): a model class.
-        ident (int or str): the primary key of the desired record.
+        pk (int or str): the primary key of the desired record.
         description (str, optional): a message for the 404 error if not found.
     """
-    rv = Model.query.get(ident)
+    rv = Model.get_by_pk(pk)
     if rv is None:
         abort(404, description=description)
     return rv
 
 
 def first_or_404(query, description=None):
     """Like ``query.first`` but aborts with 404 if not found.
@@ -143,15 +157,15 @@
 
 # Useful in alembic's env.py
 
 
 def get_url_from_app(app_factory):
     """Get the DB URI from the app configuration
 
-    Create the application if it hasn't been created yet.
+    Create the application if it hasn't been created yet. This is useful in Alembic's ``env.py``.
 
     Args: app_factory (callable): the Flask application factory, to be called if this function is
         called outside of and application context.
     """
     if not has_app_context():
         app = app_factory()
         return app.config["SQLALCHEMY_DATABASE_URI"]
```

### Comparing `sqlalchemy-helpers-0.9.0/tests/integration/app_fixture/app.py` & `sqlalchemy_helpers-1.0.0/tests/integration/app_fixture/app.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-helpers-0.9.0/tests/integration/test_integration.py` & `sqlalchemy_helpers-1.0.0/tests/integration/test_integration.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,41 +2,41 @@
 import subprocess
 import sys
 from importlib import import_module
 
 import alembic
 
 
-def test_config(full_app, tmpdir):
+def test_config(full_app, clear_metadata, tmpdir):
     """Check that the app configuration is set."""
     app_module = import_module("testapp.app")
     config = app_module.app.config
     assert config["SQLALCHEMY_DATABASE_URI"] == f"sqlite:///{tmpdir}/database.sqlite"
     assert config["DB_ALEMBIC_LOCATION"] == os.path.join(
         tmpdir, "testapp", "migrations"
     )
     assert config["DB_MODELS_LOCATION"] == "testapp.models"
 
 
-def test_models(full_app, tmpdir):
+def test_models(full_app, clear_metadata, tmpdir):
     """Check that the models were properly imported."""
     import_module("testapp.app")
     manager_module = import_module("sqlalchemy_helpers.manager")
     assert "app_users" in manager_module.Base.metadata.tables
 
 
 def test_sync_db(full_app, tmpdir):
     """Check that the CLI extension works."""
 
     def syncdb():
         return subprocess.run(
-            [sys.executable, "-m", "flask", "db", "syncdb"],
+            [sys.executable, "-m", "flask", "db", "sync"],
             check=True,
             stdout=subprocess.PIPE,
-            universal_newlines=True,
+            text=True,
         )
 
     result = syncdb()
     assert os.path.exists(os.path.join(tmpdir, "database.sqlite"))
     assert "Database created." in result.stdout
     result = syncdb()
     assert "Database already up-to-date." in result.stdout
```

### Comparing `sqlalchemy-helpers-0.9.0/tests/unit/test_flask_ext.py` & `sqlalchemy_helpers-1.0.0/tests/unit/test_flask_ext.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 def test_flask_ext_first_or_404(flask_app, flask_client):
     db = DatabaseExtension(flask_app)
     db.manager.create()
     user = make_user(db, "dummy")
 
     @flask_app.route("/user/<name>")
     def view(name):
-        user = first_or_404(User.query.filter_by(name=name), "no such user")
+        user = first_or_404(db.session.query(User).filter_by(name=name), "no such user")
         return jsonify(user.id)
 
     response = flask_client.get("/user/dummy")
     assert response.json == user.id
 
     response = flask_client.get("/user/nobody")
     assert response.status_code == 404
@@ -73,30 +73,30 @@
 def test_flask_ext_script(flask_app, mocker):
     db = DatabaseExtension(flask_app)
     with flask_app.app_context():
         alembic.command.revision(db.manager.alembic_cfg, rev_id="dummy")
         assert not exists_in_db(db.session.get_bind(), "users")
         assert db.manager.get_current_revision(db.session) is None
     assert "db" in flask_app.cli.commands
-    assert "syncdb" in flask_app.cli.commands["db"].commands
-    syncdb_cmd = flask_app.cli.commands["db"].commands["syncdb"]
+    assert "sync" in flask_app.cli.commands["db"].commands
+    sync_cmd = flask_app.cli.commands["db"].commands["sync"]
     runner = flask_app.test_cli_runner()
-    result = runner.invoke(syncdb_cmd)
+    result = runner.invoke(sync_cmd)
     with flask_app.app_context():
         assert exists_in_db(db.session.get_bind(), "users")
         assert db.manager.get_current_revision(db.session) is not None
     assert "Database created." in result.output
-    result = runner.invoke(syncdb_cmd)
+    result = runner.invoke(sync_cmd)
     assert "Database already up-to-date." in result.output
     with flask_app.app_context():
         alembic.command.revision(db.manager.alembic_cfg, rev_id="second")
-    result = runner.invoke(syncdb_cmd)
+    result = runner.invoke(sync_cmd)
     assert "Database upgraded." in result.output
     mocker.patch("sqlalchemy_helpers.flask_ext._get_manager")
-    result = runner.invoke(syncdb_cmd)
+    result = runner.invoke(sync_cmd)
     assert "Unexpected sync result:" in result.output
 
 
 def test_flask_ext_outside_context(flask_app):
     db = DatabaseExtension(flask_app)
     assert db.manager is None
```

### Comparing `sqlalchemy-helpers-0.9.0/tests/unit/test_manager.py` & `sqlalchemy_helpers-1.0.0/tests/unit/test_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,37 @@
+from unittest import mock
+
 import alembic
 import pytest
 
 from sqlalchemy_helpers.manager import (
     DatabaseManager,
+    DatabaseStatus,
     exists_in_db,
     get_or_create,
     is_sqlite,
     SyncResult,
+    update_or_create,
 )
 
 from .models import User
 
 
 @pytest.fixture
 def manager(app):
     return DatabaseManager(app["db_uri"], app["alembic_dir"])
 
 
+def test_manager_engine_args(app, monkeypatch):
+    create_engine = mock.Mock()
+    monkeypatch.setattr("sqlalchemy_helpers.manager.create_engine", create_engine)
+    DatabaseManager(app["db_uri"], app["alembic_dir"], engine_args={"foo": "bar"})
+    create_engine.assert_called_once_with(url=app["db_uri"], foo="bar")
+
+
 def test_manager_no_revision(manager):
     assert manager.get_latest_revision() is None
 
 
 def test_manager_get_latest_revision(manager):
     alembic.command.revision(manager.alembic_cfg, rev_id="dummy")
     assert manager.get_latest_revision() == "dummy"
@@ -29,14 +40,24 @@
 def test_manager_create(manager):
     alembic.command.revision(manager.alembic_cfg, rev_id="dummy")
     manager.create()
     with manager.Session() as session:
         assert manager.get_current_revision(session) == "dummy"
 
 
+def test_manager_get_status(manager):
+    assert manager.get_status() == DatabaseStatus.NO_INFO
+    alembic.command.revision(manager.alembic_cfg, rev_id="first")
+    manager.create()
+    alembic.command.revision(manager.alembic_cfg, rev_id="second")
+    assert manager.get_status() == DatabaseStatus.UPGRADE_AVAILABLE
+    alembic.command.stamp(manager.alembic_cfg, "second")
+    assert manager.get_status() == DatabaseStatus.UP_TO_DATE
+
+
 def test_manager_sync(manager):
     alembic.command.revision(manager.alembic_cfg, rev_id="first")
     assert manager.sync() == SyncResult.CREATED
     alembic.command.revision(manager.alembic_cfg, rev_id="second")
     assert manager.sync() == SyncResult.UPGRADED
     assert manager.sync() == SyncResult.ALREADY_UP_TO_DATE
 
@@ -71,14 +92,60 @@
     assert created is True
     assert user.name == "dummy"
     user2, created = User.get_or_create(name="dummy")
     assert created is False
     assert user.id == user2.id
 
 
+def test_update_or_create(manager, session):
+    manager.create()
+    user, created = update_or_create(
+        session, User, name="dummy", defaults={"full_name": "Dummy"}
+    )
+    assert created is True
+    assert isinstance(user, User)
+    assert user.name == "dummy"
+    assert user.full_name == "Dummy"
+    # Now update it
+    user2, created = update_or_create(
+        session, User, name="dummy", defaults={"full_name": "New Value"}
+    )
+    assert created is False
+    assert isinstance(user2, User)
+    assert user.id == user2.id
+    assert user.full_name == "New Value"
+    # Test create_defaults
+    user3, created = update_or_create(
+        session,
+        User,
+        name="dummy2",
+        defaults={"full_name": "Wrong Value"},
+        create_defaults={"full_name": "Correct Value"},
+    )
+    assert created is True
+    assert user3.name == "dummy2"
+    assert user3.full_name == "Correct Value"
+
+
+def test_update_or_create_property(app, monkeypatch):
+    update_or_create = mock.Mock()
+    monkeypatch.setattr("sqlalchemy_helpers.manager.update_or_create", update_or_create)
+    manager = DatabaseManager(app["db_uri"], app["alembic_dir"])
+    manager.create()
+    kwargs = dict(
+        name="dummy",
+        defaults={"full_name": "Dummy"},
+        create_defaults={"full_name": "Initial Dummy"},
+    )
+    User.update_or_create(**kwargs)
+    update_or_create.assert_called_once_with(
+        session=manager.Session(), model=User, **kwargs
+    )
+
+
 # Migration helpers
 
 
 def test_exists_in_db(manager):
     manager.create()
     bind = manager.Session.get_bind()
     assert exists_in_db(bind, "users")
```

