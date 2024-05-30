# Comparing `tmp/dbis_tm-2.0.0.tar.gz` & `tmp/dbis_tm-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbis_tm-2.0.0.tar", last modified: Tue May 14 14:11:44 2024, max compression
+gzip compressed data, was "dbis_tm-2.0.1.tar", last modified: Thu May 30 09:58:51 2024, max compression
```

## Comparing `dbis_tm-2.0.0.tar` & `dbis_tm-2.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:11:44.294080 dbis_tm-2.0.0/
--rw-r--r--   0 root         (0) root         (0)      704 2024-05-14 14:11:44.294080 dbis_tm-2.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      808 2024-05-14 14:05:53.000000 dbis_tm-2.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 14:11:44.294080 dbis_tm-2.0.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:11:44.290079 dbis_tm-2.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:11:44.290079 dbis_tm-2.0.0/src/dbis_tm/
--rw-rw-rw-   0 root         (0) root         (0)    12780 2024-04-09 12:17:44.000000 dbis_tm-2.0.0/src/dbis_tm/TM.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2024-03-08 12:03:38.000000 dbis_tm-2.0.0/src/dbis_tm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:11:44.294080 dbis_tm-2.0.0/src/dbis_tm.egg-info/
--rw-r--r--   0 root         (0) root         (0)      704 2024-05-14 14:11:44.000000 dbis_tm-2.0.0/src/dbis_tm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      247 2024-05-14 14:11:44.000000 dbis_tm-2.0.0/src/dbis_tm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 14:11:44.000000 dbis_tm-2.0.0/src/dbis_tm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       93 2024-05-14 14:11:44.000000 dbis_tm-2.0.0/src/dbis_tm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-14 14:11:44.000000 dbis_tm-2.0.0/src/dbis_tm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 14:11:44.294080 dbis_tm-2.0.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3625 2024-05-14 14:05:53.000000 dbis_tm-2.0.0/tests/test_tm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 09:58:51.444805 dbis_tm-2.0.1/
+-rw-r--r--   0 root         (0) root         (0)      704 2024-05-30 09:58:51.444805 dbis_tm-2.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      808 2024-05-30 09:56:55.000000 dbis_tm-2.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 09:58:51.444805 dbis_tm-2.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 09:58:51.440805 dbis_tm-2.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 09:58:51.440805 dbis_tm-2.0.1/src/dbis_tm/
+-rw-rw-rw-   0 root         (0) root         (0)    15282 2024-05-22 14:29:39.000000 dbis_tm-2.0.1/src/dbis_tm/TM.py
+-rw-rw-rw-   0 root         (0) root         (0)      157 2024-05-22 14:50:36.000000 dbis_tm-2.0.1/src/dbis_tm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 09:58:51.440805 dbis_tm-2.0.1/src/dbis_tm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      704 2024-05-30 09:58:51.000000 dbis_tm-2.0.1/src/dbis_tm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      247 2024-05-30 09:58:51.000000 dbis_tm-2.0.1/src/dbis_tm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 09:58:51.000000 dbis_tm-2.0.1/src/dbis_tm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2024-05-30 09:58:51.000000 dbis_tm-2.0.1/src/dbis_tm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-30 09:58:51.000000 dbis_tm-2.0.1/src/dbis_tm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 09:58:51.440805 dbis_tm-2.0.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     6897 2024-05-22 14:44:11.000000 dbis_tm-2.0.1/tests/test_tm.py
```

### Comparing `dbis_tm-2.0.0/PKG-INFO` & `dbis_tm-2.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-tm
-Version: 2.0.0
+Version: 2.0.1
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: DBIS i5 RWTH Aachen <dbis-vl@dbis.rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis/dbis-tm
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis_tm-2.0.0/pyproject.toml` & `dbis_tm-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="dbis-tm"
-version='2.0.0'
+version='2.0.1'
 description="RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme"
 
 authors = [
 	{ name = "DBIS i5 RWTH Aachen", email = "dbis-vl@dbis.rwth-aachen.de" }
 ]
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `dbis_tm-2.0.0/src/dbis_tm/TM.py` & `dbis_tm-2.0.1/src/dbis_tm/TM.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 @author: Lara
 @author: Marc
 @author: Wolfgang
 """
 from __future__ import annotations
 
 import itertools
-import sys
+import sys, re
 from enum import Enum, EnumMeta
 from typing import Union
 from graphviz import Digraph
 
 
 class OperationTypeMeta(EnumMeta):
     """
@@ -420,7 +420,76 @@
         self.tx_number = tx_number
 
     def __eq__(self, obj):
         return isinstance(obj, ConflictGraphNode) and self.tx_number == obj.tx_number
 
     def __hash__(self):
         return hash(self.tx_number)
+
+
+class SyntaxCheck:
+    """
+    I am an interface for checking the syntax of inputs.
+    You should not construct me because I am a stateless interface that merely provides static functions.
+
+    Functions:
+        check_conf_set_syntax (checks syntax of strings in tuple that denotes conflicting operations)
+    """
+
+    def __init__(self):
+        raise TypeError("Cannot create 'SyntaxCheck' instances.")
+
+    @classmethod
+    def check_schedule_syntax(cls, schedule: str) -> str:
+        """
+        check the syntax of the given schedule
+
+        Args:
+            schedule(str): the schedule to check
+
+        Returns:
+            msg: None if ok else the problem message
+        """
+        schedule = Schedule.sanitize(schedule)
+        syntax_pattern = "([rw][lu]?[1-3][(][a-z][)]|[c][1-3])?"
+        p_count = re.findall(syntax_pattern, schedule).count("")
+        msg = None
+        if schedule == "":
+            msg = "Leerer Schedule kann keine Lösung sein"
+        if p_count > 1:
+            msg = f"Schedule '{schedule}' hat keine korrekte Syntax"
+        return msg
+
+    @classmethod
+    def check_conf_set_syntax(cls, conf_set: set[tuple[str, str]]) -> str:
+        """
+        Check syntax of strings in tuple that denotes conflicting operations.
+
+        Returns:
+            None if input is formatted according to pattern
+            or an error message in case a tuple is formatted incorrectly
+        """
+        tuple_pattern = "[rw][1-3][(][a-z][)]|[rw]_[1-3][(][a-z][)]"
+        if conf_set == {}:
+            pass
+        elif not isinstance(conf_set, set):
+            return f"{conf_set} ist kein Set"
+        for t in conf_set:
+            if not len(t) == 2:
+                return f"Das Tupel {t} von {conf_set} ist kein Paar"
+            for s in sorted(list(t)):
+                if not re.match(tuple_pattern, s):
+                    return f"Das Tupel {t} von {conf_set} hat keine korrekte Syntax"
+        return None
+
+    @classmethod
+    def check(cls, index, schedule, result) -> str:
+        """
+        check the given schedule against the given result
+        """
+        msg = None
+        s_parsed, s_problem = Schedule.parse_schedule(schedule)
+        result_parsed, result_problem = Schedule.parse_schedule(result)
+        problems = Schedule.check_operations_same(s_parsed, result_parsed)
+        if not len(problems) == 0:
+            msg = f"schedule_{index} enthält unterschiedliche oder nicht alle Operationen aus s{index}"
+        return msg
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dbis_tm-2.0.0/src/dbis_tm.egg-info/PKG-INFO` & `dbis_tm-2.0.1/src/dbis_tm.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-tm
-Version: 2.0.0
+Version: 2.0.1
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: DBIS i5 RWTH Aachen <dbis-vl@dbis.rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis/dbis-tm
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

