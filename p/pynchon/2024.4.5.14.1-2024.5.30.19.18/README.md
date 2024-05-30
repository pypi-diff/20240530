# Comparing `tmp/pynchon-2024.4.5.14.1.tar.gz` & `tmp/pynchon-2024.5.30.19.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynchon-2024.4.5.14.1.tar", last modified: Fri Apr  5 14:01:10 2024, max compression
+gzip compressed data, was "pynchon-2024.5.30.19.18.tar", last modified: Thu May 30 19:18:14 2024, max compression
```

## Comparing `pynchon-2024.4.5.14.1.tar` & `pynchon-2024.5.30.19.18.tar`

### file list

```diff
@@ -1,297 +1,298 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.440942 pynchon-2024.4.5.14.1/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-05 14:01:10.440942 pynchon-2024.4.5.14.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27572 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-05 14:01:10.444942 pynchon-2024.4.5.14.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.368942 pynchon-2024.4.5.14.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.380942 pynchon-2024.4.5.14.1/src/pynchon/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-05 14:01:07.000000 pynchon-2024.4.5.14.1/src/pynchon/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.384942 pynchon-2024.4.5.14.1/src/pynchon/abcs/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/abcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/abcs/attrdict.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/abcs/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/abcs/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/abcs/visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/annotate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.384942 pynchon-2024.4.5.14.1/src/pynchon/api/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.384942 pynchon-2024.4.5.14.1/src/pynchon/api/git/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/api/git/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.384942 pynchon-2024.4.5.14.1/src/pynchon/api/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/api/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.384942 pynchon-2024.4.5.14.1/src/pynchon/api/project/
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/api/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/api/pynchon.py
--rw-r--r--   0 runner    (1001) docker     (127)     7341 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/api/render.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/app.py
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/bin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.384942 pynchon-2024.4.5.14.1/src/pynchon/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/cli/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/cli/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.384942 pynchon-2024.4.5.14.1/src/pynchon/codemod/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/codemod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.384942 pynchon-2024.4.5.14.1/src/pynchon/codemod/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/codemod/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.384942 pynchon-2024.4.5.14.1/src/pynchon/codemod/commands/docstrings/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/codemod/commands/docstrings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/codemod/commands/docstrings/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/codemod/commands/docstrings/javadoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/codemod/commands/docstrings/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.388942 pynchon-2024.4.5.14.1/src/pynchon/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/config/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.388942 pynchon-2024.4.5.14.1/src/pynchon/models/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9273 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/models/planner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/models/planning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.388942 pynchon-2024.4.5.14.1/src/pynchon/models/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/models/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/models/plugins/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/models/plugins/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/models/plugins/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/models/plugins/pynchon.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/models/plugins/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/models/plugins/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/models/python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.396942 pynchon-2024.4.5.14.1/src/pynchon/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/__template__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/cicd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/deck.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/dockerhub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.396942 pynchon-2024.4.5.14.1/src/pynchon/plugins/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/docs/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/docs/opener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.396942 pynchon-2024.4.5.14.1/src/pynchon/plugins/doctor/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/doctor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/drawio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/fixme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/github.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/griffe.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/makefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/mermaid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8015 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/mkdocs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/pandoc.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)    14638 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.396942 pynchon-2024.4.5.14.1/src/pynchon/plugins/python/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/python/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17587 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/python/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/python/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/python/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/python/libcst.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/python/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/python/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/python/pypi.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/release.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/render.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/rtd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.396942 pynchon-2024.4.5.14.1/src/pynchon/plugins/scaffolding/
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/scaffolding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/scaffolding/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7353 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/src.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/plugins/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/tagging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.372942 pynchon-2024.4.5.14.1/src/pynchon/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.396942 pynchon-2024.4.5.14.1/src/pynchon/templates/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/docker/Dockerfile.pandoc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.400942 pynchon-2024.4.5.14.1/src/pynchon/templates/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.372942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.400942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.400942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/github/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/github/header.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.372942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.400942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/VERSIONS.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.400942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bash.sh
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bashrc.sh
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/makefile.j2
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/python.j2
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.400942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/fixme/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/fixme/FIXME.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.400942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/makefile/
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/makefile/mermaid-graph.mmd.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.372942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.400942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/api/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/api/TOC.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/api/modules.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/api/names.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.372942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/gen/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.404942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/function.txt.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/module.txt.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.404942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python_cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python_cli/TOC.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python_cli/detail.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python_cli/main.module.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python_cli/script.console.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python_cli/subcommand.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.372942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.404942 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/src/header/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/src/header/jinja-md.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/src/header/jinja.j2
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/src/header/python.j2
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/pydantic-model.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.404942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.372942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/ansible/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.404942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/ansible/role/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/ansible/role/.ansible-lint
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.372942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/ansible/role/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.404942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/ansible/role/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/ansible/role/.github/workflows/ansible-lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/ansible/role/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.404942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/docker/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/docker/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/docker/.scaffold.advice.json5
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/docker/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.372942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.404942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/docs/includes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/docs/includes/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.404942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.372942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/github/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.408942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/github/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/github/.github/workflows/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/github/.github/workflows/hello-world.yml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/github/.scaffold.advice.json5
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/github/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.376942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.408942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/.ackrc
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/.libcst.codemod.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/.scaffold.advice.json5
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.408942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/docs/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.408942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/docs/html/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/docs/html/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.376942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.412942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/app.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/lme.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/tagging.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.412942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tests/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.412942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tests/integration/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tests/integration/test_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.416942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tests/smoke/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tests/smoke/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tests/smoke/test_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.416942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tests/units/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tests/units/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tests/units/test_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.416942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/workspace/.scaffold.advice.json5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.376942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/software/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.416942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/software/automation/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/software/automation/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.416942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/software/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/software/tests/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.376942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/software/tests/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.420942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/software/tests/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/software/tests/tests/integration/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.420942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/software/tests/tests/smoke/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/software/tests/tests/smoke/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.420942 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/software/tests/tests/units/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/software/tests/tests/units/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.424942 pynchon-2024.4.5.14.1/src/pynchon/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/complexity.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.428942 pynchon-2024.4.5.14.1/src/pynchon/util/console/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/console/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.428942 pynchon-2024.4.5.14.1/src/pynchon/util/files/
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/files/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/files/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/lme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.428942 pynchon-2024.4.5.14.1/src/pynchon/util/makefile/
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/makefile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/makefile/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/oop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.432942 pynchon-2024.4.5.14.1/src/pynchon/util/os/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/os/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/os/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/os/pidfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/os/pids.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/python.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/splitvt.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.432942 pynchon-2024.4.5.14.1/src/pynchon/util/text/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/text/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.436941 pynchon-2024.4.5.14.1/src/pynchon/util/text/dumpf/
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/text/dumpf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/text/dumpf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/text/dumps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.436941 pynchon-2024.4.5.14.1/src/pynchon/util/text/loadf/
--rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/text/loadf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/text/loadf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/text/loads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.436941 pynchon-2024.4.5.14.1/src/pynchon/util/text/normalize/
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/text/normalize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.440942 pynchon-2024.4.5.14.1/src/pynchon/util/text/render/
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/text/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-05 13:57:11.000000 pynchon-2024.4.5.14.1/src/pynchon/util/text/render/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-05 13:56:03.000000 pynchon-2024.4.5.14.1/src/pynchon/util/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:10.440942 pynchon-2024.4.5.14.1/src/pynchon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-05 14:01:10.000000 pynchon-2024.4.5.14.1/src/pynchon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9308 2024-04-05 14:01:10.000000 pynchon-2024.4.5.14.1/src/pynchon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:01:10.000000 pynchon-2024.4.5.14.1/src/pynchon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-05 14:01:10.000000 pynchon-2024.4.5.14.1/src/pynchon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:01:10.000000 pynchon-2024.4.5.14.1/src/pynchon.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-05 14:01:10.000000 pynchon-2024.4.5.14.1/src/pynchon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 14:01:10.000000 pynchon-2024.4.5.14.1/src/pynchon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.497947 pynchon-2024.5.30.19.18/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-30 19:18:14.497947 pynchon-2024.5.30.19.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27747 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-30 19:18:14.497947 pynchon-2024.5.30.19.18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.449946 pynchon-2024.5.30.19.18/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.461946 pynchon-2024.5.30.19.18/src/pynchon/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-30 19:18:11.000000 pynchon-2024.5.30.19.18/src/pynchon/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.465946 pynchon-2024.5.30.19.18/src/pynchon/abcs/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/abcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/abcs/attrdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/abcs/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/abcs/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/abcs/visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/annotate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.465946 pynchon-2024.5.30.19.18/src/pynchon/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.465946 pynchon-2024.5.30.19.18/src/pynchon/api/git/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/api/git/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.465946 pynchon-2024.5.30.19.18/src/pynchon/api/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/api/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.465946 pynchon-2024.5.30.19.18/src/pynchon/api/project/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/api/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/api/pynchon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/api/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/bin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.465946 pynchon-2024.5.30.19.18/src/pynchon/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/cli/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.465946 pynchon-2024.5.30.19.18/src/pynchon/codemod/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/codemod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.465946 pynchon-2024.5.30.19.18/src/pynchon/codemod/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/codemod/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.465946 pynchon-2024.5.30.19.18/src/pynchon/codemod/commands/docstrings/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/codemod/commands/docstrings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/codemod/commands/docstrings/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/codemod/commands/docstrings/javadoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/codemod/commands/docstrings/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.465946 pynchon-2024.5.30.19.18/src/pynchon/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/config/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.465946 pynchon-2024.5.30.19.18/src/pynchon/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9673 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/models/planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/models/planning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.469946 pynchon-2024.5.30.19.18/src/pynchon/models/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/models/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10630 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/models/plugins/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/models/plugins/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/models/plugins/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/models/plugins/pynchon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/models/plugins/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/models/plugins/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/models/python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.473946 pynchon-2024.5.30.19.18/src/pynchon/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/__template__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/cicd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/compose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/deck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/dockerhub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.473946 pynchon-2024.5.30.19.18/src/pynchon/plugins/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/docs/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/docs/opener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.473946 pynchon-2024.5.30.19.18/src/pynchon/plugins/doctor/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/doctor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/drawio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/fixme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/griffe.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9278 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/mermaid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/mkdocs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/pandoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14638 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.477946 pynchon-2024.5.30.19.18/src/pynchon/plugins/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/python/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17587 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/python/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/python/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/python/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/python/libcst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/python/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/python/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/python/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/rtd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.477946 pynchon-2024.5.30.19.18/src/pynchon/plugins/scaffolding/
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/scaffolding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/scaffolding/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7353 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/src.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/plugins/vhs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/tagging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.453946 pynchon-2024.5.30.19.18/src/pynchon/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.477946 pynchon-2024.5.30.19.18/src/pynchon/templates/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/docker/Dockerfile.pandoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.477946 pynchon-2024.5.30.19.18/src/pynchon/templates/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.453946 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.477946 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.477946 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/github/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/github/header.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.453946 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.477946 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/core/VERSIONS.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.477946 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bash.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bashrc.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/makefile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/python.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.477946 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/fixme/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/fixme/FIXME.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.477946 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/makefile/
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/makefile/mermaid-graph.mmd.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.453946 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.481946 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python/api/TOC.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python/api/modules.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python/api/names.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.453946 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python/gen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.481946 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/function.txt.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/module.txt.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.481946 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python_cli/TOC.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python_cli/detail.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python_cli/main.module.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python_cli/script.console.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python_cli/subcommand.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.453946 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.481946 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/src/header/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/src/header/jinja-md.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/src/header/jinja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/src/header/python.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/pydantic-model.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.481946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.453946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/ansible/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.481946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/ansible/role/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/ansible/role/.ansible-lint
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.457946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/ansible/role/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.481946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/ansible/role/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/ansible/role/.github/workflows/ansible-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/ansible/role/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.481946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/docker/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/docker/.scaffold.advice.json5
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/docker/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.457946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.481946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/docs/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/docs/includes/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.481946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.457946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/github/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.481946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/github/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/github/.github/workflows/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/github/.github/workflows/hello-world.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/github/.scaffold.advice.json5
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/github/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.457946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.485946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/.ackrc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/.libcst.codemod.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/.scaffold.advice.json5
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.485946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/docs/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.485946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/docs/html/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/docs/html/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.457946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.485946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/lme.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/tagging.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.485946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/tests/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.485946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/tests/integration/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/tests/integration/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.489946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/tests/smoke/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/tests/smoke/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/tests/smoke/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.489946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/tests/units/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/tests/units/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/tests/units/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.489946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/workspace/.scaffold.advice.json5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.457946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/software/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.489946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/software/automation/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/software/automation/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.489946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/software/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/software/tests/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.457946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/software/tests/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.489946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/software/tests/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/software/tests/tests/integration/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.489946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/software/tests/tests/smoke/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/software/tests/tests/smoke/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.489946 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/software/tests/tests/units/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/software/tests/tests/units/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.489946 pynchon-2024.5.30.19.18/src/pynchon/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/util/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/util/complexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/util/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.489946 pynchon-2024.5.30.19.18/src/pynchon/util/console/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/util/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/util/console/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/util/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/util/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.489946 pynchon-2024.5.30.19.18/src/pynchon/util/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/util/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/util/files/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/util/files/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/util/lme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.493946 pynchon-2024.5.30.19.18/src/pynchon/util/makefile/
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/util/makefile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/util/makefile/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/util/oop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.493946 pynchon-2024.5.30.19.18/src/pynchon/util/os/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/util/os/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/util/os/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/util/os/pidfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/util/os/pids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/util/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/util/splitvt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/util/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.493946 pynchon-2024.5.30.19.18/src/pynchon/util/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/util/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/util/text/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.493946 pynchon-2024.5.30.19.18/src/pynchon/util/text/dumpf/
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/util/text/dumpf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/util/text/dumpf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/util/text/dumps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.493946 pynchon-2024.5.30.19.18/src/pynchon/util/text/loadf/
+-rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/util/text/loadf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/util/text/loadf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/util/text/loads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.493946 pynchon-2024.5.30.19.18/src/pynchon/util/text/normalize/
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/util/text/normalize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.493946 pynchon-2024.5.30.19.18/src/pynchon/util/text/render/
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/util/text/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-30 19:14:13.000000 pynchon-2024.5.30.19.18/src/pynchon/util/text/render/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-30 19:13:12.000000 pynchon-2024.5.30.19.18/src/pynchon/util/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:18:14.493946 pynchon-2024.5.30.19.18/src/pynchon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-30 19:18:14.000000 pynchon-2024.5.30.19.18/src/pynchon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9338 2024-05-30 19:18:14.000000 pynchon-2024.5.30.19.18/src/pynchon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:18:14.000000 pynchon-2024.5.30.19.18/src/pynchon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 19:18:14.000000 pynchon-2024.5.30.19.18/src/pynchon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:18:14.000000 pynchon-2024.5.30.19.18/src/pynchon.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-30 19:18:14.000000 pynchon-2024.5.30.19.18/src/pynchon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 19:18:14.000000 pynchon-2024.5.30.19.18/src/pynchon.egg-info/top_level.txt
```

### Comparing `pynchon-2024.4.5.14.1/PKG-INFO` & `pynchon-2024.5.30.19.18/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pynchon
-Version: 2024.4.5.14.1
+Version: 2024.5.30.19.18
 Summary: Autodocs for python projects
 Home-page: https://github.com/elo-enterprises/pynchon/
 Author: elo
 Author-email: engineering@elo.enterprises
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/pynchon/
 Project-URL: Source, https://github.com/elo-enterprises/pynchon/
 Project-URL: Download, https://github.com/elo-enterprises/pynchon/#files
 Platform: any
 Classifier: Programming Language :: Python
 Requires-Python: >3.6
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Requires-Dist: gripe>=2024.2.24.1.31
-Requires-Dist: shil>=2023.7.17.7.1
+Requires-Dist: shil>=2024.5.30.18.30
 Requires-Dist: shimport>=2023.7.11.23.36
-Requires-Dist: fleks==2024.4.5.9.29
+Requires-Dist: fleks==2024.5.10.23.48
 Requires-Dist: memoization==0.4.0
 Requires-Dist: multipledispatch==0.6.0
 Requires-Dist: pygments
 Requires-Dist: pyjson5==1.6.1
 Requires-Dist: marko==2.0.0
 Requires-Dist: pyyaml
 Requires-Dist: trogon
```

### Comparing `pynchon-2024.4.5.14.1/README.md` & `pynchon-2024.5.30.19.18/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 ---------------------------------------------------------------------------------
 
 ## Overview
 
 Pynchon is a library, tool, and extensible framework that helps with generating documentation, working with diagrams, rendering templates, and maybe other aspects of project management.  It's useful in general but has extra features for working with python projects, including helpers for code-transformation and autogenerating documentation.
 
-This code is still experimental and interface stability is not yet guaranteed.. make sure to pin pynchon at specific versions for your project.
+This code is still experimental and interface stability is not yet guaranteed.. make sure to pin pynchon at specific versions for your project. =)
 
 ---------------------------------------------------------------------------------
 
 ## Features
 
 * Terraform-style plan / apply workflows
 * Some support for parallel execution in applies
@@ -74,17 +74,17 @@
 
 ---------------------------------------------------------------------------------
 
 ## Quick Start
 
 ### Utility Invocation
 
-If you're more interested in tools than a framework, some functionality is available without completely loading pynchon.
+If you're more interested in tools than a framework, some functionality is available without completely loading pynchon.  Most things like that are available somewhere under [pynchon.util](src/pynchon/util), and they can be used with module-invocations like `python -mpynchon.util ...`.
 
-For this you can use module-invocations like `python -mpynchon.util.text ..`. For example:
+A few random examples:
 
 ```bash
 # Helpers for loading/converting config from many file formats:
 $ python -mpynchon.util.text loadf --help
 Usage: python -m pynchon.util.text loadf [OPTIONS] COMMAND [ARGS]...
 
   pynchon.util.text.loadf CLI
@@ -112,44 +112,58 @@
   --print              if set, displays result on stdout even when `--output
                        <file>` is passed
   --include TEXT       path to use for template-root / includes
   --context TEXT       context literal.  must be JSON
   --context-file TEXT  context file.  must be JSON
   --help               Show this message and exit.
 
+
+# Makefile parser.
+# Capable of pulling make-targets even across nested/included Makefiles
+$ python -mpynchon.util.makefile --help
+Usage: python -m pynchon.util.makefile [OPTIONS] COMMAND [ARGS]...
+
+  pynchon.util.makefile CLI
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  database  Get database for Makefile (This output comes from 'make...
+  parse     Parse Makefile to JSON.
+
 ```
 
 ### CLI, Plugins, & Config
 
-For most functionality, you'll want to use the main `pynchon` tool.  Here, that functionality is provided via plugins, where every plugin is a subcommand for the main CLI.  There are several plugins which are provided by default, and you can see the plugins in use with the following command:
+For most functionality, you'll want to use the main `pynchon` tool.  Functionality here is provided via plugins, where **every plugin is a subcommand for the main CLI**.  There are several plugins which are provided by default, and you can see the plugins in use with the following command:
 
 ```bash
 # Shows the default plugin list, with no pynchon config present
 $ pynchon plugins list
 [
   "git",
   "core",
-  "src",
-  "markdown",
   "github",
+  "src",
   "docs",
-  "json",
+  "markdown",
+  "render",
   "parse",
   "gen",
-  "render",
-  "project",
-  "globals",
   "python",
+  "globals",
+  "project",
   "jinja",
   "pattern"
 ]
 
 
-# Add mermaid plugin, which is non-default, using the command-line.
-# Note that this is still without any file-based config
+# Adds the mermaid plugin, which is non-default, using the command-line.
+# (Note that this is still without any file-based config)
 $ pynchon --plugins mermaid mermaid --help
 Usage: pynchon mermaid [OPTIONS] COMMAND [ARGS]...
 
   Finds & renders Mermaid diagram files
 
 Options:
   --help  Show this message and exit.
@@ -247,15 +261,15 @@
 * **jinja.template_includes:** *(optional typing.List[str])*
     * Where to find files for use with Jinja's `include` blocks
     * Value is **user-configurable**, with no default  
 * **jinja.vars:** *(optional typing.Dict[str, str])*
     * Extra variables for template rendering
     * Value is **user-configurable**, with no default  
 * **jinja.exclude_patterns:** *(optional )*
-    * File patterns to exclude from resource-listing 
+    * File patterns to exclude from resource-listing
     * Value is **just-in-time** 
 
 
 **Crucially, the jinja context also includes the entire pynchon configuration stack for all plugins,** i.e. the current output of `pynchon cfg`.  This gives it access to context provided by other plugins.  For example the `{{github.repo_url}}` variable can be used in templates, and will be rendered as expected whenever the [Github Plugin](#github-plugin) is present and ready.
 
 Here's a typical workflow:
 
@@ -270,14 +284,46 @@
 
 # Render every jinja template we can find.
 $ pynchon jinja apply
 ```
 
 ---------------------------------------------------------------------------------
 
+### Makefile Plugin
+
+```bash
+$ pynchon makefile --help
+Usage: pynchon makefile [OPTIONS] COMMAND [ARGS]...
+
+  Visualization and parsing tools for inspecting Makefiles
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  apply    Executes the plan for this plugin
+  cfg      Shows current config for this plugin
+  mermaid  Renders mermaid diagram for makefile targets
+  parse    Parse Makefile to JSON.
+  plan     Runs a plan for this plugin
+  render   Subcommands for rendering
+
+```
+
+ 
+* **makefile.apply_hooks:** *(optional typing.List[str])*
+    * Hooks to run before/after `apply` for this plugin
+    * Value is **user-configurable**, with no default  
+* **makefile.file:** *(optional )*
+    * (Missing docstring for property)
+    * Value is **just-in-time** 
+
+
+---------------------------------------------------------------------------------
+
 
 
 ### Dockerhub Plugin
 
 ```bash
 $ pynchon dockerhub --help
 Usage: pynchon dockerhub [OPTIONS] COMMAND [ARGS]...
@@ -341,30 +387,30 @@
 * **github.apply_hooks:** *(optional typing.List[str])*
     * Hooks to run before/after `apply` for this plugin
     * Value is **user-configurable**, with no default  
 * **github.enterprise:** *(optional <class 'bool'>)*
     * (No description provided)
     * Value is **user-configurable**, with no default  
 * **github.actions:** *(optional typing.List[typing.Dict])*
-    * Github Action information 
+    * Github Action information
     * Value is **just-in-time**  
 * **github.org_name:** *(typing.Optional[str])*
-    * Org name 
+    * Org name
     * Value is **just-in-time**  
 * **github.org_url:** *(typing.Optional[str])*
-    * Org URL 
+    * Org URL
     * Value is **just-in-time**  
 * **github.raw_url:** *(optional )*
-    * URL for serving raw content 
+    * URL for serving raw content
     * Value is **just-in-time**  
 * **github.repo_ssh_url:** *(typing.Optional[str])*
-    * Repository SSH URL 
+    * Repository SSH URL
     * Value is **just-in-time**  
 * **github.repo_url:** *(typing.Optional[str])*
-    * Repository URL 
+    * Repository URL
     * Value is **just-in-time** 
 
 
 ---------------------------------------------------------------------------------
 
 
 ### Git Plugin
@@ -389,36 +435,36 @@
 ```
 
  
 * **git.apply_hooks:** *(optional typing.List[str])*
     * Hooks to run before/after `apply` for this plugin
     * Value is **user-configurable**, with no default  
 * **git.branch_name:** *(typing.Optional[str])*
-    * Name of current branch 
+    * Name of current branch
     * Value is **just-in-time**  
 * **git.github_org:** *(typing.Optional[str])*
-    * Name of this github organization 
+    * Name of this github organization
     * Value is **just-in-time**  
 * **git.hash:** *(typing.Optional[str])*
-    * Current git hash 
+    * Current git hash
     * Value is **just-in-time**  
 * **git.is_github:** *(optional <class 'bool'>)*
-    * True if this is a github repository 
+    * True if this is a github repository
     * Value is **just-in-time**  
 * **git.repo:** *(typing.Optional[str])*
-    * Repo name for this git project 
+    * Repo name for this git project
     * Value is **just-in-time**  
 * **git.repo_name:** *(typing.Optional[str])*
-    * Repository name 
+    * Repository name
     * Value is **just-in-time**  
 * **git.repo_url:** *(typing.Optional[str])*
-    * Repository URL 
+    * Repository URL
     * Value is **just-in-time**  
 * **git.root:** *(typing.Optional[str])*
-    * Root path for this git project 
+    * Root path for this git project
     * Value is **just-in-time** 
 
 
 ---------------------------------------------------------------------------------
 
 
 ### Pypi Plugin
@@ -575,15 +621,18 @@
     * (No description provided)
     * Value is **user-configurable**, with default `pandoc/extra:latest`  
 * **pandoc.docker_args:** *(optional typing.List)*
     * (No description provided)
     * Value is **user-configurable**, with default `['--toc', '--variable fontsize=10pt']`  
 * **pandoc.goals:** *(optional typing.List[typing.Dict])*
     * (No description provided)
-    * Value is **user-configurable**, with no default 
+    * Value is **user-configurable**, with no default  
+* **pandoc.service_name:** *(optional <class 'str'>)*
+    * (No description provided)
+    * Value is **user-configurable**, with default `pandoc` 
 
 
 ---------------------------------------------------------------------------------
 
 
 ### Drawio Plugin
 
@@ -595,21 +644,22 @@
 
 Options:
   --help  Show this message and exit.
 
 Commands:
   apply   Executes the plan for this plugin
   cfg     Shows current config for this plugin
-  export  Exports a given .drawio file to some output file/format...
   list    Lists affected resources (*.drawio files) for this project
   ls      (alias for `ls`)
   open    Opens a browser for the container started by `serve`
   plan    Creates a plan for this plugin
+  render  Exports a given .drawio file to some output file/format...
   run     Passes given command through to docker-image this plugin wraps
   serve   Runs the drawio-UI in a docker-container
+  stop    Stop DrawIO server
 
 ```
 
  
 * **drawio.apply_hooks:** *(optional typing.List[str])*
     * Hooks to run before/after `apply` for this plugin
     * Value is **user-configurable**, with no default  
@@ -620,24 +670,27 @@
     * (No description provided)
     * Value is **user-configurable**, with default `jgraph/drawio`  
 * **drawio.http_port:** *(optional <class 'str'>)*
     * (No description provided)
     * Value is **user-configurable**, with default `8080`  
 * **drawio.docker_args:** *(optional typing.List)*
     * (No description provided)
-    * Value is **user-configurable**, with default `['-it --rm --name=drawio-server']`  
+    * Value is **user-configurable**, with default `['--rm --name=drawio-server']`  
 * **drawio.export_docker_image:** *(optional <class 'str'>)*
     * (No description provided)
     * Value is **user-configurable**, with default `rlespinasse/drawio-desktop-headless`  
+* **drawio.format:** *(optional <class 'str'>)*
+    * (No description provided)
+    * Value is **user-configurable**, with default `png`  
 * **drawio.export_width:** *(optional <class 'int'>)*
     * (No description provided)
     * Value is **user-configurable**, with default `800`  
 * **drawio.export_args:** *(optional typing.List)*
     * (No description provided)
-    * Value is **user-configurable**, with default `['--export', '--embed-svg-images', '--embed-diagram', '--svg-theme light']` 
+    * Value is **user-configurable**, with default `['--export', '--border 10', '--crop', '--transparent']` 
 
 
 ---------------------------------------------------------------------------------
 
 
 ### Dot Plugin
 
@@ -694,104 +747,44 @@
 
 ```
 
  
 * **mkdocs.apply_hooks:** *(optional typing.List[str])*
     * Hooks to run before/after `apply` for this plugin
     * Value is **user-configurable**, with no default  
-* **mkdocs.blog_posts:** *(optional <class 'list'>)*
+* **mkdocs.blog_posts:** *(optional typing.List)*
     * returns blog posts, iff blogging plugin is installed.
         resulting files, if any, will not include index and
         will be sorted by modification time
         
     * Value is **just-in-time**  
 * **mkdocs.config:** *(optional typing.Dict)*
     * returns a dictionary with the current mkdocs configuration
         
     * Value is **just-in-time**  
 * **mkdocs.config_file:** *(typing.Optional[str])*
     * returns the path to the mkdocs config-file, if applicable
     * Value is **just-in-time**  
-* **mkdocs.drafts:** *(optional )*
+* **mkdocs.drafts:** *(optional typing.List)*
     * (Missing docstring for property)
     * Value is **just-in-time**  
 * **mkdocs.pages:** *(optional typing.List)*
     * 
     * Value is **just-in-time**  
-* **mkdocs.site_relative_url:** *(optional )*
-    * (Missing docstring for property)
+* **mkdocs.site_relative_url:** *(optional <class 'str'>)*
+    * 
     * Value is **just-in-time**  
 * **mkdocs.tags:** *(optional typing.List)*
     * 
     * Value is **just-in-time** 
 
 
 ---------------------------------------------------------------------------------
 
 
-### Json Plugin
-
-```bash
-$ pynchon json --help
-Usage: pynchon json [OPTIONS] COMMAND [ARGS]...
-
-  Tools for working with JSON & JSON5
-
-Options:
-  --help  Show this message and exit.
-
-Commands:
-  apply  Executes the plan for this plugin
-  cfg    Shows current config for this plugin
-  plan   Creates a plan for this plugin
-
-```
-
- 
-* **json.apply_hooks:** *(optional typing.List[str])*
-    * Hooks to run before/after `apply` for this plugin
-    * Value is **user-configurable**, with no default 
-
-
----------------------------------------------------------------------------------
-
-
-### Makefile Plugin
-
-```bash
-$ pynchon makefile --help
-Usage: pynchon makefile [OPTIONS] COMMAND [ARGS]...
-
-  Visualization and parsing tools for inspecting Makefiles
-
-Options:
-  --help  Show this message and exit.
-
-Commands:
-  apply    Executes the plan for this plugin
-  cfg      Shows current config for this plugin
-  mermaid  Renders mermaid diagram for makefile targets
-  parse    Parse Makefile to JSON.
-  plan     Runs a plan for this plugin
-  render   Subcommands for rendering
-
-```
-
- 
-* **makefile.apply_hooks:** *(optional typing.List[str])*
-    * Hooks to run before/after `apply` for this plugin
-    * Value is **user-configurable**, with no default  
-* **makefile.file:** *(optional )*
-    * (Missing docstring for property)
-    * Value is **just-in-time** 
-
-
----------------------------------------------------------------------------------
-
-
 ### Parse Plugin
 
 ```bash
 $ pynchon parse --help
 Usage: pynchon parse [OPTIONS] COMMAND [ARGS]...
 
   Misc tools for parsing
```

#### html2text {}

```diff
@@ -15,72 +15,78 @@
 -------------------------------------------------------------------------------
 -- ## Overview Pynchon is a library, tool, and extensible framework that helps
 with generating documentation, working with diagrams, rendering templates, and
 maybe other aspects of project management. It's useful in general but has extra
 features for working with python projects, including helpers for code-
 transformation and autogenerating documentation. This code is still
 experimental and interface stability is not yet guaranteed.. make sure to pin
-pynchon at specific versions for your project. --------------------------------
-------------------------------------------------- ## Features * Terraform-style
-plan / apply workflows * Some support for parallel execution in applies * Tight
-integration with [Jinja](#) for rendering templates * Plugin framework for
-extensions * Plugins have config * Helpers for parsing Markdown, INI, JSON,
+pynchon at specific versions for your project. =) -----------------------------
+---------------------------------------------------- ## Features * Terraform-
+style plan / apply workflows * Some support for parallel execution in applies *
+Tight integration with [Jinja](#) for rendering templates * Plugin framework
+for extensions * Plugins have config * Helpers for parsing Markdown, INI, JSON,
 JSON5 and TOML * Support for diagramming tools like [Mermaid](#mermaid-plugin),
 [DrawIO](#drawio-plugin), & [pandoc](#pandoc-plugin) * Friendly output for
 machines and for humans -------------------------------------------------------
 -------------------------- ## Installation Pynchon is on PyPI, so to get the
 latest: ```bash pip install pynchon ``` Or, for developers: ```bash # for ssh
 git clone git@github.com:elo-enterprises/pynchon.git # or for http # git clone
 https://github.com/elo-enterprises/pynchon cd pynchon pip install -e . ``` ----
 ----------------------------------------------------------------------------
 - ## Quick Start ### Utility Invocation If you're more interested in tools than
 a framework, some functionality is available without completely loading
-pynchon. For this you can use module-invocations like `python -
-mpynchon.util.text ..`. For example: ```bash # Helpers for loading/converting
-config from many file formats: $ python -mpynchon.util.text loadf --help Usage:
-python -m pynchon.util.text loadf [OPTIONS] COMMAND [ARGS]...
+pynchon. Most things like that are available somewhere under [pynchon.util]
+(src/pynchon/util), and they can be used with module-invocations like `python -
+mpynchon.util ...`. A few random examples: ```bash # Helpers for loading/
+converting config from many file formats: $ python -mpynchon.util.text loadf --
+help Usage: python -m pynchon.util.text loadf [OPTIONS] COMMAND [ARGS]...
 pynchon.util.text.loadf CLI Options: --help Show this message and exit.
 Commands: ini Parses ini file and returns JSON :param file: json loads json to
 python dictionary from given file or string :param... json5 Parses JSON-5 file
 (s) and outputs json. loadf toml Parses toml file and returns JSON :param file:
 str: (Default... yaml parses yaml file and returns JSON :param *args: :param
 **kwargs: # Helpers for rendering Jinja templates $ python -mpynchon.util.text
 render jinja --help Usage: python -m pynchon.util.text render jinja [OPTIONS]
 FILE Alias for `jinja_file` Options: -o, --output TEXT output file to write.
 (optional) --print if set, displays result on stdout even when `--output ` is
 passed --include TEXT path to use for template-root / includes --context TEXT
 context literal. must be JSON --context-file TEXT context file. must be JSON --
-help Show this message and exit. ``` ### CLI, Plugins, & Config For most
-functionality, you'll want to use the main `pynchon` tool. Here, that
-functionality is provided via plugins, where every plugin is a subcommand for
-the main CLI. There are several plugins which are provided by default, and you
-can see the plugins in use with the following command: ```bash # Shows the
-default plugin list, with no pynchon config present $ pynchon plugins list
-[ "git", "core", "src", "markdown", "github", "docs", "json", "parse", "gen",
-"render", "project", "globals", "python", "jinja", "pattern" ] # Add mermaid
-plugin, which is non-default, using the command-line. # Note that this is still
-without any file-based config $ pynchon --plugins mermaid mermaid --help Usage:
-pynchon mermaid [OPTIONS] COMMAND [ARGS]... Finds & renders Mermaid diagram
-files Options: --help Show this message and exit. Commands: cfg Shows current
-config for this plugin list Find mermaid diagrams under `{{project_root}}/**/
-*.mmd` ls (alias for `ls`) plan Run planning for this plugin render Renders
-mermaid diagram to image run Passes given command through to docker-image this
-plugin wraps ``` To get started with file-based config, run `pynchon init` in
-your project folder to create `.pynchon.json5`. From here you can modify
-`pynchon.plugins` to use a custom set of plugins, and configure the plugins as
-well. Every plugin has config, which can be overriden, which may include
-defaults, or which is dynamically determined from the current context. To show
-current plugin config, you can always use `pynchon cfg`. Below are some
-examples with the `github` plugin (see the [Github Plugin docs](#github-plugin)
-for more information about this plugin in particular.) ```bash # Outside of a
-github repository, # config is empty and not very interesting $ pynchon github
-cfg { "enterprise": false, "actions": [], "org_name": null, "org_url": null,
-"raw_url": null, "repo_ssh_url": null, "repo_url": null } # Inside of a github
-repository, # lots of useful information $ pynchon github cfg { "enterprise":
-false, "actions": [ ... ], "org_name": "elo-enterprises", "org_url": "https://
+help Show this message and exit. # Makefile parser. # Capable of pulling make-
+targets even across nested/included Makefiles $ python -mpynchon.util.makefile
+--help Usage: python -m pynchon.util.makefile [OPTIONS] COMMAND [ARGS]...
+pynchon.util.makefile CLI Options: --help Show this message and exit. Commands:
+database Get database for Makefile (This output comes from 'make... parse Parse
+Makefile to JSON. ``` ### CLI, Plugins, & Config For most functionality, you'll
+want to use the main `pynchon` tool. Functionality here is provided via
+plugins, where **every plugin is a subcommand for the main CLI**. There are
+several plugins which are provided by default, and you can see the plugins in
+use with the following command: ```bash # Shows the default plugin list, with
+no pynchon config present $ pynchon plugins list [ "git", "core", "github",
+"src", "docs", "markdown", "render", "parse", "gen", "python", "globals",
+"project", "jinja", "pattern" ] # Adds the mermaid plugin, which is non-
+default, using the command-line. # (Note that this is still without any file-
+based config) $ pynchon --plugins mermaid mermaid --help Usage: pynchon mermaid
+[OPTIONS] COMMAND [ARGS]... Finds & renders Mermaid diagram files Options: --
+help Show this message and exit. Commands: cfg Shows current config for this
+plugin list Find mermaid diagrams under `{{project_root}}/**/*.mmd` ls (alias
+for `ls`) plan Run planning for this plugin render Renders mermaid diagram to
+image run Passes given command through to docker-image this plugin wraps ``` To
+get started with file-based config, run `pynchon init` in your project folder
+to create `.pynchon.json5`. From here you can modify `pynchon.plugins` to use a
+custom set of plugins, and configure the plugins as well. Every plugin has
+config, which can be overriden, which may include defaults, or which is
+dynamically determined from the current context. To show current plugin config,
+you can always use `pynchon cfg`. Below are some examples with the `github`
+plugin (see the [Github Plugin docs](#github-plugin) for more information about
+this plugin in particular.) ```bash # Outside of a github repository, # config
+is empty and not very interesting $ pynchon github cfg { "enterprise": false,
+"actions": [], "org_name": null, "org_url": null, "raw_url": null,
+"repo_ssh_url": null, "repo_url": null } # Inside of a github repository, #
+lots of useful information $ pynchon github cfg { "enterprise": false,
+"actions": [ ... ], "org_name": "elo-enterprises", "org_url": "https://
 github.com/elo-enterprises", "raw_url": "https://raw.githubusercontent.com/elo-
 enterprises/pynchon", "repo_ssh_url": "git@github.com:elo-enterprises/
 pynchon.git", "repo_url": "https://github.com/elo-enterprises/pynchon" } ```
 You can see the the configuration schema for any given plugin like this:
 ```bash # default output is JSON schema $ pynchon plugin schema github
 { "title": "github", "type": "object", "properties": { "apply_hooks":
 { "title": "Apply Hooks", "description": "Hooks to run before/after `apply` for
@@ -110,18 +116,28 @@
 expected whenever the [Github Plugin](#github-plugin) is present and ready.
 Here's a typical workflow: ```bash # find *.j2 files under the project
 directory $ pynchon jinja list # make a plan to render every file that was
 returned by `list` above. # this will use the jinja plugin config in
 `.pynchon.json5` to determine # appropriate calls to `pynchon jinja render ...`
 $ pynchon jinja plan # Render every jinja template we can find. $ pynchon jinja
 apply ``` ---------------------------------------------------------------------
------------- ### Dockerhub Plugin ```bash $ pynchon dockerhub --help Usage:
-pynchon dockerhub [OPTIONS] COMMAND [ARGS]... Context for Dockerhub Options: --
-help Show this message and exit. Commands: cfg Shows current config for this
-plugin open Open this dockerhub project's webpage ``` *
+------------ ### Makefile Plugin ```bash $ pynchon makefile --help Usage:
+pynchon makefile [OPTIONS] COMMAND [ARGS]... Visualization and parsing tools
+for inspecting Makefiles Options: --help Show this message and exit. Commands:
+apply Executes the plan for this plugin cfg Shows current config for this
+plugin mermaid Renders mermaid diagram for makefile targets parse Parse
+Makefile to JSON. plan Runs a plan for this plugin render Subcommands for
+rendering ``` * **makefile.apply_hooks:** *(optional typing.List[str])* * Hooks
+to run before/after `apply` for this plugin * Value is **user-configurable**,
+with no default * **makefile.file:** *(optional )* * (Missing docstring for
+property) * Value is **just-in-time** -----------------------------------------
+---------------------------------------- ### Dockerhub Plugin ```bash $ pynchon
+dockerhub --help Usage: pynchon dockerhub [OPTIONS] COMMAND [ARGS]... Context
+for Dockerhub Options: --help Show this message and exit. Commands: cfg Shows
+current config for this plugin open Open this dockerhub project's webpage ``` *
 **dockerhub.apply_hooks:** *(optional typing.List[str])* * Hooks to run before/
 after `apply` for this plugin * Value is **user-configurable**, with no default
 * **dockerhub.org_name:** *(typing.Optional[str])* * (No description provided)
 * Value is **user-configurable**, with no default * **dockerhub.repo_name:** *
 (typing.Optional[str])* * (No description provided) * Value is **user-
 configurable**, with no default * **dockerhub.org_url:** *(optional
 str'>)* * (Missing docstring for property) * Value is **just-in-time** *
@@ -229,106 +245,92 @@
 [str])* * Hooks to run before/after `apply` for this plugin * Value is **user-
 configurable**, with no default * **pandoc.docker_image:** *(optional
 str'>)* * (No description provided) * Value is **user-configurable**, with
 default `pandoc/extra:latest` * **pandoc.docker_args:** *(optional
 typing.List)* * (No description provided) * Value is **user-configurable**,
 with default `['--toc', '--variable fontsize=10pt']` * **pandoc.goals:** *
 (optional typing.List[typing.Dict])* * (No description provided) * Value is
-**user-configurable**, with no default ----------------------------------------
------------------------------------------ ### Drawio Plugin ```bash $ pynchon
-drawio --help Usage: pynchon drawio [OPTIONS] COMMAND [ARGS]... Wrapper for
-docker-containers that provide the "drawio" diagramming utility Options: --help
-Show this message and exit. Commands: apply Executes the plan for this plugin
-cfg Shows current config for this plugin export Exports a given .drawio file to
-some output file/format... list Lists affected resources (*.drawio files) for
-this project ls (alias for `ls`) open Opens a browser for the container started
-by `serve` plan Creates a plan for this plugin run Passes given command through
-to docker-image this plugin wraps serve Runs the drawio-UI in a docker-
-container ``` * **drawio.apply_hooks:** *(optional typing.List[str])* * Hooks
-to run before/after `apply` for this plugin * Value is **user-configurable**,
-with no default * **drawio.file_glob:** *(optional
+**user-configurable**, with no default * **pandoc.service_name:** *(optional
+str'>)* * (No description provided) * Value is **user-configurable**, with
+default `pandoc` --------------------------------------------------------------
+------------------- ### Drawio Plugin ```bash $ pynchon drawio --help Usage:
+pynchon drawio [OPTIONS] COMMAND [ARGS]... Wrapper for docker-containers that
+provide the "drawio" diagramming utility Options: --help Show this message and
+exit. Commands: apply Executes the plan for this plugin cfg Shows current
+config for this plugin list Lists affected resources (*.drawio files) for this
+project ls (alias for `ls`) open Opens a browser for the container started by
+`serve` plan Creates a plan for this plugin render Exports a given .drawio file
+to some output file/format... run Passes given command through to docker-image
+this plugin wraps serve Runs the drawio-UI in a docker-container stop Stop
+DrawIO server ``` * **drawio.apply_hooks:** *(optional typing.List[str])* *
+Hooks to run before/after `apply` for this plugin * Value is **user-
+configurable**, with no default * **drawio.file_glob:** *(optional
 str'>)* * Where to find jinja templates * Value is **user-configurable**, with
 default `*.drawio` * **drawio.docker_image:** *(optional
 str'>)* * (No description provided) * Value is **user-configurable**, with
 default `jgraph/drawio` * **drawio.http_port:** *(optional
 str'>)* * (No description provided) * Value is **user-configurable**, with
 default `8080` * **drawio.docker_args:** *(optional typing.List)* * (No
-description provided) * Value is **user-configurable**, with default `['-it --
-rm --name=drawio-server']` * **drawio.export_docker_image:** *(optional
+description provided) * Value is **user-configurable**, with default `['--rm --
+name=drawio-server']` * **drawio.export_docker_image:** *(optional
 str'>)* * (No description provided) * Value is **user-configurable**, with
-default `rlespinasse/drawio-desktop-headless` * **drawio.export_width:** *
-(optional
+default `rlespinasse/drawio-desktop-headless` * **drawio.format:** *(optional
+str'>)* * (No description provided) * Value is **user-configurable**, with
+default `png` * **drawio.export_width:** *(optional
 int'>)* * (No description provided) * Value is **user-configurable**, with
 default `800` * **drawio.export_args:** *(optional typing.List)* * (No
 description provided) * Value is **user-configurable**, with default `['--
-export', '--embed-svg-images', '--embed-diagram', '--svg-theme light']` -------
--------------------------------------------------------------------------- ###
-Dot Plugin ```bash $ pynchon dot --help Usage: pynchon dot [OPTIONS] COMMAND
-[ARGS]... Finds / Renders (graphviz) dot files for this project Options: --help
-Show this message and exit. Commands: apply Executes the plan for this plugin
-cfg Shows current config for this plugin list plan render run Passes given
-command through to docker-image this plugin wraps ``` * **dot.apply_hooks:** *
-(optional typing.List[str])* * Hooks to run before/after `apply` for this
-plugin * Value is **user-configurable**, with no default *
-**dot.exclude_patterns:** *(optional typing.List[str])* * (No description
-provided) * Value is **user-configurable**, with no default -------------------
--------------------------------------------------------------- ### Mkdocs
-Plugin ```bash $ pynchon mkdocs --help Usage: pynchon mkdocs [OPTIONS] COMMAND
-[ARGS]... Mkdocs helper Options: --help Show this message and exit. Commands:
-apply Executes the plan for this plugin cfg Shows current config for this
-plugin list Lists site-pages based on mkdocs.yml ls (alias for `ls`) open Opens
-`dev_addr` in a webbrowser plan Runs a plan for this plugin serve Wrapper for
-`mkdocs serve` ``` * **mkdocs.apply_hooks:** *(optional typing.List[str])* *
-Hooks to run before/after `apply` for this plugin * Value is **user-
-configurable**, with no default * **mkdocs.blog_posts:** *(optional
-list'>)* * returns blog posts, iff blogging plugin is installed. resulting
-files, if any, will not include index and will be sorted by modification time *
-Value is **just-in-time** * **mkdocs.config:** *(optional typing.Dict)* *
-returns a dictionary with the current mkdocs configuration * Value is **just-
-in-time** * **mkdocs.config_file:** *(typing.Optional[str])* * returns the path
-to the mkdocs config-file, if applicable * Value is **just-in-time** *
-**mkdocs.drafts:** *(optional )* * (Missing docstring for property) * Value is
-**just-in-time** * **mkdocs.pages:** *(optional typing.List)* * * Value is
-**just-in-time** * **mkdocs.site_relative_url:** *(optional )* * (Missing
-docstring for property) * Value is **just-in-time** * **mkdocs.tags:** *
-(optional typing.List)* * * Value is **just-in-time** -------------------------
--------------------------------------------------------- ### Json Plugin
-```bash $ pynchon json --help Usage: pynchon json [OPTIONS] COMMAND [ARGS]...
-Tools for working with JSON & JSON5 Options: --help Show this message and exit.
-Commands: apply Executes the plan for this plugin cfg Shows current config for
-this plugin plan Creates a plan for this plugin ``` * **json.apply_hooks:** *
-(optional typing.List[str])* * Hooks to run before/after `apply` for this
-plugin * Value is **user-configurable**, with no default ----------------------
------------------------------------------------------------ ### Makefile Plugin
-```bash $ pynchon makefile --help Usage: pynchon makefile [OPTIONS] COMMAND
-[ARGS]... Visualization and parsing tools for inspecting Makefiles Options: --
-help Show this message and exit. Commands: apply Executes the plan for this
-plugin cfg Shows current config for this plugin mermaid Renders mermaid diagram
-for makefile targets parse Parse Makefile to JSON. plan Runs a plan for this
-plugin render Subcommands for rendering ``` * **makefile.apply_hooks:** *
-(optional typing.List[str])* * Hooks to run before/after `apply` for this
-plugin * Value is **user-configurable**, with no default * **makefile.file:** *
-(optional )* * (Missing docstring for property) * Value is **just-in-time** ---
------------------------------------------------------------------------------
-- ### Parse Plugin ```bash $ pynchon parse --help Usage: pynchon parse
-[OPTIONS] COMMAND [ARGS]... Misc tools for parsing Options: --help Show this
-message and exit. Commands: cfg Shows current config for this plugin makefile
-(Alias for `pynchon makefile parse`) markdown (Alias for `pynchon markdown
-parse`) ``` * **parse.apply_hooks:** *(optional typing.List[str])* * Hooks to
-run before/after `apply` for this plugin * Value is **user-configurable**, with
-no default --------------------------------------------------------------------
-------------- ### Src Plugin ```bash $ pynchon src --help Usage: pynchon src
-[OPTIONS] COMMAND [ARGS]... Management tool for project source Options: --help
-Show this message and exit. Commands: apply Executes the plan for this plugin
-cfg Shows current config for this plugin changed opens changed files list Lists
-resources associated with this plugin list-modified Lists modified files list-
-transforms (Alias for `pynchon python-libcst list-transforms`) ls (alias for
-`ls`) open Helper for opening project source files plan Describe plan for this
-plugin recent Opens recently changed files sorted (Alias for `pynchon python
-sorted`) transform (Alias for `pynchon python-libcst run-transform`) ``` *
+export', '--border 10', '--crop', '--transparent']` ---------------------------
+------------------------------------------------------ ### Dot Plugin ```bash $
+pynchon dot --help Usage: pynchon dot [OPTIONS] COMMAND [ARGS]... Finds /
+Renders (graphviz) dot files for this project Options: --help Show this message
+and exit. Commands: apply Executes the plan for this plugin cfg Shows current
+config for this plugin list plan render run Passes given command through to
+docker-image this plugin wraps ``` * **dot.apply_hooks:** *(optional
+typing.List[str])* * Hooks to run before/after `apply` for this plugin * Value
+is **user-configurable**, with no default * **dot.exclude_patterns:** *
+(optional typing.List[str])* * (No description provided) * Value is **user-
+configurable**, with no default -----------------------------------------------
+---------------------------------- ### Mkdocs Plugin ```bash $ pynchon mkdocs -
+-help Usage: pynchon mkdocs [OPTIONS] COMMAND [ARGS]... Mkdocs helper Options:
+--help Show this message and exit. Commands: apply Executes the plan for this
+plugin cfg Shows current config for this plugin list Lists site-pages based on
+mkdocs.yml ls (alias for `ls`) open Opens `dev_addr` in a webbrowser plan Runs
+a plan for this plugin serve Wrapper for `mkdocs serve` ``` *
+**mkdocs.apply_hooks:** *(optional typing.List[str])* * Hooks to run before/
+after `apply` for this plugin * Value is **user-configurable**, with no default
+* **mkdocs.blog_posts:** *(optional typing.List)* * returns blog posts, iff
+blogging plugin is installed. resulting files, if any, will not include index
+and will be sorted by modification time * Value is **just-in-time** *
+**mkdocs.config:** *(optional typing.Dict)* * returns a dictionary with the
+current mkdocs configuration * Value is **just-in-time** *
+**mkdocs.config_file:** *(typing.Optional[str])* * returns the path to the
+mkdocs config-file, if applicable * Value is **just-in-time** *
+**mkdocs.drafts:** *(optional typing.List)* * (Missing docstring for property)
+* Value is **just-in-time** * **mkdocs.pages:** *(optional typing.List)* * *
+Value is **just-in-time** * **mkdocs.site_relative_url:** *(optional
+str'>)* * * Value is **just-in-time** * **mkdocs.tags:** *(optional
+typing.List)* * * Value is **just-in-time** -----------------------------------
+---------------------------------------------- ### Parse Plugin ```bash $
+pynchon parse --help Usage: pynchon parse [OPTIONS] COMMAND [ARGS]... Misc
+tools for parsing Options: --help Show this message and exit. Commands: cfg
+Shows current config for this plugin makefile (Alias for `pynchon makefile
+parse`) markdown (Alias for `pynchon markdown parse`) ``` *
+**parse.apply_hooks:** *(optional typing.List[str])* * Hooks to run before/
+after `apply` for this plugin * Value is **user-configurable**, with no default
+-------------------------------------------------------------------------------
+-- ### Src Plugin ```bash $ pynchon src --help Usage: pynchon src [OPTIONS]
+COMMAND [ARGS]... Management tool for project source Options: --help Show this
+message and exit. Commands: apply Executes the plan for this plugin cfg Shows
+current config for this plugin changed opens changed files list Lists resources
+associated with this plugin list-modified Lists modified files list-transforms
+(Alias for `pynchon python-libcst list-transforms`) ls (alias for `ls`) open
+Helper for opening project source files plan Describe plan for this plugin
+recent Opens recently changed files sorted (Alias for `pynchon python sorted`)
+transform (Alias for `pynchon python-libcst run-transform`) ``` *
 **src.apply_hooks:** *(optional typing.List[str])* * Hooks to run before/after
 `apply` for this plugin * Value is **user-configurable**, with no default *
 **src.goals:** *(optional typing.List[str])* * (No description provided) *
 Value is **user-configurable**, with no default * **src.include_patterns:** *
 (optional typing.List[str])* * (No description provided) * Value is **user-
 configurable**, with no default * **src.exclude_patterns:** *(optional
 typing.List[str])* * (No description provided) * Value is **user-
```

### Comparing `pynchon-2024.4.5.14.1/pyproject.toml` & `pynchon-2024.5.30.19.18/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/setup.cfg` & `pynchon-2024.5.30.19.18/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 python_requires = >3.6
 install_requires = 
 	gripe>=2024.2.24.1.31
-	shil>=2023.7.17.7.1
+	shil>=2024.5.30.18.30
 	shimport>=2023.7.11.23.36
-	fleks==2024.4.5.9.29
+	fleks==2024.5.10.23.48
 	memoization==0.4.0
 	multipledispatch==0.6.0
 	
 	pygments
 	pyjson5==1.6.1
 	marko==2.0.0     # parsing markdown
 	pyyaml           # parsing yaml
```

### Comparing `pynchon-2024.4.5.14.1/setup.py` & `pynchon-2024.5.30.19.18/setup.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/abcs/__init__.py` & `pynchon-2024.5.30.19.18/src/pynchon/abcs/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/abcs/attrdict.py` & `pynchon-2024.5.30.19.18/src/pynchon/abcs/attrdict.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/abcs/path.py` & `pynchon-2024.5.30.19.18/src/pynchon/abcs/path.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/abcs/visitor.py` & `pynchon-2024.5.30.19.18/src/pynchon/abcs/visitor.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/annotate.py` & `pynchon-2024.5.30.19.18/src/pynchon/annotate.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/api/project/__init__.py` & `pynchon-2024.5.30.19.18/src/pynchon/api/project/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/api/render.py` & `pynchon-2024.5.30.19.18/src/pynchon/api/render.py`

 * *Files 13% similar despite different names*

```diff
@@ -59,51 +59,69 @@
 
     def invoke_helper(*args, **kwargs) -> typing.StringMaybe:
         """A jinja filter/extension"""
         strict = kwargs.pop("strict", True)
         out = invoke(*args, **kwargs)
         if not out.succeeded:
             raise Exception(out)
-        return out.stdout
+        if kwargs.get("load_json", False):
+            return out.data
+        else:
+            return out.stdout
 
-    def markdown_toc(fname: str, level=None):
-        """ """
+    def markdown_toc(fname: str, level: int = None, skip: list = []) -> str:
+        """returns a TOC for the given markdown file, wrapped inside a simple <ul>"""
         import markdown
 
         with open(fname) as fhandle:
             contents = fhandle.read()
         md = markdown.Markdown(
             extensions=["toc", "fenced_code"],
             extension_configs={"toc": {"toc_depth": level}},
         )
+        contents = contents.split("\n")
+        oskip = [s.strip().lstrip().lower() for s in skip]
+        skip = (
+            ["# " + s for s in oskip]
+            + ["## " + s for s in oskip]
+            + ["### " + s for s in oskip]
+        )
+        contents = [
+            line for line in contents if not line.lstrip().strip().lower() in skip
+        ]
+        contents = "\n".join(contents)
         html = md.convert(contents)
         return md.toc
 
-    # markdown-toc --type github  --no-write docs/blog/ambient-calculus-1.md
-    # assert fname
-    # fname = abcs.Path(fname)
-    # assert fname.exists()
-    # # script = abcs.Path(pynchon.__file__).parents[0] / "scripts" / "gh-md-toc.sh"
-    # result = invoke(
-    #     f"markdown-toc --type github --no-write {fname}",
-    #     command_logger=LOGGER.critical
-    # )
-    # assert result.succeeded
-    # return result.stdout
+    def md2latex(inp, fname=".tmp.md2latex.md"):
+        with open(fname, "w") as fhandle:
+            fhandle.write(inp)
+        invoke(f"pandoc {fname} -t latex -o {fname}.tex", strict=True)
+        with open(f"{fname}.tex") as fhandle:
+            return fhandle.read()
+
+    def strip_ansi_codes(s):
+        import re
+
+        return re.sub(r"\x1b\[([0-9,A-Z]{1,2}(;[0-9]{1,2})?(;[0-9]{3})?)?[m|K]?", "", s)
+
     return dict(
         str=str,
+        strip_ansi_codes=strip_ansi_codes,
         sh=invoke_helper,
         bash=invoke_helper,
+        open=open,
         is_markdown_list_item=is_markdown_list_item,
         invoke=invoke_helper,
         map=map,
         markdown_toc=markdown_toc,
         eval=eval,
         env=os.getenv,
         filter=filter,
+        md2latex=md2latex,
     )
 
 
 def get_jinja_includes(*includes):
     """ """
     includes = list(includes)
     includes += list(constants.PYNCHON_CORE_INCLUDES_DIRS)
@@ -136,15 +154,15 @@
         return template.render()
 
     env.filters["include"] = include_template
 
     env.filters.update(**get_jinja_filters())
     env.pynchon_includes = includes
 
-    env.globals.update(**get_jinja_globals())
+    env.globals.update(include=include_template, **get_jinja_globals())
 
     known_templates = list(map(abcs.Path, set(env.loader.list_templates())))
 
     if known_templates:
         from pynchon.util import text as util_text
 
         msg = "Known template search paths (includes folders only): "
```

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/app.py` & `pynchon-2024.5.30.19.18/src/pynchon/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,42 +29,56 @@
     # docs = manager.term.link(
     #     'https://python-enlighten.readthedocs.io/en/stable/examples.html',
     #     'Read the Docs')
 
     def __init__(self, **kwargs):
         """ """
         self.console = Console()
+        self.init_rich_tracebacks()
+
+    @classmethod
+    def init_rich_tracebacks(kls):
+        from rich import traceback
+
+        traceback.install(show_locals=True, indent_guides=True)
 
     # # FIXME: use multi-dispatch over kwargs and define `lifecyle` repeatedly
     # def lifecycle_stage(self, sender, stage=None, **kwargs):
     #     """ """
     #     if stage:
     #         tmp = getattr(sender, '__name__', str(sender))
     #         # LOGGER.critical(f"STAGE ({tmp}): {stage}")
     #         self.status_bar.update(stage=stage)
 
     @memoized_property
     def status_bar(self):
         """ """
-        tmp = self.manager.status_bar(
-            status_format="{app}{fill}{stage}{fill}{elapsed}",
-            color="bold_underline_bright_white_on_lightslategray",
-            justify=enlighten.Justify.LEFT,
-            app="Pynchon",
-            stage="...",
-            autorefresh=True,
-            min_delta=0.1,
-        )
-
-        # atexit.register(
-        #     lambda: self.events.lifecycle.send(
-        #         self, stage=r"\o/" if not self.exc else "❌", msg=""
-        #     )
-        # )  # noqa: W605
-        return tmp
+        from fleks.util import lme
+
+        if lme.COLOR_SYSTEM is not None:
+            tmp = self.manager.status_bar(
+                status_format="{app}{fill}{stage}{fill}{elapsed}",
+                color="bold_underline_bright_white_on_lightslategray",
+                justify=enlighten.Justify.LEFT,
+                app="Pynchon",
+                stage="...",
+                autorefresh=True,
+                min_delta=0.1,
+            )
+            # atexit.register(
+            #     lambda: self.events.lifecycle.send(
+            #         self, stage=r"\o/" if not self.exc else "❌", msg=""
+            #     )
+            # )  # noqa: W605
+            return tmp
+        else:
+            LOGGER.warning(
+                f"COLOR_SYSTEM={lme.COLOR_SYSTEM}, skipping attachment of status bar"
+            )
+            return {}
 
     #
     # @memoized_property
     # def lifecycle_bar(self):
     #     """ """
     #     tmp = self.manager.status_bar(
     #         status_format=u'{fill}{msg}{fill}',
```

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/bin.py` & `pynchon-2024.5.30.19.18/src/pynchon/bin.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         from pynchon import bin
 
         return bin.default
 
 
 @tui()
 @click.version_option()
-@click.option("--plugins", help="shortcut for `--set plugins=...`")
+@click.option("--plugins", "-p", help="shortcut for `--set plugins=...`")
 @click.option("--set", "set_config", help="config overrides")
 @click.option("--get", "get_config", help="config retrieval")
 @click.group(
     "pynchon",
     cls=RootGroup,
 )
 def entry(
```

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/cli/common.py` & `pynchon-2024.5.30.19.18/src/pynchon/cli/common.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/codemod/commands/docstrings/base.py` & `pynchon-2024.5.30.19.18/src/pynchon/codemod/commands/docstrings/base.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/codemod/commands/docstrings/javadoc.py` & `pynchon-2024.5.30.19.18/src/pynchon/codemod/commands/docstrings/javadoc.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/codemod/commands/docstrings/simple.py` & `pynchon-2024.5.30.19.18/src/pynchon/codemod/commands/docstrings/simple.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/config/__init__.py` & `pynchon-2024.5.30.19.18/src/pynchon/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/config/util.py` & `pynchon-2024.5.30.19.18/src/pynchon/config/util.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/constants.py` & `pynchon-2024.5.30.19.18/src/pynchon/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 CONF_FILE_SEARCH_ORDER = ["pynchon.json5", ".pynchon.json5", "pyproject.toml"]
 DEFAULT_PLUGINS = [
     "core",
     "git",
     # "pandoc",  # required by markdown
     "markdown",
+    "makefile",
     "src",
     "docs",
     "parse",
     "pattern",
     "plugins",
     "project",
     "globals",
```

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/core.py` & `pynchon-2024.5.30.19.18/src/pynchon/core.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/events.py` & `pynchon-2024.5.30.19.18/src/pynchon/events.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/models/planner.py` & `pynchon-2024.5.30.19.18/src/pynchon/models/planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,36 +116,48 @@
     @cli.options.parallelism
     @cli.options.fail_fast
     def apply(
         self,
         plan: planning.Plan = None,
         parallelism: str = "0",
         fail_fast: bool = False,
+        strict: bool = False,
         quiet: bool = False,
+        **plan_kwargs,
     ) -> planning.ApplyResults:
         """
         Executes the plan for this plugin
         """
+        if plan_kwargs:
+            self.logger.warning("extra kwargs will be passed to plan:")
+            self.logger.warning(f"\t{plan_kwargs}")
         parallelism = int(parallelism)
         # app.status_bar.update(
         #     app="Pynchon::APPLY",
         #     stage=f"plugin:{self.__class__.name}"
         # )
-        plan = plan or self.plan()
+        plan = plan or self.plan(**plan_kwargs)
         LOGGER.critical(
             f"{self.name}.apply ( {len(plan)} goals with {parallelism} workers)"
         )
-        results = plan.apply(parallelism=parallelism, git=self.siblings["git"])
+        results = plan.apply(
+            fail_fast=fail_fast,
+            strict=strict,
+            parallelism=parallelism,
+            git=self.siblings["git"],
+        )
 
         LOGGER.critical(
             f"{self.name}.apply finished ( {len(results.actions)}/{len(results.goals)} goals )"
         )
         self._dispatch_apply_hooks(results)
-        if not quiet:
+        if not any([fail_fast, quiet]):
             return results
+        if fail_fast and results.failed:
+            raise SystemExit(1)
 
     def _validate_hooks(self, hooks):
         # FIXME: validation elsewhere
         for x in hooks:
             assert isinstance(x, (str,))
             assert " " not in x
             assert "_" not in x
```

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/models/planning.py` & `pynchon-2024.5.30.19.18/src/pynchon/models/planning.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,17 +29,20 @@
         if self.command:
             return shil.fmt(self.command)
         else:
             return f"{self.owner}.{self.callable.__name__}(..)"
 
     @property
     def rel_resource(self) -> str:
-        return (
-            abcs.Path(self.resource).absolute().relative_to(abcs.Path(".").absolute())
-        )
+        tmp1 = abcs.Path(self.resource).absolute()
+        tmp2 = abcs.Path(".").absolute()
+        try:
+            return tmp1.relative_to(tmp2)
+        except ValueError:
+            return tmp1
 
 
 class Action(BaseModel):
     """ """
 
     type: str = typing.Field(default="unknown_action_type")
     ok: bool = typing.Field(default=None)
@@ -222,29 +225,41 @@
 class ApplyResults(typing.BaseModel):
     # typing.List[Action], metaclass=meta.namespace):
     """ """
     goals: typing.List[Goal] = typing.Field(default=[])
     actions: typing.List[Action] = typing.Field(default=[])
 
     @property
-    def finished(self):
+    def culprit(self) -> typing.Union[Action, None]:
+        """Returns the action that caused failure, if any"""
+        if self.failed:
+            for action in self:
+                if not action.ok:
+                    return action
+
+    @property
+    def finished(self) -> bool:
         """ """
         return len(self.goals) == len(self.actions)
 
     @property
     def ok(self) -> bool:
         return self.finished and all([a.ok for a in self])
 
     @property
-    def action_types(self):
+    def failed(self) -> bool:
+        return not self.ok
+
+    @property
+    def action_types(self) -> typing.Dict[str, typing.List]:
         tmp = list({g.type for g in self})
         return {k: [] for k in tmp}
 
     @property
-    def _dict(self):
+    def _dict(self) -> collections.OrderedDict:
         """ """
         result = collections.OrderedDict()
         result["ok"] = self.ok
         result["resources"] = list({a.resource for a in self})
         result["actions"] = [
             g.command if g.command else self.callable.__name__ for g in self
         ]
@@ -253,30 +268,36 @@
         for g in self:
             result["action_types"][g.type].append(g.resource)
         return result
 
     def __iter__(self):
         return iter(self.actions)
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self.actions)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"<{self.__class__.__name__}[{len(self)} actions]>"
 
 
 class Plan(typing.BaseModel):
     """ """
 
     goals: typing.List[Goal] = typing.Field(default=[])
     owner: typing.StringMaybe = typing.Field(
         help="Name of the plugin that owns this Plan", default=None
     )
 
-    def apply(self, parallelism: int = 0, fail_fast: bool = True, git=None):
+    def apply(
+        self,
+        parallelism: int = 0,
+        strict: bool = False,
+        fail_fast: bool = True,
+        git=None,
+    ) -> ApplyResults:
         """ """
         goals = self.goals
         total = len(goals)
 
         jobs = []
         results = []
         if parallelism:
@@ -316,14 +337,18 @@
                 # lme.CONSOLE.print(action)
                 results.append(action)
                 if fail_fast and not action.ok:
                     msg = f"fail-fast is set, so exiting early.  exception follows\n\n{action.error}"
                     LOGGER.critical(msg)
                     break
         results = ApplyResults(actions=results, goals=goals)
+        if strict and results.failed:
+            raise SystemExit(
+                f"Failure on apply with strict=True.  Error in command: {results.culprit.command}"
+            )
         return results
 
     def finalize(self):
         """
         When a plan is finished being appended to,
         it can be "finalized" to set the `ordering` value
         for individual goals.
```

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/models/plugins/__init__.py` & `pynchon-2024.5.30.19.18/src/pynchon/models/plugins/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from fleks import tagging
 
 from pynchon import abcs, api, cli, events  # noqa
 from pynchon.util import lme, typing  # noqa
 
 from . import validators  # noqa
 from .cli import CliPlugin  # noqa
-from .docker import DiagramTool, DockerWrapper  # noqa
+from .docker import DiagramTool, DockerComposeWrapper, DockerWrapper  # noqa
 from .provider import Provider  # noqa
 from .pynchon import PynchonPlugin  # noqa
 from .tool import AutomationTool, ToolPlugin  # noqa
 
 LOGGER = lme.get_logger(__name__)
 classproperty = fleks.util.typing.classproperty
```

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/models/plugins/cli.py` & `pynchon-2024.5.30.19.18/src/pynchon/models/plugins/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,25 +149,25 @@
 
         from pynchon.util.text import dumps  # noqa
 
         if not publish_to_cli:
             return
 
         def wrapper(*args, fxn=fxn, **kwargs):
-            LOGGER.warning(f"calling {fxn.__name__} from wrapper")
+            LOGGER.debug(f"calling {fxn.__name__} from wrapper")
             result = fxn(*args, **kwargs)
 
             rproto = getattr(result, "__rich__", None)
             if rproto:
                 # LOGGER.warning(f"rproto {result}")
-                from pynchon.util.lme import CONSOLE
+                from pynchon.util import lme
 
-                CONSOLE.print(rproto())
+                lme.print(rproto())
             if result:
-                print(dumps.json(result))
+                print(dumps.json(result, ensure_ascii=False))
 
         commands = [
             kls.click_create_cmd(
                 fxn,
                 wrapper=wrapper,
                 **{
                     **update_kwargs,
```

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/models/plugins/docker.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/pandoc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,87 @@
-""" pynchon.models.plugins.docker
+""" pynchon.plugins.pandoc
 """
 
-from pynchon import abcs
-from pynchon.cli import click
+from fleks import cli
 
-from .tool import ToolPlugin
+from fleks.util import tagging  # noqa
 
+from pynchon import abcs, events, models  # noqa
 from pynchon.util import lme, typing  # noqa
 
-from . import validators  # noqa
+LOGGER = lme.get_logger(__name__)
 
-LOGGER = lme.get_logger("DOCKER")
 
-
-class DockerWrapper(ToolPlugin):
+class Pandoc(models.DockerComposeWrapper, models.Planner):
     """
-    Wrappers for dockerized tools
+    Wrapper around `pandoc` docker image
     """
 
-    class BaseConfig(abcs.Config):
-        docker_image: str = typing.Field(default="docker/hello-world")
-        docker_args: typing.List = typing.Field(default=[])
-
-    cli_label = "Docker Wrappers"
-    cli_description = "Plugins that wrap invocations on containers"
-    contribute_plan_apply = False
-    priority = 2
-    __class_validators__ = [
-        validators.require_conf_key,
-    ]
-
-    @property
-    def command_extra(self):
-        import sys
-
-        command = sys.argv[sys.argv.index(self.click_group.name) + 2 :]
-        return " ".join(command)
-
-    def _get_docker_command_base(self, *args, **kwargs):
-        docker_image = kwargs.pop("docker_image", self["docker_image"])
-        docker_args = kwargs.pop("docker_args", "")
-        docker_args = (
-            docker_args + " " + " ".join(f'--{k}="{v}"' for k, v in kwargs.items())
-        )
-        return (
-            "docker run -v `pwd`:/workspace -w /workspace "
-            f"{docker_args} {docker_image} {' '.join(args)}"
+    class config_class(models.DockerWrapper.BaseConfig):
+        config_key: typing.ClassVar[str] = "pandoc"
+        docker_args: typing.List = typing.Field(
+            default=["--toc", "--variable fontsize=10pt"]
         )
+        docker_image: str = typing.Field(default="pandoc/extra:latest")
+        goals: typing.List[typing.Dict] = typing.Field(default=[], help="")
+        service_name: str = typing.Field(default="pandoc")
+
+    name = "pandoc"
+    cli_name = "pandoc"
+    cli_label = "Docs Tools"
+    # contribute_plan_apply = False
 
-    def _get_docker_command(self, *args, **kwargs):
-        """ """
-        cmd_t = self._get_docker_command_base(" ".join(args))
-        docker_args = " ".join(self["docker_args"])
-        zip_kws = " ".join(["{k}={v}" for k, v in kwargs.items()])
-        cmd_t += f" {docker_args} {zip_kws}"
-        return cmd_t
-
-    @click.command(
+    @cli.click.command(
         context_settings=dict(
             ignore_unknown_options=True,
             allow_extra_args=True,
         )
     )
-    def run(self, *args, **kwargs):
-        """Passes given command through to docker-image this plugin wraps"""
-        command = self._get_docker_command(self.command_extra)
+    def pdflatex(self, *args, **kwargs):
+        command = self._get_docker_command_base(
+            self.command_extra,
+            # docker_args='-it',
+            entrypoint="pdflatex",
+        )
         LOGGER.warning(command)
-        plan = super().plan(
-            goals=[
-                self.goal(
-                    type="render",
-                    resource=kwargs.get("output", kwargs.get("o", "")),
-                    command=command,
-                )
-            ]
+        result = self._run_docker(command)
+
+    def shell(self):
+        """Starts interactive shell for pandoc container"""
+        command = ""
+        command = self._get_docker_command_base(docker_args=["-it"], entrypoint="sh")
+        LOGGER.warning(command)
+        result = self.apply(
+            plan=super().plan(
+                goals=[
+                    self.goal(
+                        type="interactive",
+                        command=command,
+                    )
+                ]
+            )
         )
-        result = self.apply(plan=plan)
         if result.ok:
             raise SystemExit(0)
         else:
             LOGGER.critical(f"Action failed: {result.actions[0].error}")
             raise SystemExit(1)
 
-    def _run_docker(self, cmd, **kwargs):
-        """ """
-        from pynchon.util.os import invoke
-
-        LOGGER.critical(cmd)
-        result = invoke(cmd, **kwargs)
-        LOGGER.warning(result.stdout)
-        return result
-
-
-class DiagramTool(DockerWrapper):
-    cli_label = "Diagramming Tools"
-    cli_description = "View and render technical diagrams from source, in several formats.  (Usually these require docker, but no other system dependencies.)"
+    @cli.click.argument("file")
+    @cli.click.option("--output", help="output file", default="")
+    @tagging.tags(click_aliases=["markdown.to-pdf"])
+    def md_to_pdf(
+        self,
+        file: str = None,
+        output: str = "",
+    ):
+        """
+        Converts markdown files to PDF with pandoc
+        """
+        output = abcs.Path(output or f"{abcs.Path(file).stem}.pdf")
+        docker_image = self["docker_image"]
+        docker_args = " ".join(self["docker_args"] or [])
+        cmd = f"docker compose run {self.config.service_name} {file} {docker_args} -o {output}"
+        plan = super().plan(
+            goals=[self.goal(resource=output.absolute(), type="render", command=cmd)]
+        )
+        return self.apply(plan=plan, fail_fast=True, strict=True)
```

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/models/plugins/provider.py` & `pynchon-2024.5.30.19.18/src/pynchon/models/plugins/provider.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/models/plugins/pynchon.py` & `pynchon-2024.5.30.19.18/src/pynchon/models/plugins/pynchon.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/models/plugins/tool.py` & `pynchon-2024.5.30.19.18/src/pynchon/models/plugins/tool.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/models/plugins/validators.py` & `pynchon-2024.5.30.19.18/src/pynchon/models/plugins/validators.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/models/python.py` & `pynchon-2024.5.30.19.18/src/pynchon/models/python.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/__init__.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/cicd.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/cicd.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/core.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/core.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/deck.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/deck.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/dockerhub.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/dockerhub.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/docs/main.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/docs/main.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/docs/opener.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/docs/opener.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/dot.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/dot.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/drawio.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/drawio.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,76 +40,118 @@
         )
 
         docker_image: str = typing.Field(
             default="jgraph/drawio", help="Docker image to use"
         )
         http_port: str = typing.Field(help="Port to use", default=DEFAULT_HTTP_PORT)
         docker_args: typing.List = typing.Field(
-            default=[f"-it --rm --name={DEFAULT_DOCKER_NAME}"],
+            default=[f"--rm --name={DEFAULT_DOCKER_NAME}"],
             help="Docker args to use",
         )
         export_docker_image: str = typing.Field(
             default="rlespinasse/drawio-desktop-headless"
         )
+        format: str = typing.Field(help="", default="png")
         export_width: int = typing.Field(help="", default=800)
         export_args: typing.List = typing.Field(
             help="",
             default=[
                 "--export",
-                "--embed-svg-images",
-                "--embed-diagram",
-                "--svg-theme light",
+                "--border 10",
+                "--crop",
+                # "--zoom",
+                "--transparent",
+                # "--embed-svg-images",
+                # "--embed-diagram",
+                # "--svg-theme light",
             ],
         )
 
     name = "drawio"
     cli_name = "drawio"
     priority = 0
+    contribute_plan_apply = True
 
     @tagging.tags(click_aliases=["ls"])
     def list(self, changes=False, **kwargs):
         """
         Lists affected resources (*.drawio files) for this project
         """
         return self._list(changes=changes, **kwargs)
 
+    def plan(
+        self,
+        config=None,
+    ) -> typing.List:
+        """Creates a plan for this plugin"""
+        plan = super(self.__class__, self).plan()
+        for src in self.list():
+            plan.append(
+                self.goal(
+                    type="render",
+                    resource=src,
+                    command=f"pynchon drawio render {src}",
+                )
+            )
+        return plan.finalize()
+
     @cli.click.argument("output", required=False)
     @cli.click.argument("input")
-    def export(self, input, output=None, format="svg"):
+    def render(
+        self,
+        input,
+        output=None,
+    ):
         """
         Exports a given .drawio file to some
         output file/format (default format is SVG)
         """
+        format = self.config["format"]
         assert input.endswith(".drawio") or input.endswith(
             ".xml"
         ), "Expected an xml or drawio file as input"
         output = output or ".".join(
             list(filter(None, input.split(".")[:-1])) + [format]
         )
         export_args = " ".join(self.config.export_args)
-        export_args += f" --width {self.config.export_width}"
+        # export_args += f" --width {self.config.export_width} --height 600"
         export_docker_args = "-w /workspace -v `pwd`:/workspace"
         result = self._run_docker(
             (
                 f"docker run {export_docker_args} {self.config.export_docker_image} "
                 f"{export_args} --output {output} {input}"
             ),
             strict=True,
         )
         print(result.stdout if result.succeeded else result)
         raise SystemExit(0 if result.succeeded else 1)
 
-    def serve(self):
+    export = render
+
+    def stop(self):
+        """Stop DrawIO server"""
+        return self._stop_container(name=DEFAULT_DOCKER_NAME)
+
+    @cli.click.option(
+        "--background", "-b", help="Run in background", is_flag=True, default=False
+    )
+    def serve(self, background: bool = False):
         """
         Runs the drawio-UI in a docker-container
         """
         port = self.config.http_port
-        dargs = self.config.docker_args
+        dargs = " ".join(self.config.docker_args)
         dimg = self.config.docker_image
-        cmd_t = f"docker run {dargs} -p {port}:{port} {dimg}"
+        if background:
+            background = "&"
+            dargs = dargs  # f'-it {dargs}'
+        else:
+            dargs = f"-it {dargs}"
+            background = ""
+        cmd_t = f"docker run {dargs} -p {port}:{port} {dimg} {background}"
         return self._run_docker(cmd_t, strict=True, interactive=True)
 
     def open(self, *args, **kwargs):
         """
         Opens a browser for the container started by `serve`
         """
         return webbrowser.open(
```

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/fixme.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/fixme.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/gen.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/gen.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/git.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/git.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/github.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/github.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,14 +25,20 @@
         enterprise: bool = typing.Field(default=False)
         org_name: typing.StringMaybe = typing.Field(default=None)
         org_url: typing.StringMaybe = typing.Field(default=None)
         repo_url: typing.StringMaybe = typing.Field(default=None)
         actions: typing.List[abcs.Path] = typing.Field(default=[None])
         raw_url: typing.StringMaybe = typing.Field(default=None)
         repo_ssh_url: typing.StringMaybe = typing.Field(default=None)
+        # branch_name: typing.StringMaybe = typing.Field(default=None)
+
+        # @property
+        # def branch_name(self):
+        #     """URL for serving raw content"""
+        #     return config.git.branch_name
 
         @property
         def raw_url(self):
             """URL for serving raw content"""
             repo_name = config.git.repo_name
             if self.org_name and config.git.repo_name:
                 return f"https://raw.githubusercontent.com/{self.org_name}/{repo_name}"
@@ -80,72 +86,71 @@
 
     name = "github"
     cli_name = "github"
     cli_label = "Provider"
     cli_aliases = []
 
     @cli.click.option("--org", "-o")
-    def open(self, org=None):
-        """Opens org/repo github in a webbrowser
-
-        :param org: Default value = None)
-
+    @cli.click.argument("mode", required=False, default="top")
+    def open(self, mode="top", org=None):
+        """
+        Opens org/repo github in a webbrowser.
         """
         org_name = self["org_name"]
-        url = self["org_url"]
-        if not org:
-            repo_name = self[:"git.repo_name":]
-            url = f"{url}/{repo_name}"
+        if org:
+            url = self["org_url"]
+        elif mode == "top":
+            url = self[:"git.repo_url":]
+        elif mode in ["branch", "b"]:
+            branch = self[:"git.branch_name":]
+            url = self[:"git.repo_url":] + f"/tree/{branch}"
+        elif mode in ["actions", "a", "action"]:
+            url = self[:"git.repo_url":] + "/actions"
+        elif mode in ["pulls", "prs", "p"]:
+            url = self[:"git.repo_url":] + "/pulls"
+        else:
+            url = self[:"git.repo_url":]
         return webbrowser.open(url)
 
     @cli.options.org_name
     @option_api_token
     def clone_org(self, org_name: str = None, token: str = None):  # noqa
-        """Clones an entire github-org
+        """
+        Clones an entire github-org
 
         :param org_name: str:  (Default value = None)
         :param token: str:  (Default value = None)
-        :param org_name: str:  (Default value = None)
-        :param token: str:  (Default value = None)
-
         """
         raise NotImplementedError()
 
     @cli.click.argument("repo")
     @option_api_token
     def clone(self, repo: str, token: str = None):  # noqa
-        """Clones a single repo from this project's org
+        """
+        Clones a single repo from this project's org
 
         :param repo: str:
         :param token: str:  (Default value = None)
-        :param repo: str:
-        :param token: str:  (Default value = None)
-
         """
         raise NotImplementedError()
 
     # @cli.click.argument('repo')
     @tagging.tags(click_aliases=["pr"])
     @option_api_token
     def pull_request(self, repo: str, token: str = None):  # noqa
-        """Creates a pull-request from this branch
+        """
+        Creates a pull-request from this branch
 
         :param repo: str:
         :param token: str:  (Default value = None)
-        :param repo: str:
-        :param token: str:  (Default value = None)
-
         """
         raise NotImplementedError()
 
     @tagging.tags(click_aliases=["codeowners"])
     # @option_api_token
     def code_owners(self, repo: str, token: str = None):  # noqa
         """Describes code-owners for changes or for working-dir
 
         :param repo: str:
         :param token: str:  (Default value = None)
-        :param repo: str:
-        :param token: str:  (Default value = None)
-
         """
         raise NotImplementedError()
```

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/griffe.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/griffe.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/makefile.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/makefile.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,14 @@
         # help="Return only the prerequisites-graph"
         default="",
         required=False,
     )
     def parse(self, makefile: str = "", only_graph: bool = False):
         """Parse Makefile to JSON.  Includes DAGs for targets, target-body, and target-type details"""
         makefile = makefile or self.config["file"]
+        from collections import OrderedDict
+
         out = makefile_parse(makefile=makefile)
+        out = OrderedDict(sorted([k, v] for k, v in out.items()))
         if only_graph:
             out = {t: out[t]["prereqs"] for t in out}
         return out
-
-    # def bootstrap(self):
-    #     """ placeholder """
-    #     raise NotImplementedError()
```

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/markdown.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/markdown.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,14 +29,18 @@
         root: typing.Union[str, abcs.Path, None] = typing.Field(
             default=None, description=""
         )
         linter_docker_image: str = typing.Field(
             default="peterdavehello/markdownlint",
             description="Container to use for markdown linter",
         )
+        viewer_docker_image: str = typing.Field(
+            default="charmcli/glow", help="Container to use for markdown console viewer"
+        )
+
         linter_args: typing.List[str] = typing.Field(
             description="Arguments to pass to `linter_docker_image`",
             default=[
                 "--disable MD013",  # line-length
                 "--disable MD045",  # Images should have alternate text
                 "--disable MD033",  # Allow HTML
                 "--disable MD041",  # first-line-h1
@@ -93,31 +97,73 @@
                     ),
                 )
             )
         return self.apply(plan=self.plan(goals=goals))
 
     @cli.click.argument("paths", nargs=-1)
     @tagging.tags(click_aliases=["show"])
-    def preview(self, paths):
+    def preview(self, paths=[]):
         """
         Previews markdown in the terminal
         """
-        # FIXME?: rich doesn't link hypertext.  patch upstream?
-        from rich.console import Console
-        from rich.markdown import Markdown
+        import os
+
+        from python_on_whales import docker
+
+        is_pipe = not os.isatty(0)
+        if is_pipe:
+            LOGGER.critical("detected pipe")
+        if not paths:
+            assert (
+                is_pipe
+            ), "if no paths are provided, expected you would be using this command with a pipe, but no pipe is detected"
+            paths = ["/dev/stdin"]
+            interactive, tty = True, False
+        else:
+            interactive, tty = True, True
+        #     return self.preview(paths = [tmpstdin], tty=False)
 
-        console = Console()
+        # assert not paths
+        #     tty=False
+        # else:
+        #     tty=True
+        specialf = ["/dev/stdin", "-"]
         for p in paths:
-            with open(p) as fhandle:
-                md = Markdown(fhandle.read())
-                console.print(md)
+            if os.path.isabs(p) and p not in specialf:
+                volumes = [(p, p)]
+            else:
+                volumes = [
+                    # in case of relative paths
+                    (os.getcwd(), "/workspace"),
+                ]
+            dargs = (
+                self.config.viewer_docker_image,
+                ["-s", "dracula", p],
+            )
+            dkwargs = dict(
+                tty=tty,
+                interactive=tty,
+                volumes=volumes,
+                workdir="/workspace",
+            )
+            if is_pipe:
+                import sys
+
+                dkwargs.update(interactive=False, tty=True)
+                tmpstdin = ".tmp.stdin"
+                dargs = (
+                    self.config.viewer_docker_image,
+                    ["-s", "dracula", tmpstdin],
+                )
+                LOGGER.critical("reading input from stdin..")
+                with open(tmpstdin, "w") as fhandle:
+                    LOGGER.critical(f"writing tmp file {tmpstdin}")
+                    fhandle.write(sys.stdin.read())
+            docker.run(*dargs, **dkwargs)
         # FIXME: glow is awesome but using it from docker seems to strip color
-        # viewer_docker_image: str = typing.Field(
-        #     default='charmcli/glow',
-        #     help="Container to use for markdown console viewer")
         # docker_image = self["viewer_docker_image"]
         #         # viewer_args = " ".join(self["viewer_args"])
         #         return self._run_docker(
         #                         f"docker run -t -v `pwd`:/workspace "
         #                         f"-w /workspace {docker_image} "
         #                         f" {' '.join(paths)}"
         #                     )
```

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/mermaid.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/mermaid.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/mkdocs.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/mkdocs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,130 +1,127 @@
 """ pynchon.plugins.mkdocs
 """
 
+import os
 import urllib
+import webbrowser
+import urllib.parse
 from pathlib import Path
 
 import yaml
 import fleks
 from fleks import tagging
 
 from pynchon.plugins import util as plugin_util
 from pynchon.util.text import loadf
 
 from pynchon import abcs, api, events, models  # noqa
 from pynchon.util import lme, typing  # noqa
 
 LOGGER = lme.get_logger(__name__)
+DEFAULT_LOG_FILE = ".tmp.mkdocs.log"
+
+
+class MkdocsPage(fleks.config.Config):
+    config_key: typing.ClassVar[str] = "mkdocs.pages"
+    title: str = typing.Field()
+    path: typing.Union[abcs.Path, str] = typing.Field()
+    relative_url: str = typing.Field()
+    rel_path: str = typing.Field()
+    tags: typing.List[str] = typing.Field(
+        default=[], help="only used by mkdocs_blogging plugin"
+    )
+    draft: bool = typing.Field(default=False)
+    exclude_from_blog: bool = typing.Field(
+        default=False, help="only used by mkdocs_blogging plugin"
+    )
+    description: str = typing.Field(default="")
 
 
 class MkdocsPluginConfig(abcs.Config):
     config_key: typing.ClassVar[str] = "mkdocs"
     config_file: str = typing.Field(default=None)
 
     @property
     def tags(self) -> typing.List:
         """ """
         tags = set()
         for p in self.pages:
-            tags = tags.union(set(p.get("tags", [])))
+            tags = tags.union(set(p.tags))
         # NB: removes empty-string
         return sorted(list(filter(None, tags)))
 
     @property
-    def drafts(self):
+    def drafts(self) -> typing.List:
         ignore_list = ["index.md", "tags.md", "nav.md"]
         return [
             p
             for p in self.pages
             if all([p["draft"], p["path"].name not in ignore_list])
         ]
 
     @property
     def pages(self) -> typing.List:
         """ """
+        from mkdocs.config.defaults import MkDocsConfig
         from mkdocs.structure.files import File
         from mkdocs.structure.pages import Page
 
         pages = []
         mconf = self.config
         if mconf:
             ddir = abcs.Path(mconf.get("docs_dir", "docs"))
-            from mkdocs.config.defaults import MkDocsConfig
 
             cfg = MkDocsConfig()
             data = yaml.load(open(self.config_file).read(), yaml.FullLoader)
             cfg.load_dict(data)
             cfg.validate()  # fl = File(
-            #     'heredoc/ambient-calculus-1.md',
-            #     cfg.docs_dir, cfg.site_dir, cfg.use_directory_urls)
-            # config_file
-            # pconf = mconf['plugins'] if 'plugins' in mconf else {}
-            # bconf = [conf for conf in pconf if 'blogging' in list(conf.keys())]
-            # bconf = bconf[0]['blogging'] if bconf else {}
             pfiles = ddir.glob("**/*.md")
-            # pfiles = [p.relative_to(ddir) for p in pfiles]
             for pfile in pfiles:
                 rel_pfile = pfile.relative_to(ddir)
                 mfile = File(
                     str(rel_pfile), cfg.docs_dir, cfg.site_dir, cfg.use_directory_urls
                 )
                 pg = Page(
                     file=mfile,
                     config=cfg,
                     title=None,
                 )
                 pg.read_source(cfg)
-                tags = pg.meta.get("tags", [])
-                draft = any([pg.meta.get("draft", False), "draft" in str(rel_pfile)])
-                #   {%- for p in mkdocs.blog_posts|default([]) %}{% set p=p|Path %}{% set p=p.relative_to(mkdocs.config.docs_dir | default('docs/')) %}
-                # * [{{p.stem.replace('-',' ').title()}}]({{p}}){%- endfor -%}
-                pmeta = dict(
-                    title=pg.title,
+                pmeta_d = dict(
+                    title=pg.meta.pop("title", pg.title),
                     # relative_url=pg.url,
                     relative_url=f"{self.site_relative_url}/{pg.url}",
                     path=pfile.absolute(),
                     rel_path=str(rel_pfile),
-                    tags=tags,
-                    # thing=rel_pfile.stem.replace('- ',' ').title(),
-                    draft=draft,
+                    tags=pg.meta.pop("tags", []),
+                    draft=any([pg.meta.pop("draft", False), "draft" in str(rel_pfile)]),
+                    **pg.meta,  # **dict(pg.title)},
                 )
+                pmeta = MkdocsPage(**pmeta_d)
                 pages.append(pmeta)
         return pages
 
     @property
-    def blog_posts(self) -> list:
+    def blog_posts(self) -> typing.List:
         """
         returns blog posts, iff blogging plugin is installed.
         resulting files, if any, will not include index and
         will be sorted by modification time
         """
         ignore_list = ["index.md", "tags.md", "nav.md"]
         return [
             p
             for p in self.pages
             if all([not p["draft"], p["path"].name not in ignore_list])
         ]
-        # mconf = self.config
-        # if mconf:
-        #     pconf = mconf["plugins"] if "plugins" in mconf else {}
-        #     ddir = abcs.Path(mconf.get("docs_dir", "docs"))
-        #     bconf = [conf for conf in pconf if "blogging" in list(conf.keys())]
-        #     bconf = bconf[0]["blogging"] if bconf else {}
-        #     blog_dirs = [ddir / bdir for bdir in bconf.get("dirs", [])]
-        #     result = []
-        #     for bdir in blog_dirs:
-        #         result += [g for g in bdir.glob("**/*.md") if g.name not in ignore_list]
-        #     result = reversed(sorted(result, key=lambda p: p.lstat().st_mtime))
-        #     result = [str(p) for p in result]
-        #     return result
 
     @property
-    def site_relative_url(self):
-
+    def site_relative_url(self) -> str:
+        """ """
         site_url = self.config["site_url"] if "site_url" in self.config else None
         if site_url:
             return urllib.parse.urlparse(site_url).path
 
     @property
     def config(self) -> typing.Dict:
         """
@@ -156,17 +153,14 @@
         )
         for folder in [Path(c) for c in candidates]:
             cand = folder / "mkdocs.yml"
             if cand.exists():
                 return str(cand.absolute())
 
 
-DEFAULT_LOG_FILE = ".tmp.mkdocs.log"
-
-
 class Mkdocs(models.Planner):
     """Mkdocs helper"""
 
     priority = 8  # before mermaid
     name = "mkdocs"
     cli_name = "mkdocs"
     cli_label = "Docs Tools"
@@ -184,58 +178,75 @@
 
         bg = "&" if background else ""
         cmd = f"mkdocs serve --config-file {self.config_file} >> {DEFAULT_LOG_FILE} 2>&1 {bg}"
         result = invoke(cmd)
         return result
 
     @tagging.tags(click_aliases=["ls"])
-    def list(self):
+    def list(self) -> typing.List:
         """Lists site-pages based on mkdocs.yml"""
         return self.config.pages
 
     @fleks.cli.click.argument("files", nargs=-1)
     def open(
         self,
         files: tuple = tuple(),
-    ):
+    ) -> bool:
         """
         Opens `dev_addr` in a webbrowser
         """
-        import webbrowser
-
-        file = files[0] if files else "."
-        # index_f = Path(self.site_dir).absolute() / "index.html"
-        # url = f"file://{index_f}"
+        if not files:
+            file = "."
+        else:
+            file = files[0] if files else "."
         mconfig = self.config.config
+        default_path = urllib.parse.urlparse(mconfig["site_url"]).path
+        default_path = (
+            default_path[1:] if default_path.startswith("/") else default_path
+        )
+        default_path = default_path[:-1] if default_path.endswith("/") else default_path
+        docs_dir = Path(mconfig["docs_dir"]).absolute()
+        LOGGER.warning(f"opening {file}")
+        if file.startswith("/"):
+            LOGGER.warning("file is absolute..")
+            relf = Path(file[1:])
+            relf_on_docs = Path(mconfig["docs_dir"]) / relf
+            file = relf_on_docs / relf
+            file = file.absolute().relative_to(docs_dir)
+        else:
+            LOGGER.warning("file is relative..")
+            file = Path(file).absolute().relative_to(docs_dir)
+        file, ext = os.path.splitext(str(file))
+        file = file if ext == ".md" else "".join([file, ext])
         url = mconfig["dev_addr"]
+        url = f"{url}/{default_path}" if default_path else url
         url = f"{url}/{file}" if file else url
         url = f"http://{url}" if not url.startswith("http") else url
+        url = url.replace("/blog/", "/#blog/")
         self.logger.warning(f"opening {url}")
         return webbrowser.open(url)
 
     @property
     def site_dir(self) -> str:
         """
         Returns mkdocs `site_dir` if present in config, or guesses what it should be
         """
         plugin_cfg = self.config
         mkdocs_config = plugin_cfg.config
         result = str(mkdocs_config.get("site_dir", self.working_dir / "site"))
         self.logger.warning(f"returning {result}")
         return result
 
-    # def _hook_open_after_apply(self, result) -> bool:
-    #     raise Exception(result)
-
     def plan(self):
         """
         Runs a plan for this plugin
         """
         plan = super(self.__class__, self).plan()
+        command = f"mkdocs build --config-file {self.config_file}"
         plan.append(
             self.goal(
                 type="render",
                 resource=self.site_dir,
-                command=f"mkdocs build --config-file {self.config_file}",
+                command=command,
             )
         )
         return plan
```

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/pandoc.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/compose.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,52 @@
-""" pynchon.plugins.pandoc
+""" pynchon.plugins.compose
 """
 
 from fleks import cli
 
 from fleks.util import tagging  # noqa
 
 from pynchon import abcs, events, models  # noqa
 from pynchon.util import lme, typing  # noqa
 
 LOGGER = lme.get_logger(__name__)
 
 
-class Pandoc(models.DockerWrapper, models.Planner):
+class Compose(models.DockerWrapper, models.Planner):
     """
-    Wrapper around `pandoc` docker image
+    Wrapper around docker-compose
     """
 
     class config_class(models.DockerWrapper.BaseConfig):
-        config_key: typing.ClassVar[str] = "pandoc"
-        docker_args: typing.List = typing.Field(
-            default=["--toc", "--variable fontsize=10pt"]
-        )
-        docker_image: str = typing.Field(default="pandoc/extra:latest")
+        config_key: typing.ClassVar[str] = "compose"
+        compose_args: typing.List = typing.Field(default=[])
+        # docker_image: str = typing.Field(default="pandoc/extra:latest")
         goals: typing.List[typing.Dict] = typing.Field(default=[], help="")
 
-    name = "pandoc"
-    cli_name = "pandoc"
-    cli_label = "Docs Tools"
+    name = "compose"
+    cli_name = "compose"
+    # cli_label = "Docs Tools"
     # contribute_plan_apply = False
 
     @cli.click.command(
         context_settings=dict(
             ignore_unknown_options=True,
             allow_extra_args=True,
         )
     )
-    def pdflatex(self, *args, **kwargs):
+    def run(self, *args, **kwargs):
         # command = self._get_docker_command(self.command_extra)
-        command = self._get_docker_command_base(
-            self.command_extra,
-            # docker_args='-it',
-            entrypoint="pdflatex",
-        )
-        LOGGER.warning(command)
-        result = self._run_docker(command)
+        raise Exception(locals())
+        # command = self._get_docker_command_base(
+        #     self.command_extra,
+        #     # docker_args='-it',
+        #     entrypoint="pdflatex",
+        # )
+        # LOGGER.warning(command)
+        # result = self._run_docker(command)
         # result = self.apply(plan=super().plan(
         #     goals=[
         #         self.goal(
         #             type="?",
         #             # resource=kwargs.get("output", kwargs.get("o", None)),
         #             command=command,
         #         )
@@ -55,49 +54,28 @@
         # ))
         # if result.ok:
         #     raise SystemExit(0)
         # else:
         #     LOGGER.critical(f"Action failed: {result.actions[0].dict()}")
         #     raise SystemExit(1)
 
-    def shell(self):
-        """Starts interactive shell for pandoc container"""
-        command = ""
-        command = self._get_docker_command_base(docker_args="-it", entrypoint="sh")
-        LOGGER.warning(command)
-        result = self.apply(
-            plan=super().plan(
-                goals=[
-                    self.goal(
-                        type="interactive",
-                        # resource=kwargs.get("output", kwargs.get("o", None)),
-                        command=command,
-                    )
-                ]
-            )
-        )
-        if result.ok:
-            raise SystemExit(0)
-        else:
-            LOGGER.critical(f"Action failed: {result.actions[0].error}")
-            raise SystemExit(1)
-
-    @tagging.tags(click_aliases=["markdown.to-pdf"])
-    @cli.options.output_file
-    @cli.click.argument("file")
-    def md_to_pdf(
-        self,
-        file: str = None,
-        output: str = None,
-    ):
-        """
-        Converts markdown files to PDF with pandoc
-        """
-        output = abcs.Path(output or f"{abcs.Path(file).stem}.pdf")
-        # cmd = f"docker run -v `pwd`:/workspace -w /workspace {docker_image} {file} {docker_args} -o {output}"
-        return self.run(file, output=output)
-        # plan = super().plan(
-        #     goals=[
-        #         self.goal(resource=output.absolute(),
-        #         type="render", command=cmd)]
-        # )
-        # return self.apply(plan=plan)
+    # @cli.click.argument("file")
+    # @cli.click.option('--output', help='output file', default='')
+    # # @tagging.tags(click_aliases=["markdown.to-pdf"])
+    # def md_to_pdf(
+    #     self,
+    #     file: str = None,
+    #     output: str = '',
+    # ):
+    #     """
+    #     Converts markdown files to PDF with pandoc
+    #     """
+    #     output = abcs.Path(output or f"{abcs.Path(file).stem}.pdf")
+    #     docker_image = self['docker_image']
+    #     docker_args = ' '.join(self['docker_args'] or [])
+    #     cmd = f"docker run -v `pwd`:/workspace -w /workspace {docker_image} {file} {docker_args} -o {output}"
+    #     plan = super().plan(
+    #         goals=[
+    #             self.goal(resource=output.absolute(),
+    #             type="render", command=cmd)]
+    #     )
+    #     return self.apply(plan=plan,fail_fast=True)
```

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/pattern.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/pattern.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/plugins.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/project.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/project.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/python/api.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/python/api.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/python/cli.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/python/cli.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/python/libcst.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/python/libcst.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/python/platform.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/python/platform.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/python/pypi.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/python/pypi.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/release.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/release.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/render.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/render.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/scaffolding/__init__.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/scaffolding/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/scaffolding/config.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/scaffolding/config.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/src.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/src.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/tests.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/tests.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/plugins/util.py` & `pynchon-2024.5.30.19.18/src/pynchon/plugins/util.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/templates/docker/Dockerfile.pandoc` & `pynchon-2024.5.30.19.18/src/pynchon/templates/docker/Dockerfile.pandoc`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bash.sh` & `pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bash.sh`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bashrc.sh` & `pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bashrc.sh`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/tox.ini` & `pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/tox.ini`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/makefile/mermaid-graph.mmd.j2` & `pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/makefile/mermaid-graph.mmd.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2` & `pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2` & `pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2` & `pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2` & `pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python_cli/TOC.md.j2` & `pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python_cli/TOC.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python_cli/main.module.md.j2` & `pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python_cli/main.module.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/plugins/python_cli/script.console.md.j2` & `pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/plugins/python_cli/script.console.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/templates/includes/pynchon/pydantic-model.md.j2` & `pynchon-2024.5.30.19.18/src/pynchon/templates/includes/pynchon/pydantic-model.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/docker/.dockerignore` & `pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/docker/.dockerignore`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/docker/README.md.j2` & `pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/docker/README.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/.libcst.codemod.yaml` & `pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/Makefile` & `pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/Makefile`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/README.md` & `pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/README.md`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/README.md.j2` & `pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/README.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/setup.cfg` & `pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/setup.cfg`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/setup.py` & `pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/setup.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/templates/scaffolds/py/pkg/tox.ini` & `pynchon-2024.5.30.19.18/src/pynchon/templates/scaffolds/py/pkg/tox.ini`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/util/__init__.py` & `pynchon-2024.5.30.19.18/src/pynchon/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/util/complexity.py` & `pynchon-2024.5.30.19.18/src/pynchon/util/complexity.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/util/docker.py` & `pynchon-2024.5.30.19.18/src/pynchon/util/docker.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/util/events.py` & `pynchon-2024.5.30.19.18/src/pynchon/util/events.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/util/files/__init__.py` & `pynchon-2024.5.30.19.18/src/pynchon/util/files/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/util/files/__main__.py` & `pynchon-2024.5.30.19.18/src/pynchon/util/files/__main__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/util/files/diff.py` & `pynchon-2024.5.30.19.18/src/pynchon/util/files/diff.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/util/makefile/__init__.py` & `pynchon-2024.5.30.19.18/src/pynchon/util/makefile/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,29 +14,30 @@
 vvv = "# Variables"
 fff = "# files hash-table stats:"
 
 
 @cli.click.argument("makefile")
 def database(makefile: str = "", make="make") -> typing.List[str]:
     """
-    Get database for Makefile (i.e. 'make --print-data-base')
+    Get database for Makefile
+    (This output comes from 'make --print-data-base')
     """
     assert makefile
     tmp = abcs.Path(makefile)
     if not all(
         [
             tmp.exists,
             tmp.is_file,
         ]
     ):
         raise ValueError(f"{makefile} does not exist")
     else:
         LOGGER.warning(f"parsing makefile @ {makefile}")
     cmd = f"{make} --print-data-base -pqRrs -f {makefile}"
-    resp = invoke(cmd)
+    resp = invoke(cmd, command_logger=LOGGER.warning)
     out = resp.stdout.split("\n")
     return out
 
 
 def _test(x):
     """ """
     return all(
@@ -89,14 +90,15 @@
         implicit_rule_end = implicit_rule_start
     implicit_targets_section = db[implicit_rule_start:implicit_rule_end]
     file_targets_section = db[file_rule_start:file_rule_end]
     file_target_names = list(filter(_test, file_targets_section))
     implicit_target_names = list(filter(_test, implicit_targets_section))
     targets = file_target_names + implicit_target_names
     out = {}
+    targets = [t for t in targets if t != f"{makefile}:"]
     for tline in targets:
         bits = tline.split(":")
         target_name = bits.pop(0)
         childs = ":".join(bits)
         type = "implicit" if tline in implicit_targets_section else "file"
         # NB: line nos are from reformatted output, not original file
         line_start = db.index(tline)
```

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/util/oop.py` & `pynchon-2024.5.30.19.18/src/pynchon/util/oop.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/util/os/__init__.py` & `pynchon-2024.5.30.19.18/src/pynchon/util/os/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/util/os/models.py` & `pynchon-2024.5.30.19.18/src/pynchon/util/os/models.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/util/os/pids.py` & `pynchon-2024.5.30.19.18/src/pynchon/util/os/pids.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/util/python.py` & `pynchon-2024.5.30.19.18/src/pynchon/util/python.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/util/text/__init__.py` & `pynchon-2024.5.30.19.18/src/pynchon/util/text/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/util/text/dumpf/__init__.py` & `pynchon-2024.5.30.19.18/src/pynchon/util/text/dumpf/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/util/text/dumpf/__main__.py` & `pynchon-2024.5.30.19.18/src/pynchon/util/text/dumpf/__main__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/util/text/dumps.py` & `pynchon-2024.5.30.19.18/src/pynchon/util/text/dumps.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/util/text/loadf/__init__.py` & `pynchon-2024.5.30.19.18/src/pynchon/util/text/loadf/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/util/text/loadf/__main__.py` & `pynchon-2024.5.30.19.18/src/pynchon/util/text/loadf/__main__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/util/text/loads.py` & `pynchon-2024.5.30.19.18/src/pynchon/util/text/loads.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/util/text/normalize/__init__.py` & `pynchon-2024.5.30.19.18/src/pynchon/util/text/normalize/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/util/text/render/__init__.py` & `pynchon-2024.5.30.19.18/src/pynchon/util/text/render/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/util/text/render/__main__.py` & `pynchon-2024.5.30.19.18/src/pynchon/util/text/render/__main__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon/util/typing.py` & `pynchon-2024.5.30.19.18/src/pynchon/util/typing.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.5.14.1/src/pynchon.egg-info/PKG-INFO` & `pynchon-2024.5.30.19.18/src/pynchon.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pynchon
-Version: 2024.4.5.14.1
+Version: 2024.5.30.19.18
 Summary: Autodocs for python projects
 Home-page: https://github.com/elo-enterprises/pynchon/
 Author: elo
 Author-email: engineering@elo.enterprises
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/pynchon/
 Project-URL: Source, https://github.com/elo-enterprises/pynchon/
 Project-URL: Download, https://github.com/elo-enterprises/pynchon/#files
 Platform: any
 Classifier: Programming Language :: Python
 Requires-Python: >3.6
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Requires-Dist: gripe>=2024.2.24.1.31
-Requires-Dist: shil>=2023.7.17.7.1
+Requires-Dist: shil>=2024.5.30.18.30
 Requires-Dist: shimport>=2023.7.11.23.36
-Requires-Dist: fleks==2024.4.5.9.29
+Requires-Dist: fleks==2024.5.10.23.48
 Requires-Dist: memoization==0.4.0
 Requires-Dist: multipledispatch==0.6.0
 Requires-Dist: pygments
 Requires-Dist: pyjson5==1.6.1
 Requires-Dist: marko==2.0.0
 Requires-Dist: pyyaml
 Requires-Dist: trogon
```

### Comparing `pynchon-2024.4.5.14.1/src/pynchon.egg-info/SOURCES.txt` & `pynchon-2024.5.30.19.18/src/pynchon.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -55,28 +55,28 @@
 src/pynchon/models/plugins/pynchon.py
 src/pynchon/models/plugins/tool.py
 src/pynchon/models/plugins/validators.py
 src/pynchon/plugins/__init__.py
 src/pynchon/plugins/__template__.py
 src/pynchon/plugins/api.py
 src/pynchon/plugins/cicd.py
+src/pynchon/plugins/compose.py
 src/pynchon/plugins/core.py
 src/pynchon/plugins/deck.py
 src/pynchon/plugins/dockerhub.py
 src/pynchon/plugins/dot.py
 src/pynchon/plugins/drawio.py
 src/pynchon/plugins/fixme.py
 src/pynchon/plugins/gen.py
 src/pynchon/plugins/git.py
 src/pynchon/plugins/github.py
 src/pynchon/plugins/globals.py
 src/pynchon/plugins/griffe.py
 src/pynchon/plugins/hooks.py
 src/pynchon/plugins/jinja.py
-src/pynchon/plugins/json.py
 src/pynchon/plugins/makefile.py
 src/pynchon/plugins/markdown.py
 src/pynchon/plugins/mermaid.py
 src/pynchon/plugins/mkdocs.py
 src/pynchon/plugins/pandoc.py
 src/pynchon/plugins/parse.py
 src/pynchon/plugins/pattern.py
@@ -84,14 +84,15 @@
 src/pynchon/plugins/project.py
 src/pynchon/plugins/release.py
 src/pynchon/plugins/render.py
 src/pynchon/plugins/rtd.py
 src/pynchon/plugins/src.py
 src/pynchon/plugins/tests.py
 src/pynchon/plugins/util.py
+src/pynchon/plugins/vhs.py
 src/pynchon/plugins/docs/__init__.py
 src/pynchon/plugins/docs/main.py
 src/pynchon/plugins/docs/opener.py
 src/pynchon/plugins/doctor/__init__.py
 src/pynchon/plugins/python/__init__.py
 src/pynchon/plugins/python/api.py
 src/pynchon/plugins/python/cli.py
```

