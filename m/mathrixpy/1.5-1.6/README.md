# Comparing `tmp/mathrixpy-1.5.tar.gz` & `tmp/mathrixpy-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathrixpy-1.5.tar", last modified: Thu May 30 16:43:11 2024, max compression
+gzip compressed data, was "mathrixpy-1.6.tar", last modified: Thu May 30 16:53:20 2024, max compression
```

## Comparing `mathrixpy-1.5.tar` & `mathrixpy-1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 16:43:11.716762 mathrixpy-1.5/
--rw-rw-rw-   0        0        0     1087 2024-05-24 02:28:32.000000 mathrixpy-1.5/LICENSE
--rw-rw-rw-   0        0        0     5899 2024-05-30 16:43:11.716762 mathrixpy-1.5/PKG-INFO
--rw-rw-rw-   0        0        0     5136 2024-05-30 15:12:38.000000 mathrixpy-1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 16:43:11.694885 mathrixpy-1.5/mathrixpy/
--rw-rw-rw-   0        0        0       23 2024-05-24 04:53:32.000000 mathrixpy-1.5/mathrixpy/__init__.py
--rw-rw-rw-   0        0        0     8618 2024-05-30 16:42:56.000000 mathrixpy-1.5/mathrixpy/base.py
--rw-rw-rw-   0        0        0     1139 2024-05-30 16:22:06.000000 mathrixpy-1.5/mathrixpy/cambios.py
-drwxrwxrwx   0        0        0        0 2024-05-30 16:43:11.714751 mathrixpy-1.5/mathrixpy.egg-info/
--rw-rw-rw-   0        0        0     5899 2024-05-30 16:43:11.000000 mathrixpy-1.5/mathrixpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2024-05-30 16:43:11.000000 mathrixpy-1.5/mathrixpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 16:43:11.000000 mathrixpy-1.5/mathrixpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-30 16:43:11.000000 mathrixpy-1.5/mathrixpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-30 16:43:11.721749 mathrixpy-1.5/setup.cfg
--rw-rw-rw-   0        0        0      857 2024-05-30 16:43:06.000000 mathrixpy-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:53:20.298056 mathrixpy-1.6/
+-rw-rw-rw-   0        0        0     1087 2024-05-24 02:28:32.000000 mathrixpy-1.6/LICENSE
+-rw-rw-rw-   0        0        0     5899 2024-05-30 16:53:20.297095 mathrixpy-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5136 2024-05-30 15:12:38.000000 mathrixpy-1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 16:53:20.275029 mathrixpy-1.6/mathrixpy/
+-rw-rw-rw-   0        0        0       23 2024-05-24 04:53:32.000000 mathrixpy-1.6/mathrixpy/__init__.py
+-rw-rw-rw-   0        0        0     8705 2024-05-30 16:52:54.000000 mathrixpy-1.6/mathrixpy/base.py
+-rw-rw-rw-   0        0        0      921 2024-05-30 16:50:40.000000 mathrixpy-1.6/mathrixpy/cambios.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:53:20.295074 mathrixpy-1.6/mathrixpy.egg-info/
+-rw-rw-rw-   0        0        0     5899 2024-05-30 16:53:20.000000 mathrixpy-1.6/mathrixpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2024-05-30 16:53:20.000000 mathrixpy-1.6/mathrixpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 16:53:20.000000 mathrixpy-1.6/mathrixpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-30 16:53:20.000000 mathrixpy-1.6/mathrixpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-30 16:53:20.306056 mathrixpy-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      857 2024-05-30 16:53:03.000000 mathrixpy-1.6/setup.py
```

### Comparing `mathrixpy-1.5/LICENSE` & `mathrixpy-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mathrixpy-1.5/PKG-INFO` & `mathrixpy-1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathrixpy
-Version: 1.5
+Version: 1.6
 Summary: mathrixpy es una biblioteca de Python para realizar operaciones matriciales. Permite la creación, manipulación y operaciones aritméticas con matrices. Esta biblioteca es útil para aplicaciones matemáticas y científicas que requieren cálculos matriciales.
 Home-page: https://github.com/Ampere-G/mathrixPy
 Author: AmJoJADeOrg
 Author-email: glroberto1810@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mathrixpy-1.5/README.md` & `mathrixpy-1.6/README.md`

 * *Files identical despite different names*

### Comparing `mathrixpy-1.5/mathrixpy/base.py` & `mathrixpy-1.6/mathrixpy/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 class mathrix:
-    def __init__(self,datos:list)-> object:   #Incializa la clase
+    def __init__(self,datos:list)-> 'mathrix':   #Incializa la clase
         
         '''
         Convierte una lista de lista a matriz
         '''
         
         self.datos=datos #Se ingresa una lista de listas
         self.filas=len(datos) #El número de elementos de las lista de datos es igual a el numero de filas
         self.columnas=len(datos[0]) #El número de elementos de cada fila es igual al número de columnas
     
         if not self.__verificar_matriz(): 
             raise ValueError("Todas las filas deben tener la misma longitud")
         
-    def __verificar_matriz(self:object) -> bool:
+    def __verificar_matriz(self:'mathrix') -> bool:
         '''
         Comprueba que la longitud de todas las filas sea la misma
         '''
         return all(len(fila)==self.columnas for fila in self.datos)
         
     def __dimension_igual(self,other) -> bool:
         '''
         Verifica si dos matrices tienen la misma dimensión
         '''
         
         return self.filas==other.filas and self.columnas==other.columnas
     
-    def __matriz_cuadrada_error(self:object) -> bool:
+    def __matriz_cuadrada_error(self:'mathrix') -> bool:
         if self.filas!=self.columnas:
             raise ValueError('La matriz no es cuadrada')
         
         return True
     
-    def get_Datos(self:object) -> list:
+    def get_Datos(self:'mathrix') -> list:
         '''
         Regresa los datos pertenecientes a la matriz en forma de lista
         '''
         return self.datos
         
-    def __add__(self:object,other:object) -> object:
+    def __add__(self:'mathrix',other:'mathrix') -> 'mathrix':
         '''
         Suma dos matrices (Tienen que tener las mismas dimensiones)
         '''
         
         if not self.__dimension_igual(other):
             raise ValueError('Las matrices tienen que tener las mismas dimensiones')
         
@@ -49,15 +49,15 @@
         
         for i in range((self.filas)):
             for j in range((self.columnas)):  
                 matrix[i][j]=self.datos[i][j]+other.datos[i][j]
             
         return mathrix(matrix)
     
-    def __sub__(self:object,other:object) -> object:
+    def __sub__(self:'mathrix',other:'mathrix') -> 'mathrix':
         '''
         Resta de dos matrices (Tienen que tener las mismas dimensiones)
         '''
 
         if not self.__dimension_igual(other):
             raise ValueError('Las matrices tienen que tener las mismas dimensiones')
         
@@ -65,15 +65,15 @@
         
         for i in range((self.filas)):
             for j in range((self.columnas)):  
                 matrix[i][j]=self.datos[i][j]-other.datos[i][j]
             
         return mathrix(matrix)
      
-    def prod(self:object,*args:object) -> object:
+    def prod(self:'mathrix',*args:'mathrix') -> 'mathrix':
         '''
         Multiplica una matriz por otra u otras matrices
         '''
         original=self
         
         
         for matriz in args:
@@ -87,56 +87,56 @@
                     suma=0
                     for k in range(original.columnas):
                         suma+=original.datos[i][k] * matriz.datos[k][j]
                     resultado[i][j]=suma
             original=mathrix(resultado)
         return mathrix(resultado)
     
-    def scalar_mul(self:object,scalar:float) -> object:
+    def scalar_mul(self:'mathrix',scalar:float) -> 'mathrix':
         '''
         Multiplica una matriz por un escalar
         '''
         
         matrix=[[0]*self.columnas for _ in range(self.filas)]
         
         for i in range(self.filas):
             for j in range(self.columnas):
                 matrix[i][j]=self.datos[i][j]*scalar
         
         return mathrix(matrix)
 
-    def tr(self:object) -> float:
+    def tr(self:'mathrix') -> float:
         '''
         Devulve la suma de los elementos diagonales de una matriz cuadrada
         '''
         
         if not self.filas==self.columnas:
             raise ValueError('La matriz tiene que ser cuadrada')
         
         traza=0
         
         for i in range(self.filas):
                 traza+=self.datos[i][i]
                 
         return traza
         
-    def transpuesta(self:object) -> object:
+    def transpuesta(self:'mathrix') -> 'mathrix':
         '''
         Devuelve una matriz con los indices alrrevez
         '''
         matrix=[[0]*self.filas for _ in range(self.columnas)]
         
         
         for i in range(self.filas):
             for j in range(self.columnas):
                 matrix[j][i]=self.datos[i][j]
 
         return mathrix(matrix)
     
-    def potencia(self:object,potencia:int) ->object:
+    def potencia(self:'mathrix',potencia:int) ->'mathrix':
         '''
         Eleva una matriz cuadrada a una potencia entera
         '''
         self.__matriz_cuadrada_error()
         
         if potencia <-1:
             raise ValueError('La potencia tiene que ser mayor o igual que -1')
@@ -147,15 +147,15 @@
         
         if potencia==-1:
             return self.inversa()
         for _ in range(1,potencia):
             original=original.prod(self)
         return(original)
 
-    def determinante(self:object) -> float:
+    def determinante(self:'mathrix') -> float:
         '''
         Calcula la determinante de una matriz - Tiene que ser cuadrada
         '''
         
         if self.filas!=self.columnas:
             raise ValueError('La matriz tiene que ser cuadrada')
         
@@ -172,51 +172,51 @@
             
             cofactor=(-1)**columna * self.datos[0][columna]*(mathrix(menor).determinante())
             
             det+=cofactor
             
         return det
     
-    def submatriz(self:object, fila:int, columna:int) -> object:
+    def submatriz(self:'mathrix', fila:int, columna:int) -> 'mathrix':
         '''
         Devuelve una submatriz excluyendo la fila y columna especificada
         '''
         submat = [row[:columna] + row[columna + 1:] for row in (self.datos[:fila] + self.datos[fila + 1:])]
         return mathrix(submat)
         
-    def cofactor(self:object, fila:int, columna:int) ->float :
+    def cofactor(self:'mathrix', fila:int, columna:int) ->float :
         '''
         Calcula el cofactor de un elemento en la fila y columna especificada
         '''
         submat = self.submatriz(fila, columna)
         return ((-1) ** (fila + columna)) * submat.determinante()
 
-    def adjunta(self:object) ->object:
+    def adjunta(self:'mathrix') ->'mathrix':
         '''
         Devuelve la matriz adjunta de una matriz
         '''
         self.__matriz_cuadrada_error()
         
         Matrizp = [[self.cofactor(i, j) for j in range(self.columnas)] for i in range(self.filas)]
         Adj = mathrix(Matrizp).transpuesta()
         return Adj
 
-    def inversa(self:object) -> object:
+    def inversa(self:'mathrix') -> 'mathrix':
         
         '''
         Regrea la inversa de cualquier matriz cuadrada
         '''
         self.__matriz_cuadrada_error()
         
         Adjunta=self.adjunta()
         DeterminanteI=(1/self.determinante())
         Inversa=Adjunta.scalar_mul(DeterminanteI)
         return Inversa
             
-    def __str__(self: object) -> str:
+    def __str__(self: 'mathrix') -> str:
         # Calcular el ancho máximo de cada columna
         col_widths = [max(len(str(self.datos[row][col])) for row in range(self.filas)) for col in range(self.columnas)]
         
         # Formatear cada fila con elementos centrados
         mathrixSTR = '\n'.join('\t,\t'.join(f"{str(item).center(col_widths[col])}" for col, item in enumerate(fila)) for fila in self.datos)
         return f'Matriz {self.filas}x{self.columnas}:\n{mathrixSTR}'
```

### Comparing `mathrixpy-1.5/mathrixpy/cambios.py` & `mathrixpy-1.6/mathrixpy/cambios.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,18 +20,7 @@
         '''
         Aplica una función a cada elemento de la matriz
         '''
         matrix = [[func(self.datos[i][j]) for j in range(self.columnas)] for i in range(self.filas)]
         return matrizop(matrix)
 
     
-if __name__=="__main__":
-    
-    v=matrizop([[1,2], 
-                [4,5]])
-    
-    z=matrizop( [[1], 
-                 [2],
-                 [3]])
-    
-    m=matrizop.listaToMatriz([1,2,3,5,4,5],2,3)
-
```

### Comparing `mathrixpy-1.5/mathrixpy.egg-info/PKG-INFO` & `mathrixpy-1.6/mathrixpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathrixpy
-Version: 1.5
+Version: 1.6
 Summary: mathrixpy es una biblioteca de Python para realizar operaciones matriciales. Permite la creación, manipulación y operaciones aritméticas con matrices. Esta biblioteca es útil para aplicaciones matemáticas y científicas que requieren cálculos matriciales.
 Home-page: https://github.com/Ampere-G/mathrixPy
 Author: AmJoJADeOrg
 Author-email: glroberto1810@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mathrixpy-1.5/setup.py` & `mathrixpy-1.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mathrixpy",
-    version="1.5",
+    version="1.6",
     author="AmJoJADeOrg",
     license='MIT',
     author_email="glroberto1810@gmail.com",
     description="mathrixpy es una biblioteca de Python para realizar operaciones matriciales. Permite la creación, manipulación y operaciones aritméticas con matrices. Esta biblioteca es útil para aplicaciones matemáticas y científicas que requieren cálculos matriciales.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Ampere-G/mathrixPy",
```

