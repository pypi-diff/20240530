# Comparing `tmp/mathrixpy-1.3.tar.gz` & `tmp/mathrixpy-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathrixpy-1.3.tar", last modified: Wed May 29 07:04:43 2024, max compression
+gzip compressed data, was "mathrixpy-1.4.tar", last modified: Thu May 30 15:15:29 2024, max compression
```

## Comparing `mathrixpy-1.3.tar` & `mathrixpy-1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 07:04:43.343283 mathrixpy-1.3/
--rw-rw-rw-   0        0        0     1087 2024-05-24 02:28:32.000000 mathrixpy-1.3/LICENSE
--rw-rw-rw-   0        0        0      467 2024-05-29 07:04:43.342282 mathrixpy-1.3/PKG-INFO
--rw-rw-rw-   0        0        0       13 2024-05-24 02:34:08.000000 mathrixpy-1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 07:04:43.318252 mathrixpy-1.3/mathrixpy/
--rw-rw-rw-   0        0        0       23 2024-05-24 04:53:32.000000 mathrixpy-1.3/mathrixpy/__init__.py
--rw-rw-rw-   0        0        0     6585 2024-05-29 07:03:28.000000 mathrixpy-1.3/mathrixpy/base.py
--rw-rw-rw-   0        0        0     6446 2024-05-29 01:57:42.000000 mathrixpy-1.3/mathrixpy/cambios.py
-drwxrwxrwx   0        0        0        0 2024-05-29 07:04:43.340284 mathrixpy-1.3/mathrixpy.egg-info/
--rw-rw-rw-   0        0        0      467 2024-05-29 07:04:43.000000 mathrixpy-1.3/mathrixpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2024-05-29 07:04:43.000000 mathrixpy-1.3/mathrixpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 07:04:43.000000 mathrixpy-1.3/mathrixpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-29 07:04:43.000000 mathrixpy-1.3/mathrixpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-29 07:04:43.345283 mathrixpy-1.3/setup.cfg
--rw-rw-rw-   0        0        0      620 2024-05-29 07:04:40.000000 mathrixpy-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 15:15:29.765677 mathrixpy-1.4/
+-rw-rw-rw-   0        0        0     1087 2024-05-24 02:28:32.000000 mathrixpy-1.4/LICENSE
+-rw-rw-rw-   0        0        0     5899 2024-05-30 15:15:29.765677 mathrixpy-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5136 2024-05-30 15:12:38.000000 mathrixpy-1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 15:15:29.743871 mathrixpy-1.4/mathrixpy/
+-rw-rw-rw-   0        0        0       23 2024-05-24 04:53:32.000000 mathrixpy-1.4/mathrixpy/__init__.py
+-rw-rw-rw-   0        0        0     8614 2024-05-30 15:14:34.000000 mathrixpy-1.4/mathrixpy/base.py
+-rw-rw-rw-   0        0        0     6446 2024-05-29 01:57:42.000000 mathrixpy-1.4/mathrixpy/cambios.py
+drwxrwxrwx   0        0        0        0 2024-05-30 15:15:29.763660 mathrixpy-1.4/mathrixpy.egg-info/
+-rw-rw-rw-   0        0        0     5899 2024-05-30 15:15:29.000000 mathrixpy-1.4/mathrixpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2024-05-30 15:15:29.000000 mathrixpy-1.4/mathrixpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 15:15:29.000000 mathrixpy-1.4/mathrixpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-30 15:15:29.000000 mathrixpy-1.4/mathrixpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-30 15:15:29.767665 mathrixpy-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      857 2024-05-30 15:13:34.000000 mathrixpy-1.4/setup.py
```

### Comparing `mathrixpy-1.3/LICENSE` & `mathrixpy-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mathrixpy-1.3/mathrixpy/base.py` & `mathrixpy-1.4/mathrixpy/cambios.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-class mathrix:
+class matrizop:
     def __init__(self,datos:list)-> object:   #Incializa la clase
         
         '''
         Convierte una lista de lista a matriz
         '''
         
         self.datos=datos #Se ingresa una lista de listas
         self.filas=len(datos) #El número de elementos de las lista de datos es igual a el numero de filas
         self.columnas=len(datos[0]) #El número de elementos de cada fila es igual al número de columnas
     
-        if not self.__verificar_matriz(): 
+        if not self.verificar_matriz(): 
             raise ValueError("Todas las filas deben tener la misma longitud")
         
-    def __verificar_matriz(self:object) -> bool:
+    def verificar_matriz(self) -> bool:
         '''
         Comprueba que la longitud de todas las filas sea la misma
         '''
         return all(len(fila)==self.columnas for fila in self.datos)
         
-    def __dimension_igual(self,other) -> bool:
+    def dimension_igual(self,other) -> bool:
         '''
         Verifica si dos matrices tienen la misma dimensión
         '''
         
         return self.filas==other.filas and self.columnas==other.columnas
     
-    def __add__(self:object,other:object) -> object:
+    def __add__(self,other) -> object:
         '''
         Suma dos matrices (Tienen que tener las mismas dimensiones)
         '''
         
-        if not self.__dimension_igual(other):
+        if not self.dimension_igual(other):
             raise ValueError('Las matrices tienen que tener las mismas dimensiones')
         
         matrix=[[0]*self.columnas for _ in range(self.filas)]
         
         for i in range((self.filas)):
             for j in range((self.columnas)):  
                 matrix[i][j]=self.datos[i][j]+other.datos[i][j]
             
-        return mathrix(matrix)
+        return matrizop(matrix)
     
-    def __sub__(self:object,other:object) -> object:
+    def __sub__(self,other) -> object:
         '''
         Resta de dos matrices (Tienen que tener las mismas dimensiones)
         '''
 
-        if not self.__dimension_igual(other):
+        if not self.dimension_igual(other):
             raise ValueError('Las matrices tienen que tener las mismas dimensiones')
         
         matrix=[[0]*self.columnas for _ in range(self.filas)]
         
         for i in range((self.filas)):
             for j in range((self.columnas)):  
                 matrix[i][j]=self.datos[i][j]-other.datos[i][j]
             
-        return mathrix(matrix)
+        return matrizop(matrix)
      
-    def prod(self:object,*args:object) -> object:
+    def prod(self,*args) -> object:
         '''
         Multiplica una matriz por otra u otras matrices
         '''
         original=self
         
         
         for matriz in args:
@@ -72,127 +72,128 @@
             
             for i in range(original.filas):
                 for j in range(matriz.columnas):
                     suma=0
                     for k in range(original.columnas):
                         suma+=original.datos[i][k] * matriz.datos[k][j]
                     resultado[i][j]=suma
-            original=mathrix(resultado)
-        return mathrix(resultado)
+            original=matrizop(resultado)
+        return matrizop(resultado)
     
-    def scalar_mul(self:object,scalar:float) -> object:
+    def scalar_mul(self,scalar:float) -> object:
         '''
         Multiplica una matriz por un escalar
         '''
         
         matrix=[[0]*self.columnas for _ in range(self.filas)]
         
         for i in range(self.filas):
             for j in range(self.columnas):
                 matrix[i][j]=self.datos[i][j]*scalar
         
-        return mathrix(matrix)
+        return matrizop(matrix)
 
-    def tr(self:object) -> float:
+    def tr(self) -> float:
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
+    def transpuesta(self) -> object:
         '''
         Devuelve una matriz con los indices alrrevez
         '''
         matrix=[[0]*self.filas for _ in range(self.columnas)]
         
         
         for i in range(self.filas):
             for j in range(self.columnas):
                 matrix[j][i]=self.datos[i][j]
 
-        return mathrix(matrix)
+        return matrizop(matrix)
     
-    def potencia(self:object,potencia:int) ->object:
+    def mIdentidad(numFila:int) -> object:
+        '''
+        Crea una matriz diagonal con solo numeros 1 de dimensiones numFila x numFila
+        '''
+        M=[[0]*numFila for _ in range(numFila)]
+        
+        for i in range(numFila):
+            M[i][i]=1
+            
+        return matrizop(M)
+    
+    def potencia(self,potencia:int) ->object:
         '''
         Eleva una matriz cuadrada a una potencia
         '''
         
         if potencia <1:
             raise ValueError('La potencia tiene que ser mayor o igual que 1')
         original=self
         
         for _ in range(1,potencia):
             original=original.prod(self)
         return(original)
 
-    def determinante(self:object) -> float:
+    def listaToMatriz(datos:list,numFilas:int,numColumnas:int)-> object:
         '''
-        Calcula la determinante de una matriz - Tiene que ser cuadrada
+        Genera una matriz de dimensiones deseadas a partir de una lista de números
         '''
         
-        if self.filas!=self.columnas:
-            raise ValueError('La matriz tiene que ser cuadrada')
+        if numFilas*numColumnas!=len(datos):
+            raise ValueError('Verificar dimensiones')
         
-        if self.filas==1:
-            return self.datos[0][0]
         
-        if self.filas==2:
-            return self.datos[0][0]*self.datos[1][1]-self.datos[0][1]*self.datos[1][0]
+        M=[[0]*numColumnas for _ in range(numFilas)]
+
+        for i in range(numFilas):
+            for j in range(numColumnas):
+                
+                M[i][j]=datos[(numColumnas*i) + j]
         
-        det=0 
+        return matrizop(M)
+
+#Cambios  
+    def extractColumna(self,numColumna)->list:
+        resultado=[]
         
-        for columna in range(self.columnas):
-            menor = [fila[:columna] + fila[columna+1:] for fila in self.datos[1:]]
-            
-            cofactor=(-1)**columna * self.datos[0][columna]*(mathrix(menor).determinante())
-            
-            det+=cofactor
-            
-        return det
-          
-    def __str__(self:object) -> str:
+        for i in self.datos:
+            resultado.append(i[numColumna-1])
+        return resultado
+    
+    def apply_function(self, func) -> object:
+        '''
+        Aplica una función a cada elemento de la matriz
+        '''
+        matrix = [[func(self.datos[i][j]) for j in range(self.columnas)] for i in range(self.filas)]
+        return matrizop(matrix)
+    
+    def __str__(self) -> str:
         '''
         Regresa una representación en cadena de la matriz
         '''
         mathrixSTR= '\n'.join ( '\t'.join ( map(str,fila) ) for fila in self.datos )
         
         return f'Matriz {self.filas}x{self.columnas}:\n{mathrixSTR}'            
 
-
-def listaToMatriz(datos:list,numFilas:int,numColumnas:int)-> object:
-    '''
-    Genera una matriz de dimensiones deseadas a partir de una lista de números
-    '''
     
-    if numFilas*numColumnas!=len(datos):
-        raise ValueError('Verificar dimensiones')
+if __name__=="__main__":
     
+    v=matrizop([[1,2], 
+                [4,5]])
     
-    M=[[0]*numColumnas for _ in range(numFilas)]
-
-    for i in range(numFilas):
-        for j in range(numColumnas):
-            
-            M[i][j]=datos[(numColumnas*i) + j]
-    
-    return mathrix(M)
-
-def mIdentidad(numFila:int) -> object:
-        '''
-        Crea una matriz diagonal con solo numeros 1 de dimensiones numFila x numFila
-        '''
-        M=[[0]*numFila for _ in range(numFila)]
-        
-        for i in range(numFila):
-            M[i][i]=1
-            
-        return mathrix(M)
+    z=matrizop( [[1], 
+                 [2],
+                 [3]])
     
+    m=matrizop.listaToMatriz([1,2,3,5,4,5],2,3)
+
```

### Comparing `mathrixpy-1.3/mathrixpy/cambios.py` & `mathrixpy-1.4/mathrixpy/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,79 @@
-class matrizop:
+class mathrix:
     def __init__(self,datos:list)-> object:   #Incializa la clase
         
         '''
         Convierte una lista de lista a matriz
         '''
         
         self.datos=datos #Se ingresa una lista de listas
         self.filas=len(datos) #El número de elementos de las lista de datos es igual a el numero de filas
         self.columnas=len(datos[0]) #El número de elementos de cada fila es igual al número de columnas
     
-        if not self.verificar_matriz(): 
+        if not self.__verificar_matriz(): 
             raise ValueError("Todas las filas deben tener la misma longitud")
         
-    def verificar_matriz(self) -> bool:
+    def __verificar_matriz(self:object) -> bool:
         '''
         Comprueba que la longitud de todas las filas sea la misma
         '''
         return all(len(fila)==self.columnas for fila in self.datos)
         
-    def dimension_igual(self,other) -> bool:
+    def __dimension_igual(self,other) -> bool:
         '''
         Verifica si dos matrices tienen la misma dimensión
         '''
         
         return self.filas==other.filas and self.columnas==other.columnas
     
-    def __add__(self,other) -> object:
+    def __matriz_cuadrada_error(self:object) -> bool:
+        if self.filas!=self.columnas:
+            raise ValueError('La matriz no es cuadrada')
+        
+        return True
+    
+    def get_Datos(self:object) -> list:
+        '''
+        Regresa los datos pertenecientes a la matriz en forma de lista
+        '''
+        return self.datos
+        
+    def __add__(self:object,other:object) -> object:
         '''
         Suma dos matrices (Tienen que tener las mismas dimensiones)
         '''
         
-        if not self.dimension_igual(other):
+        if not self.__dimension_igual(other):
             raise ValueError('Las matrices tienen que tener las mismas dimensiones')
         
         matrix=[[0]*self.columnas for _ in range(self.filas)]
         
         for i in range((self.filas)):
             for j in range((self.columnas)):  
                 matrix[i][j]=self.datos[i][j]+other.datos[i][j]
             
-        return matrizop(matrix)
+        return mathrix(matrix)
     
-    def __sub__(self,other) -> object:
+    def __sub__(self:object,other:object) -> object:
         '''
         Resta de dos matrices (Tienen que tener las mismas dimensiones)
         '''
 
-        if not self.dimension_igual(other):
+        if not self.__dimension_igual(other):
             raise ValueError('Las matrices tienen que tener las mismas dimensiones')
         
         matrix=[[0]*self.columnas for _ in range(self.filas)]
         
         for i in range((self.filas)):
             for j in range((self.columnas)):  
                 matrix[i][j]=self.datos[i][j]-other.datos[i][j]
             
-        return matrizop(matrix)
+        return mathrix(matrix)
      
-    def prod(self,*args) -> object:
+    def prod(self:object,*args:object) -> object:
         '''
         Multiplica una matriz por otra u otras matrices
         '''
         original=self
         
         
         for matriz in args:
@@ -72,128 +84,169 @@
             
             for i in range(original.filas):
                 for j in range(matriz.columnas):
                     suma=0
                     for k in range(original.columnas):
                         suma+=original.datos[i][k] * matriz.datos[k][j]
                     resultado[i][j]=suma
-            original=matrizop(resultado)
-        return matrizop(resultado)
+            original=mathrix(resultado)
+        return mathrix(resultado)
     
-    def scalar_mul(self,scalar:float) -> object:
+    def scalar_mul(self:object,scalar:float) -> object:
         '''
         Multiplica una matriz por un escalar
         '''
         
         matrix=[[0]*self.columnas for _ in range(self.filas)]
         
         for i in range(self.filas):
             for j in range(self.columnas):
                 matrix[i][j]=self.datos[i][j]*scalar
         
-        return matrizop(matrix)
+        return mathrix(matrix)
 
-    def tr(self) -> float:
+    def tr(self:object) -> float:
         '''
         Devulve la suma de los elementos diagonales de una matriz cuadrada
         '''
         
         if not self.filas==self.columnas:
             raise ValueError('La matriz tiene que ser cuadrada')
         
         traza=0
         
         for i in range(self.filas):
                 traza+=self.datos[i][i]
                 
         return traza
         
-    def transpuesta(self) -> object:
+    def transpuesta(self:object) -> object:
         '''
         Devuelve una matriz con los indices alrrevez
         '''
         matrix=[[0]*self.filas for _ in range(self.columnas)]
         
         
         for i in range(self.filas):
             for j in range(self.columnas):
                 matrix[j][i]=self.datos[i][j]
 
-        return matrizop(matrix)
+        return mathrix(matrix)
     
-    def mIdentidad(numFila:int) -> object:
+    def potencia(self:object,potencia:int) ->object:
         '''
-        Crea una matriz diagonal con solo numeros 1 de dimensiones numFila x numFila
+        Eleva una matriz cuadrada a una potencia entera
         '''
-        M=[[0]*numFila for _ in range(numFila)]
+        self.__matriz_cuadrada_error()
         
-        for i in range(numFila):
-            M[i][i]=1
-            
-        return matrizop(M)
-    
-    def potencia(self,potencia:int) ->object:
-        '''
-        Eleva una matriz cuadrada a una potencia
-        '''
-        
-        if potencia <1:
-            raise ValueError('La potencia tiene que ser mayor o igual que 1')
+        if potencia <-1:
+            raise ValueError('La potencia tiene que ser mayor o igual que -1')
         original=self
         
+        if potencia==0:
+            return mIdentidad(self.filas)
+        
+        if potencia==-1:
+            return self.inversa()
         for _ in range(1,potencia):
             original=original.prod(self)
         return(original)
 
-    def listaToMatriz(datos:list,numFilas:int,numColumnas:int)-> object:
+    def determinante(self:object) -> float:
         '''
-        Genera una matriz de dimensiones deseadas a partir de una lista de números
+        Calcula la determinante de una matriz - Tiene que ser cuadrada
         '''
         
-        if numFilas*numColumnas!=len(datos):
-            raise ValueError('Verificar dimensiones')
+        if self.filas!=self.columnas:
+            raise ValueError('La matriz tiene que ser cuadrada')
         
+        if self.filas==1:
+            return self.datos[0][0]
         
-        M=[[0]*numColumnas for _ in range(numFilas)]
-
-        for i in range(numFilas):
-            for j in range(numColumnas):
-                
-                M[i][j]=datos[(numColumnas*i) + j]
+        if self.filas==2:
+            return self.datos[0][0]*self.datos[1][1]-self.datos[0][1]*self.datos[1][0]
         
-        return matrizop(M)
-
-#Cambios  
-    def extractColumna(self,numColumna)->list:
-        resultado=[]
+        det=0 
         
-        for i in self.datos:
-            resultado.append(i[numColumna-1])
-        return resultado
+        for columna in range(self.columnas):
+            menor = [fila[:columna] + fila[columna+1:] for fila in self.datos[1:]]
+            
+            cofactor=(-1)**columna * self.datos[0][columna]*(mathrix(menor).determinante())
+            
+            det+=cofactor
+            
+        return det
     
-    def apply_function(self, func) -> object:
+    def submatriz(self:object, fila:int, columna:int) -> object:
         '''
-        Aplica una función a cada elemento de la matriz
+        Devuelve una submatriz excluyendo la fila y columna especificada
         '''
-        matrix = [[func(self.datos[i][j]) for j in range(self.columnas)] for i in range(self.filas)]
-        return matrizop(matrix)
-    
-    def __str__(self) -> str:
+        submat = [row[:columna] + row[columna + 1:] for row in (self.datos[:fila] + self.datos[fila + 1:])]
+        return mathrix(submat)
+        
+    def cofactor(self:object, fila:int, columna:int) ->float :
+        '''
+        Calcula el cofactor de un elemento en la fila y columna especificada
+        '''
+        submat = self.submatriz(fila, columna)
+        return ((-1) ** (fila + columna)) * submat.determinante()
+
+    def adjunta(self:object) ->object:
+        '''
+        Devuelve la matriz adjunta de una matriz
+        '''
+        self.__matriz_cuadrada_error()
+        
+        Matrizp = [[self.cofactor(i, j) for j in range(self.columnas)] for i in range(self.filas)]
+        Adj = mathrix(Matrizp).transpuesta()
+        return Adj
+
+    def inversa(self:object) -> object:
+        
         '''
-        Regresa una representación en cadena de la matriz
+        Regrea la inversa de cualquier matriz cuadrada
         '''
-        mathrixSTR= '\n'.join ( '\t'.join ( map(str,fila) ) for fila in self.datos )
+        self.__matriz_cuadrada_error()
         
-        return f'Matriz {self.filas}x{self.columnas}:\n{mathrixSTR}'            
+        Adjunta=self.adjunta()
+        DeterminanteI=(1/self.determinante())
+        Inversa=Adjunta.scalar_mul(DeterminanteI)
+        return Inversa
+            
+    def __str__(self: object) -> str:
+        # Calcular el ancho máximo de cada columna
+        col_widths = [max(len(str(self.datos[row][col])) for row in range(self.filas)) for col in range(self.columnas)]
+        
+        # Formatear cada fila con elementos centrados
+        mathrixSTR = '\n'.join('\t,\t'.join(f"{str(item).center(col_widths[col])}" for col, item in enumerate(fila)) for fila in self.datos)
+        return f'Matriz {self.filas}x{self.columnas}:\n{mathrixSTR}'         
+
 
+def listaToMatriz(datos:list,numFilas:int,numColumnas:int)-> object:
+    '''
+    Genera una matriz de dimensiones deseadas a partir de una lista de números
+    '''
     
-if __name__=="__main__":
+    if numFilas*numColumnas!=len(datos):
+        raise ValueError('Verificar dimensiones')
     
-    v=matrizop([[1,2], 
-                [4,5]])
     
-    z=matrizop( [[1], 
-                 [2],
-                 [3]])
+    M=[[0]*numColumnas for _ in range(numFilas)]
+
+    for i in range(numFilas):
+        for j in range(numColumnas):
+            
+            M[i][j]=datos[(numColumnas*i) + j]
     
-    m=matrizop.listaToMatriz([1,2,3,5,4,5],2,3)
+    return mathrix(M)
+
+def mIdentidad(numFila:int) -> object:
+        '''
+        Crea una matriz diagonal con solo numeros 1 de dimensiones numFila x numFila
+        '''
+        M=[[0]*numFila for _ in range(numFila)]
+        
+        for i in range(numFila):
+            M[i][i]=1
+            
+        return mathrix(M)
```

### Comparing `mathrixpy-1.3/setup.py` & `mathrixpy-1.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mathrixpy",
-    version="1.3",
+    version="1.4",
     author="AmJoJADeOrg",
     license='MIT',
     author_email="glroberto1810@gmail.com",
-    description="Operaciones con matrices",
+    description="mathrixpy es una biblioteca de Python para realizar operaciones matriciales. Permite la creación, manipulación y operaciones aritméticas con matrices. Esta biblioteca es útil para aplicaciones matemáticas y científicas que requieren cálculos matriciales.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Ampere-G/mathrixPy",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

