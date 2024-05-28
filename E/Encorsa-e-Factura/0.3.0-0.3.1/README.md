# Comparing `tmp/encorsa_e_factura-0.3.0.tar.gz` & `tmp/encorsa_e_factura-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encorsa_e_factura-0.3.0.tar", last modified: Tue May 21 13:13:20 2024, max compression
+gzip compressed data, was "encorsa_e_factura-0.3.1.tar", last modified: Tue May 28 12:17:43 2024, max compression
```

## Comparing `encorsa_e_factura-0.3.0.tar` & `encorsa_e_factura-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 13:13:20.265640 encorsa_e_factura-0.3.0/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-21 13:13:05.000000 encorsa_e_factura-0.3.0/LICENCE
--rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-05-21 13:13:20.265640 encorsa_e_factura-0.3.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      885 2024-05-21 13:13:05.000000 encorsa_e_factura-0.3.0/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)       95 2024-05-21 13:13:17.000000 encorsa_e_factura-0.3.0/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)      679 2024-05-21 13:13:20.265640 encorsa_e_factura-0.3.0/setup.cfg
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 13:13:20.261640 encorsa_e_factura-0.3.0/src/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 13:13:20.265640 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura/
--rw-r--r--   0 vsts      (1001) docker     (127)     8253 2024-05-21 13:13:05.000000 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura/WebConRequestUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15963 2024-05-21 13:13:05.000000 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura/XMLUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)       27 2024-05-21 13:13:05.000000 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      624 2024-05-21 13:13:05.000000 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura/runLocaly.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25383 2024-05-21 13:13:05.000000 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura/sincronizare.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 13:13:20.265640 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-05-21 13:13:20.000000 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      499 2024-05-21 13:13:20.000000 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-21 13:13:20.000000 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       88 2024-05-21 13:13:20.000000 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        9 2024-05-21 13:13:20.000000 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-05-21 13:13:20.000000 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-28 12:17:43.567825 encorsa_e_factura-0.3.1/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-28 12:17:27.000000 encorsa_e_factura-0.3.1/LICENCE
+-rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-05-28 12:17:43.567825 encorsa_e_factura-0.3.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      885 2024-05-28 12:17:27.000000 encorsa_e_factura-0.3.1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)       95 2024-05-28 12:17:40.000000 encorsa_e_factura-0.3.1/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)      679 2024-05-28 12:17:43.571825 encorsa_e_factura-0.3.1/setup.cfg
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-28 12:17:43.563825 encorsa_e_factura-0.3.1/src/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-28 12:17:43.567825 encorsa_e_factura-0.3.1/src/Encorsa_e_Factura/
+-rw-r--r--   0 vsts      (1001) docker     (127)     8253 2024-05-28 12:17:27.000000 encorsa_e_factura-0.3.1/src/Encorsa_e_Factura/WebConRequestUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15963 2024-05-28 12:17:27.000000 encorsa_e_factura-0.3.1/src/Encorsa_e_Factura/XMLUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       27 2024-05-28 12:17:27.000000 encorsa_e_factura-0.3.1/src/Encorsa_e_Factura/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      624 2024-05-28 12:17:27.000000 encorsa_e_factura-0.3.1/src/Encorsa_e_Factura/runLocaly.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25703 2024-05-28 12:17:27.000000 encorsa_e_factura-0.3.1/src/Encorsa_e_Factura/sincronizare.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-28 12:17:43.567825 encorsa_e_factura-0.3.1/src/Encorsa_e_Factura.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-05-28 12:17:43.000000 encorsa_e_factura-0.3.1/src/Encorsa_e_Factura.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      499 2024-05-28 12:17:43.000000 encorsa_e_factura-0.3.1/src/Encorsa_e_Factura.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-28 12:17:43.000000 encorsa_e_factura-0.3.1/src/Encorsa_e_Factura.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       88 2024-05-28 12:17:43.000000 encorsa_e_factura-0.3.1/src/Encorsa_e_Factura.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        9 2024-05-28 12:17:43.000000 encorsa_e_factura-0.3.1/src/Encorsa_e_Factura.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-05-28 12:17:43.000000 encorsa_e_factura-0.3.1/src/Encorsa_e_Factura.egg-info/top_level.txt
```

### Comparing `encorsa_e_factura-0.3.0/LICENCE` & `encorsa_e_factura-0.3.1/LICENCE`

 * *Files identical despite different names*

### Comparing `encorsa_e_factura-0.3.0/PKG-INFO` & `encorsa_e_factura-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Encorsa_e_Factura
-Version: 0.3.0
+Version: 0.3.1
 Summary: A small example package
 Home-page: https://encorsa.ro
 Author: Dan Popescu, Razvan Ogrezeanu
 Author-email: dan.popescu@encorsa.com, razvan.ogrezeanu@encorsa.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `encorsa_e_factura-0.3.0/README.md` & `encorsa_e_factura-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `encorsa_e_factura-0.3.0/setup.cfg` & `encorsa_e_factura-0.3.1/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Encorsa_e_Factura
-version = 0.3.0
+version = 0.3.1
 author = Dan Popescu, Razvan Ogrezeanu
 author_email = dan.popescu@encorsa.com, razvan.ogrezeanu@encorsa.com
 description = A small example package
 long_description = file: README.md
 url = https://encorsa.ro
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `encorsa_e_factura-0.3.0/src/Encorsa_e_Factura/WebConRequestUtils.py` & `encorsa_e_factura-0.3.1/src/Encorsa_e_Factura/WebConRequestUtils.py`

 * *Files identical despite different names*

### Comparing `encorsa_e_factura-0.3.0/src/Encorsa_e_Factura/XMLUtils.py` & `encorsa_e_factura-0.3.1/src/Encorsa_e_Factura/XMLUtils.py`

 * *Files identical despite different names*

### Comparing `encorsa_e_factura-0.3.0/src/Encorsa_e_Factura/runLocaly.py` & `encorsa_e_factura-0.3.1/src/Encorsa_e_Factura/runLocaly.py`

 * *Files identical despite different names*

### Comparing `encorsa_e_factura-0.3.0/src/Encorsa_e_Factura/sincronizare.py` & `encorsa_e_factura-0.3.1/src/Encorsa_e_Factura/sincronizare.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,20 +209,27 @@
     except Exception as e:
         # Handle other errors
         error_message = f"Error while downloading ZIP archive with the XML. Message: {e}"
         print(error_message)
         raise Exception(error_message)
 
 
-def xml_to_pdf_to_base64(xml_data, parameters):
+def xml_to_pdf_to_base64(xml_data, parameters, document_type):
     """
     Funcția trimite date XML către un serviciu web al ANAF pentru a fi convertite
     într-un document PDF, apoi encodează conținutul binar al PDF-ului obținut în format Base64
     """
-    url = "https://webservicesp.anaf.ro/prod/FCTEL/rest/transformare/FACT1/DA"
+
+    if document_type == "Invoice":
+        url = "https://webservicesp.anaf.ro/prod/FCTEL/rest/transformare/FACT1/DA"
+    elif document_type == "CreditNote":
+        url = "https://webservicesp.anaf.ro/prod/FCTEL/rest/transformare/FCN/DA"
+    else:
+        raise ValueError("Invalid document type for XML to PDF conversion." + f" Document type: {document_type}")
+    
     headers = {'Content-Type': 'text/plain'}
     proxies = {'http': None, 'https': None}
 
     # Set proxies if provided in parameters
     if "proxi_pt_anaf_https" in parameters and parameters["proxi_pt_anaf_https"]:
         proxies["https"] = parameters["proxi_pt_anaf_https"]
     if "proxi_pt_anaf_http" in parameters and parameters["proxi_pt_anaf_http"]:
@@ -358,15 +365,15 @@
                 parameters, wtoken, invoice_id_element, company_id)
             if (parameters['how_to_handle_duplicates'] == 'SKIP'):
                 if ifInvoiceExists:
                     print(
                         f"Skipping {document_type} with ID: {invoice_id_element}, COMPANY ID: {company_id}, because it already exists in WebCon.")
                     continue
 
-            pdf_content = xml_to_pdf_to_base64(xml_text, parameters)
+            pdf_content = xml_to_pdf_to_base64(xml_text, parameters, document_type)
             xml_bytes = str(xml_text).encode('utf-8')
             base64_encoded_xml = base64.b64encode(xml_bytes)
             base64_string_xml = base64_encoded_xml.decode('utf-8')
 
             body = create_webcon_body(parameters, base64_string_xml, pdf_content, xml_text, invoice_id_element, company_id,
                                       local_xml_template_file_path, wfd_id_duplicate, local_namespaces, document_type, id, iso_data_creare)
             response = create_invoice_instance(parameters, wtoken, body)
```

### Comparing `encorsa_e_factura-0.3.0/src/Encorsa_e_Factura.egg-info/PKG-INFO` & `encorsa_e_factura-0.3.1/src/Encorsa_e_Factura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Encorsa_e_Factura
-Version: 0.3.0
+Version: 0.3.1
 Summary: A small example package
 Home-page: https://encorsa.ro
 Author: Dan Popescu, Razvan Ogrezeanu
 Author-email: dan.popescu@encorsa.com, razvan.ogrezeanu@encorsa.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

