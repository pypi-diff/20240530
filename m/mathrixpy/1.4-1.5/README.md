# Comparing `tmp/mathrixpy-1.4.tar.gz` & `tmp/mathrixpy-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathrixpy-1.4.tar", last modified: Thu May 30 15:15:29 2024, max compression
+gzip compressed data, was "mathrixpy-1.5.tar", last modified: Thu May 30 16:43:11 2024, max compression
```

## Comparing `mathrixpy-1.4.tar` & `mathrixpy-1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 15:15:29.765677 mathrixpy-1.4/
--rw-rw-rw-   0        0        0     1087 2024-05-24 02:28:32.000000 mathrixpy-1.4/LICENSE
--rw-rw-rw-   0        0        0     5899 2024-05-30 15:15:29.765677 mathrixpy-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     5136 2024-05-30 15:12:38.000000 mathrixpy-1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 15:15:29.743871 mathrixpy-1.4/mathrixpy/
--rw-rw-rw-   0        0        0       23 2024-05-24 04:53:32.000000 mathrixpy-1.4/mathrixpy/__init__.py
--rw-rw-rw-   0        0        0     8614 2024-05-30 15:14:34.000000 mathrixpy-1.4/mathrixpy/base.py
--rw-rw-rw-   0        0        0     6446 2024-05-29 01:57:42.000000 mathrixpy-1.4/mathrixpy/cambios.py
-drwxrwxrwx   0        0        0        0 2024-05-30 15:15:29.763660 mathrixpy-1.4/mathrixpy.egg-info/
--rw-rw-rw-   0        0        0     5899 2024-05-30 15:15:29.000000 mathrixpy-1.4/mathrixpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2024-05-30 15:15:29.000000 mathrixpy-1.4/mathrixpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 15:15:29.000000 mathrixpy-1.4/mathrixpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-30 15:15:29.000000 mathrixpy-1.4/mathrixpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-30 15:15:29.767665 mathrixpy-1.4/setup.cfg
--rw-rw-rw-   0        0        0      857 2024-05-30 15:13:34.000000 mathrixpy-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:43:11.716762 mathrixpy-1.5/
+-rw-rw-rw-   0        0        0     1087 2024-05-24 02:28:32.000000 mathrixpy-1.5/LICENSE
+-rw-rw-rw-   0        0        0     5899 2024-05-30 16:43:11.716762 mathrixpy-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5136 2024-05-30 15:12:38.000000 mathrixpy-1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 16:43:11.694885 mathrixpy-1.5/mathrixpy/
+-rw-rw-rw-   0        0        0       23 2024-05-24 04:53:32.000000 mathrixpy-1.5/mathrixpy/__init__.py
+-rw-rw-rw-   0        0        0     8618 2024-05-30 16:42:56.000000 mathrixpy-1.5/mathrixpy/base.py
+-rw-rw-rw-   0        0        0     1139 2024-05-30 16:22:06.000000 mathrixpy-1.5/mathrixpy/cambios.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:43:11.714751 mathrixpy-1.5/mathrixpy.egg-info/
+-rw-rw-rw-   0        0        0     5899 2024-05-30 16:43:11.000000 mathrixpy-1.5/mathrixpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2024-05-30 16:43:11.000000 mathrixpy-1.5/mathrixpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 16:43:11.000000 mathrixpy-1.5/mathrixpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-30 16:43:11.000000 mathrixpy-1.5/mathrixpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-30 16:43:11.721749 mathrixpy-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      857 2024-05-30 16:43:06.000000 mathrixpy-1.5/setup.py
```

### Comparing `mathrixpy-1.4/LICENSE` & `mathrixpy-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mathrixpy-1.4/PKG-INFO` & `mathrixpy-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathrixpy
-Version: 1.4
+Version: 1.5
 Summary: mathrixpy es una biblioteca de Python para realizar operaciones matriciales. Permite la creación, manipulación y operaciones aritméticas con matrices. Esta biblioteca es útil para aplicaciones matemáticas y científicas que requieren cálculos matriciales.
 Home-page: https://github.com/Ampere-G/mathrixPy
 Author: AmJoJADeOrg
 Author-email: glroberto1810@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mathrixpy-1.4/README.md` & `mathrixpy-1.5/README.md`

 * *Files identical despite different names*

### Comparing `mathrixpy-1.4/mathrixpy/base.py` & `mathrixpy-1.5/mathrixpy/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,15 +217,15 @@
         col_widths = [max(len(str(self.datos[row][col])) for row in range(self.filas)) for col in range(self.columnas)]
         
         # Formatear cada fila con elementos centrados
         mathrixSTR = '\n'.join('\t,\t'.join(f"{str(item).center(col_widths[col])}" for col, item in enumerate(fila)) for fila in self.datos)
         return f'Matriz {self.filas}x{self.columnas}:\n{mathrixSTR}'         
 
 
-def listaToMatriz(datos:list,numFilas:int,numColumnas:int)-> object:
+def listaToMatriz(datos:list,numFilas:int,numColumnas:int)-> mathrix:
     '''
     Genera una matriz de dimensiones deseadas a partir de una lista de números
     '''
     
     if numFilas*numColumnas!=len(datos):
         raise ValueError('Verificar dimensiones')
     
@@ -235,18 +235,18 @@
     for i in range(numFilas):
         for j in range(numColumnas):
             
             M[i][j]=datos[(numColumnas*i) + j]
     
     return mathrix(M)
 
-def mIdentidad(numFila:int) -> object:
+def mIdentidad(numFila:int) -> mathrix:
         '''
         Crea una matriz diagonal con solo numeros 1 de dimensiones numFila x numFila
         '''
         M=[[0]*numFila for _ in range(numFila)]
         
         for i in range(numFila):
             M[i][i]=1
             
         return mathrix(M)
-    
+
```

### Comparing `mathrixpy-1.4/mathrixpy.egg-info/PKG-INFO` & `mathrixpy-1.5/mathrixpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathrixpy
-Version: 1.4
+Version: 1.5
 Summary: mathrixpy es una biblioteca de Python para realizar operaciones matriciales. Permite la creación, manipulación y operaciones aritméticas con matrices. Esta biblioteca es útil para aplicaciones matemáticas y científicas que requieren cálculos matriciales.
 Home-page: https://github.com/Ampere-G/mathrixPy
 Author: AmJoJADeOrg
 Author-email: glroberto1810@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mathrixpy-1.4/setup.py` & `mathrixpy-1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mathrixpy",
-    version="1.4",
+    version="1.5",
     author="AmJoJADeOrg",
     license='MIT',
     author_email="glroberto1810@gmail.com",
     description="mathrixpy es una biblioteca de Python para realizar operaciones matriciales. Permite la creación, manipulación y operaciones aritméticas con matrices. Esta biblioteca es útil para aplicaciones matemáticas y científicas que requieren cálculos matriciales.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Ampere-G/mathrixPy",
```

