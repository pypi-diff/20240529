# Comparing `tmp/mathrixpy-1.1.tar.gz` & `tmp/mathrixpy-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathrixpy-1.1.tar", last modified: Wed May 29 01:36:15 2024, max compression
+gzip compressed data, was "mathrixpy-1.3.tar", last modified: Wed May 29 07:04:43 2024, max compression
```

## Comparing `mathrixpy-1.1.tar` & `mathrixpy-1.3.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 01:36:15.667399 mathrixpy-1.1/
--rw-rw-rw-   0        0        0     1087 2024-05-24 02:28:32.000000 mathrixpy-1.1/LICENSE
--rw-rw-rw-   0        0        0      467 2024-05-29 01:36:15.667399 mathrixpy-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       13 2024-05-24 02:34:08.000000 mathrixpy-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 01:36:15.650474 mathrixpy-1.1/mathrixpy/
--rw-rw-rw-   0        0        0       23 2024-05-24 04:53:32.000000 mathrixpy-1.1/mathrixpy/__init__.py
--rw-rw-rw-   0        0        0     6495 2024-05-29 01:35:57.000000 mathrixpy-1.1/mathrixpy/base.py
--rw-rw-rw-   0        0        0     5915 2024-05-29 00:32:26.000000 mathrixpy-1.1/mathrixpy/cambios.py
--rw-rw-rw-   0        0        0        0 2024-05-29 01:29:43.000000 mathrixpy-1.1/mathrixpy/pruebas.py
-drwxrwxrwx   0        0        0        0 2024-05-29 01:36:15.665009 mathrixpy-1.1/mathrixpy.egg-info/
--rw-rw-rw-   0        0        0      467 2024-05-29 01:36:15.000000 mathrixpy-1.1/mathrixpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-29 01:36:15.000000 mathrixpy-1.1/mathrixpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 01:36:15.000000 mathrixpy-1.1/mathrixpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-29 01:36:15.000000 mathrixpy-1.1/mathrixpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-29 01:36:15.670407 mathrixpy-1.1/setup.cfg
--rw-rw-rw-   0        0        0      620 2024-05-29 01:36:04.000000 mathrixpy-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 07:04:43.343283 mathrixpy-1.3/
+-rw-rw-rw-   0        0        0     1087 2024-05-24 02:28:32.000000 mathrixpy-1.3/LICENSE
+-rw-rw-rw-   0        0        0      467 2024-05-29 07:04:43.342282 mathrixpy-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2024-05-24 02:34:08.000000 mathrixpy-1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 07:04:43.318252 mathrixpy-1.3/mathrixpy/
+-rw-rw-rw-   0        0        0       23 2024-05-24 04:53:32.000000 mathrixpy-1.3/mathrixpy/__init__.py
+-rw-rw-rw-   0        0        0     6585 2024-05-29 07:03:28.000000 mathrixpy-1.3/mathrixpy/base.py
+-rw-rw-rw-   0        0        0     6446 2024-05-29 01:57:42.000000 mathrixpy-1.3/mathrixpy/cambios.py
+drwxrwxrwx   0        0        0        0 2024-05-29 07:04:43.340284 mathrixpy-1.3/mathrixpy.egg-info/
+-rw-rw-rw-   0        0        0      467 2024-05-29 07:04:43.000000 mathrixpy-1.3/mathrixpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2024-05-29 07:04:43.000000 mathrixpy-1.3/mathrixpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 07:04:43.000000 mathrixpy-1.3/mathrixpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-29 07:04:43.000000 mathrixpy-1.3/mathrixpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-29 07:04:43.345283 mathrixpy-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      620 2024-05-29 07:04:40.000000 mathrixpy-1.3/setup.py
```

### Comparing `mathrixpy-1.1/LICENSE` & `mathrixpy-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mathrixpy-1.1/mathrixpy/base.py` & `mathrixpy-1.3/mathrixpy/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,63 +5,63 @@
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
             
         return mathrix(matrix)
     
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
             
         return mathrix(matrix)
      
-    def prod(self,*args) -> object:
+    def prod(self:object,*args:object) -> object:
         '''
         Multiplica una matriz por otra u otras matrices
         '''
         original=self
         
         
         for matriz in args:
@@ -75,67 +75,56 @@
                     suma=0
                     for k in range(original.columnas):
                         suma+=original.datos[i][k] * matriz.datos[k][j]
                     resultado[i][j]=suma
             original=mathrix(resultado)
         return mathrix(resultado)
     
-    def scalar_mul(self,scalar:float) -> object:
+    def scalar_mul(self:object,scalar:float) -> object:
         '''
         Multiplica una matriz por un escalar
         '''
         
         matrix=[[0]*self.columnas for _ in range(self.filas)]
         
         for i in range(self.filas):
             for j in range(self.columnas):
                 matrix[i][j]=self.datos[i][j]*scalar
         
         return mathrix(matrix)
 
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
 
         return mathrix(matrix)
     
-    def mIdentidad(numFila:int) -> object:
-        '''
-        Crea una matriz diagonal con solo numeros 1 de dimensiones numFila x numFila
-        '''
-        M=[[0]*numFila for _ in range(numFila)]
-        
-        for i in range(numFila):
-            M[i][i]=1
-            
-        return mathrix(M)
-    
-    def potencia(self,potencia:int) ->object:
+    def potencia(self:object,potencia:int) ->object:
         '''
         Eleva una matriz cuadrada a una potencia
         '''
         
         if potencia <1:
             raise ValueError('La potencia tiene que ser mayor o igual que 1')
         original=self
@@ -165,15 +154,15 @@
             
             cofactor=(-1)**columna * self.datos[0][columna]*(mathrix(menor).determinante())
             
             det+=cofactor
             
         return det
           
-    def __str__(self) -> str:
+    def __str__(self:object) -> str:
         '''
         Regresa una representación en cadena de la matriz
         '''
         mathrixSTR= '\n'.join ( '\t'.join ( map(str,fila) ) for fila in self.datos )
         
         return f'Matriz {self.filas}x{self.columnas}:\n{mathrixSTR}'            
 
@@ -192,7 +181,18 @@
     for i in range(numFilas):
         for j in range(numColumnas):
             
             M[i][j]=datos[(numColumnas*i) + j]
     
     return mathrix(M)
 
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
+
```

### Comparing `mathrixpy-1.1/mathrixpy/cambios.py` & `mathrixpy-1.3/mathrixpy/cambios.py`

 * *Files 5% similar despite different names*

```diff
@@ -166,21 +166,34 @@
     def extractColumna(self,numColumna)->list:
         resultado=[]
         
         for i in self.datos:
             resultado.append(i[numColumna-1])
         return resultado
     
+    def apply_function(self, func) -> object:
+        '''
+        Aplica una función a cada elemento de la matriz
+        '''
+        matrix = [[func(self.datos[i][j]) for j in range(self.columnas)] for i in range(self.filas)]
+        return matrizop(matrix)
+    
+    def __str__(self) -> str:
+        '''
+        Regresa una representación en cadena de la matriz
+        '''
+        mathrixSTR= '\n'.join ( '\t'.join ( map(str,fila) ) for fila in self.datos )
+        
+        return f'Matriz {self.filas}x{self.columnas}:\n{mathrixSTR}'            
+
     
 if __name__=="__main__":
     
     v=matrizop([[1,2], 
                 [4,5]])
     
     z=matrizop( [[1], 
                  [2],
                  [3]])
     
     m=matrizop.listaToMatriz([1,2,3,5,4,5],2,3)
-    
-    
-    print(v.extractColumna(2))
+
```

### Comparing `mathrixpy-1.1/setup.py` & `mathrixpy-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mathrixpy",
-    version="1.1",
+    version="1.3",
     author="AmJoJADeOrg",
     license='MIT',
     author_email="glroberto1810@gmail.com",
     description="Operaciones con matrices",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Ampere-G/mathrixPy",
```

