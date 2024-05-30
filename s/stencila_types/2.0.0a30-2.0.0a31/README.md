# Comparing `tmp/stencila_types-2.0.0a30.tar.gz` & `tmp/stencila_types-2.0.0a31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stencila_types-2.0.0a30.tar", last modified: Tue May 21 05:08:03 2024, max compression
+gzip compressed data, was "stencila_types-2.0.0a31.tar", last modified: Thu May 30 04:38:03 2024, max compression
```

## Comparing `stencila_types-2.0.0a30.tar` & `stencila_types-2.0.0a31.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2734 2024-03-26 01:26:24.324834 stencila_types-2.0.0a30/README.md
--rw-r--r--   0        0        0     2020 2024-05-21 05:08:03.292657 stencila_types-2.0.0a30/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-26 01:26:24.325553 stencila_types-2.0.0a30/src/stencila_types/__init__.py
--rw-r--r--   0        0        0     8619 2024-04-02 00:34:19.791089 stencila_types-2.0.0a30/src/stencila_types/shortcuts.py
--rw-r--r--   0        0        0    81783 2024-05-21 03:23:15.045833 stencila_types-2.0.0a30/src/stencila_types/types.py
--rw-r--r--   0        0        0     3030 2024-05-21 03:23:15.046165 stencila_types-2.0.0a30/src/stencila_types/utilities.py
--rw-r--r--   0        0        0        0 2024-03-26 01:26:24.326808 stencila_types-2.0.0a30/tests/__init__.py
--rw-r--r--   0        0        0      917 2024-03-26 01:26:24.327098 stencila_types-2.0.0a30/tests/conftest.py
--rw-r--r--   0        0        0     1280 2024-03-26 01:26:24.327180 stencila_types-2.0.0a30/tests/test_shortcuts.py
--rw-r--r--   0        0        0       73 2024-03-26 01:26:24.327296 stencila_types-2.0.0a30/tests/test_shortcuts/test_emphasis.yml
--rw-r--r--   0        0        0      120 2024-03-26 01:26:24.327362 stencila_types-2.0.0a30/tests/test_shortcuts/test_link.yml
--rw-r--r--   0        0        0      104 2024-03-26 01:26:24.327422 stencila_types-2.0.0a30/tests/test_shortcuts/test_quote.yml
--rw-r--r--   0        0        0     1362 2024-05-21 03:23:15.046422 stencila_types-2.0.0a30/tests/test_types.py
--rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 stencila_types-2.0.0a30/PKG-INFO
+-rw-r--r--   0        0        0     2734 2024-05-30 04:37:42.554297 stencila_types-2.0.0a31/README.md
+-rw-r--r--   0        0        0     2020 2024-05-30 04:38:03.978334 stencila_types-2.0.0a31/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 04:37:42.554297 stencila_types-2.0.0a31/src/stencila_types/__init__.py
+-rw-r--r--   0        0        0     8619 2024-05-30 04:37:42.554297 stencila_types-2.0.0a31/src/stencila_types/shortcuts.py
+-rw-r--r--   0        0        0    81826 2024-05-30 04:37:42.554297 stencila_types-2.0.0a31/src/stencila_types/types.py
+-rw-r--r--   0        0        0     3030 2024-05-30 04:37:42.554297 stencila_types-2.0.0a31/src/stencila_types/utilities.py
+-rw-r--r--   0        0        0        0 2024-05-30 04:37:42.554297 stencila_types-2.0.0a31/tests/__init__.py
+-rw-r--r--   0        0        0      917 2024-05-30 04:37:42.554297 stencila_types-2.0.0a31/tests/conftest.py
+-rw-r--r--   0        0        0     1280 2024-05-30 04:37:42.554297 stencila_types-2.0.0a31/tests/test_shortcuts.py
+-rw-r--r--   0        0        0       73 2024-05-30 04:37:42.554297 stencila_types-2.0.0a31/tests/test_shortcuts/test_emphasis.yml
+-rw-r--r--   0        0        0      120 2024-05-30 04:37:42.554297 stencila_types-2.0.0a31/tests/test_shortcuts/test_link.yml
+-rw-r--r--   0        0        0      104 2024-05-30 04:37:42.554297 stencila_types-2.0.0a31/tests/test_shortcuts/test_quote.yml
+-rw-r--r--   0        0        0     1362 2024-05-30 04:37:42.554297 stencila_types-2.0.0a31/tests/test_types.py
+-rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 stencila_types-2.0.0a31/PKG-INFO
```

### Comparing `stencila_types-2.0.0a30/README.md` & `stencila_types-2.0.0a31/README.md`

 * *Files identical despite different names*

### Comparing `stencila_types-2.0.0a30/pyproject.toml` & `stencila_types-2.0.0a31/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "stencila_types"
-version = "2.0.0a30"
+version = "2.0.0a31"
 description = "Python types for Stencila"
 readme = "README.md"
 authors = [
     { name = "Nokome Bentley", email = "nokome@stencila.io" },
 ]
 dependencies = [
     "cattrs>=23.2.3",
```

### Comparing `stencila_types-2.0.0a30/src/stencila_types/shortcuts.py` & `stencila_types-2.0.0a31/src/stencila_types/shortcuts.py`

 * *Files identical despite different names*

### Comparing `stencila_types-2.0.0a30/src/stencila_types/types.py` & `stencila_types-2.0.0a31/src/stencila_types/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -3292,14 +3292,15 @@
     Organization,
     Paragraph,
     Periodical,
     Person,
     PostalAddress,
     Product,
     PropertyValue,
+    ProvenanceCount,
     PublicationIssue,
     PublicationVolume,
     QuoteBlock,
     QuoteInline,
     ReplaceBlock,
     ReplaceInline,
     Review,
@@ -3331,14 +3332,15 @@
     Variable,
     VideoObject,
 ]
 
 
 UNIONS = [
     Author,
+    AuthorRoleAuthor,
     Block,
     CreativeWorkType,
     ExecutionDependantNode,
     ExecutionDependencyNode,
     Hint,
     Inline,
     MessagePart,
@@ -3348,20 +3350,20 @@
     SuggestionInlineType,
     ThingType,
     Validator,
 ]
 
 
 ANON_UNIONS = [
-    int | str,
-    StringPatch | Primitive,
+    str | float,
     PropertyValue | str,
     Grant | MonetaryGrant,
-    Cite | Text,
-    SoftwareSourceCode | SoftwareApplication | str,
-    File | Directory,
     Person | Organization,
+    int | str,
+    File | Directory,
     CreativeWorkType | Text,
-    str | float,
-    PostalAddress | str,
     Person | Organization | SoftwareApplication,
+    PostalAddress | str,
+    SoftwareSourceCode | SoftwareApplication | str,
+    Cite | Text,
+    StringPatch | Primitive,
 ]
```

### Comparing `stencila_types-2.0.0a30/src/stencila_types/utilities.py` & `stencila_types-2.0.0a31/src/stencila_types/utilities.py`

 * *Files identical despite different names*

### Comparing `stencila_types-2.0.0a30/tests/conftest.py` & `stencila_types-2.0.0a31/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `stencila_types-2.0.0a30/tests/test_shortcuts.py` & `stencila_types-2.0.0a31/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `stencila_types-2.0.0a30/tests/test_types.py` & `stencila_types-2.0.0a31/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `stencila_types-2.0.0a30/PKG-INFO` & `stencila_types-2.0.0a31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stencila_types
-Version: 2.0.0a30
+Version: 2.0.0a31
 Summary: Python types for Stencila
 Keywords: programmable,reproducible,interactive,documents,python,SDK
 Author-Email: Nokome Bentley <nokome@stencila.io>
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

