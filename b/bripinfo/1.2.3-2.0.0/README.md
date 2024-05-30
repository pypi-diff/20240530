# Comparing `tmp/bripinfo-1.2.3.tar.gz` & `tmp/bripinfo-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bripinfo-1.2.3.tar", max compression
+gzip compressed data, was "bripinfo-2.0.0.tar", max compression
```

## Comparing `bripinfo-1.2.3.tar` & `bripinfo-2.0.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1080 2021-10-04 13:25:23.595255 bripinfo-1.2.3/LICENSE
--rw-r--r--   0        0        0     4147 2021-10-04 13:25:23.595255 bripinfo-1.2.3/README.md
--rw-r--r--   0        0        0        0 2021-10-04 13:25:23.595255 bripinfo-1.2.3/bripinfo/.files/.gitkeep
--rw-r--r--   0        0        0       22 2021-10-04 13:25:23.595255 bripinfo-1.2.3/bripinfo/__init__.py
--rw-r--r--   0        0        0       63 2021-10-04 13:25:23.595255 bripinfo-1.2.3/bripinfo/__main__.py
--rw-r--r--   0        0        0     1615 2021-10-04 15:24:09.472170 bripinfo-1.2.3/bripinfo/commands.py
--rw-r--r--   0        0        0     4119 2021-12-13 14:07:27.595787 bripinfo-1.2.3/bripinfo/core.py
--rw-r--r--   0        0        0     2458 2021-10-04 15:27:01.544609 bripinfo-1.2.3/bripinfo/registro_br.py
--rw-r--r--   0        0        0      736 2021-10-04 15:26:14.056470 bripinfo-1.2.3/bripinfo/settings.py
--rw-r--r--   0        0        0      732 2021-12-13 14:02:22.044404 bripinfo-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     5070 2021-12-13 14:24:15.983378 bripinfo-1.2.3/setup.py
--rw-r--r--   0        0        0     4932 2021-12-13 14:24:15.984417 bripinfo-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-05-30 19:50:50.958532 bripinfo-2.0.0/LICENSE
+-rw-r--r--   0        0        0     4147 2024-05-30 19:50:50.958532 bripinfo-2.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-30 20:09:29.301098 bripinfo-2.0.0/bripinfo/.files/.gitkeep
+-rw-r--r--   0        0        0       22 2024-05-30 19:50:50.958532 bripinfo-2.0.0/bripinfo/__init__.py
+-rw-r--r--   0        0        0       63 2024-05-30 19:50:50.958532 bripinfo-2.0.0/bripinfo/__main__.py
+-rw-r--r--   0        0        0     1615 2024-05-30 19:50:50.958532 bripinfo-2.0.0/bripinfo/commands.py
+-rw-r--r--   0        0        0     4119 2024-05-30 19:50:50.958532 bripinfo-2.0.0/bripinfo/core.py
+-rw-r--r--   0        0        0     2497 2024-05-30 20:55:21.141661 bripinfo-2.0.0/bripinfo/registro_br.py
+-rw-r--r--   0        0        0      736 2024-05-30 19:50:50.958532 bripinfo-2.0.0/bripinfo/settings.py
+-rw-r--r--   0        0        0      725 2024-05-30 20:07:58.778189 bripinfo-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4869 1970-01-01 00:00:00.000000 bripinfo-2.0.0/PKG-INFO
```

### Comparing `bripinfo-1.2.3/LICENSE` & `bripinfo-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bripinfo-1.2.3/README.md` & `bripinfo-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `bripinfo-1.2.3/bripinfo/commands.py` & `bripinfo-2.0.0/bripinfo/commands.py`

 * *Files identical despite different names*

### Comparing `bripinfo-1.2.3/bripinfo/core.py` & `bripinfo-2.0.0/bripinfo/core.py`

 * *Files identical despite different names*

### Comparing `bripinfo-1.2.3/bripinfo/registro_br.py` & `bripinfo-2.0.0/bripinfo/registro_br.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,22 +66,25 @@
     source = 'Registro.br'
 
     def _data(self) -> dict:
         content = self._raw_content
 
         settings.LOGGER.info('Estruturando o conteúdo do Registro.br')
         content = [line.split('|') for line in content.splitlines()]
+
         dataset = [
             {
                 'ref': line[0],
                 'name': line[1],
                 'cnpj': line[2],
                 'ips': list(line[3:])
             }
-            for line in content]
+            for line in content
+            if len(line) > 3
+        ]
 
         return dataset
 
     def _can_save(self):
         return True
```

### Comparing `bripinfo-1.2.3/bripinfo/settings.py` & `bripinfo-2.0.0/bripinfo/settings.py`

 * *Files identical despite different names*

### Comparing `bripinfo-1.2.3/PKG-INFO` & `bripinfo-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: bripinfo
-Version: 1.2.3
+Version: 2.0.0
 Summary: Uma maneira fácil de obter dados relativos a um IP associado ao Registro.br.
 Home-page: https://github.com/rogeriopaulos/BRIpinfo
 License: MIT
 Author: Rogerio Paulo
 Author-email: rogeriopaulos@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: click (>=8.0.0,<9.0.0)
-Requires-Dist: requests (>=2.25.0,<3.0.0)
-Requires-Dist: urllib3 (>=1.26.5)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: click (==8.1.7)
+Requires-Dist: requests (==2.32.3)
+Requires-Dist: urllib3 (==2.2.1)
 Project-URL: Documentation, https://github.com/rogeriopaulos/BRIpinfo
 Project-URL: Repository, https://github.com/rogeriopaulos/BRIpinfo
 Description-Content-Type: text/markdown
 
 # BrIpInfo
 
 ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/rogeriopaulos/BRIpinfo?label=BRIpinfo&style=flat-square)
```

