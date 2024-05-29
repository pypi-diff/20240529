# Comparing `tmp/OCR_GLS_G6-0.0.7.tar.gz` & `tmp/OCR_GLS_G6-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\OCR_GLS_G6-0.0.7.tar", last modified: Fri Feb  2 04:42:17 2024, max compression
+gzip compressed data, was "dist\OCR_GLS_G6-0.0.8.tar", last modified: Wed May 29 02:27:59 2024, max compression
```

## Comparing `OCR_GLS_G6-0.0.7.tar` & `OCR_GLS_G6-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-02-02 04:42:17.000000 OCR_GLS_G6-0.0.7/
-drwxrwxrwx   0        0        0        0 2024-02-02 04:42:17.000000 OCR_GLS_G6-0.0.7/OCR_GLS_G6/
--rw-rw-rw-   0        0        0     3896 2023-10-24 10:02:58.000000 OCR_GLS_G6-0.0.7/OCR_GLS_G6/OcrTools.py
--rw-rw-rw-   0        0        0       65 2023-10-24 10:04:57.000000 OCR_GLS_G6-0.0.7/OCR_GLS_G6/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-02 04:42:17.000000 OCR_GLS_G6-0.0.7/OCR_GLS_G6.egg-info/
--rw-rw-rw-   0        0        0     3143 2024-02-02 04:42:17.000000 OCR_GLS_G6-0.0.7/OCR_GLS_G6.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2024-02-02 04:42:17.000000 OCR_GLS_G6-0.0.7/OCR_GLS_G6.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-02 04:42:17.000000 OCR_GLS_G6-0.0.7/OCR_GLS_G6.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      917 2024-02-02 04:42:17.000000 OCR_GLS_G6-0.0.7/OCR_GLS_G6.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-02 04:42:17.000000 OCR_GLS_G6-0.0.7/OCR_GLS_G6.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3143 2024-02-02 04:42:17.000000 OCR_GLS_G6-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1954 2024-02-02 04:41:22.000000 OCR_GLS_G6-0.0.7/README.rst
--rw-rw-rw-   0        0        0       86 2024-02-02 04:42:17.000000 OCR_GLS_G6-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2215 2024-02-02 04:26:56.000000 OCR_GLS_G6-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 02:27:59.000000 OCR_GLS_G6-0.0.8/
+drwxrwxrwx   0        0        0        0 2024-05-29 02:27:59.000000 OCR_GLS_G6-0.0.8/OCR_GLS_G6/
+-rw-rw-rw-   0        0        0     4440 2024-05-29 02:26:41.000000 OCR_GLS_G6-0.0.8/OCR_GLS_G6/OcrTools.py
+-rw-rw-rw-   0        0        0       65 2023-10-24 10:04:57.000000 OCR_GLS_G6-0.0.8/OCR_GLS_G6/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 02:27:59.000000 OCR_GLS_G6-0.0.8/OCR_GLS_G6.egg-info/
+-rw-rw-rw-   0        0        0     3138 2024-05-29 02:27:59.000000 OCR_GLS_G6-0.0.8/OCR_GLS_G6.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2024-05-29 02:27:59.000000 OCR_GLS_G6-0.0.8/OCR_GLS_G6.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 02:27:59.000000 OCR_GLS_G6-0.0.8/OCR_GLS_G6.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-29 02:27:59.000000 OCR_GLS_G6-0.0.8/OCR_GLS_G6.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-29 02:27:59.000000 OCR_GLS_G6-0.0.8/OCR_GLS_G6.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3138 2024-05-29 02:27:59.000000 OCR_GLS_G6-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1954 2024-02-02 04:41:22.000000 OCR_GLS_G6-0.0.8/README.rst
+-rw-rw-rw-   0        0        0       86 2024-05-29 02:27:59.000000 OCR_GLS_G6-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1159 2024-05-29 02:27:03.000000 OCR_GLS_G6-0.0.8/setup.py
```

### Comparing `OCR_GLS_G6-0.0.7/OCR_GLS_G6/OcrTools.py` & `OCR_GLS_G6-0.0.8/OCR_GLS_G6/OcrTools.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,55 +32,64 @@
             else:
                 newFileLocation = "."
             imageLocation = OcrTools.pdfToImg(
                 locationFile, temp+"\\"+newFileLocation+".png")
             print(imageLocation)
         area_xMax = area['offset_x_min']+area['width']
         area_yMax = area['offset_y_min']+area['height']
-        if typeOfOcr == 'Text':
-            allResultDetective = []
-            reader = easyocr.Reader(languageOcr)
-            allResults = reader.readtext(imageLocation)
-            for result in allResults:
-                pos1, pos2, pos3, pos4 = result[0]
-                xMin = round(min([pos1[0], pos2[0], pos3[0], pos4[0]]))
-                xMax = round(max([pos1[0], pos2[0], pos3[0], pos4[0]]))
-                yMin = round(min([pos1[1], pos2[1], pos3[1], pos4[1]]))
-                yMax = round(max([pos1[1], pos2[1], pos3[1], pos4[1]]))
-                if (area['offset_x_min'] in range(xMin-deviation, xMin+deviation)):
-                    if (area['offset_y_min'] in range(yMin-deviation, yMin+deviation)):
-                        if (area_xMax in range(xMax-deviation, xMax+deviation)):
-                            if (area_yMax in range(area_yMax-deviation, area_yMax+deviation)):
-                                word = result[1]
-                                if word in dataCheck:
-                                    valid = True
-                                else:
-                                    valid = False
-                                accuracy_percent = str(
-                                    round(result[2]*100))+"%"
-                                allResultDetective.append({
-                                    'coordinates': result[0],
-                                    'value': word,
-                                    'valid': valid,
-                                    'accuracy_percent': accuracy_percent,
-                                })
-            os.remove(imageLocation)
-            return allResultDetective
-        elif typeOfOcr == 'qrcode':
-            image = cv2.imread(imageLocation)
-            cropped_image = image[area['offset_y_min']:area_yMax, area['offset_x_min']:area_xMax]
-            result = decode(cropped_image)
-            os.remove(imageLocation)
-            if result:
-                return {
-                    'coordinates': [area['offset_y_min'], area_yMax, area['offset_x_min'], area_xMax],
-                    'value': result[0].data,
-                    'valid': True,
-                    'accuracy_percent': '-',
-                }
+        try:
+            if typeOfOcr == 'Text':
+                allResultDetective = []
+                reader = easyocr.Reader(languageOcr)
+                allResults = reader.readtext(imageLocation)
+                #print("allResults::",allResults)
+                for result in allResults:
+                    pos1, pos2, pos3, pos4 = result[0]
+                    xMin = round(min([pos1[0], pos2[0], pos3[0], pos4[0]]))
+                    xMax = round(max([pos1[0], pos2[0], pos3[0], pos4[0]]))
+                    yMin = round(min([pos1[1], pos2[1], pos3[1], pos4[1]]))
+                    yMax = round(max([pos1[1], pos2[1], pos3[1], pos4[1]]))
+                    if (area['offset_x_min'] in range(xMin-deviation, xMin+deviation)):
+                        if (area['offset_y_min'] in range(yMin-deviation, yMin+deviation)):
+                            if (area_xMax in range(xMax-deviation, xMax+deviation)):
+                                if (area_yMax in range(area_yMax-deviation, area_yMax+deviation)):
+                                    word = result[1]
+                                    if word in dataCheck:
+                                        valid = True
+                                    else:
+                                        valid = False
+                                    accuracy_percent = str(
+                                        round(result[2]*100))+"%"
+                                    allResultDetective.append({
+                                        'coordinates': result[0],
+                                        'value': word,
+                                        'valid': valid,
+                                        'accuracy_percent': accuracy_percent,
+                                    })
+                os.remove(imageLocation)
+                return allResultDetective
+            elif typeOfOcr == 'qrcode':
+                image = cv2.imread(imageLocation)
+                cropped_image = image[area['offset_y_min']:area_yMax, area['offset_x_min']:area_xMax]
+                result = decode(cropped_image)
+                os.remove(imageLocation)
+                if result:
+                    return {
+                        'coordinates': [area['offset_y_min'], area_yMax, area['offset_x_min'], area_xMax],
+                        'value': result[0].data,
+                        'valid': True,
+                        'accuracy_percent': '-',
+                    }
+                else:
+                    return {
+                        'coordinates': [area['offset_y_min'], area_yMax, area['offset_x_min'], area_xMax],
+                        'value': result,
+                        'valid': False,
+                        'accuracy_percent': '-',
+                    }
             else:
-                return {
-                    'coordinates': [area['offset_y_min'], area_yMax, area['offset_x_min'], area_xMax],
-                    'value': result,
-                    'valid': False,
-                    'accuracy_percent': '-',
-                }
+                if os.path.exists(imageLocation):
+                    os.remove(imageLocation)
+        except Exception as e:
+            if os.path.exists(imageLocation):
+                os.remove(imageLocation)
+            return {'status':'error','msg':str(e)}
```

### Comparing `OCR_GLS_G6-0.0.7/OCR_GLS_G6.egg-info/PKG-INFO` & `OCR_GLS_G6-0.0.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
-Name: OCR-GLS-G6
-Version: 0.0.7
+Name: OCR_GLS_G6
+Version: 0.0.8
 Summary: OCR_GLS_G6 - Optical character recognition and QR codes
 Home-page: https://git.bdms.co.th/Burin.Pa/ocr_gls_g6
 Author: Burin Panchat
 Author-email: burin.gbp@gmail.com
 License: MIT
-Download-URL: https://git.bdms.co.th/Burin.Pa/ocr_gls_g6/-/archive/v0.0.6/ocr_gls_g6-v0.0.3.zip
+Download-URL: https://git.bdms.co.th/Burin.Pa/ocr_gls_g6/-/blob/master/dist/ocr_gls_g6.zip
 Description: (OCR-GLS-G6) OCR
         ----------------
         
         |github release version| |python version| |license|
         
         --------------
```

### Comparing `OCR_GLS_G6-0.0.7/PKG-INFO` & `OCR_GLS_G6-0.0.8/OCR_GLS_G6.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
-Name: OCR_GLS_G6
-Version: 0.0.7
+Name: OCR-GLS-G6
+Version: 0.0.8
 Summary: OCR_GLS_G6 - Optical character recognition and QR codes
 Home-page: https://git.bdms.co.th/Burin.Pa/ocr_gls_g6
 Author: Burin Panchat
 Author-email: burin.gbp@gmail.com
 License: MIT
-Download-URL: https://git.bdms.co.th/Burin.Pa/ocr_gls_g6/-/archive/v0.0.6/ocr_gls_g6-v0.0.3.zip
+Download-URL: https://git.bdms.co.th/Burin.Pa/ocr_gls_g6/-/blob/master/dist/ocr_gls_g6.zip
 Description: (OCR-GLS-G6) OCR
         ----------------
         
         |github release version| |python version| |license|
         
         --------------
```

### Comparing `OCR_GLS_G6-0.0.7/README.rst` & `OCR_GLS_G6-0.0.8/README.rst`

 * *Files identical despite different names*

