# Comparing `tmp/linkml_owl-0.4.1.tar.gz` & `tmp/linkml_owl-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml_owl-0.4.1.tar", max compression
+gzip compressed data, was "linkml_owl-0.4.2.tar", max compression
```

## Comparing `linkml_owl-0.4.1.tar` & `linkml_owl-0.4.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      141 2024-05-13 02:49:29.345132 linkml_owl-0.4.1/README.md
--rw-r--r--   0        0        0      301 2024-05-13 02:49:29.349132 linkml_owl-0.4.1/linkml_owl/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 02:49:29.349132 linkml_owl-0.4.1/linkml_owl/crossproducts/__init__.py
--rw-r--r--   0        0        0     5407 2024-05-13 02:49:29.349132 linkml_owl-0.4.1/linkml_owl/crossproducts/cross_product_generator.py
--rw-r--r--   0        0        0        0 2024-05-13 02:49:29.349132 linkml_owl-0.4.1/linkml_owl/dumpers/__init__.py
--rw-r--r--   0        0        0    38550 2024-05-13 02:49:29.353132 linkml_owl-0.4.1/linkml_owl/dumpers/owl_dumper.py
--rw-r--r--   0        0        0        0 2024-05-13 02:49:29.353132 linkml_owl-0.4.1/linkml_owl/util/__init__.py
--rw-r--r--   0        0        0      659 2024-05-13 02:49:29.353132 linkml_owl-0.4.1/linkml_owl/util/csv_converter.py
--rw-r--r--   0        0        0     7763 2024-05-13 02:49:29.353132 linkml_owl-0.4.1/linkml_owl/util/loader_wrapper.py
--rw-r--r--   0        0        0      454 2024-05-13 02:49:29.353132 linkml_owl-0.4.1/linkml_owl/util/trim_yaml.py
--rw-r--r--   0        0        0     1412 2024-05-13 02:49:42.109131 linkml_owl-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1445 1970-01-01 00:00:00.000000 linkml_owl-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      141 2024-05-30 17:55:22.410040 linkml_owl-0.4.2/README.md
+-rw-r--r--   0        0        0      301 2024-05-30 17:55:22.418040 linkml_owl-0.4.2/linkml_owl/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 17:55:22.418040 linkml_owl-0.4.2/linkml_owl/crossproducts/__init__.py
+-rw-r--r--   0        0        0     5407 2024-05-30 17:55:22.418040 linkml_owl-0.4.2/linkml_owl/crossproducts/cross_product_generator.py
+-rw-r--r--   0        0        0        0 2024-05-30 17:55:22.418040 linkml_owl-0.4.2/linkml_owl/dumpers/__init__.py
+-rw-r--r--   0        0        0    39609 2024-05-30 17:55:22.418040 linkml_owl-0.4.2/linkml_owl/dumpers/owl_dumper.py
+-rw-r--r--   0        0        0        0 2024-05-30 17:55:22.418040 linkml_owl-0.4.2/linkml_owl/util/__init__.py
+-rw-r--r--   0        0        0      659 2024-05-30 17:55:22.418040 linkml_owl-0.4.2/linkml_owl/util/csv_converter.py
+-rw-r--r--   0        0        0     7763 2024-05-30 17:55:22.418040 linkml_owl-0.4.2/linkml_owl/util/loader_wrapper.py
+-rw-r--r--   0        0        0      454 2024-05-30 17:55:22.418040 linkml_owl-0.4.2/linkml_owl/util/trim_yaml.py
+-rw-r--r--   0        0        0     1412 2024-05-30 17:55:34.122161 linkml_owl-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1453 1970-01-01 00:00:00.000000 linkml_owl-0.4.2/PKG-INFO
```

### Comparing `linkml_owl-0.4.1/linkml_owl/crossproducts/cross_product_generator.py` & `linkml_owl-0.4.2/linkml_owl/crossproducts/cross_product_generator.py`

 * *Files identical despite different names*

### Comparing `linkml_owl-0.4.1/linkml_owl/dumpers/owl_dumper.py` & `linkml_owl-0.4.2/linkml_owl/dumpers/owl_dumper.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     Class, \
     AnnotationAssertion, ObjectPropertyAssertion, \
     Prefix, AnonymousIndividual, ObjectAllValuesFrom, EquivalentClasses, ObjectIntersectionOf, ClassExpression, Axiom, \
     ObjectProperty, Declaration, InverseObjectProperties, ObjectPropertyDomain, ObjectPropertyRange, \
     SubObjectPropertyOf, TransitiveObjectProperty, SymmetricObjectProperty, AsymmetricObjectProperty, \
     ReflexiveObjectProperty, IrreflexiveObjectProperty, Annotation, ObjectMinCardinality, ObjectHasValue, \
     NamedIndividual, DataSomeValuesFrom, DataHasValue, DataAllValuesFrom, AnnotationProperty, DataProperty, Datatype, \
-    DisjointClasses, DisjointUnion
+    DisjointClasses, DisjointUnion, DataPropertyAssertion
 
 from linkml_runtime.dumpers.dumper_root import Dumper
 from linkml_runtime.utils.yamlutils import YAMLRoot
 
 from linkml_owl.util.loader_wrapper import load_structured_file
 
 INTERPRETATION = str
@@ -206,18 +206,31 @@
         :param is_element_an_owl_class:
         :return: IRI or node of transformation of element
         """
         logging.debug(f"transform: {element}")
         if element is None:
             return None
         try:
-            # translate Enum
+            # naive method to test if an object is an enum:
+            # try accessing the `meaning` field. If this fails,
+            # an exception is thrown, and we carry on.
+            # (when owl_duper is refactored to not be dependent on
+            #  python dataclasses this will no longer be necessary)
             meaning = element.meaning
-            return self._get_IRI_str(meaning)
+            if is_element_an_object:
+                # enum is used in an object context: translate to URI
+                if not meaning:
+                    enum_uri = schema.default_prefix + ":" + type(element).__name__
+                    meaning = enum_uri + "#" + str(element).replace(" ", "+")
+                return self._get_IRI_str(meaning)
+            else:
+                # enum is used in a data context - stringify
+                return str(element)
         except AttributeError:
+            # not an enum - carry on
             pass
         if not self._instance_of_linkml_class(element):
             # TODO: better way of detecting atoms
             if is_element_an_object:
                 # foreign key
                 return URIRef(self._get_IRI_str(element))
             elif isinstance(element, Uriorcurie):
@@ -320,14 +333,16 @@
                 slot_uri = self._get_IRI_str(schema_level_slot.slot_uri)
             else:
                 slot_uri = self._get_IRI_str(self.schemaview.get_uri(slot.name))
             logging.debug(f'SlotVal {subj}.{k} = {v} (URI={schema_level_slot.slot_uri}) // slot = {slot.name}')
             slot_interps = self._get_slot_interpretations(slot, linkml_class_name)
             logging.debug(f'OWL interpretations for {k}={slot_interps}')
             is_object_ref = slot.range in self.schema.classes
+            if "ObjectPropertyAssertion" in slot_interps or "ObjectProperty" in slot_interps:
+                is_object_ref = True
             # normalize input_vals to a list, then recursively transform
             if isinstance(v, list):
                 input_vals = v
             elif isinstance(v, dict):
                 input_vals = v.values()
             else:
                 input_vals = [v]
@@ -386,15 +401,15 @@
                     closure_axiom_parent_expr = closure_axiom_parents[0]
                 else:
                     closure_axiom_parent_expr = ObjectUnionOf(*closure_axiom_parents)
                 self.add_axiom(SubClassOf(subj, closure_axiom_parent_expr), o, [])
             #    eai.add_operands((0, SubClassOf.__name__, ObjectUnionOf.__name__), parents, axiom_annotations)
             axiom_type = None
             # TODO: make this more generic / less repetitive
-            axiom_types = [SubClassOf, SubObjectPropertyOf, ClassAssertion, ObjectPropertyAssertion, EquivalentClasses, InverseObjectProperties,ObjectPropertyDomain, ObjectPropertyRange, AnnotationAssertion]
+            axiom_types = [SubClassOf, SubObjectPropertyOf, ClassAssertion, ObjectPropertyAssertion, DataPropertyAssertion, EquivalentClasses, InverseObjectProperties,ObjectPropertyDomain, ObjectPropertyRange, AnnotationAssertion]
             for candidate_axiom_type in axiom_types:
                 if candidate_axiom_type.__name__ in slot_interps:
                     axiom_type = candidate_axiom_type
             # fill in default axiom type
             if axiom_type is None:
                 # default: SubClassOf R some V for logical; otherwise annotation
                 if is_class_logical_axiom and not is_returns_expression:
@@ -441,14 +456,16 @@
                     elif axiom_type == EquivalentClasses:
                         axiom = EquivalentClasses(subj, parent)
                     elif axiom_type == ClassAssertion:
                         # Note: ClassAssertion axioms are "inverted"
                         axiom = ClassAssertion(parent, subj)
                     elif axiom_type == ObjectPropertyAssertion:
                         axiom = ObjectPropertyAssertion(slot_uri, subj, parent)
+                    elif axiom_type == DataPropertyAssertion:
+                        axiom = DataPropertyAssertion(slot_uri, subj, parent)
                     elif axiom_type == InverseObjectProperties:
                         axiom = InverseObjectProperties(subj, parent)
                     elif axiom_type == ObjectPropertyDomain:
                         axiom = ObjectPropertyDomain(subj, parent)
                     elif axiom_type == ObjectPropertyRange:
                         axiom = ObjectPropertyRange(subj, parent)
                     elif axiom_type == AnnotationAssertion:
```

### Comparing `linkml_owl-0.4.1/linkml_owl/util/csv_converter.py` & `linkml_owl-0.4.2/linkml_owl/util/csv_converter.py`

 * *Files identical despite different names*

### Comparing `linkml_owl-0.4.1/linkml_owl/util/loader_wrapper.py` & `linkml_owl-0.4.2/linkml_owl/util/loader_wrapper.py`

 * *Files identical despite different names*

### Comparing `linkml_owl-0.4.1/pyproject.toml` & `linkml_owl-0.4.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linkml_owl"
-version = "0.4.1"
+version = "0.4.2"
 description = "OWL mappings for Linked Open Data Modeling Language"
 authors = ["Chris Mungall <cjmungall@lbl.gov>"]
 
 readme = "README.md"
 
 homepage = "https://github.com/linkml/linkml-owl"
 repository = "https://github.com/linkml/linkml-owl"
@@ -35,15 +35,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 
 click = "*"
 funowl = ">=0.2.3"
 Jinja2 = ">=3.0.3"
-linkml = ">=1.7.4"
+linkml = "^1.7.10"
 linkml-runtime = ">=1.7.0"
 
 [tool.poetry.dev-dependencies]
 tox = ">=3.24.5"
 pytest = ">=6.2.5"
 pytest-cov = ">=3.0.0"
 mkdocs = ">=1.2.3"
```

### Comparing `linkml_owl-0.4.1/PKG-INFO` & `linkml_owl-0.4.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkml_owl
-Version: 0.4.1
+Version: 0.4.2
 Summary: OWL mappings for Linked Open Data Modeling Language
 Home-page: https://github.com/linkml/linkml-owl
 Keywords: linkml,owl
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: Jinja2 (>=3.0.3)
 Requires-Dist: click
 Requires-Dist: funowl (>=0.2.3)
-Requires-Dist: linkml (>=1.7.4)
+Requires-Dist: linkml (>=1.7.10,<2.0.0)
 Requires-Dist: linkml-runtime (>=1.7.0)
 Project-URL: Documentation, https://github.com/linkml/linkml-owl
 Project-URL: Repository, https://github.com/linkml/linkml-owl
 Description-Content-Type: text/markdown
 
 # linkml-owl
```

