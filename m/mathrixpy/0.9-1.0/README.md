# Comparing `tmp/mathrixpy-0.9.tar.gz` & `tmp/mathrixpy-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathrixpy-0.9.tar", last modified: Fri May 24 04:56:04 2024, max compression
+gzip compressed data, was "mathrixpy-1.0.tar", last modified: Wed May 29 01:31:29 2024, max compression
```

## Comparing `mathrixpy-0.9.tar` & `mathrixpy-1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 04:56:04.426684 mathrixpy-0.9/
--rw-rw-rw-   0        0        0     1087 2024-05-24 02:28:32.000000 mathrixpy-0.9/LICENSE
--rw-rw-rw-   0        0        0      467 2024-05-24 04:56:04.426684 mathrixpy-0.9/PKG-INFO
--rw-rw-rw-   0        0        0       13 2024-05-24 02:34:08.000000 mathrixpy-0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 04:56:04.410768 mathrixpy-0.9/mathrixpy/
--rw-rw-rw-   0        0        0       23 2024-05-24 04:53:32.000000 mathrixpy-0.9/mathrixpy/__init__.py
--rw-rw-rw-   0        0        0     6016 2024-05-24 04:52:42.000000 mathrixpy-0.9/mathrixpy/base.py
--rw-rw-rw-   0        0        0     5906 2024-05-23 18:35:49.000000 mathrixpy-0.9/mathrixpy/cambios.py
-drwxrwxrwx   0        0        0        0 2024-05-24 04:56:04.424696 mathrixpy-0.9/mathrixpy.egg-info/
--rw-rw-rw-   0        0        0      467 2024-05-24 04:56:04.000000 mathrixpy-0.9/mathrixpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2024-05-24 04:56:04.000000 mathrixpy-0.9/mathrixpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 04:56:04.000000 mathrixpy-0.9/mathrixpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-24 04:56:04.000000 mathrixpy-0.9/mathrixpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-24 04:56:04.428677 mathrixpy-0.9/setup.cfg
--rw-rw-rw-   0        0        0      620 2024-05-24 04:55:51.000000 mathrixpy-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 01:31:29.341092 mathrixpy-1.0/
+-rw-rw-rw-   0        0        0     1087 2024-05-24 02:28:32.000000 mathrixpy-1.0/LICENSE
+-rw-rw-rw-   0        0        0      467 2024-05-29 01:31:29.341092 mathrixpy-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2024-05-24 02:34:08.000000 mathrixpy-1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 01:31:29.316950 mathrixpy-1.0/mathrixpy/
+-rw-rw-rw-   0        0        0       23 2024-05-24 04:53:32.000000 mathrixpy-1.0/mathrixpy/__init__.py
+-rw-rw-rw-   0        0        0     6620 2024-05-29 01:28:28.000000 mathrixpy-1.0/mathrixpy/base.py
+-rw-rw-rw-   0        0        0     5915 2024-05-29 00:32:26.000000 mathrixpy-1.0/mathrixpy/cambios.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 01:29:43.000000 mathrixpy-1.0/mathrixpy/pruebas.py
+drwxrwxrwx   0        0        0        0 2024-05-29 01:31:29.339084 mathrixpy-1.0/mathrixpy.egg-info/
+-rw-rw-rw-   0        0        0      467 2024-05-29 01:31:29.000000 mathrixpy-1.0/mathrixpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-29 01:31:29.000000 mathrixpy-1.0/mathrixpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 01:31:29.000000 mathrixpy-1.0/mathrixpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-29 01:31:29.000000 mathrixpy-1.0/mathrixpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-29 01:31:29.346099 mathrixpy-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      620 2024-05-29 01:31:14.000000 mathrixpy-1.0/setup.py
```

### Comparing `mathrixpy-0.9/LICENSE` & `mathrixpy-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mathrixpy-0.9/mathrixpy/base.py` & `mathrixpy-1.0/mathrixpy/cambios.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-class mathrix:
+class matrizop:
     def __init__(self,datos:list)-> object:   #Incializa la clase
         
         '''
         Convierte una lista de lista a matriz
         '''
         
         self.datos=datos #Se ingresa una lista de listas
@@ -35,15 +35,15 @@
         
         matrix=[[0]*self.columnas for _ in range(self.filas)]
         
         for i in range((self.filas)):
             for j in range((self.columnas)):  
                 matrix[i][j]=self.datos[i][j]+other.datos[i][j]
             
-        return mathrix(matrix)
+        return matrizop(matrix)
     
     def __sub__(self,other) -> object:
         '''
         Resta de dos matrices (Tienen que tener las mismas dimensiones)
         '''
 
         if not self.dimension_igual(other):
@@ -51,15 +51,15 @@
         
         matrix=[[0]*self.columnas for _ in range(self.filas)]
         
         for i in range((self.filas)):
             for j in range((self.columnas)):  
                 matrix[i][j]=self.datos[i][j]-other.datos[i][j]
             
-        return mathrix(matrix)
+        return matrizop(matrix)
      
     def prod(self,*args) -> object:
         '''
         Multiplica una matriz por otra u otras matrices
         '''
         original=self
         
@@ -72,29 +72,29 @@
             
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
     
     def scalar_mul(self,scalar:float) -> object:
         '''
         Multiplica una matriz por un escalar
         '''
         
         matrix=[[0]*self.columnas for _ in range(self.filas)]
         
         for i in range(self.filas):
             for j in range(self.columnas):
                 matrix[i][j]=self.datos[i][j]*scalar
         
-        return mathrix(matrix)
+        return matrizop(matrix)
 
     def tr(self) -> float:
         '''
         Devulve la suma de los elementos diagonales de una matriz cuadrada
         '''
         
         if not self.filas==self.columnas:
@@ -114,26 +114,26 @@
         matrix=[[0]*self.filas for _ in range(self.columnas)]
         
         
         for i in range(self.filas):
             for j in range(self.columnas):
                 matrix[j][i]=self.datos[i][j]
 
-        return mathrix(matrix)
+        return matrizop(matrix)
     
     def mIdentidad(numFila:int) -> object:
         '''
         Crea una matriz diagonal con solo numeros 1 de dimensiones numFila x numFila
         '''
         M=[[0]*numFila for _ in range(numFila)]
         
         for i in range(numFila):
             M[i][i]=1
             
-        return mathrix(M)
+        return matrizop(M)
     
     def potencia(self,potencia:int) ->object:
         '''
         Eleva una matriz cuadrada a una potencia
         '''
         
         if potencia <1:
@@ -156,27 +156,31 @@
         M=[[0]*numColumnas for _ in range(numFilas)]
 
         for i in range(numFilas):
             for j in range(numColumnas):
                 
                 M[i][j]=datos[(numColumnas*i) + j]
         
-        return mathrix(M)
-   
-    # def determinante(self:object) -> float:
-        
-    #     resultado=0
-    #     resultado2=1
-    #     if len(self.datos)==2:
-    #         return self.datos[0][0]*self.datos[1][1]-self.datos[0][1]*self.datos[1][0]
-                   
-        
-          
-    def __str__(self) -> str:
-        '''
-        Regresa una representación en cadena de la matriz
-        '''
-        mathrixSTR= '\n'.join ( '\t'.join ( map(str,fila) ) for fila in self.datos )
-        
-        return f'Matriz {self.filas}x{self.columnas}:\n{mathrixSTR}'            
-
+        return matrizop(M)
 
+#Cambios  
+    def extractColumna(self,numColumna)->list:
+        resultado=[]
+        
+        for i in self.datos:
+            resultado.append(i[numColumna-1])
+        return resultado
+    
+    
+if __name__=="__main__":
+    
+    v=matrizop([[1,2], 
+                [4,5]])
+    
+    z=matrizop( [[1], 
+                 [2],
+                 [3]])
+    
+    m=matrizop.listaToMatriz([1,2,3,5,4,5],2,3)
+    
+    
+    print(v.extractColumna(2))
```

### Comparing `mathrixpy-0.9/mathrixpy/cambios.py` & `mathrixpy-1.0/mathrixpy/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-class matrizop:
+class mathrix:
     def __init__(self,datos:list)-> object:   #Incializa la clase
         
         '''
         Convierte una lista de lista a matriz
         '''
         
         self.datos=datos #Se ingresa una lista de listas
@@ -35,15 +35,15 @@
         
         matrix=[[0]*self.columnas for _ in range(self.filas)]
         
         for i in range((self.filas)):
             for j in range((self.columnas)):  
                 matrix[i][j]=self.datos[i][j]+other.datos[i][j]
             
-        return matrizop(matrix)
+        return mathrix(matrix)
     
     def __sub__(self,other) -> object:
         '''
         Resta de dos matrices (Tienen que tener las mismas dimensiones)
         '''
 
         if not self.dimension_igual(other):
@@ -51,15 +51,15 @@
         
         matrix=[[0]*self.columnas for _ in range(self.filas)]
         
         for i in range((self.filas)):
             for j in range((self.columnas)):  
                 matrix[i][j]=self.datos[i][j]-other.datos[i][j]
             
-        return matrizop(matrix)
+        return mathrix(matrix)
      
     def prod(self,*args) -> object:
         '''
         Multiplica una matriz por otra u otras matrices
         '''
         original=self
         
@@ -72,29 +72,29 @@
             
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
     
     def scalar_mul(self,scalar:float) -> object:
         '''
         Multiplica una matriz por un escalar
         '''
         
         matrix=[[0]*self.columnas for _ in range(self.filas)]
         
         for i in range(self.filas):
             for j in range(self.columnas):
                 matrix[i][j]=self.datos[i][j]*scalar
         
-        return matrizop(matrix)
+        return mathrix(matrix)
 
     def tr(self) -> float:
         '''
         Devulve la suma de los elementos diagonales de una matriz cuadrada
         '''
         
         if not self.filas==self.columnas:
@@ -114,72 +114,92 @@
         matrix=[[0]*self.filas for _ in range(self.columnas)]
         
         
         for i in range(self.filas):
             for j in range(self.columnas):
                 matrix[j][i]=self.datos[i][j]
 
-        return matrizop(matrix)
+        return mathrix(matrix)
     
     def mIdentidad(numFila:int) -> object:
         '''
         Crea una matriz diagonal con solo numeros 1 de dimensiones numFila x numFila
         '''
         M=[[0]*numFila for _ in range(numFila)]
         
         for i in range(numFila):
             M[i][i]=1
             
-        return matrizop(M)
+        return mathrix(M)
     
     def potencia(self,potencia:int) ->object:
         '''
         Eleva una matriz cuadrada a una potencia
         '''
         
         if potencia <1:
             raise ValueError('La potencia tiene que ser mayor o igual que 1')
         original=self
         
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
-    def extractColumna(self,numColumna)->list:
-        resultado=[]
+        det=0 
         
-        for i in self.datos:
-            resultado.append(i[numColumna-1])
-        return resultado
-    
-    
-if __name__=="__main__":
-    
-    v=matrizop([[1,2], 
-                [4,5]])
+        for columna in range(self.columnas):
+            menor = [fila[:columna] + fila[columna+1:] for fila in self.datos[1:]]
+            
+            cofactor=(-1)**columna * self.datos[0][columna]*(mathrix(menor).determinante())
+            
+            det+=cofactor
+            
+        return det
+          
+    def __str__(self) -> str:
+        '''
+        Regresa una representación en cadena de la matriz
+        '''
+        mathrixSTR= '\n'.join ( '\t'.join ( map(str,fila) ) for fila in self.datos )
+        
+        return f'Matriz {self.filas}x{self.columnas}:\n{mathrixSTR}'            
+
+
+def listaToMatriz(datos:list,numFilas:int,numColumnas:int)-> object:
+    '''
+    Genera una matriz de dimensiones deseadas a partir de una lista de números
+    '''
     
-    z=matrizop( [[1], 
-                 [2],
-                 [3]])
+    if numFilas*numColumnas!=len(datos):
+        raise ValueError('Verificar dimensiones')
     
-    m=matrizop.listaToMatriz([1,2,3,5,4,5],2,3)
     
+    M=[[0]*numColumnas for _ in range(numFilas)]
+
+    for i in range(numFilas):
+        for j in range(numColumnas):
+            
+            M[i][j]=datos[(numColumnas*i) + j]
     
-    print(v.extractColumna(2))
+    return mathrix(M)
+
+matriz = mathrix([
+    [2, -3, 7,3],
+    [2, 0, -1,4],
+    [1, 4, 5,6],
+    [1, 6, 0,6]])
+
+print(matriz.determinante())
```

### Comparing `mathrixpy-0.9/setup.py` & `mathrixpy-1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mathrixpy",
-    version="0.9",
+    version="1.0",
     author="AmJoJADeOrg",
     license='MIT',
     author_email="glroberto1810@gmail.com",
     description="Operaciones con matrices",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Ampere-G/mathrixPy",
```

