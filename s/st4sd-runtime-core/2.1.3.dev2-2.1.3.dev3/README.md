# Comparing `tmp/st4sd-runtime-core-2.1.3.dev2.tar.gz` & `tmp/st4sd-runtime-core-2.1.3.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st4sd-runtime-core-2.1.3.dev2.tar", last modified: Wed Mar 27 15:31:35 2024, max compression
+gzip compressed data, was "st4sd-runtime-core-2.1.3.dev3.tar", last modified: Wed Apr  3 15:13:30 2024, max compression
```

## Comparing `st4sd-runtime-core-2.1.3.dev2.tar` & `st4sd-runtime-core-2.1.3.dev3.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 15:31:35.217311 st4sd-runtime-core-2.1.3.dev2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 15:31:35.189312 st4sd-runtime-core-2.1.3.dev2/.github/
--rw-rw-r--   0 root         (0) root         (0)      127 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/.github/dco.yml
--rw-rw-r--   0 root         (0) root         (0)     1799 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/.gitignore
--rw-rw-r--   0 root         (0) root         (0)     8177 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/.travis.yml
--rw-rw-r--   0 root         (0) root         (0)       77 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/.whitesource
--rw-rw-r--   0 root         (0) root         (0)     1017 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/CITATION.cff
--rw-rw-r--   0 root         (0) root         (0)     3347 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/CODE_OF_CONDUCT.md
--rw-rw-r--   0 root         (0) root         (0)     2643 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/CONTRIBUTING.md
--rw-rw-r--   0 root         (0) root         (0)     2442 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/Dockerfile
--rw-rw-r--   0 root         (0) root         (0)    10774 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/LICENSE.md
--rw-rw-r--   0 root         (0) root         (0)      439 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/MAINTAINERS.md
--rw-r--r--   0 root         (0) root         (0)     5273 2024-03-27 15:31:35.217311 st4sd-runtime-core-2.1.3.dev2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3735 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/README.MD
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 15:31:35.189312 st4sd-runtime-core-2.1.3.dev2/deploy/
--rw-rw-r--   0 root         (0) root         (0)      180 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/deploy/creation_payload.json
--rwxrwxr-x   0 root         (0) root         (0)      292 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/deploy/skopeo_copy.sh
--rw-rw-r--   0 root         (0) root         (0)      635 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/deploy/st4sd-runtime-core-image.deploy
--rw-rw-r--   0 root         (0) root         (0)     1426 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/deploy/st4sd-runtime-core-multiarch.deploy
--rw-rw-r--   0 root         (0) root         (0)      291 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/deploy/st4sd-runtime-core-release-tag.deploy
--rwxrwxr-x   0 root         (0) root         (0)     2445 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/deploy/triggerExternalBuild.sh
--rw-rw-r--   0 root         (0) root         (0)     2445 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/py37.Dockerfile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 15:31:35.185311 st4sd-runtime-core-2.1.3.dev2/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 15:31:35.193312 st4sd-runtime-core-2.1.3.dev2/python/experiment/
--rw-rw-r--   0 root         (0) root         (0)       80 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    38736 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/appenv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 15:31:35.193312 st4sd-runtime-core-2.1.3.dev2/python/experiment/cli/
--rw-rw-r--   0 root         (0) root         (0)      112 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/cli/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2842 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/cli/api.py
--rw-rw-r--   0 root         (0) root         (0)     2560 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/cli/configuration.py
--rw-rw-r--   0 root         (0) root         (0)     6943 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/cli/context.py
--rw-rw-r--   0 root         (0) root         (0)      267 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/cli/exit_codes.py
--rw-rw-r--   0 root         (0) root         (0)     2705 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/cli/git.py
--rw-rw-r--   0 root         (0) root         (0)     8283 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/cli/login.py
--rw-rw-r--   0 root         (0) root         (0)    22932 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/cli/package.py
--rw-rw-r--   0 root         (0) root         (0)     7051 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/cli/pull_secrets.py
--rw-rw-r--   0 root         (0) root         (0)    31124 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/cli/pvep_schema.jsonschema
--rw-rw-r--   0 root         (0) root         (0)      390 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/cli/stack.py
--rw-rw-r--   0 root         (0) root         (0)     2392 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/cli/stp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 15:31:35.193312 st4sd-runtime-core-2.1.3.dev2/python/experiment/model/
--rw-rw-r--   0 root         (0) root         (0)       80 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/model/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3003 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/model/codes.py
--rw-rw-r--   0 root         (0) root         (0)    91119 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/model/conf.py
--rw-rw-r--   0 root         (0) root         (0)   148053 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/model/data.py
--rw-rw-r--   0 root         (0) root         (0)    46347 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/model/errors.py
--rw-rw-r--   0 root         (0) root         (0)    59750 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/model/executors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 15:31:35.197311 st4sd-runtime-core-2.1.3.dev2/python/experiment/model/frontends/
--rw-rw-r--   0 root         (0) root         (0)       80 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/model/frontends/__init__.py
--rw-rw-r--   0 root         (0) root         (0)   126138 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/model/frontends/cwl.py
--rw-rw-r--   0 root         (0) root         (0)    85741 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/model/frontends/dosini.py
--rw-rw-r--   0 root         (0) root         (0)   104839 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/model/frontends/dsl.py
--rw-rw-r--   0 root         (0) root         (0)   262695 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/model/frontends/flowir.py
--rw-rw-r--   0 root         (0) root         (0)   150222 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/model/graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 15:31:35.197311 st4sd-runtime-core-2.1.3.dev2/python/experiment/model/hooks/
--rw-rw-r--   0 root         (0) root         (0)      683 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/model/hooks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4236 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/model/hooks/hooks.py
--rw-rw-r--   0 root         (0) root         (0)    36110 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/model/hooks/interface.py
--rw-rw-r--   0 root         (0) root         (0)     2394 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/model/hooks/utils.py
--rw-rw-r--   0 root         (0) root         (0)     5552 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/model/interface.py
--rw-rw-r--   0 root         (0) root         (0)    67436 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/model/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 15:31:35.197311 st4sd-runtime-core-2.1.3.dev2/python/experiment/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 15:31:35.197311 st4sd-runtime-core-2.1.3.dev2/python/experiment/resources/Template.package/
--rw-rw-r--   0 root         (0) root         (0)      544 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/resources/Template.package/README.MD
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 15:31:35.197311 st4sd-runtime-core-2.1.3.dev2/python/experiment/resources/Template.package/conf/
--rw-rw-r--   0 root         (0) root         (0)      376 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/resources/Template.package/conf/flowir_package.yaml
--rw-rw-r--   0 root         (0) root         (0)     6144 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/resources/Template.package.tar
--rw-rw-r--   0 root         (0) root         (0)      630 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/rewrite-rules.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 15:31:35.201311 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/
--rw-rw-r--   0 root         (0) root         (0)       80 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 15:31:35.201311 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/backend_interfaces/
--rw-rw-r--   0 root         (0) root         (0)       80 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/backend_interfaces/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8178 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/backend_interfaces/docker.py
--rw-rw-r--   0 root         (0) root         (0)   115031 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/backend_interfaces/k8s.py
--rw-rw-r--   0 root         (0) root         (0)     5302 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/backend_interfaces/localtask.py
--rw-rw-r--   0 root         (0) root         (0)   116500 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/backend_interfaces/lsf.py
--rwxrwxr-x   0 root         (0) root         (0)     1414 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/backend_interfaces/stage-out.sh
--rw-rw-r--   0 root         (0) root         (0)    13277 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/backend_interfaces/task_simulator.py
--rw-rw-r--   0 root         (0) root         (0)    37745 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/backends.py
--rw-rw-r--   0 root         (0) root         (0)    34800 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/backends_base.py
--rw-rw-r--   0 root         (0) root         (0)   118126 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/control.py
--rw-rw-r--   0 root         (0) root         (0)   104583 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/engine.py
--rw-rw-r--   0 root         (0) root         (0)     5429 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 15:31:35.201311 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/interpreters/
--rw-rw-r--   0 root         (0) root         (0)       80 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/interpreters/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    26290 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/interpreters/cwl.py
--rw-rw-r--   0 root         (0) root         (0)     9481 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/interpreters/cwl_cmdline.py
--rw-rw-r--   0 root         (0) root         (0)     8089 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/interpreters/js.py
--rw-rw-r--   0 root         (0) root         (0)    20080 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/monitor.py
--rw-rw-r--   0 root         (0) root         (0)    68147 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/optimizer.py
--rw-rw-r--   0 root         (0) root         (0)    34954 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/output.py
--rw-rw-r--   0 root         (0) root         (0)    45119 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/span.py
--rw-rw-r--   0 root         (0) root         (0)    35543 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/status.py
--rw-rw-r--   0 root         (0) root         (0)     5622 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 15:31:35.205311 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/utilities/
--rw-rw-r--   0 root         (0) root         (0)       80 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/utilities/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3878 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/utilities/container_image_cache.py
--rw-rw-r--   0 root         (0) root         (0)     4089 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/utilities/rx.py
--rw-rw-r--   0 root         (0) root         (0)     5384 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/utilities/s3.py
--rw-rw-r--   0 root         (0) root         (0)    36584 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 15:31:35.205311 st4sd-runtime-core-2.1.3.dev2/python/experiment/service/
--rw-rw-r--   0 root         (0) root         (0)       80 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/service/__init__.py
--rw-rw-r--   0 root         (0) root         (0)   260764 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/service/db.py
--rw-rw-r--   0 root         (0) root         (0)     8206 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/service/errors.py
--rw-rw-r--   0 root         (0) root         (0)     7213 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/settings.py
--rw-rw-r--   0 root         (0) root         (0)     6441 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 15:31:35.205311 st4sd-runtime-core-2.1.3.dev2/python/experiment/utilities/
--rw-rw-r--   0 root         (0) root         (0)      104 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/utilities/README
--rw-rw-r--   0 root         (0) root         (0)      317 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/utilities/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    58393 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/utilities/data.py
--rw-rw-r--   0 root         (0) root         (0)     4705 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/python/experiment/utilities/fsearch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 15:31:35.217311 st4sd-runtime-core-2.1.3.dev2/python/st4sd_runtime_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5273 2024-03-27 15:31:35.000000 st4sd-runtime-core-2.1.3.dev2/python/st4sd_runtime_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4707 2024-03-27 15:31:35.000000 st4sd-runtime-core-2.1.3.dev2/python/st4sd_runtime_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 15:31:35.000000 st4sd-runtime-core-2.1.3.dev2/python/st4sd_runtime_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      291 2024-03-27 15:31:35.000000 st4sd-runtime-core-2.1.3.dev2/python/st4sd_runtime_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-03-27 15:31:35.000000 st4sd-runtime-core-2.1.3.dev2/python/st4sd_runtime_core.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 15:31:35.205311 st4sd-runtime-core-2.1.3.dev2/requirement_files/
--rw-rw-r--   0 root         (0) root         (0)      133 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/requirement_files/requirements_base_3.7.txt
--rw-rw-r--   0 root         (0) root         (0)      423 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/requirement_files/requirements_base_3.txt
--rw-rw-r--   0 root         (0) root         (0)       18 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/requirement_files/requirements_deploy.txt
--rw-rw-r--   0 root         (0) root         (0)       94 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/requirement_files/requirements_lsf.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 15:31:35.209312 st4sd-runtime-core-2.1.3.dev2/scripts/
--rwxrwxr-x   0 root         (0) root         (0)     7054 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/scripts/ccommand.py
--rwxrwxr-x   0 root         (0) root         (0)    11995 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/scripts/cexecute.py
--rwxrwxr-x   0 root         (0) root         (0)     1239 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/scripts/checkpackage.py
--rwxrwxr-x   0 root         (0) root         (0)     4286 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/scripts/ctest.py
--rwxrwxr-x   0 root         (0) root         (0)     2567 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/scripts/ecreate.py
--rwxrwxr-x   0 root         (0) root         (0)     4196 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/scripts/eflowir.py
--rwxrwxr-x   0 root         (0) root         (0)     8094 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/scripts/einputs.py
--rwxrwxr-x   0 root         (0) root         (0)     8246 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/scripts/einspect.py
--rwxrwxr-x   0 root         (0) root         (0)   109140 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/scripts/elaunch.py
--rwxrwxr-x   0 root         (0) root         (0)    17228 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/scripts/ememo.py
--rwxrwxr-x   0 root         (0) root         (0)    46782 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/scripts/epatch-apply.py
--rwxrwxr-x   0 root         (0) root         (0)    33324 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/scripts/epatch.py
--rwxrwxr-x   0 root         (0) root         (0)    17371 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/scripts/etest.py
--rwxrwxr-x   0 root         (0) root         (0)    10430 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/scripts/ewrap.py
--rwxrwxr-x   0 root         (0) root         (0)      821 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/scripts/expstatus.sh
--rw-rw-r--   0 root         (0) root         (0)     3840 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/scripts/k8srun.py
--rwxrwxr-x   0 root         (0) root         (0)   109140 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/scripts/launchexperiment.py
--rwxrwxr-x   0 root         (0) root         (0)    14013 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/scripts/lsfsub.py
--rwxrwxr-x   0 root         (0) root         (0)      262 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/scripts/stp
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-27 15:31:35.217311 st4sd-runtime-core-2.1.3.dev2/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     4892 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 15:31:35.213312 st4sd-runtime-core-2.1.3.dev2/tests/
--rw-rw-r--   0 root         (0) root         (0)       80 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10844 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/conftest.py
--rw-rw-r--   0 root         (0) root         (0)    11290 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/dont_test_cwl.py
--rw-rw-r--   0 root         (0) root         (0)     4541 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/reactive_testutils.py
--rw-rw-r--   0 root         (0) root         (0)    14765 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/saltcurve_paragon.py
--rw-rw-r--   0 root         (0) root         (0)    11225 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/test_array_variables.py
--rw-rw-r--   0 root         (0) root         (0)    10570 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/test_command.py
--rw-rw-r--   0 root         (0) root         (0)     9710 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/test_component.py
--rw-rw-r--   0 root         (0) root         (0)     2432 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/test_container_image_uri_manipulation.py
--rw-rw-r--   0 root         (0) root         (0)    44829 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/test_control.py
--rw-rw-r--   0 root         (0) root         (0)     4840 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/test_data.py
--rw-rw-r--   0 root         (0) root         (0)     5588 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/test_db.py
--rw-rw-r--   0 root         (0) root         (0)    40808 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/test_dosini.py
--rw-rw-r--   0 root         (0) root         (0)    35269 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/test_dowhile.py
--rw-rw-r--   0 root         (0) root         (0)    44807 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/test_dsl.py
--rw-rw-r--   0 root         (0) root         (0)    30930 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/test_engines.py
--rw-rw-r--   0 root         (0) root         (0)    57895 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/test_flowir.py
--rw-rw-r--   0 root         (0) root         (0)    23888 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/test_graph.py
--rw-rw-r--   0 root         (0) root         (0)     3286 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/test_identifier.py
--rw-rw-r--   0 root         (0) root         (0)    22923 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/test_interface.py
--rw-rw-r--   0 root         (0) root         (0)     6059 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/test_k8s.py
--rw-rw-r--   0 root         (0) root         (0)     2467 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/test_memoization.py
--rw-rw-r--   0 root         (0) root         (0)    18732 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/test_package_load.py
--rw-rw-r--   0 root         (0) root         (0)     1673 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/test_service.py
--rw-rw-r--   0 root         (0) root         (0)     2085 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/test_settings.py
--rw-rw-r--   0 root         (0) root         (0)     5825 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tests/utils.py
--rw-rw-r--   0 root         (0) root         (0)     3119 2024-03-27 15:27:35.000000 st4sd-runtime-core-2.1.3.dev2/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:13:30.381803 st4sd-runtime-core-2.1.3.dev3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:13:30.345803 st4sd-runtime-core-2.1.3.dev3/.github/
+-rw-rw-r--   0 root         (0) root         (0)      127 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/.github/dco.yml
+-rw-rw-r--   0 root         (0) root         (0)     1799 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/.gitignore
+-rw-rw-r--   0 root         (0) root         (0)     8177 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/.travis.yml
+-rw-rw-r--   0 root         (0) root         (0)       77 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/.whitesource
+-rw-rw-r--   0 root         (0) root         (0)     1017 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/CITATION.cff
+-rw-rw-r--   0 root         (0) root         (0)     3347 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 root         (0) root         (0)     2643 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/CONTRIBUTING.md
+-rw-rw-r--   0 root         (0) root         (0)     2442 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/Dockerfile
+-rw-rw-r--   0 root         (0) root         (0)    10774 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/LICENSE.md
+-rw-rw-r--   0 root         (0) root         (0)      439 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/MAINTAINERS.md
+-rw-r--r--   0 root         (0) root         (0)     5273 2024-04-03 15:13:30.381803 st4sd-runtime-core-2.1.3.dev3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3735 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/README.MD
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:13:30.349803 st4sd-runtime-core-2.1.3.dev3/deploy/
+-rw-rw-r--   0 root         (0) root         (0)      180 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/deploy/creation_payload.json
+-rwxrwxr-x   0 root         (0) root         (0)      292 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/deploy/skopeo_copy.sh
+-rw-rw-r--   0 root         (0) root         (0)      635 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/deploy/st4sd-runtime-core-image.deploy
+-rw-rw-r--   0 root         (0) root         (0)     1426 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/deploy/st4sd-runtime-core-multiarch.deploy
+-rw-rw-r--   0 root         (0) root         (0)      291 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/deploy/st4sd-runtime-core-release-tag.deploy
+-rwxrwxr-x   0 root         (0) root         (0)     2445 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/deploy/triggerExternalBuild.sh
+-rw-rw-r--   0 root         (0) root         (0)     2445 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/py37.Dockerfile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:13:30.345803 st4sd-runtime-core-2.1.3.dev3/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:13:30.349803 st4sd-runtime-core-2.1.3.dev3/python/experiment/
+-rw-rw-r--   0 root         (0) root         (0)       80 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    38736 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/appenv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:13:30.353803 st4sd-runtime-core-2.1.3.dev3/python/experiment/cli/
+-rw-rw-r--   0 root         (0) root         (0)      112 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/cli/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2842 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/cli/api.py
+-rw-rw-r--   0 root         (0) root         (0)     2560 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/cli/configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     6943 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/cli/context.py
+-rw-rw-r--   0 root         (0) root         (0)      267 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/cli/exit_codes.py
+-rw-rw-r--   0 root         (0) root         (0)     2705 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/cli/git.py
+-rw-rw-r--   0 root         (0) root         (0)     8283 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/cli/login.py
+-rw-rw-r--   0 root         (0) root         (0)    22932 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/cli/package.py
+-rw-rw-r--   0 root         (0) root         (0)     7051 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/cli/pull_secrets.py
+-rw-rw-r--   0 root         (0) root         (0)    31124 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/cli/pvep_schema.jsonschema
+-rw-rw-r--   0 root         (0) root         (0)      390 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/cli/stack.py
+-rw-rw-r--   0 root         (0) root         (0)     2392 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/cli/stp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:13:30.353803 st4sd-runtime-core-2.1.3.dev3/python/experiment/model/
+-rw-rw-r--   0 root         (0) root         (0)       80 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/model/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3003 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/model/codes.py
+-rw-rw-r--   0 root         (0) root         (0)    91119 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/model/conf.py
+-rw-rw-r--   0 root         (0) root         (0)   148053 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/model/data.py
+-rw-rw-r--   0 root         (0) root         (0)    46347 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/model/errors.py
+-rw-rw-r--   0 root         (0) root         (0)    59750 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/model/executors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:13:30.357803 st4sd-runtime-core-2.1.3.dev3/python/experiment/model/frontends/
+-rw-rw-r--   0 root         (0) root         (0)       80 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/model/frontends/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)   126138 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/model/frontends/cwl.py
+-rw-rw-r--   0 root         (0) root         (0)    85741 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/model/frontends/dosini.py
+-rw-rw-r--   0 root         (0) root         (0)   104839 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/model/frontends/dsl.py
+-rw-rw-r--   0 root         (0) root         (0)   262695 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/model/frontends/flowir.py
+-rw-rw-r--   0 root         (0) root         (0)   150222 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/model/graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:13:30.357803 st4sd-runtime-core-2.1.3.dev3/python/experiment/model/hooks/
+-rw-rw-r--   0 root         (0) root         (0)      683 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/model/hooks/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4236 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/model/hooks/hooks.py
+-rw-rw-r--   0 root         (0) root         (0)    36110 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/model/hooks/interface.py
+-rw-rw-r--   0 root         (0) root         (0)     2394 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/model/hooks/utils.py
+-rw-rw-r--   0 root         (0) root         (0)     5552 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/model/interface.py
+-rw-rw-r--   0 root         (0) root         (0)    67436 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/model/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:13:30.357803 st4sd-runtime-core-2.1.3.dev3/python/experiment/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:13:30.357803 st4sd-runtime-core-2.1.3.dev3/python/experiment/resources/Template.package/
+-rw-rw-r--   0 root         (0) root         (0)      544 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/resources/Template.package/README.MD
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:13:30.357803 st4sd-runtime-core-2.1.3.dev3/python/experiment/resources/Template.package/conf/
+-rw-rw-r--   0 root         (0) root         (0)      376 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/resources/Template.package/conf/flowir_package.yaml
+-rw-rw-r--   0 root         (0) root         (0)     6144 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/resources/Template.package.tar
+-rw-rw-r--   0 root         (0) root         (0)      630 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/rewrite-rules.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:13:30.361803 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/
+-rw-rw-r--   0 root         (0) root         (0)       80 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:13:30.365803 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/backend_interfaces/
+-rw-rw-r--   0 root         (0) root         (0)       80 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/backend_interfaces/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8178 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/backend_interfaces/docker.py
+-rw-rw-r--   0 root         (0) root         (0)   115031 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/backend_interfaces/k8s.py
+-rw-rw-r--   0 root         (0) root         (0)     5302 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/backend_interfaces/localtask.py
+-rw-rw-r--   0 root         (0) root         (0)   116500 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/backend_interfaces/lsf.py
+-rwxrwxr-x   0 root         (0) root         (0)     1414 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/backend_interfaces/stage-out.sh
+-rw-rw-r--   0 root         (0) root         (0)    13277 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/backend_interfaces/task_simulator.py
+-rw-rw-r--   0 root         (0) root         (0)    37745 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/backends.py
+-rw-rw-r--   0 root         (0) root         (0)    34800 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/backends_base.py
+-rw-rw-r--   0 root         (0) root         (0)   118126 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/control.py
+-rw-rw-r--   0 root         (0) root         (0)   104583 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/engine.py
+-rw-rw-r--   0 root         (0) root         (0)     5429 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:13:30.365803 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/interpreters/
+-rw-rw-r--   0 root         (0) root         (0)       80 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/interpreters/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    26290 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/interpreters/cwl.py
+-rw-rw-r--   0 root         (0) root         (0)     9481 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/interpreters/cwl_cmdline.py
+-rw-rw-r--   0 root         (0) root         (0)     8089 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/interpreters/js.py
+-rw-rw-r--   0 root         (0) root         (0)    20080 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/monitor.py
+-rw-rw-r--   0 root         (0) root         (0)    68147 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/optimizer.py
+-rw-rw-r--   0 root         (0) root         (0)    34954 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/output.py
+-rw-rw-r--   0 root         (0) root         (0)    45119 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/span.py
+-rw-rw-r--   0 root         (0) root         (0)    35543 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/status.py
+-rw-rw-r--   0 root         (0) root         (0)     5622 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:13:30.365803 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/utilities/
+-rw-rw-r--   0 root         (0) root         (0)       80 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/utilities/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3878 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/utilities/container_image_cache.py
+-rw-rw-r--   0 root         (0) root         (0)     4089 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/utilities/rx.py
+-rw-rw-r--   0 root         (0) root         (0)     5384 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/utilities/s3.py
+-rw-rw-r--   0 root         (0) root         (0)    36584 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:13:30.365803 st4sd-runtime-core-2.1.3.dev3/python/experiment/service/
+-rw-rw-r--   0 root         (0) root         (0)       80 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/service/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)   260764 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/service/db.py
+-rw-rw-r--   0 root         (0) root         (0)     8206 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/service/errors.py
+-rw-rw-r--   0 root         (0) root         (0)     7213 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/settings.py
+-rw-rw-r--   0 root         (0) root         (0)     6441 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:13:30.365803 st4sd-runtime-core-2.1.3.dev3/python/experiment/utilities/
+-rw-rw-r--   0 root         (0) root         (0)      104 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/utilities/README
+-rw-rw-r--   0 root         (0) root         (0)      317 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/utilities/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    58393 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/utilities/data.py
+-rw-rw-r--   0 root         (0) root         (0)     4705 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/python/experiment/utilities/fsearch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:13:30.381803 st4sd-runtime-core-2.1.3.dev3/python/st4sd_runtime_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5273 2024-04-03 15:13:30.000000 st4sd-runtime-core-2.1.3.dev3/python/st4sd_runtime_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4707 2024-04-03 15:13:30.000000 st4sd-runtime-core-2.1.3.dev3/python/st4sd_runtime_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 15:13:30.000000 st4sd-runtime-core-2.1.3.dev3/python/st4sd_runtime_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      291 2024-04-03 15:13:30.000000 st4sd-runtime-core-2.1.3.dev3/python/st4sd_runtime_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-03 15:13:30.000000 st4sd-runtime-core-2.1.3.dev3/python/st4sd_runtime_core.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:13:30.369803 st4sd-runtime-core-2.1.3.dev3/requirement_files/
+-rw-rw-r--   0 root         (0) root         (0)      133 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/requirement_files/requirements_base_3.7.txt
+-rw-rw-r--   0 root         (0) root         (0)      423 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/requirement_files/requirements_base_3.txt
+-rw-rw-r--   0 root         (0) root         (0)       18 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/requirement_files/requirements_deploy.txt
+-rw-rw-r--   0 root         (0) root         (0)       94 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/requirement_files/requirements_lsf.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:13:30.373803 st4sd-runtime-core-2.1.3.dev3/scripts/
+-rwxrwxr-x   0 root         (0) root         (0)     7054 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/scripts/ccommand.py
+-rwxrwxr-x   0 root         (0) root         (0)    11995 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/scripts/cexecute.py
+-rwxrwxr-x   0 root         (0) root         (0)     1239 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/scripts/checkpackage.py
+-rwxrwxr-x   0 root         (0) root         (0)     4286 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/scripts/ctest.py
+-rwxrwxr-x   0 root         (0) root         (0)     2567 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/scripts/ecreate.py
+-rwxrwxr-x   0 root         (0) root         (0)     4196 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/scripts/eflowir.py
+-rwxrwxr-x   0 root         (0) root         (0)     8094 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/scripts/einputs.py
+-rwxrwxr-x   0 root         (0) root         (0)     8246 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/scripts/einspect.py
+-rwxrwxr-x   0 root         (0) root         (0)   110012 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/scripts/elaunch.py
+-rwxrwxr-x   0 root         (0) root         (0)    17228 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/scripts/ememo.py
+-rwxrwxr-x   0 root         (0) root         (0)    46782 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/scripts/epatch-apply.py
+-rwxrwxr-x   0 root         (0) root         (0)    33324 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/scripts/epatch.py
+-rwxrwxr-x   0 root         (0) root         (0)    17371 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/scripts/etest.py
+-rwxrwxr-x   0 root         (0) root         (0)    10430 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/scripts/ewrap.py
+-rwxrwxr-x   0 root         (0) root         (0)      821 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/scripts/expstatus.sh
+-rw-rw-r--   0 root         (0) root         (0)     3840 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/scripts/k8srun.py
+-rwxrwxr-x   0 root         (0) root         (0)   110012 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/scripts/launchexperiment.py
+-rwxrwxr-x   0 root         (0) root         (0)    14013 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/scripts/lsfsub.py
+-rwxrwxr-x   0 root         (0) root         (0)      262 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/scripts/stp
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 15:13:30.381803 st4sd-runtime-core-2.1.3.dev3/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     4892 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:13:30.381803 st4sd-runtime-core-2.1.3.dev3/tests/
+-rw-rw-r--   0 root         (0) root         (0)       80 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10844 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/conftest.py
+-rw-rw-r--   0 root         (0) root         (0)    11290 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/dont_test_cwl.py
+-rw-rw-r--   0 root         (0) root         (0)     4541 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/reactive_testutils.py
+-rw-rw-r--   0 root         (0) root         (0)    14765 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/saltcurve_paragon.py
+-rw-rw-r--   0 root         (0) root         (0)    11225 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/test_array_variables.py
+-rw-rw-r--   0 root         (0) root         (0)    10570 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/test_command.py
+-rw-rw-r--   0 root         (0) root         (0)     9710 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/test_component.py
+-rw-rw-r--   0 root         (0) root         (0)     2432 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/test_container_image_uri_manipulation.py
+-rw-rw-r--   0 root         (0) root         (0)    44829 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/test_control.py
+-rw-rw-r--   0 root         (0) root         (0)     4840 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/test_data.py
+-rw-rw-r--   0 root         (0) root         (0)     5588 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/test_db.py
+-rw-rw-r--   0 root         (0) root         (0)    40808 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/test_dosini.py
+-rw-rw-r--   0 root         (0) root         (0)    35269 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/test_dowhile.py
+-rw-rw-r--   0 root         (0) root         (0)    44807 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/test_dsl.py
+-rw-rw-r--   0 root         (0) root         (0)    30930 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/test_engines.py
+-rw-rw-r--   0 root         (0) root         (0)    57895 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/test_flowir.py
+-rw-rw-r--   0 root         (0) root         (0)    23888 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/test_graph.py
+-rw-rw-r--   0 root         (0) root         (0)     3286 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/test_identifier.py
+-rw-rw-r--   0 root         (0) root         (0)    22923 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/test_interface.py
+-rw-rw-r--   0 root         (0) root         (0)     6059 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/test_k8s.py
+-rw-rw-r--   0 root         (0) root         (0)     2467 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/test_memoization.py
+-rw-rw-r--   0 root         (0) root         (0)    18732 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/test_package_load.py
+-rw-rw-r--   0 root         (0) root         (0)     1673 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/test_service.py
+-rw-rw-r--   0 root         (0) root         (0)     2085 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/test_settings.py
+-rw-rw-r--   0 root         (0) root         (0)     5825 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tests/utils.py
+-rw-rw-r--   0 root         (0) root         (0)     3119 2024-04-03 15:08:37.000000 st4sd-runtime-core-2.1.3.dev3/tox.ini
```

### Comparing `st4sd-runtime-core-2.1.3.dev2/.gitignore` & `st4sd-runtime-core-2.1.3.dev3/.gitignore`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/.travis.yml` & `st4sd-runtime-core-2.1.3.dev3/.travis.yml`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/CITATION.cff` & `st4sd-runtime-core-2.1.3.dev3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/CODE_OF_CONDUCT.md` & `st4sd-runtime-core-2.1.3.dev3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/CONTRIBUTING.md` & `st4sd-runtime-core-2.1.3.dev3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/Dockerfile` & `st4sd-runtime-core-2.1.3.dev3/Dockerfile`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/LICENSE.md` & `st4sd-runtime-core-2.1.3.dev3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/PKG-INFO` & `st4sd-runtime-core-2.1.3.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st4sd-runtime-core
-Version: 2.1.3.dev2
+Version: 2.1.3.dev3
 Summary: A tool for creating and deploying computational experiments
 Home-page: https://github.com/st4sd/st4sd-runtime-core
 Author: Michael A. Johnston
 Author-email: michaelj@ie.ibm.com
 License: Apache 2.0
 Keywords: hpc kubernetes openshift lsf workflows experiments computational-chemistry simulation science
 Classifier: Development Status :: 4 - Beta
```

### Comparing `st4sd-runtime-core-2.1.3.dev2/README.MD` & `st4sd-runtime-core-2.1.3.dev3/README.MD`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/deploy/st4sd-runtime-core-image.deploy` & `st4sd-runtime-core-2.1.3.dev3/deploy/st4sd-runtime-core-image.deploy`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/deploy/st4sd-runtime-core-multiarch.deploy` & `st4sd-runtime-core-2.1.3.dev3/deploy/st4sd-runtime-core-multiarch.deploy`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/deploy/triggerExternalBuild.sh` & `st4sd-runtime-core-2.1.3.dev3/deploy/triggerExternalBuild.sh`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/py37.Dockerfile` & `st4sd-runtime-core-2.1.3.dev3/py37.Dockerfile`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/appenv.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/appenv.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/cli/api.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/cli/api.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/cli/configuration.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/cli/configuration.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/cli/context.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/cli/context.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/cli/git.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/cli/git.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/cli/login.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/cli/login.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/cli/package.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/cli/package.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/cli/pull_secrets.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/cli/pull_secrets.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/cli/pvep_schema.jsonschema` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/cli/pvep_schema.jsonschema`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/cli/stp.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/cli/stp.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/model/codes.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/model/codes.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/model/conf.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/model/conf.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/model/data.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/model/data.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/model/errors.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/model/errors.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/model/executors.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/model/executors.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/model/frontends/cwl.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/model/frontends/cwl.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/model/frontends/dosini.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/model/frontends/dosini.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/model/frontends/dsl.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/model/frontends/dsl.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/model/frontends/flowir.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/model/frontends/flowir.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/model/graph.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/model/graph.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/model/hooks/__init__.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/model/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/model/hooks/hooks.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/model/hooks/hooks.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/model/hooks/interface.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/model/hooks/interface.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/model/hooks/utils.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/model/hooks/utils.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/model/interface.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/model/interface.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/model/storage.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/model/storage.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/resources/Template.package/README.MD` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/resources/Template.package/README.MD`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/resources/Template.package.tar` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/resources/Template.package.tar`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/rewrite-rules.json` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/rewrite-rules.json`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/backend_interfaces/docker.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/backend_interfaces/docker.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/backend_interfaces/k8s.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/backend_interfaces/k8s.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/backend_interfaces/localtask.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/backend_interfaces/localtask.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/backend_interfaces/lsf.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/backend_interfaces/lsf.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/backend_interfaces/stage-out.sh` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/backend_interfaces/stage-out.sh`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/backend_interfaces/task_simulator.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/backend_interfaces/task_simulator.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/backends.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/backends.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/backends_base.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/backends_base.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/control.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/control.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/engine.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/engine.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/errors.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/errors.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/interpreters/cwl.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/interpreters/cwl.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/interpreters/cwl_cmdline.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/interpreters/cwl_cmdline.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/interpreters/js.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/interpreters/js.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/monitor.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/monitor.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/optimizer.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/optimizer.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/output.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/output.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/span.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/span.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/status.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/status.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/task.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/task.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/utilities/container_image_cache.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/utilities/container_image_cache.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/utilities/rx.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/utilities/rx.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/utilities/s3.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/utilities/s3.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/runtime/workflow.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/runtime/workflow.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/service/db.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/service/db.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/service/errors.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/service/errors.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/settings.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/settings.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/test.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/test.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/utilities/data.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/utilities/data.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/experiment/utilities/fsearch.py` & `st4sd-runtime-core-2.1.3.dev3/python/experiment/utilities/fsearch.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/st4sd_runtime_core.egg-info/PKG-INFO` & `st4sd-runtime-core-2.1.3.dev3/python/st4sd_runtime_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st4sd-runtime-core
-Version: 2.1.3.dev2
+Version: 2.1.3.dev3
 Summary: A tool for creating and deploying computational experiments
 Home-page: https://github.com/st4sd/st4sd-runtime-core
 Author: Michael A. Johnston
 Author-email: michaelj@ie.ibm.com
 License: Apache 2.0
 Keywords: hpc kubernetes openshift lsf workflows experiments computational-chemistry simulation science
 Classifier: Development Status :: 4 - Beta
```

### Comparing `st4sd-runtime-core-2.1.3.dev2/python/st4sd_runtime_core.egg-info/SOURCES.txt` & `st4sd-runtime-core-2.1.3.dev3/python/st4sd_runtime_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/scripts/ccommand.py` & `st4sd-runtime-core-2.1.3.dev3/scripts/ccommand.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/scripts/cexecute.py` & `st4sd-runtime-core-2.1.3.dev3/scripts/cexecute.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/scripts/checkpackage.py` & `st4sd-runtime-core-2.1.3.dev3/scripts/checkpackage.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/scripts/ctest.py` & `st4sd-runtime-core-2.1.3.dev3/scripts/ctest.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/scripts/ecreate.py` & `st4sd-runtime-core-2.1.3.dev3/scripts/ecreate.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/scripts/eflowir.py` & `st4sd-runtime-core-2.1.3.dev3/scripts/eflowir.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/scripts/einputs.py` & `st4sd-runtime-core-2.1.3.dev3/scripts/einputs.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/scripts/einspect.py` & `st4sd-runtime-core-2.1.3.dev3/scripts/einspect.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/scripts/elaunch.py` & `st4sd-runtime-core-2.1.3.dev3/scripts/elaunch.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,33 +191,43 @@
 SetupExceptions = Union[experiment.model.errors.ExperimentInvalidConfigurationError,
                         Optional[experiment.model.errors.ExperimentSetupError]]
 SetupReturnType = Tuple[SetupExceptions, Optional[experiment.model.data.Experiment],
                         Optional[experiment.runtime.output.OutputAgent], Optional[
                             experiment.runtime.output.StatusMonitor]]
 
 
-def extract_application_dependency_source(options):
-    # type: (optparse.Values) -> Dict[str, str]
+
+def extract_application_dependency_source(app_dep_sources: List[str], package_path: str) -> Dict[str, str]:
     """Parses --applicationDependencySource commandline arguments (`applicationDependencyEntry:/path/to/new/source`)
 
     Args:
-        options(optparse.Values): commandline arguments to elaunch
+        app_dep_sources:
+            A list of $appDepSourceName(=:)/path/to/new/source[:optional link or copy]
+        package_path:
+            Path to the package that's being loaded
 
     Returns
         A dictionary whose keys are application dependency names and values are absolute paths
     """
     application_dependency_source = {}  # type: Dict[str, str]
 
-    for s in options.application_dependency_source:
+    for app_and_src in app_dep_sources or []:
         try:
-            app_dep, new_source = s.split(':', 1)
+            app_dep, new_source = app_and_src.split('=', 1)
         except ValueError:
-            raise ValueError('Application dependency source "%s" does not have the format '
-                             '`applicationDependencyEntry:/path/to/new/source`' % s)
-        application_dependency_source[app_dep] = new_source
+            try:
+                app_dep, new_source = app_and_src.split(':', 1)
+            except ValueError:
+                raise ValueError('Application dependency source "%s" does not have the format '
+                                 '`applicationDependencyEntry:/path/to/new/source`' % s)
+        if new_source.startswith("%(package)s"):
+            new_source = new_source.replace("%(package)s", package_path)
+
+        application_dependency_source[app_dep] = os.path.abspath(new_source)
+
     return application_dependency_source
 
 
 def Setup(setupPath, options):
     # type: (str, optparse.Values) -> SetupReturnType
     '''Wraps setting up the experiment for running.
 
@@ -248,15 +258,18 @@
 
     if options.cwlJobOrderFile is not None:
         cwl_options['cwlJobOrderFile'] = options.cwlJobOrderFile
 
     compExperiment = None
     rootLogger = None
 
-    custom_application_sources = extract_application_dependency_source(options)
+    custom_application_sources = extract_application_dependency_source(
+        options.application_dependency_source,
+        package_path=setupPath
+    )
 
     if options.restart is None:
         packagePath = setupPath
         isValid, error, compExperiment = experiment.test.ValidatePackage(
             packagePath, platform=options.platform, format_priority=options.formatPriority,
             inputs=options.inputs, data=options.data, variables=options.variables, timestamp=options.stamp,
             instance_name=options.instance_name, custom_application_sources=custom_application_sources,
@@ -1255,18 +1268,21 @@
                                   "to use a spec.securityContext (which among other things, sets a non-root user id, "
                                   "non-root group id, and a fs-group identifier). This can be problematic for "
                                   "containers which expect to be run as root. Setting this to Yes will instruct "
                                   "flow to not inject a securityContext to pods it generates. Doing so can be "
                                   "considered a security risk and should be avoided. Default is No.")
     launchOptions.add_option("-s", "--applicationDependencySource", dest="application_dependency_source",
                              help="Point an application dependency to a specific "
-                                  "path on the filesystem `applicationDependencyEntry:/path/to/new/source[:link/:copy]`"
-                                  "The :link and :copy suffixes determine whether to link or copy the path under the "
-                                  "instance directory. They suffix is optional and defaults to :link. If the path "
-                                  "contains a ':' character, use '%3A' instead (i.e. url-encode the : character)",
+                                  "path on the filesystem `applicationDependencyEntry=/path/to/new/source[:link/:copy]`"
+                                  ". The :link and :copy suffixes determine whether to link or copy the path under the "
+                                  "instance directory. The suffix is optional and defaults to :link. If the path "
+                                  "contains a ':' character, use '%3A' instead (i.e. url-encode the : character). "
+                                  "You may also use `:` to separate the name of the application dependency entry "
+                                  "and its path. Finally, if the path starts with '%(package)s' then elaunch.py "
+                                  "resolves that reference to the package path.",
                              default=[], metavar="APPLICATION_DEPENDENCY_SOURCE", action="append")
     launchOptions.add_option('', '--manifest', dest="manifest", metavar="PATH_TO_MANIFEST_FILE", default=None,
                              help="Optional path to manifest YAML file to use when setting up package directory from a "
                                   "FlowIR YAML file. The manifest should contain a dictionary, with "
                                   "targetFolder: sourceFolder entries. Each sourceFolder will be copied or linked to "
                                   "populate the respective targetFolder. Source folders can be absolute paths, or "
                                   "paths relative to the path of the FlowIR YAML file. SourceFolders may also be "
@@ -1822,15 +1838,18 @@
         LivePatcher.controller = controller
         LivePatcher.output_agent = outputAgent
         LivePatcher.mon_status = statusMonitor
         LivePatcher.components = components
         LivePatcher.initial_stage = initial_stage
         LivePatcher.format_priority = list(options.formatPriority)
         LivePatcher.platform_name = options.platform or experiment.model.frontends.flowir.FlowIR.LabelDefault
-        LivePatcher.custom_application_sources = extract_application_dependency_source(options)
+        LivePatcher.custom_application_sources = extract_application_dependency_source(
+            options.application_dependency_source,
+            package_path=packagePath
+        )
 
         signal.signal(signal.SIGALRM, lambda _signal, frame: live_patch_trigger())
 
         # VV: Right now we only have 1 variables file, but there's no reason to limit ourselves to just 1
         user_variables = {}
         if options.variables:
             try:
```

### Comparing `st4sd-runtime-core-2.1.3.dev2/scripts/ememo.py` & `st4sd-runtime-core-2.1.3.dev3/scripts/ememo.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/scripts/epatch-apply.py` & `st4sd-runtime-core-2.1.3.dev3/scripts/epatch-apply.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/scripts/epatch.py` & `st4sd-runtime-core-2.1.3.dev3/scripts/epatch.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/scripts/etest.py` & `st4sd-runtime-core-2.1.3.dev3/scripts/etest.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/scripts/ewrap.py` & `st4sd-runtime-core-2.1.3.dev3/scripts/ewrap.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/scripts/expstatus.sh` & `st4sd-runtime-core-2.1.3.dev3/scripts/expstatus.sh`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/scripts/k8srun.py` & `st4sd-runtime-core-2.1.3.dev3/scripts/k8srun.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/scripts/launchexperiment.py` & `st4sd-runtime-core-2.1.3.dev3/scripts/launchexperiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,33 +191,43 @@
 SetupExceptions = Union[experiment.model.errors.ExperimentInvalidConfigurationError,
                         Optional[experiment.model.errors.ExperimentSetupError]]
 SetupReturnType = Tuple[SetupExceptions, Optional[experiment.model.data.Experiment],
                         Optional[experiment.runtime.output.OutputAgent], Optional[
                             experiment.runtime.output.StatusMonitor]]
 
 
-def extract_application_dependency_source(options):
-    # type: (optparse.Values) -> Dict[str, str]
+
+def extract_application_dependency_source(app_dep_sources: List[str], package_path: str) -> Dict[str, str]:
     """Parses --applicationDependencySource commandline arguments (`applicationDependencyEntry:/path/to/new/source`)
 
     Args:
-        options(optparse.Values): commandline arguments to elaunch
+        app_dep_sources:
+            A list of $appDepSourceName(=:)/path/to/new/source[:optional link or copy]
+        package_path:
+            Path to the package that's being loaded
 
     Returns
         A dictionary whose keys are application dependency names and values are absolute paths
     """
     application_dependency_source = {}  # type: Dict[str, str]
 
-    for s in options.application_dependency_source:
+    for app_and_src in app_dep_sources or []:
         try:
-            app_dep, new_source = s.split(':', 1)
+            app_dep, new_source = app_and_src.split('=', 1)
         except ValueError:
-            raise ValueError('Application dependency source "%s" does not have the format '
-                             '`applicationDependencyEntry:/path/to/new/source`' % s)
-        application_dependency_source[app_dep] = new_source
+            try:
+                app_dep, new_source = app_and_src.split(':', 1)
+            except ValueError:
+                raise ValueError('Application dependency source "%s" does not have the format '
+                                 '`applicationDependencyEntry:/path/to/new/source`' % s)
+        if new_source.startswith("%(package)s"):
+            new_source = new_source.replace("%(package)s", package_path)
+
+        application_dependency_source[app_dep] = os.path.abspath(new_source)
+
     return application_dependency_source
 
 
 def Setup(setupPath, options):
     # type: (str, optparse.Values) -> SetupReturnType
     '''Wraps setting up the experiment for running.
 
@@ -248,15 +258,18 @@
 
     if options.cwlJobOrderFile is not None:
         cwl_options['cwlJobOrderFile'] = options.cwlJobOrderFile
 
     compExperiment = None
     rootLogger = None
 
-    custom_application_sources = extract_application_dependency_source(options)
+    custom_application_sources = extract_application_dependency_source(
+        options.application_dependency_source,
+        package_path=setupPath
+    )
 
     if options.restart is None:
         packagePath = setupPath
         isValid, error, compExperiment = experiment.test.ValidatePackage(
             packagePath, platform=options.platform, format_priority=options.formatPriority,
             inputs=options.inputs, data=options.data, variables=options.variables, timestamp=options.stamp,
             instance_name=options.instance_name, custom_application_sources=custom_application_sources,
@@ -1255,18 +1268,21 @@
                                   "to use a spec.securityContext (which among other things, sets a non-root user id, "
                                   "non-root group id, and a fs-group identifier). This can be problematic for "
                                   "containers which expect to be run as root. Setting this to Yes will instruct "
                                   "flow to not inject a securityContext to pods it generates. Doing so can be "
                                   "considered a security risk and should be avoided. Default is No.")
     launchOptions.add_option("-s", "--applicationDependencySource", dest="application_dependency_source",
                              help="Point an application dependency to a specific "
-                                  "path on the filesystem `applicationDependencyEntry:/path/to/new/source[:link/:copy]`"
-                                  "The :link and :copy suffixes determine whether to link or copy the path under the "
-                                  "instance directory. They suffix is optional and defaults to :link. If the path "
-                                  "contains a ':' character, use '%3A' instead (i.e. url-encode the : character)",
+                                  "path on the filesystem `applicationDependencyEntry=/path/to/new/source[:link/:copy]`"
+                                  ". The :link and :copy suffixes determine whether to link or copy the path under the "
+                                  "instance directory. The suffix is optional and defaults to :link. If the path "
+                                  "contains a ':' character, use '%3A' instead (i.e. url-encode the : character). "
+                                  "You may also use `:` to separate the name of the application dependency entry "
+                                  "and its path. Finally, if the path starts with '%(package)s' then elaunch.py "
+                                  "resolves that reference to the package path.",
                              default=[], metavar="APPLICATION_DEPENDENCY_SOURCE", action="append")
     launchOptions.add_option('', '--manifest', dest="manifest", metavar="PATH_TO_MANIFEST_FILE", default=None,
                              help="Optional path to manifest YAML file to use when setting up package directory from a "
                                   "FlowIR YAML file. The manifest should contain a dictionary, with "
                                   "targetFolder: sourceFolder entries. Each sourceFolder will be copied or linked to "
                                   "populate the respective targetFolder. Source folders can be absolute paths, or "
                                   "paths relative to the path of the FlowIR YAML file. SourceFolders may also be "
@@ -1822,15 +1838,18 @@
         LivePatcher.controller = controller
         LivePatcher.output_agent = outputAgent
         LivePatcher.mon_status = statusMonitor
         LivePatcher.components = components
         LivePatcher.initial_stage = initial_stage
         LivePatcher.format_priority = list(options.formatPriority)
         LivePatcher.platform_name = options.platform or experiment.model.frontends.flowir.FlowIR.LabelDefault
-        LivePatcher.custom_application_sources = extract_application_dependency_source(options)
+        LivePatcher.custom_application_sources = extract_application_dependency_source(
+            options.application_dependency_source,
+            package_path=packagePath
+        )
 
         signal.signal(signal.SIGALRM, lambda _signal, frame: live_patch_trigger())
 
         # VV: Right now we only have 1 variables file, but there's no reason to limit ourselves to just 1
         user_variables = {}
         if options.variables:
             try:
```

### Comparing `st4sd-runtime-core-2.1.3.dev2/scripts/lsfsub.py` & `st4sd-runtime-core-2.1.3.dev3/scripts/lsfsub.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/setup.py` & `st4sd-runtime-core-2.1.3.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/conftest.py` & `st4sd-runtime-core-2.1.3.dev3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/dont_test_cwl.py` & `st4sd-runtime-core-2.1.3.dev3/tests/dont_test_cwl.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/reactive_testutils.py` & `st4sd-runtime-core-2.1.3.dev3/tests/reactive_testutils.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/saltcurve_paragon.py` & `st4sd-runtime-core-2.1.3.dev3/tests/saltcurve_paragon.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/test_array_variables.py` & `st4sd-runtime-core-2.1.3.dev3/tests/test_array_variables.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/test_command.py` & `st4sd-runtime-core-2.1.3.dev3/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/test_component.py` & `st4sd-runtime-core-2.1.3.dev3/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/test_container_image_uri_manipulation.py` & `st4sd-runtime-core-2.1.3.dev3/tests/test_container_image_uri_manipulation.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/test_control.py` & `st4sd-runtime-core-2.1.3.dev3/tests/test_control.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/test_data.py` & `st4sd-runtime-core-2.1.3.dev3/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/test_db.py` & `st4sd-runtime-core-2.1.3.dev3/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/test_dosini.py` & `st4sd-runtime-core-2.1.3.dev3/tests/test_dosini.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/test_dowhile.py` & `st4sd-runtime-core-2.1.3.dev3/tests/test_dowhile.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/test_dsl.py` & `st4sd-runtime-core-2.1.3.dev3/tests/test_dsl.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/test_engines.py` & `st4sd-runtime-core-2.1.3.dev3/tests/test_engines.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/test_flowir.py` & `st4sd-runtime-core-2.1.3.dev3/tests/test_flowir.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/test_graph.py` & `st4sd-runtime-core-2.1.3.dev3/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/test_identifier.py` & `st4sd-runtime-core-2.1.3.dev3/tests/test_identifier.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/test_interface.py` & `st4sd-runtime-core-2.1.3.dev3/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/test_k8s.py` & `st4sd-runtime-core-2.1.3.dev3/tests/test_k8s.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/test_memoization.py` & `st4sd-runtime-core-2.1.3.dev3/tests/test_memoization.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/test_package_load.py` & `st4sd-runtime-core-2.1.3.dev3/tests/test_package_load.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/test_service.py` & `st4sd-runtime-core-2.1.3.dev3/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/test_settings.py` & `st4sd-runtime-core-2.1.3.dev3/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tests/utils.py` & `st4sd-runtime-core-2.1.3.dev3/tests/utils.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.1.3.dev2/tox.ini` & `st4sd-runtime-core-2.1.3.dev3/tox.ini`

 * *Files identical despite different names*

