# Comparing `tmp/mutt_html_reply-0.3.0.tar.gz` & `tmp/mutt_html_reply-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutt_html_reply-0.3.0.tar", last modified: Thu May 30 03:18:30 2024, max compression
+gzip compressed data, was "mutt_html_reply-0.3.1.tar", last modified: Thu May 30 03:24:05 2024, max compression
```

## Comparing `mutt_html_reply-0.3.0.tar` & `mutt_html_reply-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-30 03:18:30.356745 mutt_html_reply-0.3.0/
--rw-r--r--   0 erik      (1000) erik      (1000)     1062 2024-05-22 16:41:30.000000 mutt_html_reply-0.3.0/LICENSE
--rw-r--r--   0 erik      (1000) erik      (1000)     2275 2024-05-30 03:18:30.356745 mutt_html_reply-0.3.0/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)      728 2024-05-22 16:51:01.000000 mutt_html_reply-0.3.0/README.md
--rw-r--r--   0 erik      (1000) erik      (1000)      623 2024-05-30 03:18:04.000000 mutt_html_reply-0.3.0/pyproject.toml
--rw-r--r--   0 erik      (1000) erik      (1000)       38 2024-05-30 03:18:30.356745 mutt_html_reply-0.3.0/setup.cfg
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-30 03:18:30.356745 mutt_html_reply-0.3.0/src/
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-30 03:18:30.356745 mutt_html_reply-0.3.0/src/mutt_html_reply/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2024-05-22 16:37:47.000000 mutt_html_reply-0.3.0/src/mutt_html_reply/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     3441 2024-05-30 03:02:53.000000 mutt_html_reply-0.3.0/src/mutt_html_reply/mutt_html_reply.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-30 03:18:30.356745 mutt_html_reply-0.3.0/src/mutt_html_reply.egg-info/
--rw-r--r--   0 erik      (1000) erik      (1000)     2275 2024-05-30 03:18:30.000000 mutt_html_reply-0.3.0/src/mutt_html_reply.egg-info/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)      363 2024-05-30 03:18:30.000000 mutt_html_reply-0.3.0/src/mutt_html_reply.egg-info/SOURCES.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        1 2024-05-30 03:18:30.000000 mutt_html_reply-0.3.0/src/mutt_html_reply.egg-info/dependency_links.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       73 2024-05-30 03:18:30.000000 mutt_html_reply-0.3.0/src/mutt_html_reply.egg-info/entry_points.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       15 2024-05-30 03:18:30.000000 mutt_html_reply-0.3.0/src/mutt_html_reply.egg-info/requires.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       16 2024-05-30 03:18:30.000000 mutt_html_reply-0.3.0/src/mutt_html_reply.egg-info/top_level.txt
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-30 03:24:05.974913 mutt_html_reply-0.3.1/
+-rw-r--r--   0 erik      (1000) erik      (1000)     1062 2024-05-22 16:41:30.000000 mutt_html_reply-0.3.1/LICENSE
+-rw-r--r--   0 erik      (1000) erik      (1000)     2354 2024-05-30 03:24:05.974913 mutt_html_reply-0.3.1/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)      807 2024-05-30 03:23:26.000000 mutt_html_reply-0.3.1/README.md
+-rw-r--r--   0 erik      (1000) erik      (1000)      623 2024-05-30 03:22:28.000000 mutt_html_reply-0.3.1/pyproject.toml
+-rw-r--r--   0 erik      (1000) erik      (1000)       38 2024-05-30 03:24:05.974913 mutt_html_reply-0.3.1/setup.cfg
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-30 03:24:05.974913 mutt_html_reply-0.3.1/src/
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-30 03:24:05.974913 mutt_html_reply-0.3.1/src/mutt_html_reply/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2024-05-22 16:37:47.000000 mutt_html_reply-0.3.1/src/mutt_html_reply/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     3441 2024-05-30 03:02:53.000000 mutt_html_reply-0.3.1/src/mutt_html_reply/mutt_html_reply.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-30 03:24:05.974913 mutt_html_reply-0.3.1/src/mutt_html_reply.egg-info/
+-rw-r--r--   0 erik      (1000) erik      (1000)     2354 2024-05-30 03:24:05.000000 mutt_html_reply-0.3.1/src/mutt_html_reply.egg-info/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)      363 2024-05-30 03:24:05.000000 mutt_html_reply-0.3.1/src/mutt_html_reply.egg-info/SOURCES.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        1 2024-05-30 03:24:05.000000 mutt_html_reply-0.3.1/src/mutt_html_reply.egg-info/dependency_links.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       73 2024-05-30 03:24:05.000000 mutt_html_reply-0.3.1/src/mutt_html_reply.egg-info/entry_points.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       15 2024-05-30 03:24:05.000000 mutt_html_reply-0.3.1/src/mutt_html_reply.egg-info/requires.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       16 2024-05-30 03:24:05.000000 mutt_html_reply-0.3.1/src/mutt_html_reply.egg-info/top_level.txt
```

### Comparing `mutt_html_reply-0.3.0/LICENSE` & `mutt_html_reply-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mutt_html_reply-0.3.0/PKG-INFO` & `mutt_html_reply-0.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutt-html-reply
-Version: 0.3.0
+Version: 0.3.1
 Summary: Create an Outlook-style HTML reply
 Author-email: Erik Rogers <erik@rogers-family.net>
 Maintainer-email: Erik Rogers <erik@rogers-family.net>
 License: Copyright © 2024 Erik Rogers
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -31,12 +31,12 @@
 
 ```
 pip install mutt-html-reply
 ```
 
 ## Usage
 
-This command is meant to be embedded in a neomutt macro when replying, but can also be used as a standalone program.
+This command is meant to be embedded in a neomutt macro when replying, but can also be used as a standalone program. The original message ("-m" flag) must be a file. The reply and output can either come from a file or stdin/stdout.
 
 ```
-mutt-html-reply [html reply] [html original message] [headers to include in quote] [output path]
+mutt-html-reply [-h] [-m [MESSAGE]] [-r REPLY] [-o [OUTPUT]]
 ```
```

### Comparing `mutt_html_reply-0.3.0/README.md` & `mutt_html_reply-0.3.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 
 ```
 pip install mutt-html-reply
 ```
 
 ## Usage
 
-This command is meant to be embedded in a neomutt macro when replying, but can also be used as a standalone program.
+This command is meant to be embedded in a neomutt macro when replying, but can also be used as a standalone program. The original message ("-m" flag) must be a file. The reply and output can either come from a file or stdin/stdout.
 
 ```
-mutt-html-reply [html reply] [html original message] [headers to include in quote] [output path]
+mutt-html-reply [-h] [-m [MESSAGE]] [-r REPLY] [-o [OUTPUT]]
 ```
```

### Comparing `mutt_html_reply-0.3.0/pyproject.toml` & `mutt_html_reply-0.3.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mutt-html-reply"
-version = "0.3.0"
+version = "0.3.1"
 dependencies = [
 	"bs4",
 	"css_inline"
 ]
 authors = [
 	{name = "Erik Rogers", email = "erik@rogers-family.net"}
 ]
```

### Comparing `mutt_html_reply-0.3.0/src/mutt_html_reply/mutt_html_reply.py` & `mutt_html_reply-0.3.1/src/mutt_html_reply/mutt_html_reply.py`

 * *Files identical despite different names*

### Comparing `mutt_html_reply-0.3.0/src/mutt_html_reply.egg-info/PKG-INFO` & `mutt_html_reply-0.3.1/src/mutt_html_reply.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutt-html-reply
-Version: 0.3.0
+Version: 0.3.1
 Summary: Create an Outlook-style HTML reply
 Author-email: Erik Rogers <erik@rogers-family.net>
 Maintainer-email: Erik Rogers <erik@rogers-family.net>
 License: Copyright © 2024 Erik Rogers
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -31,12 +31,12 @@
 
 ```
 pip install mutt-html-reply
 ```
 
 ## Usage
 
-This command is meant to be embedded in a neomutt macro when replying, but can also be used as a standalone program.
+This command is meant to be embedded in a neomutt macro when replying, but can also be used as a standalone program. The original message ("-m" flag) must be a file. The reply and output can either come from a file or stdin/stdout.
 
 ```
-mutt-html-reply [html reply] [html original message] [headers to include in quote] [output path]
+mutt-html-reply [-h] [-m [MESSAGE]] [-r REPLY] [-o [OUTPUT]]
 ```
```

