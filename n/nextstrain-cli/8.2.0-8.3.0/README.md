# Comparing `tmp/nextstrain-cli-8.2.0.tar.gz` & `tmp/nextstrain_cli-8.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextstrain-cli-8.2.0.tar", last modified: Wed Feb  7 00:09:11 2024, max compression
+gzip compressed data, was "nextstrain_cli-8.3.0.tar", last modified: Tue Apr 30 20:04:19 2024, max compression
```

## Comparing `nextstrain-cli-8.2.0.tar` & `nextstrain_cli-8.3.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 00:09:11.406479 nextstrain-cli-8.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/LICENSE.cognito-srp
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/LICENSE.id3c
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/LICENSE.sphinx
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-02-07 00:09:11.406479 nextstrain-cli-8.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 00:09:11.390478 nextstrain-cli-8.2.0/nextstrain/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 00:09:11.394478 nextstrain-cli-8.2.0/nextstrain/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/argparse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 00:09:11.394478 nextstrain-cli-8.2.0/nextstrain/cli/authn/
--rw-r--r--   0 runner    (1001) docker     (127)     8863 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/authn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/authn/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/authn/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    30176 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/authn/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 00:09:11.394478 nextstrain-cli-8.2.0/nextstrain/cli/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 00:09:11.394478 nextstrain-cli-8.2.0/nextstrain/cli/aws/cognito/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/aws/cognito/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11366 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/aws/cognito/srp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/browser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 00:09:11.398478 nextstrain-cli-8.2.0/nextstrain/cli/command/
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/command/authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    16574 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/command/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/command/check_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/command/debugger.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/command/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/command/init_shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/command/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/command/logout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 00:09:11.398478 nextstrain-cli-8.2.0/nextstrain/cli/command/remote/
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/command/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/command/remote/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/command/remote/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/command/remote/ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/command/remote/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/command/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/command/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/command/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/command/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    16451 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/command/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/command/whoami.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/console.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     7623 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/gzip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/hostenv.py
--rw-r--r--   0 runner    (1001) docker     (127)    15260 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/net.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 00:09:11.398478 nextstrain-cli-8.2.0/nextstrain/cli/remote/
--rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35020 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/remote/nextstrain_dot_org.py
--rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/remote/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 00:09:11.402478 nextstrain-cli-8.2.0/nextstrain/cli/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/resources/bashrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 00:09:11.402478 nextstrain-cli-8.2.0/nextstrain/cli/rst/
--rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/rst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40693 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/rst/sphinx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 00:09:11.402478 nextstrain-cli-8.2.0/nextstrain/cli/runner/
--rw-r--r--   0 runner    (1001) docker     (127)    11804 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/runner/ambient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 00:09:11.402478 nextstrain-cli-8.2.0/nextstrain/cli/runner/aws_batch/
--rw-r--r--   0 runner    (1001) docker     (127)    19979 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/runner/aws_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/runner/aws_batch/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/runner/aws_batch/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/runner/aws_batch/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)    25739 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/runner/conda.py
--rw-r--r--   0 runner    (1001) docker     (127)    25250 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/runner/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)    20768 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/runner/singularity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/url.py
--rw-r--r--   0 runner    (1001) docker     (127)    22157 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/nextstrain/cli/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 00:09:11.402478 nextstrain-cli-8.2.0/nextstrain_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-02-07 00:09:11.000000 nextstrain-cli-8.2.0/nextstrain_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-02-07 00:09:11.000000 nextstrain-cli-8.2.0/nextstrain_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 00:09:11.000000 nextstrain-cli-8.2.0/nextstrain_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-07 00:09:11.000000 nextstrain-cli-8.2.0/nextstrain_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-02-07 00:09:11.000000 nextstrain-cli-8.2.0/nextstrain_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-07 00:09:11.000000 nextstrain-cli-8.2.0/nextstrain_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 00:09:11.406479 nextstrain-cli-8.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-02-07 00:09:00.000000 nextstrain-cli-8.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:04:19.404151 nextstrain_cli-8.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/LICENSE.cognito-srp
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/LICENSE.id3c
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/LICENSE.sphinx
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-30 20:04:19.400150 nextstrain_cli-8.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:04:19.384150 nextstrain_cli-8.3.0/nextstrain/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:04:19.392150 nextstrain_cli-8.3.0/nextstrain/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/argparse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:04:19.392150 nextstrain_cli-8.3.0/nextstrain/cli/authn/
+-rw-r--r--   0 runner    (1001) docker     (127)     8863 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/authn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/authn/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/authn/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30176 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/authn/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:04:19.392150 nextstrain_cli-8.3.0/nextstrain/cli/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:04:19.392150 nextstrain_cli-8.3.0/nextstrain/cli/aws/cognito/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/aws/cognito/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11366 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/aws/cognito/srp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/browser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:04:19.396150 nextstrain_cli-8.3.0/nextstrain/cli/command/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/command/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16574 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/command/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/command/check_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/command/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/command/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/command/init_shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/command/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/command/logout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:04:19.396150 nextstrain_cli-8.3.0/nextstrain/cli/command/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/command/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/command/remote/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/command/remote/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/command/remote/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/command/remote/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/command/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/command/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/command/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/command/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16451 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/command/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/command/whoami.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7623 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/gzip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/hostenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15260 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:04:19.396150 nextstrain_cli-8.3.0/nextstrain/cli/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35020 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/remote/nextstrain_dot_org.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/remote/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:04:19.396150 nextstrain_cli-8.3.0/nextstrain/cli/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/resources/bashrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:04:19.396150 nextstrain_cli-8.3.0/nextstrain/cli/rst/
+-rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/rst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40693 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/rst/sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:04:19.396150 nextstrain_cli-8.3.0/nextstrain/cli/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)    12318 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/runner/ambient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:04:19.400150 nextstrain_cli-8.3.0/nextstrain/cli/runner/aws_batch/
+-rw-r--r--   0 runner    (1001) docker     (127)    19979 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/runner/aws_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/runner/aws_batch/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/runner/aws_batch/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/runner/aws_batch/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25739 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/runner/conda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25250 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/runner/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20768 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/runner/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22157 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/nextstrain/cli/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:04:19.400150 nextstrain_cli-8.3.0/nextstrain_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-30 20:04:19.000000 nextstrain_cli-8.3.0/nextstrain_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-30 20:04:19.000000 nextstrain_cli-8.3.0/nextstrain_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:04:19.000000 nextstrain_cli-8.3.0/nextstrain_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-30 20:04:19.000000 nextstrain_cli-8.3.0/nextstrain_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-30 20:04:19.000000 nextstrain_cli-8.3.0/nextstrain_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 20:04:19.000000 nextstrain_cli-8.3.0/nextstrain_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 20:04:19.404151 nextstrain_cli-8.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-04-30 20:04:13.000000 nextstrain_cli-8.3.0/setup.py
```

### Comparing `nextstrain-cli-8.2.0/LICENSE` & `nextstrain_cli-8.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/LICENSE.cognito-srp` & `nextstrain_cli-8.3.0/LICENSE.cognito-srp`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/LICENSE.id3c` & `nextstrain_cli-8.3.0/LICENSE.id3c`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/LICENSE.sphinx` & `nextstrain_cli-8.3.0/LICENSE.sphinx`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/PKG-INFO` & `nextstrain_cli-8.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextstrain-cli
-Version: 8.2.0
+Version: 8.3.0
 Summary: Nextstrain command-line tool
 Home-page: https://docs.nextstrain.org/projects/cli/
 Author: Thomas Sibley
 Author-email: tsibley@fredhutch.org
 License: MIT
 Project-URL: Bug Reports, https://github.com/nextstrain/cli/issues
 Project-URL: Change Log, https://github.com/nextstrain/cli/blob/master/CHANGES.md
```

### Comparing `nextstrain-cli-8.2.0/README.md` & `nextstrain_cli-8.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/__init__.py` & `nextstrain_cli-8.3.0/nextstrain/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/__main__.py` & `nextstrain_cli-8.3.0/nextstrain/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/argparse.py` & `nextstrain_cli-8.3.0/nextstrain/cli/argparse.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/authn/__init__.py` & `nextstrain_cli-8.3.0/nextstrain/cli/authn/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/authn/configuration.py` & `nextstrain_cli-8.3.0/nextstrain/cli/authn/configuration.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/authn/errors.py` & `nextstrain_cli-8.3.0/nextstrain/cli/authn/errors.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/authn/session.py` & `nextstrain_cli-8.3.0/nextstrain/cli/authn/session.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/aws/__init__.py` & `nextstrain_cli-8.3.0/nextstrain/cli/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/aws/cognito/srp.py` & `nextstrain_cli-8.3.0/nextstrain/cli/aws/cognito/srp.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/browser.py` & `nextstrain_cli-8.3.0/nextstrain/cli/browser.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/command/__init__.py` & `nextstrain_cli-8.3.0/nextstrain/cli/command/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/command/authorization.py` & `nextstrain_cli-8.3.0/nextstrain/cli/command/authorization.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/command/build.py` & `nextstrain_cli-8.3.0/nextstrain/cli/command/build.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/command/check_setup.py` & `nextstrain_cli-8.3.0/nextstrain/cli/command/check_setup.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/command/deploy.py` & `nextstrain_cli-8.3.0/nextstrain/cli/command/deploy.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/command/init_shell.py` & `nextstrain_cli-8.3.0/nextstrain/cli/command/init_shell.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/command/login.py` & `nextstrain_cli-8.3.0/nextstrain/cli/command/login.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/command/logout.py` & `nextstrain_cli-8.3.0/nextstrain/cli/command/logout.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/command/remote/__init__.py` & `nextstrain_cli-8.3.0/nextstrain/cli/command/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/command/remote/delete.py` & `nextstrain_cli-8.3.0/nextstrain/cli/command/remote/delete.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/command/remote/download.py` & `nextstrain_cli-8.3.0/nextstrain/cli/command/remote/download.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/command/remote/ls.py` & `nextstrain_cli-8.3.0/nextstrain/cli/command/remote/ls.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/command/remote/upload.py` & `nextstrain_cli-8.3.0/nextstrain/cli/command/remote/upload.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/command/setup.py` & `nextstrain_cli-8.3.0/nextstrain/cli/command/setup.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/command/shell.py` & `nextstrain_cli-8.3.0/nextstrain/cli/command/shell.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/command/update.py` & `nextstrain_cli-8.3.0/nextstrain/cli/command/update.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/command/version.py` & `nextstrain_cli-8.3.0/nextstrain/cli/command/version.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/command/view.py` & `nextstrain_cli-8.3.0/nextstrain/cli/command/view.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/command/whoami.py` & `nextstrain_cli-8.3.0/nextstrain/cli/command/whoami.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/config.py` & `nextstrain_cli-8.3.0/nextstrain/cli/config.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/console.py` & `nextstrain_cli-8.3.0/nextstrain/cli/console.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/debug.py` & `nextstrain_cli-8.3.0/nextstrain/cli/debug.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/env.py` & `nextstrain_cli-8.3.0/nextstrain/cli/env.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/errors.py` & `nextstrain_cli-8.3.0/nextstrain/cli/errors.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/gzip.py` & `nextstrain_cli-8.3.0/nextstrain/cli/gzip.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/hostenv.py` & `nextstrain_cli-8.3.0/nextstrain/cli/hostenv.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/markdown.py` & `nextstrain_cli-8.3.0/nextstrain/cli/markdown.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/net.py` & `nextstrain_cli-8.3.0/nextstrain/cli/net.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/paths.py` & `nextstrain_cli-8.3.0/nextstrain/cli/paths.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/remote/__init__.py` & `nextstrain_cli-8.3.0/nextstrain/cli/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/remote/nextstrain_dot_org.py` & `nextstrain_cli-8.3.0/nextstrain/cli/remote/nextstrain_dot_org.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/remote/s3.py` & `nextstrain_cli-8.3.0/nextstrain/cli/remote/s3.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/resources/__init__.py` & `nextstrain_cli-8.3.0/nextstrain/cli/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/resources/bashrc` & `nextstrain_cli-8.3.0/nextstrain/cli/resources/bashrc`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/rst/__init__.py` & `nextstrain_cli-8.3.0/nextstrain/cli/rst/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/rst/sphinx.py` & `nextstrain_cli-8.3.0/nextstrain/cli/rst/sphinx.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/runner/__init__.py` & `nextstrain_cli-8.3.0/nextstrain/cli/runner/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
-from argparse import ArgumentParser
+import os
+from argparse import ArgumentParser, ArgumentTypeError
 from typing import cast, List, Union, TYPE_CHECKING
 # TODO: Use typing.TypeAlias once Python 3.10 is the minimum supported version.
 from typing_extensions import TypeAlias
 from . import (
     docker as __docker,
     conda as __conda,
     singularity as __singularity,
@@ -169,14 +170,15 @@
         metavar = "<path>",
         help    = "Set environment variables from the envdir at ``<path>``. "
                   "May be specified more than once. "
                   "An envdir is a directory containing files describing environment variables. "
                   "Each filename is used as the variable name. "
                   "The first line of the contents of each file is used as the variable value. "
                   "When this option or :option:`--env` is given, the default behaviour of automatically passing thru several \"well-known\" variables is disabled. "
+                  f"Envdirs may also be specified by setting ``NEXTSTRAIN_RUNTIME_ENVDIRS`` in the environment to a ``{os.pathsep}``-separated list of paths. "
                   "See the description of :option:`--env` for more details. "
                   f"{SKIP_AUTO_DEFAULT_IN_HELP}",
         type    = DirectoryPath,
         action  = "append",
         default = [])
 
     # Development arguments for all runners
@@ -260,14 +262,22 @@
             """)
 
     # Account for potentially different defaults for --image depending on the
     # selected runner.
     if opts.__runner__ is singularity and opts.image is docker.DEFAULT_IMAGE: # type: ignore
         opts.image = singularity.DEFAULT_IMAGE # type: ignore
 
+    if envdirs := os.environ.get("NEXTSTRAIN_RUNTIME_ENVDIRS"):
+        try:
+            opts.envdir = [
+                *[DirectoryPath(d) for d in envdirs.split(os.pathsep) if d],
+                *opts.envdir ]
+        except ArgumentTypeError as err:
+            raise UserError(f"{err} (in NEXTSTRAIN_RUNTIME_ENVDIRS)")
+
     # Add env from automatically forwarded vars xor from --envdir and --env
     # without overriding values explicitly set by our commands' own internals
     # (i.e. the callers of this function).
     if opts.envdir or opts.env:
         extra_env = {
             **dict(env.from_dirs(opts.envdir)),
             **dict(env.from_vars(opts.env)),
```

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/runner/ambient.py` & `nextstrain_cli-8.3.0/nextstrain/cli/runner/ambient.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/runner/aws_batch/__init__.py` & `nextstrain_cli-8.3.0/nextstrain/cli/runner/aws_batch/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/runner/aws_batch/jobs.py` & `nextstrain_cli-8.3.0/nextstrain/cli/runner/aws_batch/jobs.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/runner/aws_batch/logs.py` & `nextstrain_cli-8.3.0/nextstrain/cli/runner/aws_batch/logs.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/runner/aws_batch/s3.py` & `nextstrain_cli-8.3.0/nextstrain/cli/runner/aws_batch/s3.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/runner/conda.py` & `nextstrain_cli-8.3.0/nextstrain/cli/runner/conda.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/runner/docker.py` & `nextstrain_cli-8.3.0/nextstrain/cli/runner/docker.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/runner/singularity.py` & `nextstrain_cli-8.3.0/nextstrain/cli/runner/singularity.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/types.py` & `nextstrain_cli-8.3.0/nextstrain/cli/types.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/url.py` & `nextstrain_cli-8.3.0/nextstrain/cli/url.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/util.py` & `nextstrain_cli-8.3.0/nextstrain/cli/util.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain/cli/volume.py` & `nextstrain_cli-8.3.0/nextstrain/cli/volume.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain_cli.egg-info/PKG-INFO` & `nextstrain_cli-8.3.0/nextstrain_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextstrain-cli
-Version: 8.2.0
+Version: 8.3.0
 Summary: Nextstrain command-line tool
 Home-page: https://docs.nextstrain.org/projects/cli/
 Author: Thomas Sibley
 Author-email: tsibley@fredhutch.org
 License: MIT
 Project-URL: Bug Reports, https://github.com/nextstrain/cli/issues
 Project-URL: Change Log, https://github.com/nextstrain/cli/blob/master/CHANGES.md
```

### Comparing `nextstrain-cli-8.2.0/nextstrain_cli.egg-info/SOURCES.txt` & `nextstrain_cli-8.3.0/nextstrain_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/nextstrain_cli.egg-info/requires.txt` & `nextstrain_cli-8.3.0/nextstrain_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-8.2.0/setup.py` & `nextstrain_cli-8.3.0/setup.py`

 * *Files identical despite different names*

