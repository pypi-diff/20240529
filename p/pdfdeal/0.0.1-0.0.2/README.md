# Comparing `tmp/pdfdeal-0.0.1.tar.gz` & `tmp/pdfdeal-0.0.2.tar.gz`

## Comparing `pdfdeal-0.0.1.tar` & `pdfdeal-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pdfdeal-0.0.1/src/pdfdeal/__init__.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 pdfdeal-0.0.1/src/pdfdeal/file_tools.py
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 pdfdeal-0.0.1/src/pdfdeal/get_file.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 pdfdeal-0.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pdfdeal-0.0.1/LICENSE
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 pdfdeal-0.0.1/README.md
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 pdfdeal-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 pdfdeal-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 pdfdeal-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pdfdeal-0.0.2/src/pdfdeal/__init__.py
+-rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 pdfdeal-0.0.2/src/pdfdeal/file_tools.py
+-rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 pdfdeal-0.0.2/src/pdfdeal/get_file.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 pdfdeal-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pdfdeal-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 pdfdeal-0.0.2/README.md
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 pdfdeal-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 pdfdeal-0.0.2/PKG-INFO
```

### Comparing `pdfdeal-0.0.1/src/pdfdeal/file_tools.py` & `pdfdeal-0.0.2/src/pdfdeal/file_tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import io
 from PIL import Image
 from pypdf import PdfReader
 import re
 import emoji
 import unicodedata
 import os
-import easyocr
 
 
 def OCR_easyocr(path, language=["ch_sim", "en"], GPU=False):
+    try:
+        import easyocr
+    except ImportError:
+        raise ImportError("Please install easyocr first, use 'pip install easyocr'")
     reader = easyocr.Reader(language, gpu=GPU)
     texts = ""
     if os.path.isfile(path) and path.endswith((".jpg", ".png", ".jpeg")):
         result = reader.readtext(path, detail=0, paragraph=True)
         texts += "\n".join(result)
     elif os.path.isdir(path):
         for root, dirs, files in os.walk(path):
@@ -20,14 +23,37 @@
                 file_path = os.path.join(root, file)
                 if file_path.endswith((".jpg", ".png", ".jpeg")):
                     result = reader.readtext(file_path, detail=0, paragraph=True)
                     texts += "\n".join(result)
     return texts
 
 
+def OCR_pytesseract(path, language=["eng"], GPU=False):
+    try:
+        import pytesseract
+    except ImportError:
+        raise ImportError(
+            "Please install pytesseract first, use 'pip install pytesseract'"
+        )
+    text = ""
+    if os.path.isfile(path) and path.endswith((".jpg", ".png", ".jpeg")):
+        text += pytesseract.image_to_string(path, lang=language[0])
+    elif os.path.isdir(path):
+        for root, dirs, files in os.walk(path):
+            for file in files:
+                file_path = os.path.join(root, file)
+                if file_path.endswith((".jpg", ".png", ".jpeg")):
+                    text += pytesseract.image_to_string(file_path, lang=language[0])
+                    text += "\n"
+    return text
+
+
+def OCR_pass(path, language=["ch_sim", "en"], GPU=False):
+    return ""
+
 def clean_text(text):
     # remove extra whitespaces
     text = re.sub(r"\n\s*\n", "\n\n", text)
 
     # remove special characters
     text = re.sub(r"-\d+-", "", text)
```

### Comparing `pdfdeal-0.0.1/.gitignore` & `pdfdeal-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pdfdeal-0.0.1/LICENSE` & `pdfdeal-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfdeal-0.0.1/pyproject.toml` & `pdfdeal-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 [project]
 name = "pdfdeal"
-version = "0.0.1"
+version = "0.0.2"
 authors = [{ name = "Menghuan1918", email = "menghuan@menghuan1918.com" }]
 description = "Easier to deal with PDF, extract readable text and OCR to recognise image text and clean the format. Make it more suitable for knowledge base construction."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ["emoji", "pypdf", "Pillow", "easyocr", "requests", "reportlab"]
+dependencies = ["emoji", "pypdf", "Pillow", "requests", "reportlab"]
+
+[project.optional-dependencies]
+default = ["easyocr"]
+pytesseract = ["pytesseract"]
+custom = []
 
 [project.urls]
 Homepage = "https://github.com/Menghuan1918/pdfdeal"
 Issues = "https://github.com/Menghuan1918/pdfdeal/issues"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/pdfdeal"]
```

### Comparing `pdfdeal-0.0.1/PKG-INFO` & `pdfdeal-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,44 @@
-Metadata-Version: 2.3
-Name: pdfdeal
-Version: 0.0.1
-Summary: Easier to deal with PDF, extract readable text and OCR to recognise image text and clean the format. Make it more suitable for knowledge base construction.
-Project-URL: Homepage, https://github.com/Menghuan1918/pdfdeal
-Project-URL: Issues, https://github.com/Menghuan1918/pdfdeal/issues
-Author-email: Menghuan1918 <menghuan@menghuan1918.com>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Requires-Dist: easyocr
-Requires-Dist: emoji
-Requires-Dist: pillow
-Requires-Dist: pypdf
-Requires-Dist: reportlab
-Requires-Dist: requests
-Description-Content-Type: text/markdown
-
 # pdfdeal
 
 Easier to deal with PDF, extract readable text and OCR to recognise image text and clean the format. Make it more suitable for knowledge base construction.
 
-Its going to use [easyocr](https://github.com/JaidedAI/EasyOCR) to recognise the image and add it to the original text. If the output format uses pdf format, this ensures that the text is on the same number of pages in the new PDF as the original. You can use knowledge base applications (such as [Dify](https://github.com/langgenius/dify),[FastGPT](https://github.com/labring/FastGPT)) before the PDF processing, so that theoretically can reach a better recognition rate.
+Its going to use [easyocr](https://github.com/JaidedAI/EasyOCR) to recognise the image and add it to the original text. If the output format uses pdf format, this ensures that the text is on the same number of pages in the new PDF as the original. You can use knowledge base applications (such as [Dify](https://github.com/langgenius/dify),[FastGPT](https://github.com/labring/FastGPT)) after the PDF processing, so that theoretically can reach a better recognition rate.
 
 ![image](https://github.com/Menghuan1918/pdfdeal/assets/122662527/371a17c5-e0cb-464b-a1c4-61d2963c772f)
 
 > The figure above shows a comparison of the results before and after the processing of the same PDF
 > Unprocessed document encoding results <----> Processed file encoding results
 
 ## Usage
+### Install
+Install from PyPI:
+
+```bash
+pip install pdfdeal
+```
+
+Using `pytesseract` instead of default `easyocr`:
+
+```bash
+pip install pdfdeal[pytesseract]
+```
+
+Using own custom OCR function or skip OCR:
+
+```bash
+pip install pdfdeal[custom]
+```
+
+Install from source:
+
+```bash
+pip install git+https://github.com/Menghuan1918/pdfdeal.git
+```
+
 ### Parameters
 Import the function by`from pdfdeal import deal_pdf`. Explanation of the parameters accepted by the function:
 
 - **input**: `str`
   - Description: The URL or local path to the PDF file that you want to process.
   - Example: `"https://example.com/sample.pdf"` or `"/path/to/local/sample.pdf"`
 
@@ -42,43 +47,64 @@
     - `"text"`: Extracted text from the PDF as a single string.
     - `"texts"`: Extracted text from the PDF as a list of strings, one per page.
     - `"md"`: Markdown formatted text.
     - `"pdf"`: A new PDF file with the extracted text.
   - Example: `"md"`
 
 - **ocr**: `function`, optional, default: `None`
-  - Description: A custom OCR (Optical Character Recognition) function. If not provided, the default OCR function will be used.
-  - Example: `custom_ocr_function`, input is :`(path, language=["ch_sim", "en"], GPU=False)`, return a `string`
+  - Description: A custom OCR (Optical Character Recognition) function. If not provided, the default OCR function will be used. Use string "pytesseract" to use pytesseract, string "pass" to skip OCR
+  - Example custom OCR function: `custom_ocr_function`, input is :`(path, language=["ch_sim", "en"], GPU=False)`, return a `string`
 
 
 - **language**: `list`, optional, default: `["ch_sim", "en"]`
-  - Description: A list of languages to be used in OCR. The default languages are Simplified Chinese (`"ch_sim"`) and English (`"en"`).
+  - Description: A list of languages to be used in OCR. The default languages are Simplified Chinese (`"ch_sim"`) and English (`"en"`). ["eng"] for pytesseract.
   - Example: `["en", "fr"]`
 
 - **GPU**: `bool`, optional, default: `False`
   - Description: A boolean flag indicating whether to use GPU for OCR processing. If set to `True`, GPU will be used.
   - Example: `True`
 
 - **path**: `str`, optional, default: `None`
   - Description: The directory path where the output file will be saved. This parameter is only used when the `output` type is `"md"` or `"pdf"`.
   - Example: `"/path/to/save/output"`
 
 ### Processes all the files in a file and saves them in the Output folder
+
 ```python
 import os
 from pdfdeal import deal_pdf
 for root, dirs, files in os.walk("./PPT"):
     for file in files:
         file_path = os.path.join(root, file)
         deal_pdf(
             input=file_path, output="pdf", language=["en"], path="./Output", GPU=True
         )
         print(f"Deal with {file_path} successfully!")
 ```
 
-### Get the the list of the pdf
+### Get the the list of text in the pdf
+
 ```python
 from pdfdeal import deal_pdf
 Text = deal_pdf(input="test.pdf", output="texts", language=["en"], GPU=True)
 for text in Text:
   print(text)
 ```
+
+### Using pytesseract to do OCR
+
+```python
+output_path = deal_pdf(
+    input="test.pdf",
+    output="md",
+    ocr="pytesseract",
+    language=["eng"],
+    path="markdown"
+)
+print(f"Save processed file to {output_path}")
+```
+
+### Skip OCR
+
+```python
+print(deal_pdf(input="test.pdf",ocr="pass"))
+```
```

