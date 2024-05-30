# Comparing `tmp/zerotk.zops-0.5.3.tar.gz` & `tmp/zerotk_zops-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zerotk.zops-0.5.3.tar", last modified: Tue Dec 12 22:26:52 2017, max compression
+gzip compressed data, was "zerotk_zops-2.0.0b1.tar", max compression
```

## Comparing `zerotk.zops-0.5.3.tar` & `zerotk_zops-2.0.0b1.tar`

### file list

```diff
@@ -1,24 +1,94 @@
-drwxr-xr-x   0 aandrade (1298332388) 1010544492        0 2017-12-12 22:26:52.000000 zerotk.zops-0.5.3/
-drwxr-xr-x   0 aandrade (1298332388) 1010544492        0 2017-12-12 22:26:52.000000 zerotk.zops-0.5.3/.github/
--rw-r--r--   0 aandrade (1298332388) 1010544492      321 2017-11-14 12:57:21.000000 zerotk.zops-0.5.3/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 aandrade (1298332388) 1010544492      794 2017-11-14 12:57:21.000000 zerotk.zops-0.5.3/.gitignore
--rw-r--r--   0 aandrade (1298332388) 1010544492     1077 2017-11-14 12:57:21.000000 zerotk.zops-0.5.3/LICENSE
--rw-r--r--   0 aandrade (1298332388) 1010544492      802 2017-12-12 22:26:52.000000 zerotk.zops-0.5.3/PKG-INFO
--rw-r--r--   0 aandrade (1298332388) 1010544492      751 2017-11-14 12:57:21.000000 zerotk.zops-0.5.3/README.md
--rw-r--r--   0 aandrade (1298332388) 1010544492       38 2017-12-12 22:26:52.000000 zerotk.zops-0.5.3/setup.cfg
--rw-r--r--   0 aandrade (1298332388) 1010544492     1245 2017-11-14 12:57:21.000000 zerotk.zops-0.5.3/setup.py
-drwxr-xr-x   0 aandrade (1298332388) 1010544492        0 2017-12-12 22:26:52.000000 zerotk.zops-0.5.3/tests/
--rw-r--r--   0 aandrade (1298332388) 1010544492      195 2017-11-14 12:57:21.000000 zerotk.zops-0.5.3/tests/test_zops.py
-drwxr-xr-x   0 aandrade (1298332388) 1010544492        0 2017-12-12 22:26:52.000000 zerotk.zops-0.5.3/zerotk/
--rw-r--r--   0 aandrade (1298332388) 1010544492      154 2017-11-14 12:57:21.000000 zerotk.zops-0.5.3/zerotk/__init__.py
-drwxr-xr-x   0 aandrade (1298332388) 1010544492        0 2017-12-12 22:26:52.000000 zerotk.zops-0.5.3/zerotk/zops/
--rw-r--r--   0 aandrade (1298332388) 1010544492     2025 2017-12-07 12:13:48.000000 zerotk.zops-0.5.3/zerotk/zops/__init__.py
--rw-r--r--   0 aandrade (1298332388) 1010544492      291 2017-11-14 12:57:21.000000 zerotk.zops-0.5.3/zerotk/zops/cli.py
-drwxr-xr-x   0 aandrade (1298332388) 1010544492        0 2017-12-12 22:26:52.000000 zerotk.zops-0.5.3/zerotk.zops.egg-info/
--rw-r--r--   0 aandrade (1298332388) 1010544492        1 2017-12-12 22:26:51.000000 zerotk.zops-0.5.3/zerotk.zops.egg-info/dependency_links.txt
--rw-r--r--   0 aandrade (1298332388) 1010544492       47 2017-12-12 22:26:51.000000 zerotk.zops-0.5.3/zerotk.zops.egg-info/entry_points.txt
--rw-r--r--   0 aandrade (1298332388) 1010544492        7 2017-12-12 22:26:51.000000 zerotk.zops-0.5.3/zerotk.zops.egg-info/namespace_packages.txt
--rw-r--r--   0 aandrade (1298332388) 1010544492      802 2017-12-12 22:26:51.000000 zerotk.zops-0.5.3/zerotk.zops.egg-info/PKG-INFO
--rw-r--r--   0 aandrade (1298332388) 1010544492       20 2017-12-12 22:26:51.000000 zerotk.zops-0.5.3/zerotk.zops.egg-info/requires.txt
--rw-r--r--   0 aandrade (1298332388) 1010544492      400 2017-12-12 22:26:52.000000 zerotk.zops-0.5.3/zerotk.zops.egg-info/SOURCES.txt
--rw-r--r--   0 aandrade (1298332388) 1010544492        7 2017-12-12 22:26:51.000000 zerotk.zops-0.5.3/zerotk.zops.egg-info/top_level.txt
+-rw-r--r--   0        0        0      751 2024-05-24 18:17:35.811234 zerotk_zops-2.0.0b1/README.md
+-rw-r--r--   0        0        0     1327 2024-05-30 12:18:27.900271 zerotk_zops-2.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/__init__.py
+-rw-r--r--   0        0        0        9 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/_tests/test_gitignored/test_00/.gitignore
+-rw-r--r--   0        0        0        0 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/_tests/test_gitignored/test_00/git-root.txt
+-rw-r--r--   0        0        0        0 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/_tests/test_gitignored/test_00/included/alpha.txt
+-rw-r--r--   0        0        0        0 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/_tests/test_gitignored/test_00/placed-holder.txt
+-rw-r--r--   0        0        0     1874 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/_tests/test_gitignored.py
+-rw-r--r--   0        0        0      682 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/_tests/test_text.py
+-rw-r--r--   0        0        0     1280 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/_tests/test_url.py
+-rw-r--r--   0        0        0     5109 2024-05-25 02:33:50.314092 zerotk_zops-2.0.0b1/src/zerotk/_tests/test_wires.py
+-rw-r--r--   0        0        0     4286 2024-05-29 20:11:53.156678 zerotk_zops-2.0.0b1/src/zerotk/_tests/test_wiring.py
+-rw-r--r--   0        0        0      940 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/_tests/test_yaml.py
+-rw-r--r--   0        0        0       40 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/clikit/__init__.py
+-rw-r--r--   0        0        0    24241 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/clikit/app.py
+-rw-r--r--   0        0        0    15144 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/clikit/command.py
+-rw-r--r--   0        0        0    13446 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/clikit/console.py
+-rw-r--r--   0        0        0      138 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/easyfs/__init__.py
+-rw-r--r--   0        0        0    66411 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/easyfs/_easyfs.py
+-rw-r--r--   0        0        0      303 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/easyfs/_easyfs_win32.py
+-rw-r--r--   0        0        0     4981 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/easyfs/_exceptions.py
+-rw-r--r--   0        0        0     6270 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/easyfs/fixtures.py
+-rw-r--r--   0        0        0     3267 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/gitignored.py
+-rw-r--r--   0        0        0      746 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/path.py
+-rw-r--r--   0        0        0     1774 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/pushpop.py
+-rw-r--r--   0        0        0    12653 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/text.py
+-rw-r--r--   0        0        0      599 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/url.py
+-rw-r--r--   0        0        0      187 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/version.py
+-rw-r--r--   0        0        0     2276 2024-05-27 12:54:56.696787 zerotk_zops-2.0.0b1/src/zerotk/wires.py
+-rw-r--r--   0        0        0      537 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zerotk/yaml.py
+-rw-r--r--   0        0        0     2030 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/__init__.py
+-rw-r--r--   0        0        0     1840 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/anatomy/__init__.py
+-rw-r--r--   0        0        0      341 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/anatomy/assertions.py
+-rw-r--r--   0        0        0     2932 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/anatomy/cli_commands.py
+-rw-r--r--   0        0        0        0 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/anatomy/layers/__init__.py
+-rw-r--r--   0        0        0     7586 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/anatomy/layers/feature.py
+-rw-r--r--   0        0        0     2503 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/anatomy/layers/playbook.py
+-rw-r--r--   0        0        0    14196 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/anatomy/layers/tree.py
+-rw-r--r--   0        0        0        0 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/aws/__init__.py
+-rw-r--r--   0        0        0     8367 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/aws/autoscaling.py
+-rw-r--r--   0        0        0     1204 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/aws/cli.py
+-rw-r--r--   0        0        0    30355 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/aws/cli_commands.py
+-rw-r--r--   0        0        0     1017 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/aws/cli_config.py
+-rw-r--r--   0        0        0    23698 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/aws/cluster.py
+-rw-r--r--   0        0        0     4926 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/aws/config.yml
+-rw-r--r--   0        0        0      884 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/aws/ecs.py
+-rw-r--r--   0        0        0     4430 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/aws/image.py
+-rw-r--r--   0        0        0     1095 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/aws/instance.py
+-rw-r--r--   0        0        0     1544 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/aws/utils.py
+-rw-r--r--   0        0        0      431 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/aws/utils_click.py
+-rw-r--r--   0        0        0     1704 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/aws/utils_shell.py
+-rw-r--r--   0        0        0        0 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/codegen/__init__.py
+-rw-r--r--   0        0        0      227 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/codegen/cli.py
+-rw-r--r--   0        0        0     8955 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/codegen/cli_commands.py
+-rw-r--r--   0        0        0       31 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/terraform/__init__.py
+-rw-r--r--   0        0        0      213 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/terraform/__main__.py
+-rw-r--r--   0        0        0     6596 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/terraform/cli_commands.py
+-rw-r--r--   0        0        0      462 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/terraformer/__init__.py
+-rw-r--r--   0        0        0      160 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/terraformer/_version.py
+-rw-r--r--   0        0        0     8004 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/terraformer/apply_log.py
+-rw-r--r--   0        0        0       40 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/terraformer/authentication.py
+-rw-r--r--   0        0        0        0 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/terraformer/conf/__init__.py
+-rw-r--r--   0        0        0      255 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/terraformer/conf/settings.py
+-rw-r--r--   0        0        0      519 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/terraformer/exceptions.py
+-rw-r--r--   0        0        0     3118 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/terraformer/mixins.py
+-rw-r--r--   0        0        0     5150 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/terraformer/plan.py
+-rw-r--r--   0        0        0       27 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/terraformer/py.typed
+-rw-r--r--   0        0        0       60 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/terraformer/settings.py
+-rw-r--r--   0        0        0     4966 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zops/terraformer/workspace.py
+-rw-r--r--   0        0        0        0 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zz/__init__.py
+-rw-r--r--   0        0        0      249 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zz/__main__.py
+-rw-r--r--   0        0        0     2106 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zz/anatomy/__init__.py
+-rw-r--r--   0        0        0      337 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zz/anatomy/assertions.py
+-rw-r--r--   0        0        0        0 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zz/anatomy/layers/__init__.py
+-rw-r--r--   0        0        0     7586 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zz/anatomy/layers/feature.py
+-rw-r--r--   0        0        0     2499 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zz/anatomy/layers/playbook.py
+-rw-r--r--   0        0        0     8210 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zz/anatomy/layers/tree.py
+-rw-r--r--   0        0        0     2173 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zz/cli/aws.py
+-rw-r--r--   0        0        0      326 2024-05-29 12:24:01.405903 zerotk_zops-2.0.0b1/src/zz/cli/codegen.py
+-rw-r--r--   0        0        0     3134 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zz/cli/test.py
+-rw-r--r--   0        0        0     1673 2024-05-29 11:58:31.176058 zerotk_zops-2.0.0b1/src/zz/cli/tf.py
+-rw-r--r--   0        0        0     2326 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zz/codegen.py
+-rw-r--r--   0        0        0        0 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zz/services/__init__.py
+-rw-r--r--   0        0        0     2675 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zz/services/aws_provider.py
+-rw-r--r--   0        0        0      734 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zz/services/config.py
+-rw-r--r--   0        0        0     2982 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zz/services/console.py
+-rw-r--r--   0        0        0     1631 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zz/services/filesystem.py
+-rw-r--r--   0        0        0     1851 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zz/services/formatter.py
+-rw-r--r--   0        0        0      461 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zz/services/requests.py
+-rw-r--r--   0        0        0     6839 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zz/services/template_engine.py
+-rw-r--r--   0        0        0      554 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zz/services/terraform.py
+-rw-r--r--   0        0        0     9461 2024-05-24 22:00:17.239203 zerotk_zops-2.0.0b1/src/zz/terraform.py
+-rw-r--r--   0        0        0     1877 1970-01-01 00:00:00.000000 zerotk_zops-2.0.0b1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `zerotk.zops-0.5.3/README.md` & `zerotk_zops-2.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `zerotk.zops-0.5.3/zerotk/zops/__init__.py` & `zerotk_zops-2.0.0b1/src/zops/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,87 +1,92 @@
 # -*- coding: utf-8 -*-
 
 
 def setenv(name, value):
     import os
+
     os.environ[name] = value
-    Console.setting('{}={}'.format(name, os.environ[name]))
+    Console.setting("{}={}".format(name, os.environ[name]))
 
 
 def add_pythonpath(value):
-    import sys
     import os
+    import sys
+
     value = os.path.normpath(value)
     sys.path.insert(0, value)
-    Console.setting('SYS.PATH={}'.format(value))
+    Console.setting("SYS.PATH={}".format(value))
 
 
 def call_main(main_func, *argv):
     import sys
+
     old_argv = sys.argv
-    sys.argv = [''] + list(argv)
+    sys.argv = [""] + list(argv)
     try:
         return main_func()
     except SystemExit as e:
         return e.code
     finally:
         sys.argv = old_argv
 
 
 def ensure_dir(path):
     import os
+
     os.makedirs(path, exist_ok=True)
-    Console.setting('DIRECTORY: {}'.format(path))
+    Console.setting("DIRECTORY: {}".format(path))
 
 
 class Console(object):
 
-    TITLE_COLOR = 'yellow'
-    EXECUTION_COLOR = 'green'
-    SETTING_COLOR = 'blue'
-    OUTPUT_COLOR = 'white'
-    INFO_COLOR = 'white'
-    DEBUG_COLOR = 'red'
+    TITLE_COLOR = "yellow"
+    EXECUTION_COLOR = "green"
+    SETTING_COLOR = "blue"
+    OUTPUT_COLOR = "white"
+    INFO_COLOR = "white"
+    DEBUG_COLOR = "red"
 
     @classmethod
     def title(cls, *args):
-        cls._secho(['#'] + list(args), cls.TITLE_COLOR)
+        cls._secho(["#"] + list(args), cls.TITLE_COLOR)
 
     @classmethod
     def execution(cls, *args):
-        cls._secho(['$'] + list(args), cls.EXECUTION_COLOR)
+        cls._secho(["$"] + list(args), cls.EXECUTION_COLOR)
 
     @classmethod
     def setting(cls, *args):
-        cls._secho(['!'] + list(args), cls.SETTING_COLOR)
+        cls._secho(["!"] + list(args), cls.SETTING_COLOR)
 
     @classmethod
     def item(cls, *args, ident=0):
-        prefix = cls._idented('*', ident)
+        prefix = cls._idented("*", ident)
         cls._secho([prefix] + list(args), cls.OUTPUT_COLOR)
 
     @classmethod
     def output(cls, *args):
         cls._secho(args, cls.OUTPUT_COLOR)
 
     @classmethod
     def response(cls, *args):
-        cls._secho(['>'] + list(args), cls.OUTPUT_COLOR)
+        cls._secho([">"] + list(args), cls.OUTPUT_COLOR)
 
     @classmethod
     def info(cls, *args):
-        cls._secho(['\U0001F6C8'] + list(args), cls.INFO_COLOR)
+        cls._secho(["\U0001F6C8"] + list(args), cls.INFO_COLOR)
 
     @classmethod
     def debug(cls, *args):
-        cls._secho(['***'] + list(args), cls.DEBUG_COLOR)
+        cls._secho(["***"] + list(args), cls.DEBUG_COLOR)
 
     @classmethod
     def _idented(cls, text, ident):
-        return '  ' * ident + text
+        return "  " * ident + text
 
     @classmethod
-    def _secho(cls, args, fg, join_char=' '):
+    def _secho(cls, args, fg, join_char=" "):
         import click
+
         message = join_char.join(args)
-        message.rstrip('\n')
+        message.rstrip("\n")
         click.secho(message, fg=fg)
```

