# Comparing `tmp/baml_py-0.30.0-cp38-abi3-win_amd64.whl.zip` & `tmp/baml_py-0.30.2-cp38-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 4450385 bytes, number of entries: 13
--rw-r--r--  4.6 unx      337 b- defN 24-May-30 08:33 baml_py-0.30.0.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 24-May-30 08:33 baml_py-0.30.0.dist-info/WHEEL
--rw-r--r--  4.6 unx       54 b- defN 24-May-30 08:33 baml_py-0.30.0.dist-info/entry_points.txt
--rw-r--r--  4.6 unx    11556 b- defN 24-May-30 08:33 baml_py-0.30.0.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx    11556 b- defN 24-May-30 08:33 baml_py-0.30.0.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx     3422 b- defN 24-May-30 08:33 baml_py/async_context_vars.py
--rw-r--r--  4.6 unx     4095 b- defN 24-May-30 08:33 baml_py/baml_py.pyi
--rw-r--r--  4.6 unx        0 b- defN 24-May-30 08:33 baml_py/py.typed
--rw-r--r--  4.6 unx     2474 b- defN 24-May-30 08:33 baml_py/stream.py
--rw-r--r--  4.6 unx     4330 b- defN 24-May-30 08:33 baml_py/type_builder.py
--rw-r--r--  4.6 unx      506 b- defN 24-May-30 08:33 baml_py/__init__.py
--rwxr-xr-x  4.6 unx 11762688 b- defN 24-May-30 08:33 baml_py/baml_py.pyd
--rw-r--r--  4.6 unx     1053 b- defN 24-May-30 08:33 baml_py-0.30.0.dist-info/RECORD
-13 files, 11802165 bytes uncompressed, 4448637 bytes compressed:  62.3%
+Zip file size: 4450387 bytes, number of entries: 13
+-rw-r--r--  4.6 unx      354 b- defN 24-May-30 16:08 baml_py-0.30.2.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 24-May-30 16:08 baml_py-0.30.2.dist-info/WHEEL
+-rw-r--r--  4.6 unx       54 b- defN 24-May-30 16:08 baml_py-0.30.2.dist-info/entry_points.txt
+-rw-r--r--  4.6 unx    11556 b- defN 24-May-30 16:08 baml_py-0.30.2.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx    11556 b- defN 24-May-30 16:08 baml_py-0.30.2.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx     3422 b- defN 24-May-30 16:08 baml_py/async_context_vars.py
+-rw-r--r--  4.6 unx     4070 b- defN 24-May-30 16:08 baml_py/baml_py.pyi
+-rw-r--r--  4.6 unx        0 b- defN 24-May-30 16:08 baml_py/py.typed
+-rw-r--r--  4.6 unx     2474 b- defN 24-May-30 16:08 baml_py/stream.py
+-rw-r--r--  4.6 unx     4330 b- defN 24-May-30 16:08 baml_py/type_builder.py
+-rw-r--r--  4.6 unx      506 b- defN 24-May-30 16:08 baml_py/__init__.py
+-rwxr-xr-x  4.6 unx 11762688 b- defN 24-May-30 16:08 baml_py/baml_py.pyd
+-rw-r--r--  4.6 unx     1053 b- defN 24-May-30 16:08 baml_py-0.30.2.dist-info/RECORD
+13 files, 11802157 bytes uncompressed, 4448639 bytes compressed:  62.3%
```

## zipnote {}

```diff
@@ -1,20 +1,20 @@
-Filename: baml_py-0.30.0.dist-info/METADATA
+Filename: baml_py-0.30.2.dist-info/METADATA
 Comment: 
 
-Filename: baml_py-0.30.0.dist-info/WHEEL
+Filename: baml_py-0.30.2.dist-info/WHEEL
 Comment: 
 
-Filename: baml_py-0.30.0.dist-info/entry_points.txt
+Filename: baml_py-0.30.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: baml_py-0.30.0.dist-info/license_files/LICENSE
+Filename: baml_py-0.30.2.dist-info/license_files/LICENSE
 Comment: 
 
-Filename: baml_py-0.30.0.dist-info/license_files/LICENSE
+Filename: baml_py-0.30.2.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: baml_py/async_context_vars.py
 Comment: 
 
 Filename: baml_py/baml_py.pyi
 Comment: 
@@ -30,11 +30,11 @@
 
 Filename: baml_py/__init__.py
 Comment: 
 
 Filename: baml_py/baml_py.pyd
 Comment: 
 
-Filename: baml_py-0.30.0.dist-info/RECORD
+Filename: baml_py-0.30.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## baml_py/baml_py.pyi

```diff
@@ -88,15 +88,15 @@
     def float(self) -> FieldType: ...
     def bool(self) -> FieldType: ...
     def list(self, element_type: FieldType) -> FieldType: ...
     def null(self) -> FieldType: ...
     def optional(self, inner_type: FieldType) -> FieldType: ...
 
 class FieldType:
-    def list(self, element_type: FieldType) -> FieldType: ...
+    def list(self) -> FieldType: ...
     def optional(self) -> FieldType: ...
 
 class EnumBuilder:
     def value(self, name: str) -> EnumValueBuilder: ...
     def alias(self, alias: Optional[str]) -> EnumBuilder: ...
     def field(self) -> FieldType: ...
```

## Comparing `baml_py-0.30.0.dist-info/license_files/LICENSE` & `baml_py-0.30.2.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

## Comparing `baml_py-0.30.0.dist-info/RECORD` & `baml_py-0.30.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-baml_py-0.30.0.dist-info/METADATA,sha256=lVJEJWOjCw5PuJGyIFwxUFuMwv34DMqOQd02U14eedc,337
-baml_py-0.30.0.dist-info/WHEEL,sha256=_-pO1V0R3bpcg5FhWC82Cl79freIhF1O9I5uv0may5k,94
-baml_py-0.30.0.dist-info/entry_points.txt,sha256=9Uu_VcUjoI2qQMjVb0PRjEgI6pQ55WqBbzNparAPJyA,54
-baml_py-0.30.0.dist-info/license_files/LICENSE,sha256=WtjCEwlcVzkh1ziO35P2qfVEkLjr87Flro7xlHz3CEY,11556
-baml_py-0.30.0.dist-info/license_files/LICENSE,sha256=WtjCEwlcVzkh1ziO35P2qfVEkLjr87Flro7xlHz3CEY,11556
+baml_py-0.30.2.dist-info/METADATA,sha256=OT4XjteRU8DL6x5-WBSI3wVmCB38IRXYvvSzJsgBsK0,354
+baml_py-0.30.2.dist-info/WHEEL,sha256=_-pO1V0R3bpcg5FhWC82Cl79freIhF1O9I5uv0may5k,94
+baml_py-0.30.2.dist-info/entry_points.txt,sha256=9Uu_VcUjoI2qQMjVb0PRjEgI6pQ55WqBbzNparAPJyA,54
+baml_py-0.30.2.dist-info/license_files/LICENSE,sha256=WtjCEwlcVzkh1ziO35P2qfVEkLjr87Flro7xlHz3CEY,11556
+baml_py-0.30.2.dist-info/license_files/LICENSE,sha256=WtjCEwlcVzkh1ziO35P2qfVEkLjr87Flro7xlHz3CEY,11556
 baml_py/async_context_vars.py,sha256=gU_H0abCPxxULNRUArMlsx2aeLNp7E7fIVBY6nLY_F0,3422
-baml_py/baml_py.pyi,sha256=loMZFT2iecP59NwPzqtFxvRvNIjgB8bgLvmufg9Y8sQ,4095
+baml_py/baml_py.pyi,sha256=wGHs0y6RjeTl3-aqY9tCAdvo-fCqeb6i4k0fvK-m93Q,4070
 baml_py/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 baml_py/stream.py,sha256=B4mpGnqAmU7DFHJPiAAAiNIeX5wgLJhXLZp9Pqb9-AY,2474
 baml_py/type_builder.py,sha256=v3yiY2VtGuCEECr0jh7OB3ueWSiSwj-8IETXQuSIYl0,4330
 baml_py/__init__.py,sha256=-y49naDuvHdmpkmUEqZBESlBNx6W4qsPOPu9KlrMT10,506
-baml_py/baml_py.pyd,sha256=Uqq7VoFkJfBr6N7RMLFU5JEybBgoNkyOeVP-ZytNUZ8,11762688
-baml_py-0.30.0.dist-info/RECORD,,
+baml_py/baml_py.pyd,sha256=XLtuC_XkQw2dM5bQY9UCV2dsOkLUZUi8KV5KnFO9vwM,11762688
+baml_py-0.30.2.dist-info/RECORD,,
```

