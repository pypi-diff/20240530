# Comparing `tmp/bl_python_web-0.2.3.tar.gz` & `tmp/bl_python_web-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bl_python_web-0.2.3.tar", last modified: Fri May 17 19:19:28 2024, max compression
+gzip compressed data, was "bl_python_web-0.2.4.tar", last modified: Thu May 30 16:56:59 2024, max compression
```

## Comparing `bl_python_web-0.2.3.tar` & `bl_python_web-0.2.4.tar`

### file list

```diff
@@ -1,192 +1,194 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.824339 bl_python_web-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.792339 bl_python_web-0.2.3/BL_Python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.800340 bl_python_web-0.2.3/BL_Python/web/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.800340 bl_python_web-0.2.3/BL_Python/web/encryption/
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/encryption/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.800340 bl_python_web-0.2.3/BL_Python/web/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/middleware/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/middleware/dependency_injection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.800340 bl_python_web-0.2.3/BL_Python/web/middleware/flask/
--rw-r--r--   0 runner    (1001) docker     (127)     8425 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/middleware/flask/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.800340 bl_python_web-0.2.3/BL_Python/web/middleware/openapi/
--rw-r--r--   0 runner    (1001) docker     (127)    18898 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/middleware/openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/middleware/openapi/cors.py
--rw-r--r--   0 runner    (1001) docker     (127)    16920 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/middleware/sso.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.804340 bl_python_web-0.2.3/BL_Python/web/scaffolding/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24782 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/scaffolder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.792339 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.804340 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/base/
--rw-r--r--   0 runner    (1001) docker     (127)    18110 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/base/LICENSE.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/base/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.804340 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/base/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/base/docs/CONFIGURATION.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/base/pyproject.toml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.804340 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/__main__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/_app_type.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/_version.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.804340 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/endpoints/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/endpoints/application.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.792339 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/basic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.804340 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/basic/{{application.module_name}}/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/basic/{{application.module_name}}/config.toml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.792339 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/openapi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.804340 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/__main__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/_app_type.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/config.toml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.804340 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/endpoints/application.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/openapi.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.796339 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/optional/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.796339 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.804340 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/endpoints/{{operation.module_name}}.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.796339 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.804340 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/__hook__.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.804340 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/templates/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.804340 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/__hook__.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/__meta__.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.808339 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/templates/conftest.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/templates/test.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/templates/test_{{meta.operation.module_name}}.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.808339 bl_python_web-0.2.3/BL_Python/web/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/testing/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    28165 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/BL_Python/web/testing/create_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.824339 bl_python_web-0.2.3/BL_Python.web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-17 19:19:28.000000 bl_python_web-0.2.3/BL_Python.web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-05-17 19:19:28.000000 bl_python_web-0.2.3/BL_Python.web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 19:19:28.000000 bl_python_web-0.2.3/BL_Python.web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-17 19:19:28.000000 bl_python_web-0.2.3/BL_Python.web.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-17 19:19:28.000000 bl_python_web-0.2.3/BL_Python.web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-17 19:19:28.000000 bl_python_web-0.2.3/BL_Python.web.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-17 19:19:28.824339 bl_python_web-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 19:19:28.824339 bl_python_web-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.796339 bl_python_web-0.2.3/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.808339 bl_python_web-0.2.3/test/unit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.808339 bl_python_web-0.2.3/test/unit/application/
--rw-r--r--   0 runner    (1001) docker     (127)    14313 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/test/unit/application/test_create_flask_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/test/unit/application/test_create_openapi_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.808339 bl_python_web-0.2.3/test/unit/encryption/
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/test/unit/encryption/test_encryption.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.808339 bl_python_web-0.2.3/test/unit/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/test/unit/middleware/test_api_request_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/test/unit/middleware/test_api_response_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/test/unit/middleware/test_dependency_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/test/unit/middleware/test_error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/test/unit/middleware/test_flask_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    10642 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/test/unit/middleware/test_openapi_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/test/unit/middleware/test_sso.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.808339 bl_python_web-0.2.3/test/unit/scaffolding/
--rw-r--r--   0 runner    (1001) docker     (127)    17778 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/test/unit/scaffolding/test_scaffolding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/test/unit/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.796339 bl_python_web-0.2.3/typings/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.812339 bl_python_web-0.2.3/typings/connexion/
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/__main__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.812339 bl_python_web-0.2.3/typings/connexion/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/apps/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/apps/abstract.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/apps/asynchronous.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/apps/flask.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/context.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/datastructures.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.816339 bl_python_web-0.2.3/typings/connexion/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/decorators/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/decorators/main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/decorators/parameter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/decorators/response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/exceptions.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.816339 bl_python_web-0.2.3/typings/connexion/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/frameworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/frameworks/abstract.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/frameworks/flask.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/frameworks/starlette.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/handlers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/http_facts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/json_schema.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/jsonifier.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/lifecycle.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.816339 bl_python_web-0.2.3/typings/connexion/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/middleware/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/middleware/abstract.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/middleware/context.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/middleware/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/middleware/lifespan.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10777 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/middleware/main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/middleware/request_validation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/middleware/response_validation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/middleware/routing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/middleware/security.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/middleware/server_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/middleware/swagger_ui.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/mock.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.820340 bl_python_web-0.2.3/typings/connexion/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/operations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/operations/abstract.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/operations/openapi.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/operations/swagger2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/options.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/problem.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/resolver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/security.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/spec.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/testing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/types.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/uri_parsing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.820340 bl_python_web-0.2.3/typings/connexion/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/validators/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/validators/abstract.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/validators/form_data.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/validators/json.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/connexion/validators/parameter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.820340 bl_python_web-0.2.3/typings/flask_injector/
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/flask_injector/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/flask_injector/tests.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.820340 bl_python_web-0.2.3/typings/flask_login/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/flask_login/__about__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/flask_login/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/flask_login/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/flask_login/login_manager.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/flask_login/mixins.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/flask_login/signals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/flask_login/test_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/flask_login/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.820340 bl_python_web-0.2.3/typings/json_logging/
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/json_logging/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.820340 bl_python_web-0.2.3/typings/json_logging/framework/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/json_logging/framework/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.824339 bl_python_web-0.2.3/typings/json_logging/framework/connexion/
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/json_logging/framework/connexion/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.824339 bl_python_web-0.2.3/typings/json_logging/framework/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/json_logging/framework/fastapi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/json_logging/framework/fastapi/implementation.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.824339 bl_python_web-0.2.3/typings/json_logging/framework/flask/
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/json_logging/framework/flask/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.824339 bl_python_web-0.2.3/typings/json_logging/framework/quart/
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/json_logging/framework/quart/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:19:28.824339 bl_python_web-0.2.3/typings/json_logging/framework/sanic/
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/json_logging/framework/sanic/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/json_logging/framework_base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-17 19:19:24.000000 bl_python_web-0.2.3/typings/json_logging/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.090794 bl_python_web-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.058794 bl_python_web-0.2.4/BL_Python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.066794 bl_python_web-0.2.4/BL_Python/web/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.070794 bl_python_web-0.2.4/BL_Python/web/encryption/
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/encryption/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.070794 bl_python_web-0.2.4/BL_Python/web/host/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/host/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.070794 bl_python_web-0.2.4/BL_Python/web/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/middleware/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/middleware/dependency_injection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.070794 bl_python_web-0.2.4/BL_Python/web/middleware/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)     8425 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/middleware/flask/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.070794 bl_python_web-0.2.4/BL_Python/web/middleware/openapi/
+-rw-r--r--   0 runner    (1001) docker     (127)    22099 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/middleware/openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/middleware/openapi/cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16920 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/middleware/sso.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.070794 bl_python_web-0.2.4/BL_Python/web/scaffolding/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24782 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/scaffolder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.062794 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.070794 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/base/
+-rw-r--r--   0 runner    (1001) docker     (127)    18110 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/base/LICENSE.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/base/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.070794 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/base/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/base/docs/CONFIGURATION.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/base/pyproject.toml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.070794 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/__main__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/_app_type.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/_version.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.070794 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/endpoints/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/endpoints/application.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.062794 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/basic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.070794 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/basic/{{application.module_name}}/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/basic/{{application.module_name}}/config.toml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.062794 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/openapi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.074794 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/__main__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/_app_type.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/config.toml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.074794 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/endpoints/application.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/openapi.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.062794 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/optional/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.062794 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.074794 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/endpoints/{{operation.module_name}}.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.062794 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.074794 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/__hook__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.074794 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/templates/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.074794 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/__hook__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/__meta__.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.074794 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/templates/conftest.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/templates/test.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/templates/test_{{meta.operation.module_name}}.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.074794 bl_python_web-0.2.4/BL_Python/web/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/testing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28165 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/BL_Python/web/testing/create_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.090794 bl_python_web-0.2.4/BL_Python.web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-30 16:56:59.000000 bl_python_web-0.2.4/BL_Python.web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-05-30 16:56:59.000000 bl_python_web-0.2.4/BL_Python.web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:56:59.000000 bl_python_web-0.2.4/BL_Python.web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-30 16:56:59.000000 bl_python_web-0.2.4/BL_Python.web.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-30 16:56:59.000000 bl_python_web-0.2.4/BL_Python.web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 16:56:59.000000 bl_python_web-0.2.4/BL_Python.web.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-30 16:56:59.090794 bl_python_web-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 16:56:59.090794 bl_python_web-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.062794 bl_python_web-0.2.4/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.074794 bl_python_web-0.2.4/test/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.074794 bl_python_web-0.2.4/test/unit/application/
+-rw-r--r--   0 runner    (1001) docker     (127)    14313 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/test/unit/application/test_create_flask_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/test/unit/application/test_create_openapi_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.074794 bl_python_web-0.2.4/test/unit/encryption/
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/test/unit/encryption/test_encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.078794 bl_python_web-0.2.4/test/unit/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/test/unit/middleware/test_api_request_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/test/unit/middleware/test_api_response_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/test/unit/middleware/test_dependency_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/test/unit/middleware/test_error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/test/unit/middleware/test_flask_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10642 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/test/unit/middleware/test_openapi_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/test/unit/middleware/test_sso.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.078794 bl_python_web-0.2.4/test/unit/scaffolding/
+-rw-r--r--   0 runner    (1001) docker     (127)    17778 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/test/unit/scaffolding/test_scaffolding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/test/unit/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.066794 bl_python_web-0.2.4/typings/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.078794 bl_python_web-0.2.4/typings/connexion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/__main__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.082794 bl_python_web-0.2.4/typings/connexion/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/apps/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/apps/abstract.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/apps/asynchronous.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/apps/flask.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/context.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/datastructures.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.082794 bl_python_web-0.2.4/typings/connexion/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/decorators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/decorators/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/decorators/parameter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/decorators/response.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/exceptions.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.082794 bl_python_web-0.2.4/typings/connexion/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/frameworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/frameworks/abstract.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/frameworks/flask.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/frameworks/starlette.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/handlers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/http_facts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/json_schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/jsonifier.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/lifecycle.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.086794 bl_python_web-0.2.4/typings/connexion/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/middleware/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/middleware/abstract.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/middleware/context.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/middleware/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/middleware/lifespan.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10777 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/middleware/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/middleware/request_validation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/middleware/response_validation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/middleware/routing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/middleware/security.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/middleware/server_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/middleware/swagger_ui.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/mock.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.086794 bl_python_web-0.2.4/typings/connexion/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/operations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/operations/abstract.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/operations/openapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/operations/swagger2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/options.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/problem.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/resolver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/security.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/spec.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/testing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/types.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/uri_parsing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.086794 bl_python_web-0.2.4/typings/connexion/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/validators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/validators/abstract.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/validators/form_data.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/validators/json.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/connexion/validators/parameter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.086794 bl_python_web-0.2.4/typings/flask_injector/
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/flask_injector/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/flask_injector/tests.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.086794 bl_python_web-0.2.4/typings/flask_login/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/flask_login/__about__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/flask_login/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/flask_login/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/flask_login/login_manager.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/flask_login/mixins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/flask_login/signals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/flask_login/test_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/flask_login/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.086794 bl_python_web-0.2.4/typings/json_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/json_logging/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.086794 bl_python_web-0.2.4/typings/json_logging/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/json_logging/framework/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.086794 bl_python_web-0.2.4/typings/json_logging/framework/connexion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/json_logging/framework/connexion/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.086794 bl_python_web-0.2.4/typings/json_logging/framework/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/json_logging/framework/fastapi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/json_logging/framework/fastapi/implementation.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.086794 bl_python_web-0.2.4/typings/json_logging/framework/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/json_logging/framework/flask/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.090794 bl_python_web-0.2.4/typings/json_logging/framework/quart/
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/json_logging/framework/quart/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:56:59.090794 bl_python_web-0.2.4/typings/json_logging/framework/sanic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/json_logging/framework/sanic/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/json_logging/framework_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-30 16:56:54.000000 bl_python_web-0.2.4/typings/json_logging/util.pyi
```

### Comparing `bl_python_web-0.2.3/BL_Python/web/application.py` & `bl_python_web-0.2.4/BL_Python/web/application.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python/web/config.py` & `bl_python_web-0.2.4/BL_Python/web/config.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python/web/encryption/__init__.py` & `bl_python_web-0.2.4/BL_Python/web/encryption/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python/web/middleware/__init__.py` & `bl_python_web-0.2.4/BL_Python/web/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python/web/middleware/consts.py` & `bl_python_web-0.2.4/BL_Python/web/middleware/consts.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python/web/middleware/dependency_injection.py` & `bl_python_web-0.2.4/BL_Python/web/middleware/dependency_injection.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python/web/middleware/flask/__init__.py` & `bl_python_web-0.2.4/BL_Python/web/middleware/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python/web/middleware/openapi/__init__.py` & `bl_python_web-0.2.4/BL_Python/web/middleware/openapi/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 import re
 import uuid
+from collections.abc import Iterable
 from contextlib import ExitStack
 from contextvars import Token
 from logging import Logger
 from typing import Any, Awaitable, Callable, Literal, TypeVar, cast
 from uuid import uuid4
 
 import json_logging
+import starlette
+import starlette.datastructures
+import starlette.requests
 from BL_Python.programming.collections.dict import AnyDict, merge
 from connexion import ConnexionMiddleware, FlaskApp, context, utils
 from connexion.middleware import MiddlewarePosition
 from flask import Flask, Request, Response, request
 from flask.ctx import AppContext
 from flask.globals import _cv_app  # pyright: ignore[reportPrivateUsage]
 from flask.globals import current_app
 from flask.typing import (
     AfterRequestCallable,
     BeforeRequestCallable,
     ResponseReturnValue,
 )
+from flask_login import AnonymousUserMixin, current_user
 from injector import inject
+from starlette.datastructures import Address
 from starlette.types import ASGIApp, Receive, Scope, Send
 from typing_extensions import TypedDict, final
+from werkzeug.local import LocalProxy
 
 from ...config import Config
 from ..consts import (
     CONTENT_SECURITY_POLICY_HEADER,
     CORRELATION_ID_HEADER,
     INCOMING_REQUEST_MESSAGE,
     OUTGOING_RESPONSE_MESSAGE,
@@ -196,25 +203,27 @@
     ):
         request_headers_safe[REQUEST_COOKIE_HEADER] = re.sub(
             rf"({config.flask.session.cookie.name}=)[^;]+(;|$)",
             r"\1<redacted>\2",
             request_headers_safe[REQUEST_COOKIE_HEADER],
         )
 
-    server = request.get("server")
-    client = request.get("client")
+    server = get_server_address()
+    client = get_remote_address()
     log.info(
         INCOMING_REQUEST_MESSAGE,
         request["method"],
         request["path"],
         # ASGI spec states `server` and `client`
         # can be `None` if not available.
-        f"{server[0]}:{server[1]}" if server else "None",
-        f"{client[0]}:{client[1]}" if client else "None",
-        request.get("remote_user"),  # FIXME fix this when auth is done
+        f"{server.host}:{server.port}",
+        f"{client.host}:{client.port}",
+        "Anonymous"
+        if isinstance(current_user, AnonymousUserMixin)
+        else current_user.get_id(),
         extra={
             "props": {
                 "correlation_id": correlation_id,
                 "headers": request_headers_safe,
             }
         },
     )
@@ -427,14 +436,90 @@
                     f"Badly formatted {CORRELATION_ID_HEADER} received in request."
                 )
                 raise e
 
         await self._app(scope, receive, wrapped_send)
 
 
+_DEFAULT_HOSTNAME = "localhost"
+_DEFAULT_PORT = 80
+
+
+def get_server_address() -> Address:
+    request_proxy = cast(LocalProxy[starlette.requests.Request], context.request)
+    starlette_request = cast(
+        starlette.requests.Request, request_proxy._starlette_request
+    )
+    scope = starlette_request.scope
+    server_hostname = starlette_request.base_url.hostname
+    server_port = starlette_request.base_url.port
+    if not server_hostname or not server_port:
+        # there is the possibility this value in scope is "127.0.0.1" when using "localhost"
+        # which is not consistent with the _starlette_request value.
+        server = cast(tuple[str, int] | None, scope.get("server"))
+        if server:
+            if not server_hostname:
+                server_hostname = server[0]
+            if not server_port:
+                server_port = server[1]
+        else:
+            app_server_name = cast(dict[str, str | None], current_app.config).get(
+                "SERVER_NAME"
+            )
+            if app_server_name:
+                if not server_hostname:
+                    server_hostname = app_server_name[: app_server_name.index(":")]
+                if not server_port:
+                    server_port = app_server_name[app_server_name.index(":") + 1 :]
+    if isinstance(server_port, str):
+        try:
+            server_port = int(server_port)
+        except:
+            # this is the same default port that
+            # Starlette uses in starlette.middleware.wsgi.build_environ
+            server_port = _DEFAULT_PORT
+
+    return Address(
+        host=server_hostname or _DEFAULT_HOSTNAME, port=server_port or _DEFAULT_PORT
+    )
+
+
+def get_remote_address() -> Address:
+    request_proxy = cast(LocalProxy[starlette.requests.Request], context.request)
+    starlette_request = cast(
+        starlette.requests.Request, request_proxy._starlette_request
+    )
+    scope = starlette_request.scope
+    request_client = starlette_request.client
+
+    remote_hostname = ""
+    remote_port = 0
+
+    if request_client:
+        remote_hostname = request_client.host
+        remote_port = request_client.port
+
+    if not remote_hostname or not remote_port:
+        # it's actually a 2-item list whose first item
+        # is a string, and second item is an int ...
+        client = cast(tuple[str, int] | None, scope.get("client"))
+        if client and isinstance(client, Iterable):  # pyright: ignore[reportUnnecessaryIsInstance]
+            if not remote_hostname:
+                remote_hostname = client[0]
+
+            if not remote_port:
+                remote_port = client[1]
+
+    return Address(host=remote_hostname, port=remote_port)
+
+
+def address_to_str(address: Address):
+    return f"{address.host}:{address.port}"
+
+
 @final
 class FlaskContextMiddleware:
     """
     Connexion does not set Flask contexts in all cases they may be needed, like
     in middlewares that execute before ContextMiddleware. This middleware creates
     the Flask application, request, and session contexts if they are not currently set.
     """
@@ -464,48 +549,63 @@
             with ExitStack() as exit_stack:
                 if not isinstance(current_app, Flask):  # pyright: ignore[reportUnnecessaryIsInstance] it is not a Flask if it is not set
                     app_ctx = exit_stack.enter_context(app.app_context())
 
                     app_ctx_token = _cv_app.set(app_ctx)
 
                 if not isinstance(request, Request):  # pyright: ignore[reportUnnecessaryIsInstance] it is not a Request if it is not set
+                    request_proxy = cast(
+                        LocalProxy[starlette.requests.Request], context.request
+                    )
+                    starlette_request = cast(
+                        starlette.requests.Request, request_proxy._starlette_request
+                    )
+                    request_headers = cast(
+                        starlette.datastructures.Headers, request_proxy.headers
+                    )
+                    path_info = (
+                        "PATH_INFO",
+                        str(scope.get("path") or starlette_request.url.path),
+                    )
+                    wsgi_url_scheme = (
+                        "wsgi.url_scheme",
+                        str(scope.get("scheme") or starlette_request.url.scheme),
+                    )
+                    request_method = (
+                        "REQUEST_METHOD",
+                        str(scope.get("method") or starlette_request.method),
+                    )
+                    (server_hostname, server_port) = get_server_address()
+                    server_name = ("SERVER_NAME", server_hostname)
+                    server_port = ("SERVER_PORT", server_port)
+                    query_string = (
+                        "QUERY_STRING",
+                        scope.get("query_string") or starlette_request.url.query,
+                    )
+                    remote_addr = ("REMOTE_ADDR", address_to_str(get_remote_address()))
+                    headers = dict({
+                        (
+                            f"{'HTTP_' if header.upper() not in ['CONTENT_TYPE', 'CONTENT_LENGTH'] else ''}{header.upper().replace('-', '_')}",
+                            value,
+                        )
+                        for header, value in request_headers.items()
+                    })
+
                     request_environ = merge(
-                        {
-                            "PATH_INFO": scope.get("path")
-                            or context.request._starlette_request.url.path,
-                            "wsgi.url_scheme": scope.get("scheme")
-                            or context.request._starlette_request.url.scheme,
-                            "REQUEST_METHOD": scope.get("method")
-                            or context.request._starlette_request.method,
-                            # there is the possibility this value in scope is "127.0.0.1" when using "localhost"
-                            # which is not consistent with the _starlette_request value.
-                            "SERVER_NAME": (
-                                scope["server"][0]
-                                if scope.get("server")
-                                else context.request._starlette_request.base_url.hostname
-                            ),
-                            "SERVER_PORT": (
-                                scope["server"][1]
-                                if scope.get("server")
-                                else context.request._starlette_request.base_url.port
-                            ),
-                            "QUERY_STRING": scope.get("query_string")
-                            or context.request._starlette_request.url.query,
-                            "REMOTE_ADDR": ":".join([
-                                str(value) for value in scope["client"]
-                            ])
-                            or f"{context.request._starlette_request.client.host}:{context.request._starlette_request.client.port}",
-                        },
-                        dict({
-                            (
-                                f"{'HTTP_' if header.upper() not in ['CONTENT_TYPE', 'CONTENT_LENGTH'] else ''}{header.upper().replace('-', '_')}",
-                                value,
-                            )
-                            for header, value in context.request.headers.items()
-                        }),
+                        dict([
+                            path_info,
+                            wsgi_url_scheme,
+                            request_method,
+                            server_name,
+                            server_port,
+                            query_string,
+                            remote_addr,
+                        ]),
+                        headers,
+                        True,
                     )
 
                     # Some values, like the query string, are stored as bytes.
                     # Decode as a UTF-8 str so encoding later doesn't fail.
                     for key, value in request_environ.items():
                         if isinstance(value, bytes):
                             request_environ[key] = value.decode("utf-8")
```

### Comparing `bl_python_web-0.2.3/BL_Python/web/middleware/openapi/cors.py` & `bl_python_web-0.2.4/BL_Python/web/middleware/openapi/cors.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python/web/middleware/sso.py` & `bl_python_web-0.2.4/BL_Python/web/middleware/sso.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python/web/scaffolding/__main__.py` & `bl_python_web-0.2.4/BL_Python/web/scaffolding/__main__.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python/web/scaffolding/scaffolder.py` & `bl_python_web-0.2.4/BL_Python/web/scaffolding/scaffolder.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/base/LICENSE.md.j2` & `bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/base/LICENSE.md.j2`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/base/README.md.j2` & `bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/base/README.md.j2`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/base/docs/CONFIGURATION.md.j2` & `bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/base/docs/CONFIGURATION.md.j2`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/base/pyproject.toml.j2` & `bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/base/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/__init__.py.j2` & `bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/endpoints/application.py.j2` & `bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/endpoints/application.py.j2`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/basic/{{application.module_name}}/config.toml.j2` & `bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/basic/{{application.module_name}}/config.toml.j2`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/config.toml.j2` & `bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/config.toml.j2`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/openapi.yaml.j2` & `bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/openapi.yaml.j2`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/endpoints/{{operation.module_name}}.py.j2` & `bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/endpoints/{{operation.module_name}}.py.j2`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/__hook__.py` & `bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/__hook__.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/templates/test_{{meta.operation.module_name}}.py.j2` & `bl_python_web-0.2.4/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/templates/test_{{meta.operation.module_name}}.py.j2`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python/web/testing/config.py` & `bl_python_web-0.2.4/BL_Python/web/testing/config.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python/web/testing/create_app.py` & `bl_python_web-0.2.4/BL_Python/web/testing/create_app.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/BL_Python.web.egg-info/PKG-INFO` & `bl_python_web-0.2.4/BL_Python.web.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BL_Python.web
-Version: 0.2.3
+Version: 0.2.4
 Summary: Libraries for building web applications in Boutros Lab.
 Author-email: Aaron Holmes <aholmes@mednet.ucla.edu>
 Project-URL: Homepage, https://github.com/uclahs-cds/BL_Python
 Project-URL: Bug Tracker, https://github.com/uclahs-cds/BL_Python/issues
 Project-URL: Repository, https://github.com/uclahs-cds/BL_Python.git
 Project-URL: Changelog, https://github.com/uclahs-cds/BL_Python/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
@@ -25,14 +25,15 @@
 Requires-Dist: BL_Python.identity
 Requires-Dist: BL_Python.database
 Requires-Dist: Flask==3.0.2
 Requires-Dist: flask-injector
 Requires-Dist: flask-login
 Requires-Dist: connexion==3.0.6
 Requires-Dist: connexion[uvicorn]
+Requires-Dist: uvicorn-worker
 Requires-Dist: swagger_ui_bundle
 Requires-Dist: python-dotenv
 Requires-Dist: json-logging
 Requires-Dist: lib_programname
 Requires-Dist: toml
 Requires-Dist: pydantic
 Requires-Dist: a2wsgi
```

### Comparing `bl_python_web-0.2.3/BL_Python.web.egg-info/SOURCES.txt` & `bl_python_web-0.2.4/BL_Python.web.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 BL_Python.web.egg-info/entry_points.txt
 BL_Python.web.egg-info/requires.txt
 BL_Python.web.egg-info/top_level.txt
 BL_Python/web/__init__.py
 BL_Python/web/application.py
 BL_Python/web/config.py
 BL_Python/web/encryption/__init__.py
+BL_Python/web/host/__init__.py
 BL_Python/web/middleware/__init__.py
 BL_Python/web/middleware/consts.py
 BL_Python/web/middleware/dependency_injection.py
 BL_Python/web/middleware/sso.py
 BL_Python/web/middleware/flask/__init__.py
 BL_Python/web/middleware/openapi/__init__.py
 BL_Python/web/middleware/openapi/cors.py
```

### Comparing `bl_python_web-0.2.3/LICENSE.md` & `bl_python_web-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/PKG-INFO` & `bl_python_web-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BL_Python.web
-Version: 0.2.3
+Version: 0.2.4
 Summary: Libraries for building web applications in Boutros Lab.
 Author-email: Aaron Holmes <aholmes@mednet.ucla.edu>
 Project-URL: Homepage, https://github.com/uclahs-cds/BL_Python
 Project-URL: Bug Tracker, https://github.com/uclahs-cds/BL_Python/issues
 Project-URL: Repository, https://github.com/uclahs-cds/BL_Python.git
 Project-URL: Changelog, https://github.com/uclahs-cds/BL_Python/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
@@ -25,14 +25,15 @@
 Requires-Dist: BL_Python.identity
 Requires-Dist: BL_Python.database
 Requires-Dist: Flask==3.0.2
 Requires-Dist: flask-injector
 Requires-Dist: flask-login
 Requires-Dist: connexion==3.0.6
 Requires-Dist: connexion[uvicorn]
+Requires-Dist: uvicorn-worker
 Requires-Dist: swagger_ui_bundle
 Requires-Dist: python-dotenv
 Requires-Dist: json-logging
 Requires-Dist: lib_programname
 Requires-Dist: toml
 Requires-Dist: pydantic
 Requires-Dist: a2wsgi
```

### Comparing `bl_python_web-0.2.3/README.md` & `bl_python_web-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/pyproject.toml` & `bl_python_web-0.2.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     "BL_Python.database",
 
     "Flask == 3.0.2",
     "flask-injector",
     "flask-login",
     "connexion == 3.0.6",
     "connexion[uvicorn]",
+    "uvicorn-worker",
     "swagger_ui_bundle",
     "python-dotenv",
     "json-logging",
     "lib_programname",
     "toml",
     "pydantic",
     "a2wsgi"
```

### Comparing `bl_python_web-0.2.3/test/unit/application/test_create_flask_app.py` & `bl_python_web-0.2.4/test/unit/application/test_create_flask_app.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/test/unit/application/test_create_openapi_app.py` & `bl_python_web-0.2.4/test/unit/application/test_create_openapi_app.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/test/unit/encryption/test_encryption.py` & `bl_python_web-0.2.4/test/unit/encryption/test_encryption.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/test/unit/middleware/test_api_request_handlers.py` & `bl_python_web-0.2.4/test/unit/middleware/test_api_request_handlers.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/test/unit/middleware/test_api_response_handlers.py` & `bl_python_web-0.2.4/test/unit/middleware/test_api_response_handlers.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/test/unit/middleware/test_dependency_injection.py` & `bl_python_web-0.2.4/test/unit/middleware/test_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/test/unit/middleware/test_error_handlers.py` & `bl_python_web-0.2.4/test/unit/middleware/test_error_handlers.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/test/unit/middleware/test_flask_middleware.py` & `bl_python_web-0.2.4/test/unit/middleware/test_flask_middleware.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/test/unit/middleware/test_openapi_middleware.py` & `bl_python_web-0.2.4/test/unit/middleware/test_openapi_middleware.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/test/unit/scaffolding/test_scaffolding.py` & `bl_python_web-0.2.4/test/unit/scaffolding/test_scaffolding.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/test/unit/test_config.py` & `bl_python_web-0.2.4/test/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/__init__.pyi` & `bl_python_web-0.2.4/typings/connexion/__init__.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/apps/abstract.pyi` & `bl_python_web-0.2.4/typings/connexion/apps/abstract.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/apps/asynchronous.pyi` & `bl_python_web-0.2.4/typings/connexion/apps/asynchronous.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/apps/flask.pyi` & `bl_python_web-0.2.4/typings/connexion/apps/flask.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/cli.pyi` & `bl_python_web-0.2.4/typings/connexion/cli.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/datastructures.pyi` & `bl_python_web-0.2.4/typings/connexion/datastructures.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/decorators/main.pyi` & `bl_python_web-0.2.4/typings/connexion/decorators/main.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/decorators/parameter.pyi` & `bl_python_web-0.2.4/typings/connexion/decorators/parameter.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/decorators/response.pyi` & `bl_python_web-0.2.4/typings/connexion/decorators/response.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/exceptions.pyi` & `bl_python_web-0.2.4/typings/connexion/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/frameworks/abstract.pyi` & `bl_python_web-0.2.4/typings/connexion/frameworks/abstract.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/frameworks/flask.pyi` & `bl_python_web-0.2.4/typings/connexion/frameworks/flask.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/frameworks/starlette.pyi` & `bl_python_web-0.2.4/typings/connexion/frameworks/starlette.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/handlers.pyi` & `bl_python_web-0.2.4/typings/connexion/handlers.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/json_schema.pyi` & `bl_python_web-0.2.4/typings/connexion/json_schema.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/jsonifier.pyi` & `bl_python_web-0.2.4/typings/connexion/jsonifier.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/lifecycle.pyi` & `bl_python_web-0.2.4/typings/connexion/lifecycle.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/middleware/abstract.pyi` & `bl_python_web-0.2.4/typings/connexion/middleware/abstract.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/middleware/context.pyi` & `bl_python_web-0.2.4/typings/connexion/middleware/context.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/middleware/exceptions.pyi` & `bl_python_web-0.2.4/typings/connexion/middleware/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/middleware/lifespan.pyi` & `bl_python_web-0.2.4/typings/connexion/middleware/lifespan.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/middleware/main.pyi` & `bl_python_web-0.2.4/typings/connexion/middleware/main.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/middleware/request_validation.pyi` & `bl_python_web-0.2.4/typings/connexion/middleware/request_validation.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/middleware/response_validation.pyi` & `bl_python_web-0.2.4/typings/connexion/middleware/response_validation.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/middleware/routing.pyi` & `bl_python_web-0.2.4/typings/connexion/middleware/routing.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/middleware/security.pyi` & `bl_python_web-0.2.4/typings/connexion/middleware/security.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/middleware/server_error.pyi` & `bl_python_web-0.2.4/typings/connexion/middleware/server_error.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/middleware/swagger_ui.pyi` & `bl_python_web-0.2.4/typings/connexion/middleware/swagger_ui.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/mock.pyi` & `bl_python_web-0.2.4/typings/connexion/mock.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/operations/__init__.pyi` & `bl_python_web-0.2.4/typings/connexion/operations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/operations/abstract.pyi` & `bl_python_web-0.2.4/typings/connexion/operations/abstract.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/operations/openapi.pyi` & `bl_python_web-0.2.4/typings/connexion/operations/openapi.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/operations/swagger2.pyi` & `bl_python_web-0.2.4/typings/connexion/operations/swagger2.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/options.pyi` & `bl_python_web-0.2.4/typings/connexion/options.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/problem.pyi` & `bl_python_web-0.2.4/typings/connexion/problem.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/resolver.pyi` & `bl_python_web-0.2.4/typings/connexion/resolver.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/security.pyi` & `bl_python_web-0.2.4/typings/connexion/security.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/spec.pyi` & `bl_python_web-0.2.4/typings/connexion/spec.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/testing.pyi` & `bl_python_web-0.2.4/typings/connexion/testing.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/types.pyi` & `bl_python_web-0.2.4/typings/connexion/types.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/uri_parsing.pyi` & `bl_python_web-0.2.4/typings/connexion/uri_parsing.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/utils.pyi` & `bl_python_web-0.2.4/typings/connexion/utils.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/validators/__init__.pyi` & `bl_python_web-0.2.4/typings/connexion/validators/__init__.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/validators/abstract.pyi` & `bl_python_web-0.2.4/typings/connexion/validators/abstract.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/validators/form_data.pyi` & `bl_python_web-0.2.4/typings/connexion/validators/form_data.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/validators/json.pyi` & `bl_python_web-0.2.4/typings/connexion/validators/json.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/connexion/validators/parameter.pyi` & `bl_python_web-0.2.4/typings/connexion/validators/parameter.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/flask_injector/__init__.pyi` & `bl_python_web-0.2.4/typings/flask_injector/__init__.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/flask_injector/tests.pyi` & `bl_python_web-0.2.4/typings/flask_injector/tests.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/flask_login/__init__.pyi` & `bl_python_web-0.2.4/typings/flask_login/__init__.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/flask_login/login_manager.pyi` & `bl_python_web-0.2.4/typings/flask_login/login_manager.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/flask_login/mixins.pyi` & `bl_python_web-0.2.4/typings/flask_login/mixins.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/flask_login/utils.pyi` & `bl_python_web-0.2.4/typings/flask_login/utils.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/json_logging/__init__.pyi` & `bl_python_web-0.2.4/typings/json_logging/__init__.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/json_logging/framework/connexion/__init__.pyi` & `bl_python_web-0.2.4/typings/json_logging/framework/connexion/__init__.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/json_logging/framework/fastapi/implementation.pyi` & `bl_python_web-0.2.4/typings/json_logging/framework/fastapi/implementation.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/json_logging/framework/flask/__init__.pyi` & `bl_python_web-0.2.4/typings/json_logging/framework/flask/__init__.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/json_logging/framework/quart/__init__.pyi` & `bl_python_web-0.2.4/typings/json_logging/framework/quart/__init__.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/json_logging/framework/sanic/__init__.pyi` & `bl_python_web-0.2.4/typings/json_logging/framework/sanic/__init__.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/json_logging/framework_base.pyi` & `bl_python_web-0.2.4/typings/json_logging/framework_base.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.3/typings/json_logging/util.pyi` & `bl_python_web-0.2.4/typings/json_logging/util.pyi`

 * *Files identical despite different names*

