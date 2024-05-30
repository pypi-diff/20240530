# Comparing `tmp/lute3_mandarin-0.0.3.tar.gz` & `tmp/lute3_mandarin-0.0.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lute3_mandarin-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lute3_mandarin-0.0.3b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lute3_mandarin-0.0.3.tar` & `lute3_mandarin-0.0.3b1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      313 2024-05-18 03:42:18.966723 lute3_mandarin-0.0.3/.pytest.ini
--rw-r--r--   0        0        0      205 2024-05-27 23:47:17.825356 lute3_mandarin-0.0.3/README.md
--rw-r--r--   0        0        0     1365 2024-05-27 23:47:17.825551 lute3_mandarin-0.0.3/README_PyPi.md
--rw-r--r--   0        0        0      416 2024-05-18 03:42:18.966791 lute3_mandarin-0.0.3/definition.yaml
--rw-r--r--   0        0        0       52 2024-05-30 03:06:17.811546 lute3_mandarin-0.0.3/lute_mandarin_parser/__init__.py
--rw-r--r--   0        0        0     4772 2024-05-27 23:47:17.826015 lute3_mandarin-0.0.3/lute_mandarin_parser/parser.py
--rw-r--r--   0        0        0      523 2024-05-30 03:06:17.811596 lute3_mandarin-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1538 2024-05-18 03:42:18.967830 lute3_mandarin-0.0.3/requirements.txt
--rw-r--r--   0        0        0        0 2024-05-27 23:47:17.826244 lute3_mandarin-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      823 2024-05-18 03:42:18.968199 lute3_mandarin-0.0.3/tests/conftest.py
--rw-r--r--   0        0        0     4608 2024-05-27 23:47:17.826704 lute3_mandarin-0.0.3/tests/test_MandarinParser.py
--rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 lute3_mandarin-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      313 2024-05-18 03:42:18.966723 lute3_mandarin-0.0.3b1/.pytest.ini
+-rw-r--r--   0        0        0      205 2024-05-27 23:47:17.825356 lute3_mandarin-0.0.3b1/README.md
+-rw-r--r--   0        0        0     1365 2024-05-27 23:47:17.825551 lute3_mandarin-0.0.3b1/README_PyPi.md
+-rw-r--r--   0        0        0      416 2024-05-18 03:42:18.966791 lute3_mandarin-0.0.3b1/definition.yaml
+-rw-r--r--   0        0        0       54 2024-05-27 23:53:11.681963 lute3_mandarin-0.0.3b1/lute_mandarin_parser/__init__.py
+-rw-r--r--   0        0        0     4772 2024-05-27 23:47:17.826015 lute3_mandarin-0.0.3b1/lute_mandarin_parser/parser.py
+-rw-r--r--   0        0        0      525 2024-05-27 23:53:11.682082 lute3_mandarin-0.0.3b1/pyproject.toml
+-rw-r--r--   0        0        0     1538 2024-05-18 03:42:18.967830 lute3_mandarin-0.0.3b1/requirements.txt
+-rw-r--r--   0        0        0        0 2024-05-27 23:47:17.826244 lute3_mandarin-0.0.3b1/tests/__init__.py
+-rw-r--r--   0        0        0      823 2024-05-18 03:42:18.968199 lute3_mandarin-0.0.3b1/tests/conftest.py
+-rw-r--r--   0        0        0     4608 2024-05-27 23:47:17.826704 lute3_mandarin-0.0.3b1/tests/test_MandarinParser.py
+-rw-r--r--   0        0        0     1649 1970-01-01 00:00:00.000000 lute3_mandarin-0.0.3b1/PKG-INFO
```

### Comparing `lute3_mandarin-0.0.3/README_PyPi.md` & `lute3_mandarin-0.0.3b1/README_PyPi.md`

 * *Files identical despite different names*

### Comparing `lute3_mandarin-0.0.3/lute_mandarin_parser/parser.py` & `lute3_mandarin-0.0.3b1/lute_mandarin_parser/parser.py`

 * *Files identical despite different names*

### Comparing `lute3_mandarin-0.0.3/pyproject.toml` & `lute3_mandarin-0.0.3b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 requires-python = ">=3.8"
 authors = [
   {name = "Chris Ghyzel"}
 ]
 readme = "README_PyPi.md"
 
 dependencies = [
-  "lute3>=3.4.2",
+  "lute3>=3.4.2b1",
   "jieba>=0.42.1",
   "pypinyin>=0.51.0"
 ]
 
 
 [project.entry-points."lute.plugin.parse"]
 lute_mandarin = "lute_mandarin_parser.parser:MandarinParser"
```

### Comparing `lute3_mandarin-0.0.3/requirements.txt` & `lute3_mandarin-0.0.3b1/requirements.txt`

 * *Files identical despite different names*

### Comparing `lute3_mandarin-0.0.3/tests/conftest.py` & `lute3_mandarin-0.0.3b1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lute3_mandarin-0.0.3/tests/test_MandarinParser.py` & `lute3_mandarin-0.0.3b1/tests/test_MandarinParser.py`

 * *Files identical despite different names*

### Comparing `lute3_mandarin-0.0.3/PKG-INFO` & `lute3_mandarin-0.0.3b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: lute3-mandarin
-Version: 0.0.3
+Version: 0.0.3b1
 Summary: Learning Using Texts - Chinese Parser
 Author: Chris Ghyzel
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: lute3>=3.4.2
+Requires-Dist: lute3>=3.4.2b1
 Requires-Dist: jieba>=0.42.1
 Requires-Dist: pypinyin>=0.51.0
 
 # `lute3-mandarin`
 
 A Mandarin parser for Lute (`lute3`) using the `jieba` library, and
 `pypinyin` for readings.
```

