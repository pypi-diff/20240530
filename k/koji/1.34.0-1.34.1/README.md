# Comparing `tmp/koji-1.34.0.tar.gz` & `tmp/koji-1.34.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koji-1.34.0.tar", last modified: Wed Jan 24 09:11:01 2024, max compression
+gzip compressed data, was "koji-1.34.1.tar", last modified: Thu May 30 11:20:17 2024, max compression
```

## Comparing `koji-1.34.0.tar` & `koji-1.34.1.tar`

### file list

```diff
@@ -1,47 +1,59 @@
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-01-24 09:11:01.811210 koji-1.34.0/
--rw-rw-r--   0 tkopecek  (1000) tkopecek  (1000)      796 2021-05-31 13:08:21.000000 koji-1.34.0/COPYING
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3063 2024-01-24 09:11:01.811210 koji-1.34.0/PKG-INFO
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     2216 2024-01-02 15:09:17.000000 koji-1.34.0/README.md
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-01-24 09:11:01.800210 koji-1.34.0/cli/
--rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    13338 2024-01-08 14:17:05.000000 koji-1.34.0/cli/koji
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-01-24 09:11:01.802210 koji-1.34.0/cli/koji_cli/
--rw-rw-r--   0 tkopecek  (1000) tkopecek  (1000)        0 2021-05-31 13:15:50.000000 koji-1.34.0/cli/koji_cli/__init__.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)   354937 2024-01-23 12:08:31.000000 koji-1.34.0/cli/koji_cli/commands.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    32640 2024-01-22 08:53:01.000000 koji-1.34.0/cli/koji_cli/lib.py
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-01-24 09:11:01.807210 koji-1.34.0/koji/
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)   138199 2024-01-22 08:53:01.000000 koji-1.34.0/koji/__init__.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       89 2024-01-24 09:02:23.000000 koji-1.34.0/koji/_version.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    14256 2023-11-29 10:56:34.000000 koji-1.34.0/koji/arch.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     2634 2023-03-13 16:13:03.000000 koji-1.34.0/koji/context.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    63681 2024-01-22 08:53:01.000000 koji-1.34.0/koji/daemon.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     7590 2024-01-22 08:53:01.000000 koji-1.34.0/koji/plugin.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    12060 2024-01-08 13:02:03.000000 koji-1.34.0/koji/policy.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     9441 2023-11-29 10:56:34.000000 koji-1.34.0/koji/rpmdiff.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     1154 2023-11-29 10:56:34.000000 koji-1.34.0/koji/server.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    33947 2024-01-08 14:17:05.000000 koji-1.34.0/koji/tasks.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    30846 2024-01-22 08:53:01.000000 koji-1.34.0/koji/util.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3575 2024-01-16 15:43:03.000000 koji-1.34.0/koji/xmlrpcplus.py
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-01-24 09:11:01.808210 koji-1.34.0/koji.egg-info/
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3063 2024-01-24 09:11:01.000000 koji-1.34.0/koji.egg-info/PKG-INFO
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)      677 2024-01-24 09:11:01.000000 koji-1.34.0/koji.egg-info/SOURCES.txt
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)        1 2024-01-24 09:11:01.000000 koji-1.34.0/koji.egg-info/dependency_links.txt
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       45 2024-01-24 09:11:01.000000 koji-1.34.0/koji.egg-info/requires.txt
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       31 2024-01-24 09:11:01.000000 koji-1.34.0/koji.egg-info/top_level.txt
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-01-24 09:11:01.799210 koji-1.34.0/plugins/
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-01-24 09:11:01.809210 koji-1.34.0/plugins/cli/
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3165 2023-11-29 10:56:34.000000 koji-1.34.0/plugins/cli/dud.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3607 2023-11-29 10:56:34.000000 koji-1.34.0/plugins/cli/kiwi.py
--rw-rw-r--   0 tkopecek  (1000) tkopecek  (1000)     7385 2023-11-29 11:55:30.000000 koji-1.34.0/plugins/cli/pungi.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     4759 2023-11-29 10:56:34.000000 koji-1.34.0/plugins/cli/runroot.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     2631 2023-11-29 10:56:34.000000 koji-1.34.0/plugins/cli/save_failed_tree.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     4972 2023-11-29 10:56:34.000000 koji-1.34.0/plugins/cli/sidetag_cli.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       38 2024-01-24 09:11:01.811210 koji-1.34.0/setup.cfg
--rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)     2467 2023-11-29 10:56:34.000000 koji-1.34.0/setup.py
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-01-24 09:11:01.809210 koji-1.34.0/tests/
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     1467 2023-11-29 10:56:34.000000 koji-1.34.0/tests/test_docs_version.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    26795 2023-11-29 10:56:34.000000 koji-1.34.0/tests/test_scm.py
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-01-24 09:11:01.811210 koji-1.34.0/util/
--rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    41460 2024-01-16 15:43:03.000000 koji-1.34.0/util/koji-gc
--rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    53664 2023-11-29 10:56:34.000000 koji-1.34.0/util/koji-shadow
--rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    11369 2024-01-23 12:08:31.000000 koji-1.34.0/util/koji-sweep-db
--rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    56348 2023-11-29 10:56:34.000000 koji-1.34.0/util/kojira
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-05-30 11:20:17.768725 koji-1.34.1/
+-rw-rw-r--   0 tkopecek  (1000) tkopecek  (1000)      796 2021-05-31 13:08:21.000000 koji-1.34.1/COPYING
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3063 2024-05-30 11:20:17.768725 koji-1.34.1/PKG-INFO
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     2216 2024-03-05 12:28:44.000000 koji-1.34.1/README.md
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-05-30 11:20:17.763725 koji-1.34.1/cli/
+-rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    13338 2024-03-25 10:23:32.000000 koji-1.34.1/cli/koji
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-05-30 11:20:17.763725 koji-1.34.1/cli/koji_cli/
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)        0 2024-02-21 12:05:04.000000 koji-1.34.1/cli/koji_cli/__init__.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)   356649 2024-05-30 11:20:13.000000 koji-1.34.1/cli/koji_cli/commands.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    32592 2024-05-06 11:41:24.000000 koji-1.34.1/cli/koji_cli/lib.py
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-05-30 11:20:17.766725 koji-1.34.1/koji/
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)   139313 2024-05-30 11:20:13.000000 koji-1.34.1/koji/__init__.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    66938 2024-04-24 12:57:03.000000 koji-1.34.1/koji/__init__.pyi
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       89 2024-05-30 11:11:41.000000 koji-1.34.1/koji/_version.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       82 2023-06-21 10:16:25.000000 koji-1.34.1/koji/_version.pyi
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    14256 2024-02-21 12:05:04.000000 koji-1.34.1/koji/arch.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     1348 2023-06-21 10:16:25.000000 koji-1.34.1/koji/arch.pyi
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     2634 2024-02-21 12:05:04.000000 koji-1.34.1/koji/context.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)      301 2023-06-21 10:16:25.000000 koji-1.34.1/koji/context.pyi
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    64208 2024-05-30 11:20:13.000000 koji-1.34.1/koji/daemon.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     4292 2024-03-26 14:42:02.000000 koji-1.34.1/koji/daemon.pyi
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     7590 2024-03-20 11:41:52.000000 koji-1.34.1/koji/plugin.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     1358 2024-03-26 14:45:09.000000 koji-1.34.1/koji/plugin.pyi
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    12060 2024-05-30 11:20:13.000000 koji-1.34.1/koji/policy.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     1428 2024-03-26 14:25:42.000000 koji-1.34.1/koji/policy.pyi
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)        8 2024-03-26 15:30:24.000000 koji-1.34.1/koji/py.typed
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     9441 2024-03-05 12:28:44.000000 koji-1.34.1/koji/rpmdiff.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)      756 2023-06-21 10:16:25.000000 koji-1.34.1/koji/rpmdiff.pyi
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     1154 2024-03-05 12:28:44.000000 koji-1.34.1/koji/server.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)      169 2023-06-21 10:16:25.000000 koji-1.34.1/koji/server.pyi
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    34036 2024-05-30 11:08:06.000000 koji-1.34.1/koji/tasks.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     5770 2024-03-26 14:32:23.000000 koji-1.34.1/koji/tasks.pyi
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    35966 2024-05-30 11:08:06.000000 koji-1.34.1/koji/util.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     6451 2024-05-23 10:47:54.000000 koji-1.34.1/koji/util.pyi
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3846 2024-05-06 11:41:24.000000 koji-1.34.1/koji/xmlrpcplus.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)      920 2024-03-26 15:13:04.000000 koji-1.34.1/koji/xmlrpcplus.pyi
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-05-30 11:20:17.767725 koji-1.34.1/koji.egg-info/
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3063 2024-05-30 11:20:17.000000 koji-1.34.1/koji.egg-info/PKG-INFO
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)      867 2024-05-30 11:20:17.000000 koji-1.34.1/koji.egg-info/SOURCES.txt
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)        1 2024-05-30 11:20:17.000000 koji-1.34.1/koji.egg-info/dependency_links.txt
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       56 2024-05-30 11:20:17.000000 koji-1.34.1/koji.egg-info/requires.txt
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       31 2024-05-30 11:20:17.000000 koji-1.34.1/koji.egg-info/top_level.txt
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-05-30 11:20:17.762725 koji-1.34.1/plugins/
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-05-30 11:20:17.767725 koji-1.34.1/plugins/cli/
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3165 2024-03-05 12:28:44.000000 koji-1.34.1/plugins/cli/dud.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3607 2024-05-20 09:41:52.000000 koji-1.34.1/plugins/cli/kiwi.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     4759 2024-03-05 12:28:44.000000 koji-1.34.1/plugins/cli/runroot.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     2631 2024-03-05 12:28:44.000000 koji-1.34.1/plugins/cli/save_failed_tree.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     4972 2024-03-05 12:28:44.000000 koji-1.34.1/plugins/cli/sidetag_cli.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       38 2024-05-30 11:20:17.768725 koji-1.34.1/setup.cfg
+-rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)     2434 2024-05-23 09:54:45.000000 koji-1.34.1/setup.py
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-05-30 11:20:17.767725 koji-1.34.1/tests/
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     1467 2024-03-05 12:28:44.000000 koji-1.34.1/tests/test_docs_version.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    26795 2024-03-05 12:28:44.000000 koji-1.34.1/tests/test_scm.py
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2024-05-30 11:20:17.768725 koji-1.34.1/util/
+-rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    41430 2024-05-06 11:41:24.000000 koji-1.34.1/util/koji-gc
+-rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    53664 2024-03-05 12:28:44.000000 koji-1.34.1/util/koji-shadow
+-rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    11387 2024-05-06 11:41:24.000000 koji-1.34.1/util/koji-sweep-db
+-rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    54617 2024-05-30 11:08:06.000000 koji-1.34.1/util/kojira
```

### Comparing `koji-1.34.0/COPYING` & `koji-1.34.1/COPYING`

 * *Files identical despite different names*

### Comparing `koji-1.34.0/PKG-INFO` & `koji-1.34.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koji
-Version: 1.34.0
+Version: 1.34.1
 Summary: Koji is a system for building and tracking RPMS. The base package contains shared libraries and the command-line interface.
 Home-page: http://pagure.io/koji/
 Author: Koji developers
 Author-email: koji-devel@lists.fedorahosted.org
 License: LGPLv2 and GPLv2+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `koji-1.34.0/README.md` & `koji-1.34.1/README.md`

 * *Files identical despite different names*

### Comparing `koji-1.34.0/cli/koji` & `koji-1.34.1/cli/koji`

 * *Files identical despite different names*

### Comparing `koji-1.34.0/cli/koji_cli/commands.py` & `koji-1.34.1/cli/koji_cli/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,17 +320,16 @@
     try:
         channel_id = session.addChannel(channel_name, description=options.description)
     except koji.GenericError as ex:
         msg = str(ex)
         if 'channel %s already exists' % channel_name in msg:
             error("channel %s already exists" % channel_name)
         elif 'Invalid method:' in msg:
-            version = session.getKojiVersion()
             error("addChannel is available on hub from Koji 1.26 version, your version is %s" %
-                  version)
+                  session.hub_version_str)
         else:
             error(msg)
     print("%s added: id %d" % (args[0], channel_id))
 
 
 def handle_edit_channel(goptions, session, args):
     "[admin] Edit a channel"
@@ -352,17 +351,16 @@
         error("No such channel: %s" % args[0])
     result = None
     try:
         result = session.editChannel(args[0], **vals)
     except koji.GenericError as ex:
         msg = str(ex)
         if 'Invalid method:' in msg:
-            version = session.getKojiVersion()
             error("editChannel is available on hub from Koji 1.26 version, your version is %s" %
-                  version)
+                  session.hub_version_str)
         else:
             warn(msg)
     if not result:
         error("No changes made, please correct the command line")
 
 
 def handle_enable_channel(goptions, session, args):
@@ -6291,22 +6289,14 @@
     parser.add_option("--justone", action="store_true", help="Do not cancel subtasks")
     parser.add_option("--full", action="store_true", help="Full cancellation (admin only)")
     parser.add_option("--force", action="store_true", help="Allow subtasks with --full")
     (options, args) = parser.parse_args(args)
     if len(args) == 0:
         parser.error("You must specify at least one task id or build")
     activate_session(session, goptions)
-    older_hub = False
-    try:
-        hub_version = session.getKojiVersion()
-        v = tuple([int(x) for x in hub_version.split('.')])
-        if v < (1, 33, 0):
-            older_hub = True
-    except koji.GenericError:
-        older_hub = True
     tlist = []
     blist = []
     for arg in args:
         try:
             tlist.append(int(arg))
         except ValueError:
             try:
@@ -6325,15 +6315,15 @@
             elif options.full:
                 remote_fn = m.cancelTaskFull
                 if options.force:
                     opts['strict'] = False
             for task_id in tlist:
                 results.append(remote_fn(task_id, **opts))
         for build in blist:
-            if not older_hub:
+            if session.hub_version >= (1, 33, 0):
                 results.append(m.cancelBuild(build, strict=True))
             else:
                 results.append(m.cancelBuild(build))
 
     err = False
     for r in results:
         if isinstance(r._result, dict):
@@ -7571,15 +7561,15 @@
     activate_session(session, options)
     u = session.getLoggedInUser()
     if not u:
         print("Not authenticated")
         u = {'name': 'anonymous user'}
     print("%s, %s!" % (_printable_unicode(random.choice(greetings)), u["name"]))
     print("")
-    print("You are using the hub at %s" % session.baseurl)
+    print("You are using the hub at %s (Koji %s)" % (session.baseurl, session.hub_version_str))
     authtype = u.get('authtype', getattr(session, 'authtype', None))
     if authtype == koji.AUTHTYPES['NORMAL']:
         print("Authenticated via password")
     elif authtype == koji.AUTHTYPES['GSSAPI']:
         print("Authenticated via GSSAPI")
     elif authtype == koji.AUTHTYPES['KERBEROS']:
         print("Authenticated via Kerberos principal %s" % session.krb_principal)
@@ -7998,14 +7988,16 @@
     parser.add_option("-t", "--task", action="store", type=int, default=None,
                       help="Limit data to given task id")
     parser.add_option("--host", action="store", default=None,
                       help="Limit data to given builder id")
     parser.add_option("--state", action="store", type='choice', default=None,
                       choices=[x for x in koji.TASK_STATES.keys()],
                       help="Limit data to task state")
+    parser.add_option("--limit", action="store", type=int, default=100,
+                      help="Limit data to last N items [default: %default]")
     (options, args) = parser.parse_args(args)
     if len(args) > 0:
         parser.error("This command takes no arguments")
 
     ensure_connection(session, goptions)
 
     host_id = None
@@ -8020,18 +8012,35 @@
     if options.task:
         clauses.append(('task_id', options.task))
     if options.host:
         clauses.append(('host_id', options.host))
     if options.state:
         clauses.append(('state', koji.TASK_STATES[options.state]))
 
-    runs = session.scheduler.getTaskRuns(
-        clauses=clauses,
-        fields=('task_id', 'host_name', 'state', 'create_ts', 'start_ts', 'completion_ts')
-    )
+    fields = ('id', 'task_id', 'host_name', 'state', 'create_ts', 'start_ts', 'completion_ts')
+    kwargs = {'clauses': clauses, 'fields': fields}
+    if session.hub_version < (1, 34, 0):
+        error("Hub version is %s and doesn't support scheduler methods "
+              "introduced in 1.34." % session.hub_version_str)
+    if options.limit is not None:
+        if session.hub_version >= (1, 34, 1):
+            kwargs['opts'] = {'order': '-id', 'limit': options.limit}
+    runs = session.scheduler.getTaskRuns(**kwargs)
+
+    if options.limit is not None:
+        if session.hub_version >= (1, 34, 1):
+            # server did it for us, but we need to reverse
+            runs = reversed(runs)
+        else:
+            # emulate limit
+            runs = runs[-options.limit:]
+    if session.hub_version < (1, 34, 1):
+        # emulate order
+        runs.sort(key=lambda r: r['id'])
+
     mask = '%(task_id)-9s %(host_name)-20s %(state)-7s ' \
            '%(create_ts)-17s %(start_ts)-17s %(completion_ts)-17s'
     if not goptions.quiet:
         header = mask % {
             'task_id': 'Task',
             'host_name': 'Host',
             'state': 'State',
@@ -8064,17 +8073,21 @@
                       help="Filter by task ID")
     parser.add_option("--host", type="str", action="store",
                       help="Filter by host (name/ID)")
     parser.add_option("--from", type="float", action="store", dest="from_ts",
                       help="Logs from given timestamp")
     parser.add_option("--to", type="float", action="store", dest="to_ts",
                       help="Logs until given timestamp (included)")
+    parser.add_option("--limit", action="store", type=int, default=None,
+                      help="Limit data to last N items. [default: %default]")
     (options, args) = parser.parse_args(args)
     if len(args) != 0:
         parser.error("There are no arguments for this command")
+    if options.from_ts and options.to_ts and options.limit is not None:
+        parser.error("If both --from and --to are used, --limit shouldn't be used")
 
     clauses = []
     if options.task:
         clauses.append(['task_id', options.task])
     if options.host:
         try:
             host_id = int(options.host)
@@ -8082,20 +8095,40 @@
             host_id = session.getHost(options.host)['id']
         clauses.append(['host_id', host_id])
     if options.from_ts:
         clauses.append(['msg_ts', '>=', options.from_ts])
     if options.to_ts:
         clauses.append(['msg_ts', '<', options.to_ts])
 
-    logs = session.scheduler.getLogMessages(clauses, fields=('task_id', 'host_id', 'host_name',
-                                                             'msg_ts', 'msg'))
+    fields = ('id', 'task_id', 'host_id', 'host_name', 'msg_ts', 'msg')
+    kwargs = {'clauses': clauses, 'fields': fields}
+    if session.hub_version < (1, 34, 0):
+        error("Hub version is %s and doesn't support scheduler methods "
+              "introduced in 1.34." % session.hub_version_str)
+    if options.limit is not None:
+        if session.hub_version >= (1, 34, 1):
+            kwargs['opts'] = {'order': '-id', 'limit': options.limit}
+    logs = session.scheduler.getLogMessages(**kwargs)
+
+    if options.limit is not None:
+        if session.hub_version >= (1, 34, 1):
+            # server did it for us, but we need to reverse
+            # don't use reversed() as it will be exhausted after modification loop later
+            logs.reverse()
+        else:
+            # emulate limit
+            logs = logs[-options.limit:]
+    if session.hub_version < (1, 34, 1):
+        # emulate order
+        logs.sort(key=lambda r: r['id'])
+
     for log in logs:
         log['time'] = time.asctime(time.localtime(log['msg_ts']))
 
-    mask = ("%(task_id)s\t%(host_name)s\t%(time)s\t%(msg)s")
+    mask = ("%(task_id)-10s %(host_name)-20s %(time)-25s %(msg)-30s")
     if not goptions.quiet:
         h = mask % {
             'task_id': 'Task',
             'host_name': 'Host',
             'time': 'Time',
             'msg': 'Message',
         }
```

### Comparing `koji-1.34.0/cli/koji_cli/lib.py` & `koji-1.34.1/cli/koji_cli/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from six.moves import range
 
 import koji
 # import parse_arches to current namespace for backward compatibility
 from koji import parse_arches
 from koji import _  # noqa: F401
 from koji.util import md5_constructor, to_list
-from koji.xmlrpcplus import xmlrpc_client
 
 
 # for compatibility with plugins based on older version of lib
 # Use optparse imports directly in new code.
 # Nevertheless, TimeOption can be used from here.
 OptionParser = optparse.OptionParser
 
@@ -204,15 +203,15 @@
     def get_failure(self):
         """Print information about task completion"""
         if self.info['state'] != koji.TASK_STATES['FAILED']:
             return ''
         error = None
         try:
             self.session.getTaskResult(self.id)
-        except (six.moves.xmlrpc_client.Fault, koji.GenericError) as e:
+        except (koji.xmlrpcplus.Fault, koji.GenericError) as e:
             error = e
         if error is None:
             # print("%s: complete" % self.str())
             # We already reported this task as complete in update()
             return ''
         else:
             return '%s: %s' % (error.__class__.__name__, str(error).strip())
@@ -918,10 +917,10 @@
             return s
     else:
         return ''
 
 
 class DatetimeJSONEncoder(json.JSONEncoder):
     def default(self, o):
-        if isinstance(o, xmlrpc_client.DateTime):
+        if isinstance(o, koji.xmlrpcplus.DateTime):
             return str(o)
         return json.JSONEncoder.default(self, o)
```

### Comparing `koji-1.34.0/koji/__init__.py` & `koji-1.34.1/koji/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 import six.moves.urllib
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 from requests.packages.urllib3.exceptions import MaxRetryError, HostChangedError
 from six.moves import range, zip
 
 from koji.tasks import parse_task_params
-from koji.xmlrpcplus import Fault, dumps, getparser, loads, xmlrpc_client
+from koji.xmlrpcplus import DateTime, Fault, dumps, getparser, loads
 from koji.util import deprecated
 from . import util
 from . import _version
 __version__ = _version.__version__
 __version_info__ = _version.__version_info__
 
 try:
@@ -1499,21 +1499,23 @@
             'either a path to a pom file or the contents of a pom file must be specified')
 
     # A common problem is non-UTF8 characters in XML files, so we'll convert the string first
 
     contents = fixEncoding(contents)
 
     try:
-        xml.sax.parseString(contents, handler)  # nosec - trusted data
+        # trusted data, skipping bandit test
+        xml.sax.parseString(contents, handler)  # nosec
     except xml.sax.SAXParseException:
         # likely an undefined entity reference, so lets try replacing
         # any entity refs we can find and see if we get something parseable
         handler.reset()
         contents = ENTITY_RE.sub('?', contents)
-        xml.sax.parseString(contents, handler)  # nosec - trusted data
+        # trusted data, skipping bandit test
+        xml.sax.parseString(contents, handler)  # nosec
 
     for field in fields:
         if field not in util.to_list(values.keys()):
             raise GenericError('could not extract %s from POM: %s' %
                                (field, (path or '<contents>')))
     return values
 
@@ -2619,14 +2621,38 @@
         self._calls = []
         self.logger = logging.getLogger('koji')
         self.rsession = None
         self.new_session()
         self.opts.setdefault('timeout', DEFAULT_REQUEST_TIMEOUT)
         self.exclusive = False
         self.auth_method = auth_method
+        self.__hub_version = None
+
+    @property
+    def hub_version(self):
+        """Return the hub version as a tuple of ints"""
+        return tuple([int(x) for x in self.hub_version_str.split('.')])
+
+    @property
+    def hub_version_str(self):
+        """Return the hub version as string"""
+        # If any call was made before, it should be populated by Koji-Version header
+        # for hub >= 1.35
+        if self.__hub_version is None:
+            # no call was made yet OR hub_version < 1.35
+            try:
+                self.__hub_version = self.getKojiVersion()
+            except GenericError as e:
+                if 'Invalid method' in str(e):
+                    # use latest version without the getKojiVersion handler
+                    self.logger.debug("hub is older than 1.23, assuming 1.22.0")
+                    self.__hub_version = '1.22.0'
+                else:
+                    raise
+        return self.__hub_version
 
     @property
     def multicall(self):
         """The multicall property acts as a settable boolean or a callable
 
         This setup allows preserving the original multicall interface
         alongside the new one without adding yet another similar sounding
@@ -3050,14 +3076,17 @@
                     if len(_val) > 1024:
                         _val = _val[:1024] + '...'
                 self.logger.debug("%s: %r" % (_key, _val))
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             r = self.rsession.post(handler, **callopts)
             r.raise_for_status()
+            hub_version = r.headers.get('Koji-Version')
+            if hub_version:
+                self.__hub_version = hub_version
             try:
                 ret = self._read_xmlrpc_response(r)
             finally:
                 r.close()
         return ret
 
     def _read_xmlrpc_response(self, response):
@@ -3657,15 +3686,15 @@
             self.handleError(record)
 
 
 def formatTime(value):
     """Format a timestamp so it looks nicer"""
     if not value and not isinstance(value, (int, float)):
         return ''
-    if isinstance(value, xmlrpc_client.DateTime):
+    if isinstance(value, DateTime):
         value = datetime.datetime.strptime(value.value, "%Y%m%dT%H:%M:%S")
     elif isinstance(value, (int, float)):
         value = datetime.datetime.fromtimestamp(value)
     if isinstance(value, datetime.datetime):
         return value.strftime('%Y-%m-%d %H:%M:%S')
     else:
         # trim off the microseconds, if present
@@ -3680,15 +3709,15 @@
     """Format a timestamp to a more human-reable format, i.e.:
     Sat, 07 Sep 2002 00:00:01 GMT
     """
     if not value and not isinstance(value, (int, float)):
         return ''
     if isinstance(value, six.string_types):
         t = dateutil.parser.parse(value)
-    elif isinstance(value, xmlrpc_client.DateTime):
+    elif isinstance(value, DateTime):
         t = dateutil.parser.parse(value.value)
     elif isinstance(value, (int, float)):
         t = datetime.datetime.fromtimestamp(value)
     else:
         t = value
     # return date in local timezone, py 2.6 has tzone as astimezone required parameter
     # would work simply as t.astimezone() for py 2.7+
```

### Comparing `koji-1.34.0/koji/arch.py` & `koji-1.34.1/koji/arch.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.0/koji/context.py` & `koji-1.34.1/koji/context.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.0/koji/daemon.py` & `koji-1.34.1/koji/daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1021,17 +1021,28 @@
                 elif tinfo['host_id'] != self.host_id:
                     self.logger.info("Killing reassigned task %r (pid %r)" % (id, pid))
                     if self.cleanupTask(id):
                         del self.pids[id]
                 else:
                     self.logger.info("Lingering task %r (pid %r)" % (id, pid))
 
+    def _get_host_data(self):
+        data = {
+            'methods': list(self.handlers.keys()),
+            'maxjobs': self.options.maxjobs,
+            # TODO: now it would be duplicated by updateHost
+            # 'ready': self.ready,
+            # 'task_load': self.task_load,
+            # cpu_load, free_mem, free_disk, ...
+        }
+        return data
+
     def getNextTask(self):
         self.ready = self.readyForTask()
-        self.session.host.updateHost(self.task_load, self.ready)
+        self.session.host.updateHost(self.task_load, self.ready, data=self._get_host_data())
         if not self.ready:
             self.logger.info("Not ready for task")
             return False
         hosts, tasks = self.session.host.getLoadData()
         self.logger.debug("Load Data:")
         self.logger.debug("  hosts: %r" % hosts)
         self.logger.debug("  tasks: %r" % tasks)
@@ -1500,14 +1511,17 @@
         except koji.xmlrpcplus.Fault as fault:
             response = koji.xmlrpcplus.dumps(fault)
             tb = ''.join(traceback.format_exception(*sys.exc_info())).replace(r"\n", "\n")
             self.logger.warning("FAULT:\n%s" % tb)
         except (SystemExit, koji.tasks.ServerExit, KeyboardInterrupt):
             # we do not trap these
             raise
+        except koji.tasks.RefuseTask as refuse:
+            self.session.host.refuseTask(handler.id, msg=str(refuse))
+            return
         except koji.tasks.ServerRestart:
             # freeing this task will allow the pending restart to take effect
             self.session.host.freeTasks([handler.id])
             return
         except Exception:
             tb = ''.join(traceback.format_exception(*sys.exc_info()))
             self.logger.warning("TRACEBACK: %s" % tb)
```

### Comparing `koji-1.34.0/koji/plugin.py` & `koji-1.34.1/koji/plugin.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.0/koji/policy.py` & `koji-1.34.1/koji/policy.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.0/koji/rpmdiff.py` & `koji-1.34.1/koji/rpmdiff.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.0/koji/server.py` & `koji-1.34.1/koji/server.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.0/koji/tasks.py` & `koji-1.34.1/koji/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,14 +106,19 @@
 
 
 class ServerRestart(Exception):
     """Raised to restart the server"""
     pass
 
 
+class RefuseTask(Exception):
+    """Raise to task handler to refuse a task"""
+    pass
+
+
 def parse_task_params(method, params):
     """Parse task params into a dictionary
 
     New tasks should already be dictionaries
     """
 
     # check for new style
```

### Comparing `koji-1.34.0/koji/util.py` & `koji-1.34.1/koji/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,23 +21,25 @@
 from __future__ import absolute_import, division
 
 import base64
 import calendar
 import datetime
 import errno
 import hashlib
+import json
 import logging
 import os
 import os.path
 import re
 import resource
 import shutil
 import stat
 import struct
 import sys
+import tempfile
 import time
 import warnings
 from fnmatch import fnmatch
 from zlib import adler32
 
 import six
 from six.moves import range, zip
@@ -429,43 +431,176 @@
 
 
 class _RetryRmtree(Exception):
     """This exception is used internally by rmtree"""
     # We raise this exception only when it makes sense for rmtree to retry from the top
 
 
-def rmtree(path, logger=None):
-    """Delete a directory tree without crossing fs boundaries"""
+def rmtree(path, logger=None, background=False):
+    """Delete a directory tree without crossing fs boundaries
+
+    :param str path: the directory to remove
+    :param Logger logger: Logger object
+    :param bool background: if True, runs in the background returning a cleanup function
+    :return: None or [pid, check_function]
+
+    In the background case, caller is responsible for waiting on pid and should call
+    the returned check function once it finishes.
+    """
+    # we use the fake logger to avoid issues with logging locks while forking
+    fd, logfile = tempfile.mkstemp(suffix='.jsonl')
+    os.close(fd)
+    pid = os.fork()
+
+    if not pid:
+        # child process
+        try:
+            status = 1
+            with SimpleProxyLogger(logfile) as mylogger:
+                try:
+                    _rmtree_nofork(path, logger=mylogger)
+                except Exception as e:
+                    mylogger.error('rmtree failed: %s' % e)
+                    raise
+            status = 0
+        finally:
+            # diediedie
+            os._exit(status)
+        # not reached
+
+    # parent process
+    logger = logger or logging.getLogger('koji')
+
+    def _rmtree_check():
+        if not background:
+            # caller will wait in background case
+            _pid, status = os.waitpid(pid, 0)
+        try:
+            SimpleProxyLogger.send(logfile, logger)
+        except Exception as err:
+            logger.error("Failed to get rmtree logs -- %s" % err)
+        try:
+            os.unlink(logfile)
+        except Exception:
+            pass
+        if not background:
+            # caller should check status in background case
+            if not isSuccess(status):
+                raise koji.GenericError(parseStatus(status, "rmtree process"))
+        if os.path.exists(path):
+            raise koji.GenericError("Failed to remove directory: %s" % path)
+
+    if background:
+        return pid, _rmtree_check
+    else:
+        return _rmtree_check()
+
+
+class SimpleProxyLogger(object):
+    """Save log messages to a file and log them later"""
+
+    DEBUG = logging.DEBUG
+    INFO = logging.INFO
+    WARNING = logging.WARNING
+    ERROR = logging.ERROR
+
+    def __init__(self, filename):
+        self.outfile = koji._open_text_file(filename, mode='wt')
+
+    # so we can use as a context manager
+    def __enter__(self):
+        return self
+
+    def __exit__(self, _type, value, traceback):
+        self.outfile.close()
+        # don't eat exceptions
+        return False
+
+    def log(self, level, msg, *args, **kwargs):
+        # jsonl output
+        data = [level, msg, args, kwargs]
+        try:
+            line = json.dumps(data, indent=None)
+        except Exception:
+            try:
+                data = [logging.ERROR, "Unable to log: %s" % data, (), {}]
+                line = json.dumps(data, indent=None)
+            except Exception:
+                line = '[40, "Invalid log data", [], {}]'
+        try:
+            self.outfile.write(line)
+            self.outfile.write('\n')
+        except Exception:
+            pass
+
+    def info(self, msg, *args, **kwargs):
+        self.log(self.INFO, msg, *args, **kwargs)
+
+    def warning(self, msg, *args, **kwargs):
+        self.log(self.WARNING, msg, *args, **kwargs)
+
+    def error(self, msg, *args, **kwargs):
+        self.log(self.ERROR, msg, *args, **kwargs)
+
+    def debug(self, msg, *args, **kwargs):
+        self.log(self.DEBUG, msg, *args, **kwargs)
+
+    @staticmethod
+    def send(filename, logger):
+        with koji._open_text_file(filename, mode='rt') as fo:
+            for line in fo:
+                try:
+                    level, msg, args, kwargs = json.loads(line)
+                except Exception:
+                    level = logging.ERROR
+                    msg = "Bad log data: %r"
+                    args = (line,)
+                    kwargs = {}
+                logger.log(level, msg, *args, **kwargs)
+
+
+def _rmtree_nofork(path, logger=None):
+    """Delete a directory tree without crossing fs boundaries
+
+    This function is not thread safe because it relies on chdir to avoid
+    forming long paths.
+    """
     # implemented to avoid forming long paths
     # see: https://pagure.io/koji/issue/201
     logger = logger or logging.getLogger('koji')
     try:
         st = os.lstat(path)
     except FileNotFoundError:
         logger.warning("No such file/dir %s for removal" % path)
         return
     if not stat.S_ISDIR(st.st_mode):
         raise koji.GenericError("Not a directory: %s" % path)
     dev = st.st_dev
     cwd = os.getcwd()
+    abspath = os.path.abspath(path)
 
     try:
         # retry loop
         while True:
             try:
                 os.chdir(path)
+                new_cwd = os.getcwd()
+                # make sure we're where we think we are
+                if not os.path.samefile(new_cwd, abspath):
+                    raise koji.GenericError('chdir to %s resulted in different cwd %s',
+                                            path, new_cwd)
             except OSError as e:
                 if e.errno in (errno.ENOENT, errno.ESTALE):
                     # likely racing with another rmtree
                     # if the dir doesn't exist, we're done
                     logger.warning("Directory to remove has disappeared: %s" % path)
                     return
                 raise
             try:
-                _rmtree(dev, logger)
+                _rmtree(dev, new_cwd, logger)
             except _RetryRmtree as e:
                 # reset and retry
                 os.chdir(cwd)
                 logger.warning("Retrying rmtree due to %s" % e)
                 continue
             break
     finally:
@@ -475,97 +610,123 @@
     try:
         os.rmdir(path)
     except OSError as e:
         if e.errno != errno.ENOENT:
             raise
 
 
-def _rmtree(dev, logger):
+def _rmtree(dev, cwd, logger):
     """Remove all contents of CWD"""
     # This implementation avoids forming long paths and recursion. Otherwise
     # we will have errors with very deep directory trees.
     # - to avoid forming long paths we change directory as we go
     # - to avoid recursion we maintain our own stack
     dirstack = []
-    # Each entry in dirstack is a list of subdirs for that level
+    # Each entry in dirstack contains data for a level of directory traversal
+    #    - path
+    #    - subdirs
     # As we descend into the tree, we append a new entry to dirstack
     # When we ascend back up after removal, we pop them off
+
     while True:
-        dirs = _stripcwd(dev, logger)
+        dirs = _stripcwd(dev, cwd, logger)
 
         # if cwd has no subdirs, walk back up until we find some
         while not dirs and dirstack:
+            _assert_cwd(cwd)
             try:
                 os.chdir('..')
             except OSError as e:
+                _assert_cwd(cwd)
                 if e.errno in (errno.ENOENT, errno.ESTALE):
                     # likely in a race with another rmtree
                     # however, we cannot proceed from here, so we return to the top
                     raise _RetryRmtree(str(e))
                 raise
             dirs = dirstack.pop()
+            cwd = os.path.dirname(cwd)
 
-            # now that we've ascended back up by one, the first dir entry is
+            # now that we've ascended back up by one, the last dir entry is
             # one we've just cleared, so we should remove it
             empty_dir = dirs.pop()
+            _assert_cwd(cwd)
             try:
                 os.rmdir(empty_dir)
             except OSError as e:
+                _assert_cwd(cwd)
                 # If this happens, either something else is writing to the dir,
                 # or there is a bug in our code.
                 # For now, we ignore this and proceed, but we'll still fail at
                 # the top level rmdir
                 logger.error("Unable to remove directory %s: %s" % (empty_dir, e))
                 pass
 
         if not dirs:
             # we are done
             break
 
         # otherwise we descend into the next subdir
         subdir = dirs[-1]
         # note: we do not pop here because we need to remember to remove subdir later
+        _assert_cwd(cwd)
         try:
             os.chdir(subdir)
         except OSError as e:
+            _assert_cwd(cwd)
             if e.errno == errno.ENOENT:
                 # likely in a race with another rmtree
                 # we'll ignore this and continue
                 # since subdir doesn't exist, we'll pop it off and forget about it
                 dirs.pop()
                 logger.warning("Subdir disappeared during rmtree %s: %s" % (subdir, e))
                 continue  # with dirstack unchanged
             raise
+        cwd = os.path.join(cwd, subdir)
         dirstack.append(dirs)
 
 
-def _stripcwd(dev, logger):
+def _assert_cwd(cwd):
+    try:
+        actual = os.getcwd()
+    except OSError as e:
+        if e.errno == errno.ENOENT:
+            # subsequent calls should fail with better handling
+            return
+        raise
+    if cwd != actual:
+        raise koji.GenericError('CWD changed unexpectedly: %s -> %s' % (cwd, actual))
+
+
+def _stripcwd(dev, cwd, logger):
     """Unlink all files in cwd and return list of subdirs"""
     dirs = []
+    _assert_cwd(cwd)
     try:
         fdirs = os.listdir('.')
     except OSError as e:
         if e.errno in (errno.ENOENT, errno.ESTALE):
             # cwd could have been removed by others, just return an empty list
             logger.warning("Unable to read directory: %s" % e)
             return dirs
         raise
     for fn in fdirs:
         try:
             st = os.lstat(fn)
         except OSError as e:
+            _assert_cwd(cwd)
             if e.errno == errno.ENOENT:
                 continue
             raise
         if st.st_dev != dev:
             # don't cross fs boundary
             continue
         if stat.S_ISDIR(st.st_mode):
             dirs.append(fn)
         else:
+            _assert_cwd(cwd)
             try:
                 os.unlink(fn)
             except OSError:
                 # we'll still fail at the top level
                 pass
     return dirs
```

### Comparing `koji-1.34.0/koji/xmlrpcplus.py` & `koji-1.34.1/koji/xmlrpcplus.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,24 @@
 Custom xmlrpc handling for Koji
 """
 
 from __future__ import absolute_import
 
 import types
 
+import defusedxml.xmlrpc as defusedxmlrpc
 import re
 import six
+# importing here for references in koji by defused.xmlrpc.monkey_patch() below
 import six.moves.xmlrpc_client as xmlrpc_client
+import six.moves.xmlrpc_server as xmlrpc_server  # noqa: F401
+
+
+# patching xmlrpc to protect against XML related attacks
+defusedxmlrpc.monkey_patch()
 
 # duplicate a few values that we need
 getparser = xmlrpc_client.getparser
 loads = xmlrpc_client.loads
 Fault = xmlrpc_client.Fault
 DateTime = xmlrpc_client.DateTime
```

### Comparing `koji-1.34.0/koji.egg-info/PKG-INFO` & `koji-1.34.1/koji.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koji
-Version: 1.34.0
+Version: 1.34.1
 Summary: Koji is a system for building and tracking RPMS. The base package contains shared libraries and the command-line interface.
 Home-page: http://pagure.io/koji/
 Author: Koji developers
 Author-email: koji-devel@lists.fedorahosted.org
 License: LGPLv2 and GPLv2+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `koji-1.34.0/koji.egg-info/SOURCES.txt` & `koji-1.34.1/koji.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -2,33 +2,45 @@
 README.md
 setup.py
 cli/koji
 cli/koji_cli/__init__.py
 cli/koji_cli/commands.py
 cli/koji_cli/lib.py
 koji/__init__.py
+koji/__init__.pyi
 koji/_version.py
+koji/_version.pyi
 koji/arch.py
+koji/arch.pyi
 koji/context.py
+koji/context.pyi
 koji/daemon.py
+koji/daemon.pyi
 koji/plugin.py
+koji/plugin.pyi
 koji/policy.py
+koji/policy.pyi
+koji/py.typed
 koji/rpmdiff.py
+koji/rpmdiff.pyi
 koji/server.py
+koji/server.pyi
 koji/tasks.py
+koji/tasks.pyi
 koji/util.py
+koji/util.pyi
 koji/xmlrpcplus.py
+koji/xmlrpcplus.pyi
 koji.egg-info/PKG-INFO
 koji.egg-info/SOURCES.txt
 koji.egg-info/dependency_links.txt
 koji.egg-info/requires.txt
 koji.egg-info/top_level.txt
 plugins/cli/dud.py
 plugins/cli/kiwi.py
-plugins/cli/pungi.py
 plugins/cli/runroot.py
 plugins/cli/save_failed_tree.py
 plugins/cli/sidetag_cli.py
 tests/test_docs_version.py
 tests/test_scm.py
 util/koji-gc
 util/koji-shadow
```

### Comparing `koji-1.34.0/plugins/cli/dud.py` & `koji-1.34.1/plugins/cli/dud.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.0/plugins/cli/kiwi.py` & `koji-1.34.1/plugins/cli/kiwi.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.0/plugins/cli/runroot.py` & `koji-1.34.1/plugins/cli/runroot.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.0/plugins/cli/save_failed_tree.py` & `koji-1.34.1/plugins/cli/save_failed_tree.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.0/plugins/cli/sidetag_cli.py` & `koji-1.34.1/plugins/cli/sidetag_cli.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.0/setup.py` & `koji-1.34.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 def get_install_requires():
     # To install all build requires:
     # $ dnf install python-pip git krb5-devel gcc redhat-rpm-config \
     #               glib2-devel sqlite-devel libxml2-devel python-devel \
     #               openssl-devel libffi-devel
 
     requires = [
+        'defusedxml',
         'python-dateutil',
         'requests',
         'requests-gssapi',
         'six',
         # 'libcomps',
-        # 'rpm-py-installer', # it is optional feature
         # 'rpm',
     ]
     return requires
 
 
 def get_version():
     cwd = os.path.dirname(__file__)
```

### Comparing `koji-1.34.0/tests/test_docs_version.py` & `koji-1.34.1/tests/test_docs_version.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.0/tests/test_scm.py` & `koji-1.34.1/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `koji-1.34.0/util/koji-gc` & `koji-1.34.1/util/koji-gc`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import fnmatch
 import optparse
 import os
 import pprint
 import smtplib
 import sys
 import time
-import xmlrpc.client  # for Fault
 from email.mime import text as MIMEText
 from string import Template
 
 import requests
 
 import koji
 import koji.policy
@@ -1002,15 +1001,15 @@
                         untagged.setdefault(nvr, {})[tagname] = 1
                     else:
                         print("Untagging build %s from %s" % (nvr, tagname))
                         try:
                             session.untagBuildBypass(taginfo['id'], entry['build_id'],
                                                      force=bypass or is_admin)
                             untagged.setdefault(nvr, {})[tagname] = 1
-                        except (xmlrpc.client.Fault, koji.GenericError) as e:
+                        except (koji.xmlrpcplus.Fault, koji.GenericError) as e:
                             print("Warning: untag operation failed: %s" % e)
                             pass
                 # if action == 'keep' do nothing
     if options.purge and untagged:
         print("Attempting to purge %i builds" % len(untagged))
         for nvr in untagged:
             build_id = build_ids[nvr]
@@ -1036,15 +1035,15 @@
 
             if options.test:
                 print("Would have deleted build: %s" % nvr)
             else:
                 print("Deleting untagged build: %s" % nvr)
                 try:
                     session.deleteBuild(build_id, strict=True)
-                except (xmlrpc.client.Fault, koji.GenericError) as e:
+                except (koji.xmlrpcplus.Fault, koji.GenericError) as e:
                     print("Warning: deletion failed: %s" % e)
                     # server issue
                     pass
 
 
 if __name__ == "__main__":
```

### Comparing `koji-1.34.0/util/koji-shadow` & `koji-1.34.1/util/koji-shadow`

 * *Files identical despite different names*

### Comparing `koji-1.34.0/util/koji-sweep-db` & `koji-1.34.1/util/koji-sweep-db`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/python3
 
 import os
-import xmlrpc.client
 from optparse import OptionParser
 from koji.context import context
 
 import koji
 import kojihub.db
+import koji.xmlrpcplus
 from kojihub.db import DeleteProcessor, QueryProcessor, BulkInsertProcessor
 
 
 def clean_sessions(cursor, vacuum, test, age, absolute):
     clause = f"(update_time < NOW() - '{age:d} days'::interval)"
     if absolute is not None:
         clause += f"OR (start_time < NOW() - '{absolute:d} days'::interval)"
@@ -75,15 +75,15 @@
     # will be dropped automatically in the end of script/connection
     cursor.execute("CREATE TEMPORARY TABLE temp_scratch_tasks (task_id INTEGER NOT NULL)")
     query = QueryProcessor(tables=['task'], columns=['id', 'request'], clauses=clauses)
     for row in query.execute():
         task_id = row['id']
         request = row['request']
         try:
-            params, _ = xmlrpc.client.loads(request)
+            params, _ = koji.xmlrpcplus.xmlrpc_client.loads(request)
             opts = params[2]
             if opts['scratch']:
                 ids.append(task_id)
         except Exception:
             continue
         insert = BulkInsertProcessor('temp_scratch_tasks')
         for task_id in ids:
```

### Comparing `koji-1.34.0/util/kojira` & `koji-1.34.1/util/kojira`

 * *Files 3% similar despite different names*

```diff
@@ -281,61 +281,14 @@
     def deleted(self):
         return self.state == koji.REPO_DELETED
 
     def problem(self):
         return self.state == koji.REPO_PROBLEM
 
 
-class LoggingLockManager(object):
-    """A context manager that acquires all the logging locks"""
-
-    # This lock business is a workaround for https://pagure.io/koji/issue/2714
-
-    def __enter__(self):
-        self.acquire_locks()
-        return self
-
-    def __exit__(self, exc_type, exc_val, traceback):
-        # we want to free the locks regardless of what happend inside the with statement
-        self.release_locks()
-        return False  # don't eat exceptions
-
-    def acquire_locks(self):
-        # init
-        self.locks = []
-        self.module_lock = False
-        toplogger = logging.getLogger('koji')
-
-        # module level lock
-        if hasattr(logging, '_acquireLock'):
-            logging._acquireLock()
-            self.module_lock = True
-
-        # also each handler can have its own lock
-        # in kojira, the we should only have handlers attached to the koji logger
-        self.locks = [h.lock for h in toplogger.handlers if h.lock]
-        for lock in self.locks:
-            lock.acquire()
-
-    def release_locks(self):
-        # Only parent process should have locked locks in 3.9+, child ones will
-        # be reinitilized to free state
-        # In older pythons, state could be random (and no module_lock)
-        if self.module_lock:
-            try:
-                logging._releaseLock()
-            except RuntimeError:
-                pass
-        for lock in self.locks:
-            try:
-                lock.release()
-            except RuntimeError:
-                pass
-
-
 class RepoManager(object):
 
     def __init__(self, options, session):
         self.options = options
         self._local = threading.local()
         self._local.session = session
         self.repos = {}
@@ -359,70 +312,58 @@
         self._local.session = value
 
     def printState(self):
         self.logger.debug('Tracking %i repos, %i child processes',
                           len(self.repos), len(self.delete_pids))
         for tag_id, task_id in self.tasks.items():
             self.logger.debug("Tracking task %s for tag %s", task_id, tag_id)
-        for pid, desc in self.delete_pids.items():
-            self.logger.debug("Delete job %s: %r", pid, desc)
+        for pid in self.delete_pids:
+            path = self.delete_pids[pid][0]
+            self.logger.debug("Delete job %s: %r", pid, path)
 
     def rmtree(self, path):
         """Spawn (or queue) and rmtree job"""
         self.logger.info("Queuing rmtree job for %s", path)
         if path not in self.delete_queue:
             self.delete_queue.append(path)
 
     def checkQueue(self):
         finished = [pid for pid in self.delete_pids if self.waitPid(pid)]
         for pid in finished:
-            path = self.delete_pids[pid]
-            self.logger.info("Completed rmtree job for %s", path)
+            path, check_func = self.delete_pids[pid]
             del self.delete_pids[pid]
+            try:
+                check_func()
+            except Exception as e:
+                self.logger.error("Failed rmtree job for %s: %s", path, e)
+                continue
+            self.logger.info("Completed rmtree job for %s", path)
         while self.delete_queue and len(self.delete_pids) <= self.options.max_delete_processes:
             path = self.delete_queue.pop(0)
-            pid = self._rmtree(path)
+            pid, check_func = rmtree(path, background=True)  # koji.util.rmtree
             self.logger.info("Started rmtree (pid %i) for %s", pid, path)
-            self.delete_pids[pid] = path
+            self.delete_pids[pid] = (path, check_func)
 
     def waitPid(self, pid):
         # XXX - can we unify with TaskManager?
-        prefix = "pid %i (%s)" % (pid, self.delete_pids.get(pid))
+        prefix = "pid %i (%s)" % (pid, self.delete_pids.get(pid)[0])
         try:
             (childpid, status) = os.waitpid(pid, os.WNOHANG)
         except OSError as e:
             if e.errno != errno.ECHILD:
                 # should not happen
                 raise
             # otherwise assume the process is gone
             self.logger.info("%s: %s" % (prefix, e))
             return True
         if childpid != 0:
             self.logger.info(parseStatus(status, prefix))
             return True
         return False
 
-    def _rmtree(self, path):
-        with LoggingLockManager():
-            pid = os.fork()
-        if pid:
-            return pid
-        # no return
-        try:
-            status = 1
-            self.session._forget()
-            try:
-                rmtree(path)
-                status = 0
-            except BaseException:
-                logger.error(''.join(traceback.format_exception(*sys.exc_info())))
-                logging.shutdown()
-        finally:
-            os._exit(status)
-
     def killChildren(self):
         # XXX - unify with TaskManager?
         sig = signal.SIGTERM
         for pid in self.delete_pids:
             try:
                 os.kill(pid, sig)
             except OSError as e:
```

