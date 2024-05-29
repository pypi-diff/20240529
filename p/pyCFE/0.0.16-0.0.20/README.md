# Comparing `tmp/pyCFE-0.0.16.tar.gz` & `tmp/pyCFE-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyCFE-0.0.16.tar", last modified: Sun Dec 31 01:24:22 2023, max compression
+gzip compressed data, was "pyCFE-0.0.20.tar", last modified: Wed May 29 15:45:21 2024, max compression
```

## Comparing `pyCFE-0.0.16.tar` & `pyCFE-0.0.20.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-12-31 01:24:22.888450 pyCFE-0.0.16/
--rw-rw-r--   0 alex      (1000) alex      (1000)    35124 2023-08-04 00:43:36.000000 pyCFE-0.0.16/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)     1053 2023-12-31 01:24:22.884448 pyCFE-0.0.16/PKG-INFO
--rwxrwxr-x   0 alex      (1000) alex      (1000)      380 2023-08-10 21:06:42.000000 pyCFE-0.0.16/README.rst
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-12-31 01:24:22.880446 pyCFE-0.0.16/pyCFE.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1053 2023-12-31 01:24:22.000000 pyCFE-0.0.16/pyCFE.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      549 2023-12-31 01:24:22.000000 pyCFE-0.0.16/pyCFE.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-12-31 01:24:22.000000 pyCFE-0.0.16/pyCFE.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       43 2023-12-31 01:24:22.000000 pyCFE-0.0.16/pyCFE.egg-info/entry_points.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       27 2023-12-31 01:24:22.000000 pyCFE-0.0.16/pyCFE.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        6 2023-12-31 01:24:22.000000 pyCFE-0.0.16/pyCFE.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-12-31 01:24:22.888450 pyCFE-0.0.16/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1443 2023-12-31 01:22:29.000000 pyCFE-0.0.16/setup.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-12-31 01:24:22.880446 pyCFE-0.0.16/src/
--rw-rw-r--   0 alex      (1000) alex      (1000)       47 2023-08-04 00:43:36.000000 pyCFE-0.0.16/src/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-12-31 01:24:22.880446 pyCFE-0.0.16/src/biller/
--rw-rw-r--   0 alex      (1000) alex      (1000)       54 2023-08-04 00:43:36.000000 pyCFE-0.0.16/src/biller/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6699 2023-12-31 01:22:29.000000 pyCFE-0.0.16/src/biller/biller.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3019 2023-12-31 01:22:29.000000 pyCFE-0.0.16/src/biller/cliente.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-12-31 01:24:22.884448 pyCFE-0.0.16/src/common/
--rw-rw-r--   0 alex      (1000) alex      (1000)       49 2023-08-04 00:43:36.000000 pyCFE-0.0.16/src/common/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7786 2023-12-31 01:22:29.000000 pyCFE-0.0.16/src/common/documento.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1802 2023-08-10 21:06:42.000000 pyCFE-0.0.16/src/common/empresa.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      714 2023-08-10 21:06:42.000000 pyCFE-0.0.16/src/common/servidor.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-12-31 01:24:22.884448 pyCFE-0.0.16/src/efactura/
--rw-rw-r--   0 alex      (1000) alex      (1000)       73 2023-08-04 00:43:36.000000 pyCFE-0.0.16/src/efactura/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5198 2023-08-04 00:43:36.000000 pyCFE-0.0.16/src/efactura/cliente.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    16229 2023-08-04 00:43:36.000000 pyCFE-0.0.16/src/efactura/efactura.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-12-31 01:24:22.884448 pyCFE-0.0.16/src/facturaexpress/
--rw-rw-r--   0 alex      (1000) alex      (1000)       70 2023-08-10 21:06:42.000000 pyCFE-0.0.16/src/facturaexpress/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5330 2023-08-10 21:06:42.000000 pyCFE-0.0.16/src/facturaexpress/cliente.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6153 2023-08-10 21:06:42.000000 pyCFE-0.0.16/src/facturaexpress/facturaexpress.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-29 15:45:21.494817 pyCFE-0.0.20/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    35124 2023-08-04 00:43:36.000000 pyCFE-0.0.20/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1053 2024-05-29 15:45:21.494817 pyCFE-0.0.20/PKG-INFO
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      380 2023-08-10 21:06:42.000000 pyCFE-0.0.20/README.rst
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-29 15:45:21.490817 pyCFE-0.0.20/pyCFE.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1053 2024-05-29 15:45:21.000000 pyCFE-0.0.20/pyCFE.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      549 2024-05-29 15:45:21.000000 pyCFE-0.0.20/pyCFE.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2024-05-29 15:45:21.000000 pyCFE-0.0.20/pyCFE.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       43 2024-05-29 15:45:21.000000 pyCFE-0.0.20/pyCFE.egg-info/entry_points.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       27 2024-05-29 15:45:21.000000 pyCFE-0.0.20/pyCFE.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        6 2024-05-29 15:45:21.000000 pyCFE-0.0.20/pyCFE.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2024-05-29 15:45:21.494817 pyCFE-0.0.20/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1443 2024-05-29 15:41:25.000000 pyCFE-0.0.20/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-29 15:45:21.490817 pyCFE-0.0.20/src/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       47 2023-08-04 00:43:36.000000 pyCFE-0.0.20/src/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-29 15:45:21.490817 pyCFE-0.0.20/src/biller/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       54 2023-08-04 00:43:36.000000 pyCFE-0.0.20/src/biller/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7658 2024-03-20 15:48:02.000000 pyCFE-0.0.20/src/biller/biller.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3019 2023-12-31 01:22:29.000000 pyCFE-0.0.20/src/biller/cliente.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-29 15:45:21.490817 pyCFE-0.0.20/src/common/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       49 2023-08-04 00:43:36.000000 pyCFE-0.0.20/src/common/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8345 2024-03-19 17:32:15.000000 pyCFE-0.0.20/src/common/documento.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1802 2023-08-10 21:06:42.000000 pyCFE-0.0.20/src/common/empresa.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      714 2023-08-10 21:06:42.000000 pyCFE-0.0.20/src/common/servidor.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-29 15:45:21.490817 pyCFE-0.0.20/src/efactura/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       73 2023-08-04 00:43:36.000000 pyCFE-0.0.20/src/efactura/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5198 2023-08-04 00:43:36.000000 pyCFE-0.0.20/src/efactura/cliente.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    16231 2024-05-29 15:41:08.000000 pyCFE-0.0.20/src/efactura/efactura.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-29 15:45:21.490817 pyCFE-0.0.20/src/facturaexpress/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       70 2023-08-10 21:06:42.000000 pyCFE-0.0.20/src/facturaexpress/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5330 2023-08-10 21:06:42.000000 pyCFE-0.0.20/src/facturaexpress/cliente.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6153 2023-08-10 21:06:42.000000 pyCFE-0.0.20/src/facturaexpress/facturaexpress.py
```

### Comparing `pyCFE-0.0.16/LICENSE` & `pyCFE-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `pyCFE-0.0.16/PKG-INFO` & `pyCFE-0.0.20/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCFE
-Version: 0.0.16
+Version: 0.0.20
 Summary: Facturacion Electronica Uruguaya
 Home-page: 
 Author: Alex Cuellar
 Author-email: acuellar@grupoyacck.com
 Maintainer: Alex Cuellar
 Maintainer-email: acuellar@grupoyacck.com
 License: GPLv3
```

### Comparing `pyCFE-0.0.16/pyCFE.egg-info/PKG-INFO` & `pyCFE-0.0.20/pyCFE.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCFE
-Version: 0.0.16
+Version: 0.0.20
 Summary: Facturacion Electronica Uruguaya
 Home-page: 
 Author: Alex Cuellar
 Author-email: acuellar@grupoyacck.com
 Maintainer: Alex Cuellar
 Maintainer-email: acuellar@grupoyacck.com
 License: GPLv3
```

### Comparing `pyCFE-0.0.16/pyCFE.egg-info/SOURCES.txt` & `pyCFE-0.0.20/pyCFE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyCFE-0.0.16/setup.py` & `pyCFE-0.0.20/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 INSTALL_REQUIRES = ['lxml','pysimplesoap','requests']
 PACKAGE_NAME = 'pyCFE'
 PACKAGE_DIR = 'src'
 
 setup(
     name=PACKAGE_NAME,
-    version='0.0.16',
+    version='0.0.20',
     author='Alex Cuellar',
     author_email='acuellar@grupoyacck.com',
     maintainer='Alex Cuellar',
     maintainer_email='acuellar@grupoyacck.com',
     description=(
         "Facturacion Electronica Uruguaya"
     ),
```

### Comparing `pyCFE-0.0.16/src/biller/biller.py` & `pyCFE-0.0.20/src/biller/biller.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,27 +5,34 @@
 
     def __init__(self, documento=None):
         self.documento = documento
 
     def _get_voucher(self):
         vals = {}
         vals['tipo_comprobante'] = int(self.documento.tipoCFE)
-        if self.documento.fecVencimiento:
-            vals['fecha_vencimiento'] = self.documento.fecVencimiento
-        vals['forma_pago'] = self.documento.formaPago
-        vals['fecha_emision'] = self.documento.fecEmision
+        if self.documento.tipoCFE not in ['182']:
+            if self.documento.fecVencimiento:
+                vals['fecha_vencimiento'] = self.documento.fecVencimiento
+            vals['forma_pago'] = self.documento.formaPago
+            vals['fecha_emision'] = self.documento.fecEmision
 
         vals['moneda'] = self.documento.moneda
         if self.documento.moneda != "UYU":
             vals['tasa_cambio'] = self.documento.tasaCambio
-        vals['montos_brutos'] = self.documento.montosBrutos == '1' and True or False
+        if self.documento.tipoCFE not in ['182']:
+            if self.documento.tipoCFE not in ['151']:
+                vals['montos_brutos'] = self.documento.montosBrutos == '1' and True or False
+            else:
+                vals['montos_brutos'] = self.documento.montosBrutos
         for sucursal in self.documento.emisor.sucursal:
             vals['sucursal'] = sucursal.codigo or "1"
             break
         vals['numero_interno'] = self.documento.numero_interno
+        if self.documento.numero_orden:
+            vals['numero_orden'] = self.documento.numero_orden
         return vals
 
     def _get_ref(self):
         vals = {}
         #vals['referencia_global'] = (self.documento.referencias and self.documento.referencias[0].serie) and 0 or 1
         #vals['razon_referencia'] = self.documento.referencias and self.documento.referencias[0].descripcion or ""
         ref_vals = []
@@ -91,19 +98,32 @@
             if line.descuentoMonto > 0.0:
                 vals['descuento_cantidad'] = round(line.descuentoMonto, 2)
             vals['recargo_tipo'] = '$'
             vals['recargo_cantidad'] = 0
             lines.append(vals)
         return {'items': lines}
 
+    def _get_retencionesPercepciones(self):
+        retencionesPercepciones = []
+        for ret in self.documento.retencionesPercepciones:
+            vals = {}
+            vals['codigo'] = ret.codigo
+            vals['tasa'] = ret.tasa
+            vals['monto_sujeto'] = ret.base
+            retencionesPercepciones.append(vals)
+        return {'retencionesPercepciones': retencionesPercepciones}
+
     def get_document(self):
         documento = {}
         documento.update(self._get_voucher())
         documento.update(self._get_partner())
-        documento.update(self._get_lines())
+        if self.documento.items:
+            documento.update(self._get_lines())
+        if self.documento.retencionesPercepciones and self.documento.tipoCFE in ['182']:
+            documento.update(self._get_retencionesPercepciones())
         if self.documento.tipoCFE in ['102', '103', '112', '113']:
             documento.update(self._get_ref())
         if self.documento.adenda:
             documento['adenda'] = self.documento.adenda
         if self.documento.clauVenta:
             documento['clausula_venta'] = self.documento.clauVenta
         if self.documento.modVenta:
```

### Comparing `pyCFE-0.0.16/src/biller/cliente.py` & `pyCFE-0.0.20/src/biller/cliente.py`

 * *Files identical despite different names*

### Comparing `pyCFE-0.0.16/src/common/documento.py` & `pyCFE-0.0.20/src/common/documento.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,15 +116,18 @@
         self.modalidadVenta = vals.get('modalidadVenta', '')
         self.viaTransporte = vals.get('viaTransporte', '')
 
         items = set()
         for item_val in vals.get('items', []):
             items.add(Items(item_val))
         self.items = items
-
+        retencionesPercepciones = set()
+        for ret_per_val in vals.get('retencionesPercepciones', []):
+            retencionesPercepciones.add(RetencionesPercepciones(ret_per_val))
+        self.retencionesPercepciones = retencionesPercepciones
         descuentos = set()
         for desc_val in vals.get('descuentos', []):
             descuentos.add(Descuento(desc_val))
         self.descuentos = descuentos
         self.mntNoGrv = round(vals.get('mntNoGrv', 0.0), 2)
         self.mntNetoIVATasaMin = round(vals.get('mntNetoIVATasaMin', 0.0), 2)
         self.mntNetoIVATasaBasica = round(vals.get('mntNetoIVATasaBasica', 0.0), 2)
@@ -140,14 +143,15 @@
         self.referencia = vals.get("referencia", "")
         referencias = set()
         for ref in vals.get('referencias', []):
             referencias.add(Referencia(ref))
         self.referencias = referencias
 
         self.numero_interno = vals.get("numero_interno", "")
+        self.numero_orden = vals.get("numero_orden", "")
 
 class Referencia:
     def __init__(self, vals):
         self.motivo = vals.get('motivo', '')
         self.tipoDocRef = vals.get('tipoDocRef', '')
         self.serie = vals.get('serie', '')
         self.numero = vals.get('numero', '')
@@ -167,14 +171,21 @@
         self.codProducto = vals.get('codProducto', '')
         # self.descuentoTipo = vals.get('descuentoTipo', '%')
         self.descuento = vals.get('descuento', 0.0)
         self.descuentoMonto = vals.get('descuentoMonto', 0.0)
         self.recargoMonto = vals.get('recargoMonto', 0.0)
         self.recargo = vals.get('recargo', 0.0)
 
+class RetencionesPercepciones:
+
+    def __init__(self, vals):
+        self.codigo = vals.get('codigo', '')
+        self.tasa = vals.get('tasa', 0.0)
+        self.base = round(vals.get('base', 0.0),2)
+        self.monto = round(vals.get('monto', 0.0), 2)
 
 class Descuento:
 
     def __init__(self, vals):
         self.descripcion = vals.get('descripcion', '')
         self.monto = round(vals.get('monto', 0.0), 2)
         self.indicadorFacturacion = vals.get('indicadorFacturacion', '')
```

### Comparing `pyCFE-0.0.16/src/common/empresa.py` & `pyCFE-0.0.20/src/common/empresa.py`

 * *Files identical despite different names*

### Comparing `pyCFE-0.0.16/src/common/servidor.py` & `pyCFE-0.0.20/src/common/servidor.py`

 * *Files identical despite different names*

### Comparing `pyCFE-0.0.16/src/efactura/cliente.py` & `pyCFE-0.0.20/src/efactura/cliente.py`

 * *Files identical despite different names*

### Comparing `pyCFE-0.0.16/src/efactura/efactura.py` & `pyCFE-0.0.20/src/efactura/efactura.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,15 @@
     def getInvoice(self, documento):
         xmlns=etree.QName(None, 'CFE')
         nsmap1=OrderedDict([('ns0', self._ns0)] )
         self._root=etree.Element("CFE", version="1.0", nsmap=nsmap1)
         if documento.tipoCFE in ['101', '102', '103', '201', '202', '203']:
             tag = etree.QName(self._ns0, 'eTck')
             etck=etree.SubElement(self._root, tag.text, nsmap={'ns0':tag.namespace})
-        if documento.tipoCFE in ['121', '122', '123']:
+        elif documento.tipoCFE in ['121', '122', '123']:
             tag = etree.QName(self._ns0, 'eFact_Exp')
             etck = etree.SubElement(self._root, tag.text, nsmap={'ns0': tag.namespace})
         else:
             tag = etree.QName(self._ns0, 'eFact')
             etck=etree.SubElement(self._root, tag.text, nsmap={'ns0':tag.namespace})
         tag = etree.QName(self._ns0, 'Encabezado')
         encabezado = etree.SubElement(etck, tag.text, nsmap={'ns0':tag.namespace})
```

### Comparing `pyCFE-0.0.16/src/facturaexpress/cliente.py` & `pyCFE-0.0.20/src/facturaexpress/cliente.py`

 * *Files identical despite different names*

### Comparing `pyCFE-0.0.16/src/facturaexpress/facturaexpress.py` & `pyCFE-0.0.20/src/facturaexpress/facturaexpress.py`

 * *Files identical despite different names*

