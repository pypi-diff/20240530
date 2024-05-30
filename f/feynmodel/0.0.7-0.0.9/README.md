# Comparing `tmp/feynmodel-0.0.7.tar.gz` & `tmp/feynmodel-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feynmodel-0.0.7.tar", max compression
+gzip compressed data, was "feynmodel-0.0.9.tar", max compression
```

## Comparing `feynmodel-0.0.7.tar` & `feynmodel-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35149 2024-04-07 20:35:03.588693 feynmodel-0.0.7/LICENSE
--rw-r--r--   0        0        0     2374 2024-04-07 20:35:03.588693 feynmodel-0.0.7/README.md
--rw-r--r--   0        0        0      176 2024-04-07 20:35:03.588693 feynmodel-0.0.7/feynmodel/__init__.py
--rw-r--r--   0        0        0      336 2024-04-07 20:35:03.588693 feynmodel-0.0.7/feynmodel/coupling.py
--rw-r--r--   0        0        0      284 2024-04-07 20:35:03.588693 feynmodel-0.0.7/feynmodel/coupling_order.py
--rw-r--r--   0        0        0      447 2024-04-07 20:35:03.588693 feynmodel-0.0.7/feynmodel/decay.py
--rw-r--r--   0        0        0     7475 2024-04-07 20:35:03.588693 feynmodel-0.0.7/feynmodel/feyn_model.py
--rw-r--r--   0        0        0      340 2024-04-07 20:35:03.588693 feynmodel-0.0.7/feynmodel/form_factor.py
--rw-r--r--   0        0        0      383 2024-04-07 20:35:03.588693 feynmodel-0.0.7/feynmodel/function.py
--rw-r--r--   0        0        0        0 2024-04-07 20:35:03.588693 feynmodel-0.0.7/feynmodel/interface/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 20:35:03.588693 feynmodel-0.0.7/feynmodel/interface/feynarts.py
--rw-r--r--   0        0        0     3183 2024-04-07 20:35:03.588693 feynmodel-0.0.7/feynmodel/interface/qgraf.py
--rw-r--r--   0        0        0     5250 2024-04-07 20:35:03.588693 feynmodel-0.0.7/feynmodel/interface/ufo.py
--rw-r--r--   0        0        0      354 2024-04-07 20:35:03.588693 feynmodel-0.0.7/feynmodel/lorentz.py
--rw-r--r--   0        0        0        0 2024-04-07 20:35:03.592693 feynmodel-0.0.7/feynmodel/model/__init__.py
--rw-r--r--   0        0        0      277 2024-04-07 20:35:03.592693 feynmodel-0.0.7/feynmodel/model/mssm.py
--rw-r--r--   0        0        0      248 2024-04-07 20:35:03.592693 feynmodel-0.0.7/feynmodel/model/sm.py
--rw-r--r--   0        0        0      689 2024-04-07 20:35:03.592693 feynmodel-0.0.7/feynmodel/parameter.py
--rw-r--r--   0        0        0     3252 2024-04-07 20:35:03.592693 feynmodel-0.0.7/feynmodel/particle.py
--rw-r--r--   0        0        0     1313 2024-04-07 20:35:03.592693 feynmodel-0.0.7/feynmodel/ufo_base_class.py
--rw-r--r--   0        0        0      777 2024-04-07 20:35:03.592693 feynmodel-0.0.7/feynmodel/util.py
--rw-r--r--   0        0        0      563 2024-04-07 20:35:03.592693 feynmodel-0.0.7/feynmodel/vertex.py
--rw-r--r--   0        0        0     1937 2024-04-07 20:35:04.880676 feynmodel-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3222 1970-01-01 00:00:00.000000 feynmodel-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-30 08:53:26.843416 feynmodel-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2374 2024-05-30 08:53:26.843416 feynmodel-0.0.9/README.md
+-rw-r--r--   0        0        0      176 2024-05-30 08:53:26.843416 feynmodel-0.0.9/feynmodel/__init__.py
+-rw-r--r--   0        0        0      336 2024-05-30 08:53:26.843416 feynmodel-0.0.9/feynmodel/coupling.py
+-rw-r--r--   0        0        0      284 2024-05-30 08:53:26.843416 feynmodel-0.0.9/feynmodel/coupling_order.py
+-rw-r--r--   0        0        0      447 2024-05-30 08:53:26.843416 feynmodel-0.0.9/feynmodel/decay.py
+-rw-r--r--   0        0        0     7781 2024-05-30 08:53:26.843416 feynmodel-0.0.9/feynmodel/feyn_model.py
+-rw-r--r--   0        0        0      340 2024-05-30 08:53:26.843416 feynmodel-0.0.9/feynmodel/form_factor.py
+-rw-r--r--   0        0        0      383 2024-05-30 08:53:26.843416 feynmodel-0.0.9/feynmodel/function.py
+-rw-r--r--   0        0        0        0 2024-05-30 08:53:26.843416 feynmodel-0.0.9/feynmodel/interface/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 08:53:26.843416 feynmodel-0.0.9/feynmodel/interface/feynarts.py
+-rw-r--r--   0        0        0     3239 2024-05-30 08:53:26.843416 feynmodel-0.0.9/feynmodel/interface/qgraf.py
+-rw-r--r--   0        0        0     5250 2024-05-30 08:53:26.843416 feynmodel-0.0.9/feynmodel/interface/ufo.py
+-rw-r--r--   0        0        0      354 2024-05-30 08:53:26.843416 feynmodel-0.0.9/feynmodel/lorentz.py
+-rw-r--r--   0        0        0        0 2024-05-30 08:53:26.843416 feynmodel-0.0.9/feynmodel/model/__init__.py
+-rw-r--r--   0        0        0      277 2024-05-30 08:53:26.843416 feynmodel-0.0.9/feynmodel/model/mssm.py
+-rw-r--r--   0        0        0      248 2024-05-30 08:53:26.843416 feynmodel-0.0.9/feynmodel/model/sm.py
+-rw-r--r--   0        0        0      689 2024-05-30 08:53:26.843416 feynmodel-0.0.9/feynmodel/parameter.py
+-rw-r--r--   0        0        0     3392 2024-05-30 08:53:26.843416 feynmodel-0.0.9/feynmodel/particle.py
+-rw-r--r--   0        0        0     1313 2024-05-30 08:53:26.843416 feynmodel-0.0.9/feynmodel/ufo_base_class.py
+-rw-r--r--   0        0        0      777 2024-05-30 08:53:26.843416 feynmodel-0.0.9/feynmodel/util.py
+-rw-r--r--   0        0        0      563 2024-05-30 08:53:26.843416 feynmodel-0.0.9/feynmodel/vertex.py
+-rw-r--r--   0        0        0     1937 2024-05-30 08:53:28.063411 feynmodel-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3222 1970-01-01 00:00:00.000000 feynmodel-0.0.9/PKG-INFO
```

### Comparing `feynmodel-0.0.7/LICENSE` & `feynmodel-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `feynmodel-0.0.7/README.md` & `feynmodel-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `feynmodel-0.0.7/feynmodel/feyn_model.py` & `feynmodel-0.0.9/feynmodel/feyn_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,42 +46,47 @@
 
         Contrary to the direct remove functions, this function will also remove
         all references to the object in other objects. For example, if a particle
         is removed, all vertices containing the particle will also be removed.
         """
         if isinstance(obj, Particle):
             self.remove_particle(obj)
-            rmv = []
-            for v in self.vertices:
-                if obj in v.particles:
-                    rmv += [v]
-            for v in rmv:
-                self.remove_vertex(v)
-            rmd = []
-            for d in self.decays:
-                if obj == d.particle:
-                    rmd += [d]
-            for d in rmd:
-                self.remove_decay(d)
         else:
             raise NotImplementedError("remove_object %s" % obj.__class__.__name__)
 
     ##############################
     # Particle related functions #
     ##############################
 
     def add_particle(self, particle):
         if particle not in self.particles:
             self.particles.append(particle)
         else:
             raise Exception("Particle %s already exists" % particle)
 
-    def remove_particle(self, particle):
+    def remove_particle(self, particle, remove_vertices=True, remove_decays=True):
         if particle in self.particles:
             self.particles.remove(particle)
+            rmv = []
+            for vertex in self.vertices:
+                if particle in vertex.particles:
+                    rmv += [vertex]
+            for vertex in rmv:
+                self.remove_vertex(vertex)
+            rmd = []
+            for decay in self.decays:
+                if particle == decay.particle:
+                    rmd += [decay]
+            for decay in rmd:
+                self.remove_decay(decay)
+            # remove anti if anti exists
+            if particle.has_anti():
+                anti = self.get_particle(particle.antiname)
+                if anti:
+                    self.remove_particle(anti)
         else:
             raise Exception("Particle %s does not exist" % particle)
 
     def get_particle(self, name=None, pdg_code=None):
         """Return particle with given name or pdg_code"""
         for particle in self.particles:
             if (name is None or particle.name == name) and (
```

### Comparing `feynmodel-0.0.7/feynmodel/interface/qgraf.py` & `feynmodel-0.0.9/feynmodel/interface/qgraf.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 
 
 def pdg_id_to_qgraf_name(
     feynmodel: FeynModel, pdg_id: int, use_pdg_names: bool = False
 ) -> Optional[str]:
     for p in feynmodel.particles:
         if p.pdg_code == pdg_id:
-            return get_particle_name(p, use_pdg_names, anti=pdg_id < 0)
+            #return get_particle_name(p, use_pdg_names, anti=pdg_id < 0)
+            return get_particle_name(p, use_pdg_names)
     return None
 
 
 def feynmodel_to_qgraf(
     feynmodel: FeynModel,
     use_pdg_names: bool = False,
     include_antiparticles: bool = False,
```

### Comparing `feynmodel-0.0.7/feynmodel/interface/ufo.py` & `feynmodel-0.0.9/feynmodel/interface/ufo.py`

 * *Files identical despite different names*

### Comparing `feynmodel-0.0.7/feynmodel/parameter.py` & `feynmodel-0.0.9/feynmodel/parameter.py`

 * *Files identical despite different names*

### Comparing `feynmodel-0.0.7/feynmodel/particle.py` & `feynmodel-0.0.9/feynmodel/particle.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from feynmodel.ufo_base_class import UFOBaseClass
 
 
 class Particle(UFOBaseClass):
     """A standard Particle"""
 
     require_args = [
@@ -108,15 +109,21 @@
         elif spin == 5:
             return "double"
         elif spin == -1:
             return "dotted"
         else:
             return "dashed"  # not supported yet
 
+    def has_anti(self):
+        return not self.selfconjugate
+
     def anti(self):
+        """
+        This function might be less 
+        """
         if self.selfconjugate:
             raise Exception("%s has no anti particle." % self.name)
         outdic = {}
         for k, v in self.__dict__.items():
             if k not in self.require_args_all:
                 outdic[k] = -v
         if self.color in [1, 8]:
```

### Comparing `feynmodel-0.0.7/feynmodel/ufo_base_class.py` & `feynmodel-0.0.9/feynmodel/ufo_base_class.py`

 * *Files identical despite different names*

### Comparing `feynmodel-0.0.7/feynmodel/util.py` & `feynmodel-0.0.9/feynmodel/util.py`

 * *Files identical despite different names*

### Comparing `feynmodel-0.0.7/feynmodel/vertex.py` & `feynmodel-0.0.9/feynmodel/vertex.py`

 * *Files identical despite different names*

### Comparing `feynmodel-0.0.7/pyproject.toml` & `feynmodel-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "feynmodel"
-version = "0.0.7"
+version = "0.0.9"
 description = "Models for constructing Feynman diagrams"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/feynmodel"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `feynmodel-0.0.7/PKG-INFO` & `feynmodel-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feynmodel
-Version: 0.0.7
+Version: 0.0.9
 Summary: Models for constructing Feynman diagrams
 Home-page: https://github.com/APN-Pucky/feynmodel
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

