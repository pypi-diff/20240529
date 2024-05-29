# Comparing `tmp/autoanki-1.2.0.tar.gz` & `tmp/autoanki-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoanki-1.2.0.tar", last modified: Thu May 16 00:50:40 2024, max compression
+gzip compressed data, was "autoanki-1.2.1.tar", last modified: Wed May 29 00:26:35 2024, max compression
```

## Comparing `autoanki-1.2.0.tar` & `autoanki-1.2.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-16 00:50:40.083384 autoanki-1.2.0/
--rw-r--r--   0 owner      (501) staff       (20)     1062 2024-04-04 21:53:37.000000 autoanki-1.2.0/LICENSE.txt
--rw-r--r--   0 owner      (501) staff       (20)      108 2024-05-14 11:15:45.000000 autoanki-1.2.0/MANIFEST.in
--rw-r--r--   0 owner      (501) staff       (20)     5810 2024-05-16 00:50:40.083314 autoanki-1.2.0/PKG-INFO
--rw-r--r--   0 owner      (501) staff       (20)     5053 2024-05-16 00:38:17.000000 autoanki-1.2.0/README.md
--rw-r--r--   0 owner      (501) staff       (20)      272 2024-05-12 08:57:48.000000 autoanki-1.2.0/pyproject.toml
--rw-r--r--   0 owner      (501) staff       (20)      119 2024-05-12 09:05:06.000000 autoanki-1.2.0/requirements.txt
--rw-r--r--   0 owner      (501) staff       (20)      845 2024-05-16 00:50:40.083684 autoanki-1.2.0/setup.cfg
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-16 00:50:40.068505 autoanki-1.2.0/src/
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-16 00:50:40.070674 autoanki-1.2.0/src/autoanki/
--rw-r--r--   0 owner      (501) staff       (20)     9130 2024-05-16 00:05:35.000000 autoanki-1.2.0/src/autoanki/AutoAnki.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-16 00:50:40.072234 autoanki-1.2.0/src/autoanki/BookCleaner/
--rw-r--r--   0 owner      (501) staff       (20)     4461 2024-05-14 08:51:38.000000 autoanki-1.2.0/src/autoanki/BookCleaner/BookCleaner.py
--rw-r--r--   0 owner      (501) staff       (20)       37 2023-04-17 16:36:34.000000 autoanki-1.2.0/src/autoanki/BookCleaner/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-16 00:50:40.073577 autoanki-1.2.0/src/autoanki/DatabaseManager/
--rw-r--r--   0 owner      (501) staff       (20)    13253 2024-05-16 00:46:33.000000 autoanki-1.2.0/src/autoanki/DatabaseManager/ChineseDatabaseManager.py
--rw-r--r--   0 owner      (501) staff       (20)     1873 2024-05-14 10:45:18.000000 autoanki-1.2.0/src/autoanki/DatabaseManager/DatabaseManager.py
--rw-r--r--   0 owner      (501) staff       (20)       59 2024-05-14 09:37:30.000000 autoanki-1.2.0/src/autoanki/DatabaseManager/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)      208 2023-04-18 23:52:52.000000 autoanki-1.2.0/src/autoanki/DatabaseManager/book_table.sql
--rw-r--r--   0 owner      (501) staff       (20)      186 2023-04-17 16:36:34.000000 autoanki-1.2.0/src/autoanki/DatabaseManager/book_table_view.sql
--rw-r--r--   0 owner      (501) staff       (20)      904 2023-04-17 16:36:34.000000 autoanki-1.2.0/src/autoanki/DatabaseManager/databases_init.sql
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-16 00:50:40.074223 autoanki-1.2.0/src/autoanki/DeckManager/
--rw-r--r--   0 owner      (501) staff       (20)     4929 2024-05-16 00:46:57.000000 autoanki-1.2.0/src/autoanki/DeckManager/DeckManager.py
--rw-r--r--   0 owner      (501) staff       (20)       67 2024-04-04 22:41:18.000000 autoanki-1.2.0/src/autoanki/DeckManager/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)     2829 2024-05-16 00:46:57.000000 autoanki-1.2.0/src/autoanki/DeckManager/template_decks.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-16 00:50:40.075205 autoanki-1.2.0/src/autoanki/Dictionary/
--rw-r--r--   0 owner      (501) staff       (20)     6148 2024-05-14 08:26:48.000000 autoanki-1.2.0/src/autoanki/Dictionary/.DS_Store
--rw-r--r--   0 owner      (501) staff       (20)     6599 2024-05-16 00:46:57.000000 autoanki-1.2.0/src/autoanki/Dictionary/CEDictionary.py
--rw-r--r--   0 owner      (501) staff       (20)      285 2024-05-14 08:51:38.000000 autoanki-1.2.0/src/autoanki/Dictionary/Dictionary.py
--rw-r--r--   0 owner      (501) staff       (20)       39 2024-05-14 08:51:38.000000 autoanki-1.2.0/src/autoanki/Dictionary/__init__.py
--rw-rw-r--   0 owner      (501) staff       (20)  9650508 2024-04-10 22:45:58.000000 autoanki-1.2.0/src/autoanki/Dictionary/cedict_ts.u8
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-16 00:50:40.082499 autoanki-1.2.0/src/autoanki/Tokenizer/
--rw-r--r--   0 owner      (501) staff       (20)     6665 2024-05-16 00:46:57.000000 autoanki-1.2.0/src/autoanki/Tokenizer/ChineseTokenizer.py
--rw-r--r--   0 owner      (501) staff       (20)      222 2024-05-14 08:51:38.000000 autoanki-1.2.0/src/autoanki/Tokenizer/Tokenizer.py
--rw-r--r--   0 owner      (501) staff       (20)       47 2024-05-14 08:51:38.000000 autoanki-1.2.0/src/autoanki/Tokenizer/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)       31 2024-05-14 08:51:38.000000 autoanki-1.2.0/src/autoanki/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-16 00:50:40.082965 autoanki-1.2.0/src/autoanki.egg-info/
--rw-r--r--   0 owner      (501) staff       (20)     5810 2024-05-16 00:50:40.000000 autoanki-1.2.0/src/autoanki.egg-info/PKG-INFO
--rw-r--r--   0 owner      (501) staff       (20)     1169 2024-05-16 00:50:40.000000 autoanki-1.2.0/src/autoanki.egg-info/SOURCES.txt
--rw-r--r--   0 owner      (501) staff       (20)        1 2024-05-16 00:50:40.000000 autoanki-1.2.0/src/autoanki.egg-info/dependency_links.txt
--rw-r--r--   0 owner      (501) staff       (20)        1 2023-05-05 21:37:00.000000 autoanki-1.2.0/src/autoanki.egg-info/not-zip-safe
--rw-r--r--   0 owner      (501) staff       (20)      118 2024-05-16 00:50:40.000000 autoanki-1.2.0/src/autoanki.egg-info/requires.txt
--rw-r--r--   0 owner      (501) staff       (20)        9 2024-05-16 00:50:40.000000 autoanki-1.2.0/src/autoanki.egg-info/top_level.txt
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-16 00:50:40.082779 autoanki-1.2.0/tests/
--rw-r--r--   0 owner      (501) staff       (20)     1294 2024-05-14 10:48:54.000000 autoanki-1.2.0/tests/test_AutoAnki.py
--rw-r--r--   0 owner      (501) staff       (20)      467 2024-05-14 08:51:38.000000 autoanki-1.2.0/tests/test_DeckManager.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-29 00:26:35.800963 autoanki-1.2.1/
+-rw-r--r--   0 owner      (501) staff       (20)     1062 2024-04-04 21:53:37.000000 autoanki-1.2.1/LICENSE.txt
+-rw-r--r--   0 owner      (501) staff       (20)      108 2024-05-14 11:15:45.000000 autoanki-1.2.1/MANIFEST.in
+-rw-r--r--   0 owner      (501) staff       (20)     5911 2024-05-29 00:26:35.800899 autoanki-1.2.1/PKG-INFO
+-rw-r--r--   0 owner      (501) staff       (20)     5053 2024-05-16 00:38:17.000000 autoanki-1.2.1/README.md
+-rw-r--r--   0 owner      (501) staff       (20)      272 2024-05-12 08:57:48.000000 autoanki-1.2.1/pyproject.toml
+-rw-r--r--   0 owner      (501) staff       (20)      179 2024-05-29 00:26:28.000000 autoanki-1.2.1/requirements.txt
+-rw-r--r--   0 owner      (501) staff       (20)      890 2024-05-29 00:26:35.801248 autoanki-1.2.1/setup.cfg
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-29 00:26:35.789980 autoanki-1.2.1/src/
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-29 00:26:35.791659 autoanki-1.2.1/src/autoanki/
+-rw-r--r--   0 owner      (501) staff       (20)    13985 2024-05-28 23:57:57.000000 autoanki-1.2.1/src/autoanki/AutoAnki.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-29 00:26:35.792605 autoanki-1.2.1/src/autoanki/BookCleaner/
+-rw-r--r--   0 owner      (501) staff       (20)     4461 2024-05-14 08:51:38.000000 autoanki-1.2.1/src/autoanki/BookCleaner/BookCleaner.py
+-rw-r--r--   0 owner      (501) staff       (20)       37 2023-04-17 16:36:34.000000 autoanki-1.2.1/src/autoanki/BookCleaner/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-29 00:26:35.793653 autoanki-1.2.1/src/autoanki/DatabaseManager/
+-rw-r--r--   0 owner      (501) staff       (20)    14966 2024-05-28 23:57:57.000000 autoanki-1.2.1/src/autoanki/DatabaseManager/ChineseDatabaseManager.py
+-rw-r--r--   0 owner      (501) staff       (20)     1952 2024-05-25 16:56:43.000000 autoanki-1.2.1/src/autoanki/DatabaseManager/DatabaseManager.py
+-rw-r--r--   0 owner      (501) staff       (20)       59 2024-05-14 09:37:30.000000 autoanki-1.2.1/src/autoanki/DatabaseManager/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)      208 2023-04-18 23:52:52.000000 autoanki-1.2.1/src/autoanki/DatabaseManager/book_table.sql
+-rw-r--r--   0 owner      (501) staff       (20)      186 2023-04-17 16:36:34.000000 autoanki-1.2.1/src/autoanki/DatabaseManager/book_table_view.sql
+-rw-r--r--   0 owner      (501) staff       (20)     1323 2024-05-25 05:55:06.000000 autoanki-1.2.1/src/autoanki/DatabaseManager/databases_init.sql
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-29 00:26:35.794076 autoanki-1.2.1/src/autoanki/DeckManager/
+-rw-r--r--   0 owner      (501) staff       (20)     9951 2024-05-28 23:57:57.000000 autoanki-1.2.1/src/autoanki/DeckManager/DeckManager.py
+-rw-r--r--   0 owner      (501) staff       (20)       67 2024-04-04 22:41:18.000000 autoanki-1.2.1/src/autoanki/DeckManager/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)     3191 2024-05-28 23:57:57.000000 autoanki-1.2.1/src/autoanki/DeckManager/template_decks.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-29 00:26:35.794709 autoanki-1.2.1/src/autoanki/Dictionary/
+-rw-r--r--   0 owner      (501) staff       (20)     6148 2024-05-14 08:26:48.000000 autoanki-1.2.1/src/autoanki/Dictionary/.DS_Store
+-rw-r--r--   0 owner      (501) staff       (20)     6837 2024-05-25 05:56:09.000000 autoanki-1.2.1/src/autoanki/Dictionary/CEDictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)      290 2024-05-20 17:28:58.000000 autoanki-1.2.1/src/autoanki/Dictionary/Dictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)       39 2024-05-14 08:51:38.000000 autoanki-1.2.1/src/autoanki/Dictionary/__init__.py
+-rw-rw-r--   0 owner      (501) staff       (20)  9650508 2024-04-10 22:45:58.000000 autoanki-1.2.1/src/autoanki/Dictionary/cedict_ts.u8
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-29 00:26:35.800178 autoanki-1.2.1/src/autoanki/Tokenizer/
+-rw-r--r--   0 owner      (501) staff       (20)     6794 2024-05-25 00:02:00.000000 autoanki-1.2.1/src/autoanki/Tokenizer/ChineseTokenizer.py
+-rw-r--r--   0 owner      (501) staff       (20)      222 2024-05-14 08:51:38.000000 autoanki-1.2.1/src/autoanki/Tokenizer/Tokenizer.py
+-rw-r--r--   0 owner      (501) staff       (20)       47 2024-05-14 08:51:38.000000 autoanki-1.2.1/src/autoanki/Tokenizer/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)       31 2024-05-14 08:51:38.000000 autoanki-1.2.1/src/autoanki/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-29 00:26:35.800629 autoanki-1.2.1/src/autoanki.egg-info/
+-rw-r--r--   0 owner      (501) staff       (20)     5911 2024-05-29 00:26:35.000000 autoanki-1.2.1/src/autoanki.egg-info/PKG-INFO
+-rw-r--r--   0 owner      (501) staff       (20)     1169 2024-05-29 00:26:35.000000 autoanki-1.2.1/src/autoanki.egg-info/SOURCES.txt
+-rw-r--r--   0 owner      (501) staff       (20)        1 2024-05-29 00:26:35.000000 autoanki-1.2.1/src/autoanki.egg-info/dependency_links.txt
+-rw-r--r--   0 owner      (501) staff       (20)        1 2023-05-05 21:37:00.000000 autoanki-1.2.1/src/autoanki.egg-info/not-zip-safe
+-rw-r--r--   0 owner      (501) staff       (20)      159 2024-05-29 00:26:35.000000 autoanki-1.2.1/src/autoanki.egg-info/requires.txt
+-rw-r--r--   0 owner      (501) staff       (20)        9 2024-05-29 00:26:35.000000 autoanki-1.2.1/src/autoanki.egg-info/top_level.txt
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-29 00:26:35.800456 autoanki-1.2.1/tests/
+-rw-r--r--   0 owner      (501) staff       (20)     1294 2024-05-14 10:48:54.000000 autoanki-1.2.1/tests/test_AutoAnki.py
+-rw-r--r--   0 owner      (501) staff       (20)      467 2024-05-14 08:51:38.000000 autoanki-1.2.1/tests/test_DeckManager.py
```

### Comparing `autoanki-1.2.0/LICENSE.txt` & `autoanki-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autoanki-1.2.0/PKG-INFO` & `autoanki-1.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: autoanki
-Version: 1.2.0
+Version: 1.2.1
 Summary: Automatically make Anki Decks for Chinese text
 Home-page: https://github.com/timmy6figures/autoanki
 Author: Jarvis Coghlin
 Author-email: jarviscoghlin@gmail.com
 Project-URL: Bug Tracker, https://github.com/timmy6figures/autoanki/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: chinese-converter>=1.1.1
 Requires-Dist: beautifulsoup4~=4.12.2
+Requires-Dist: ebooklib
 Requires-Dist: genanki~=0.13.0
 Requires-Dist: jieba~=0.42.1
+Requires-Dist: pandas
+Requires-Dist: pdfplumber~=0.11.0
 Requires-Dist: pinyin~=0.4.0
+Requires-Dist: pydub
 Requires-Dist: requests~=2.31.0
 Requires-Dist: wordfreq
 
 # autoanki
 Tool for generating Chinese flashcards for Anki
 
 ![PyPI - Version](https://img.shields.io/pypi/v/autoanki)
```

### Comparing `autoanki-1.2.0/README.md` & `autoanki-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `autoanki-1.2.0/setup.cfg` & `autoanki-1.2.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = autoanki
-version = 1.2.0
+version = 1.2.1
 author = Jarvis Coghlin
 author_email = jarviscoghlin@gmail.com
 description = Automatically make Anki Decks for Chinese text
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/timmy6figures/autoanki
 project_urls = 
@@ -20,17 +20,21 @@
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.10
 install_requires = 
 	chinese-converter>=1.1.1
 	beautifulsoup4~=4.12.2
+	ebooklib
 	genanki~=0.13.0
 	jieba~=0.42.1
+	pandas
+	pdfplumber~=0.11.0
 	pinyin~=0.4.0
+	pydub
 	requests~=2.31.0
 	wordfreq
 
 [options.packages.find]
 where = src
 
 [egg_info]
```

### Comparing `autoanki-1.2.0/src/autoanki/AutoAnki.py` & `autoanki-1.2.1/src/autoanki/AutoAnki.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 import logging
+import pandas as pd
+import pdfplumber
+import os
+import ebooklib
+from ebooklib import epub
+from bs4 import BeautifulSoup
 
 from autoanki.BookCleaner import BookCleaner
 from autoanki.DatabaseManager import ChineseDatabaseManager
 from autoanki.DatabaseManager.DatabaseManager import DatabaseManager
 from autoanki.Dictionary import CEDictionary
 from autoanki.DeckManager import DeckManager
 from autoanki.Dictionary.Dictionary import Dictionary
@@ -81,14 +87,15 @@
 
         # self.book_cleaner = BookCleaner(debug_level, self.force)
 
         start = time.time()
         self.logger.info("Loading dictionary...")
         if dictionary:
             self.logger.info("Using custom dictionary")
+            self.dictionary = dictionary
         else:
             self.dictionary = CEDictionary(debug_level)
         end = time.time()
         self.logger.info(f"Done in {end - start:0.4f} seconds")
 
         self.database_filepath = database_filepath
         if database_filepath == "":
@@ -119,98 +126,209 @@
         total_end = time.time()
         self.logger.info(
             f"===== {GREEN}Done loading profile in {total_end - total_start:0.4f} seconds {RESET}====="
         )
 
     def add_book_from_string(self, contents: str, book_name: str = "Book Name"):
         """
-        Add a directory full of files to the database
+        Add a book as a string to the database
         Args:
-            `contents`: path to the directory that contains the files to add
+            `contents`: the contents of the book
             `book_name`: The name of the book being added e.g. "Lost Prince"
         """
         self.logger.debug(f"autoanki: Adding book [{book_name}] from string")
         if not contents:
             self.logger.info(f"No contents supplied")
             return
 
+        # TODO Handle pdfs in file
+        # TODO Restructure so each file can be passed to database_manager and still get added to the same book
+
         # Add the book to the database
         if not self.database_manager.add_book_from_string(contents, book_name):
             self.logger.warning("Unable to add [" + book_name + "] to database.")
             return
 
         self.logger.info("autoanki: Added book from string.")
 
     def add_book_from_file(self, filepath: str, book_name: str = "Book Name"):
-        """
-        Add a directory full of files to the database
+        """Add a file to the database
         Args:
             `filepath`: path to the directory that contains the files to add
             `book_name`: The name of the book being added e.g. "Lost Prince"
         """
         self.logger.debug(
             f"autoanki: Adding book [{book_name}] from file: [{filepath}]"
         )
         if not filepath:
             self.logger.info(f"No filepath supplied")
             return
+        # pip3 install pdfplumber
+
+        # Handle pdf
+        extension = os.path.splitext(filepath)[1]
+
+        if extension == ".pdf":
+            self.logger.info(f"PDF detected")
+            # for every page
+            print(filepath)
+            print(os.path.exists(filepath))
+
+            with pdfplumber.open(filepath) as pdf:
+                print(pdf)
+                for pages in pdf.pages:
+                    print(pages.pages)
+                    print(pages.extract_text())
+                    if not self.database_manager.add_book_from_string(
+                        pages.extract_text(), book_name
+                    ):
+                        self.logger.warning(
+                            "Unable to add [" + book_name + "] to database."
+                        )
+                        return
+        elif extension == ".epub":
+            book = epub.read_epub(filepath)
+            # Get the chapters
+            chapters = ""
+            for html_element in book.get_items_of_type(ebooklib.ITEM_DOCUMENT):
+                self.logger.info(html_element)
+                chapters += str(html_element.get_content(), "utf-8")
+            blacklist = [
+                "[document]",
+                "noscript",
+                "header",
+                "html",
+                "meta",
+                "head",
+                "input",
+                "script",
+            ]
+            # These come out as html, so convert to text
+            contents = ""
+            soup = BeautifulSoup(chapters, "html.parser")
+            text = soup.get_text()
+
+            text = soup.find_all(text=True)
+            for t in text:
+                if t.parent.name not in blacklist:
+                    contents += "{} ".format(t)
+            if not self.database_manager.add_book_from_string(contents, book_name):
+                self.logger.warning("Unable to add [" + book_name + "] to database.")
+                return
+        elif extension == ".txt":
+            self.logger.info(f"txt detected")
+            # Add the book to the database
+            if not self.database_manager.add_book_from_file(filepath, book_name):
+                self.logger.warning("Unable to add [" + book_name + "] to database.")
+                return
+
+        self.logger.info("autoanki: Added [" + filepath + "].")
+
+    def add_book_from_folder(self, directory: str, book_name: str = "Book Name"):
+        """
+        Add a directory full of files to the database
+        Args:
+            `filepath`: path to the directory that contains the files to add
+            `book_name`: The name of the book being added e.g. "Lost Prince"
+        """
+        self.logger.debug(
+            f"autoanki: Adding book [{book_name}] from directory: [{directory}]"
+        )
+        if not directory:
+            self.logger.info(f"No directory supplied")
+            return
 
         # Add the book to the database
-        if not self.database_manager.add_book_from_file(filepath, book_name):
+        if not self.database_manager.add_book_from_folder(directory, book_name):
             self.logger.warning("Unable to add [" + book_name + "] to database.")
             return
 
-        self.logger.info("autoanki: Added [" + filepath + "].")
+        self.logger.info("autoanki: Added [" + directory + "].")
+
+    def add_book_from_pleco(self, filepath: str, book_name: str):
+        """Reads the contents of a Pleco export file (txt, not xml)
+        Args:
+            `filepath`: path to the directory that contains the files to add
+            `book_name`: The name of the book being added e.g. "Lost Prince"
+        """
+        self.logger.debug(
+            f"autoanki: Adding book [{book_name}] from pleco: [{filepath}]"
+        )
+        if not filepath:
+            self.logger.info(f"No filepath supplied")
+            return
+
+        with open(filepath, "r") as file:
+            contents = file.read()
+            for line in file.readlines():
+                split_line = line.split(" ")
+                if split_line:
+                    contents += split_line[0]
+
+        contents = ""
+        self.logger.debug(f"Done reading Pleco. len: {len(contents)}")
+        self.database_manager.add_book_from_string(contents, book_name)
 
     def complete_unfinished_definitions(self):
         """
         autoanki contains an internal definitions table that is scraped from the internet. As words are added to
         autoanki, their definitions must be found.
         This function finds definitions and adds them to the table
         """
+        start = time.time()
         self.logger.info("Checking for records...")
-        self.database_manager.cursor.execute(
-            "SELECT word FROM dictionary WHERE definition IS NULL"
-        )
-        response_rows = self.database_manager.cursor.fetchall()
+        response_rows = self.database_manager.unfinished_definitions()
         if len(response_rows) == 0:
             self.logger.info("No new rows to complete in dictionary table")
             return
 
         self.logger.info(
             "Adding " + str(len(response_rows)) + " rows to dictionary table"
         )
         self.tokenizer = ChineseTokenizer(dictionary=self.dictionary)
         for row in response_rows:
             word = str(row[0])
 
             # self.logger.debug(f"Finding: [{word}]")
             # self.logger.debug("Trying local dictionary...")
             params = self.dictionary.find_word(word)
+            # self.logger.info(params)
             if params:
                 # self.logger.debug(f"✅Found: [{params[8]}]")
                 self.database_manager.update_definition(params)
                 continue
 
             self.logger.info(f"❌Could not find: [{word}]")
+        end = time.time()
+        self.logger.info(
+            f"Finished collecting definitions in {end - start:0.4f} seconds"
+        )
 
     def deck_settings(
         self,
-        inclue_traditional=True,
-        inclue_part_of_speech=True,
+        include_traditional=True,
+        include_part_of_speech=True,
+        include_audio=False,
+        include_pinyin=True,
+        include_zhuyin=False,
+        hsk_filter=None,
         word_frequency_filter=None,
     ):
         """Configures settings for what's in the deck, and how it looks"
 
         `word_frequency_filter`: Float between 0 and 1. 1 being every word is included, 0 being none are included
         """
         self.deck_manager.settings(
-            inclue_traditional,
-            inclue_part_of_speech,
-            word_frequency_filter,
+            include_traditional=include_traditional,
+            include_pinyin=include_pinyin,
+            include_zhuyin=include_zhuyin,
+            include_part_of_speech=include_part_of_speech,
+            include_audio=include_audio,
+            word_frequency_filter=word_frequency_filter,
+            hsk_filter=hsk_filter,
         )
 
     def print_database_info(self):
         self.database_manager.print_info()
 
     @staticmethod
     def is_database(db_path):
@@ -235,14 +353,25 @@
         if deck_path is None:
             self.logger.warning(
                 "Was not able to create deck file for [", deck_name, "]"
             )
         else:
             self.logger.info("Generated deck file [" + deck_path + "]")
 
+    def save_dictionary_as_csv(self, filepath: str):
+        self.logger.info("Saving to csv...")
+        all = self.database_manager.get_all_definitions()
+        # pprint(all)
+
+        df = pd.DataFrame(all)
+        headers = self.database_manager.get_columns()
+        df.columns = headers
+        df.to_csv(filepath)
+        self.logger.info("Done saving to csv...")
+
     @property
     def book_list(self):
         """
         Get a list of the books in the database
         :return: List of book names
         """
         return self.database_manager.books
```

### Comparing `autoanki-1.2.0/src/autoanki/BookCleaner/BookCleaner.py` & `autoanki-1.2.1/src/autoanki/BookCleaner/BookCleaner.py`

 * *Files identical despite different names*

### Comparing `autoanki-1.2.0/src/autoanki/DatabaseManager/ChineseDatabaseManager.py` & `autoanki-1.2.1/src/autoanki/DatabaseManager/ChineseDatabaseManager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import sqlite3
 import logging
+from glob import glob
 
 from pathlib import Path
 
 from autoanki.Tokenizer.ChineseTokenizer import ChineseTokenizer
 from autoanki.DatabaseManager.DatabaseManager import DatabaseManager
 
 
@@ -174,16 +175,19 @@
         if len(all_rows) == 0:
             # self.logger.info("  Inserting")
             self.cursor.execute(f"INSERT INTO dictionary (word) VALUES (?)", [word])
             self.connection.commit()
 
     def remove_word(self, word: str):
         # TODO: Make more stringent constraints on removing words. This should be extremely rare
+        if len(word) > 10:
+            self.logger.warning(f"Not executing: [{word}]. Suspiciously large")
+            return
         if "*" in word:
-            self.logger.info(f"Not executing: [{word}]. Star in command")
+            self.logger.warning(f"Not executing: [{word}]. Star in command")
             return
         self.cursor.execute(f"DELETE FROM dictionary WHERE word=(?)", [word])
         self.connection.commit()
 
     def add_book_from_string(self, contents: str, book_name: str) -> bool:
         return self._add_book(contents, book_name)
 
@@ -192,25 +196,38 @@
             self.logger.info(f"File does not exist: [{filepath}]")
             return False
 
         with open(filepath, "r") as file:
             contents = file.read()
             return self._add_book(contents, book_name)
 
-    # def add_book_from_folder(directory):
-    # TODO This
+    def add_book_from_folder(self, directory: str, book_name: str) -> bool:
+        """Adds a book from a folder full of files
+        Only opens any .txt files in the subdirectory
+        """
+        self.logger.info(f"Adding folder [{directory}] to database")
+
+        # Read all files into a string, and use to add from string
+        all_files_contents = ""
 
-    # Legacy code from _add_book()
-    # self.logger.debug("Bookpath: " + filepath)
-    # if os.path.isdir(filepath):
-    #     self.logger.debug("Directory found:")
-    #     result = [y for x in os.walk(filepath + '/' + CLEANED_FILES_DIRECTORY) for y in glob(os.path.join(x[0], '*.txt'))]
-    #     for path in result:
-    #         self.logger.debug(path)
-    #         self.add_file_to_database(path, book_tablename)
+        self.logger.debug("Bookpath: " + directory)
+        if os.path.isdir(directory):
+            self.logger.debug("Directory found:")
+            text_files = [
+                y for x in os.walk(directory) for y in glob(os.path.join(x[0], "*.txt"))
+            ]
+            for path in text_files:
+                self.logger.debug(path)
+                # Open and append to string
+                with open(path) as f:
+                    contents = f.read()
+                    all_files_contents += contents
+
+        self.add_book_from_string(all_files_contents, book_name)
+        return True
 
     def _add_book(self, contents: str, book_name: str) -> bool:
         """Adds a file to the autoanki database.
         This involves the following steps:\n
         1 - Add book to the `book_list` table
         2 - Add all the files in "bookpath" to the definitions table and book table
         Args:
@@ -228,14 +245,37 @@
 
         # Add all the words in the book to the `definitions` table
         self.add_contents_to_database(contents, book_tablename)
 
         self.logger.info("Done adding book.")
         return True
 
+    def get_columns(self) -> list:
+
+        return [
+            "word_id",
+            "word",
+            "word_traditional",
+            "pinyin",
+            "pinyin_numbers",
+            "zhuyin",
+            "jyutping",
+            "part_of_speech",
+            "number_of_strokes",
+            "sub_components",
+            "definition",
+            "frequency",
+            "hsk_level",
+            "tocfl_level",
+            "audio_path",
+            "image_path",
+            "character_graphic",
+            "examples",
+        ]
+
     def print_info(self):
         """Print basic information about the database"""
         self.cursor.execute("SELECT word FROM dictionary")
         all_rows = self.cursor.fetchall()
         self.cursor.execute("SELECT word FROM dictionary WHERE definition IS NULL")
         unfinished_rows = self.cursor.fetchall()
         format_string_int = "{:<30} | {:>8}"
@@ -252,82 +292,98 @@
         )
         print("Dictionary Table:")
         print(format_string_int.format("Number of rows:", len(all_rows)))
         print(
             format_string_int.format("Number of unfinished rows:", len(unfinished_rows))
         )
 
-    def update_definition(self, params: list):
+    def update_definition(self, params: dict[str, str]):
+        """ """
         f"""Complete a definition for one word in the dictionary table\n
-        traditional_script = params[0]\n
-        word_type = params[1]\n
-        pinyin = params[2]\n
-        pinyin_numbers = params[3]\n
-        sub_components = params[4]\n
-        hsk_level = params[5]\n
-        top_level = params[6]\n
-        definition = params[7]\n
-        frequency = params[8]
-        word = params[9]
+		Here is all of the fields that a card could have:
+			word
+			word traditional 
+			pinyin
+			pinyin numbers
+			zhuyin
+			jyutping
+			part of speech
+			number of strokes
+			sub components
+			definition
+			frequency
+			HSK level
+			tocfl level
+			audio path
+			image path
+			stroke order graphic
+			examples
         :param params: A list of params for the database:
         :return:
         """
-        # TODO Some sanatization here might be a good idea
-        #   Make sure junk data can't crash this function
-        self.cursor.execute(
-            "UPDATE dictionary "
-            "SET word_traditional = ?, "
-            "word_type = ?,"
-            "pinyin = ?, "
-            "pinyin_numbers = ?,"
-            "sub_components = ?,"
-            "hsk_level = ?,"
-            "top_level = ?,"
-            "definition = ?,"
-            "frequency = ?"
-            "WHERE word = ?",
-            params,
-        )
-        self.connection.commit()
 
-    def get_all_completed_definitions(self):
+        try:
+            self.cursor.execute(
+                "UPDATE dictionary SET "
+                "word_traditional = ?,"
+                "pinyin = ?,"
+                "pinyin_numbers = ?,"
+                "zhuyin = ?,"
+                "jyutping = ?,"
+                "part_of_speech = ?,"
+                "number_of_strokes = ?,"
+                "sub_components = ?,"
+                "definition = ?,"
+                "frequency = ?,"
+                "HSK_level = ?,"
+                "tocfl_level = ?,"
+                "audio_path = ?,"
+                "image_path = ?,"
+                "character_graphic= ?,"
+                "examples = ?"
+                "WHERE word = ?",
+                [
+                    params.get("word_traditional"),
+                    params.get("pinyin"),
+                    params.get("pinyin_numbers"),
+                    params.get("zhuyin"),
+                    params.get("jyutping"),
+                    params.get("part_of_speech"),
+                    params.get("number_of_strokes"),
+                    params.get("sub_components"),
+                    params.get("definition"),
+                    params.get("frequency"),
+                    params.get("HSK_level"),
+                    params.get("tocfl_level"),
+                    params.get("audio_path"),
+                    params.get("image_path"),
+                    params.get("character_graphic"),
+                    params.get("examples"),
+                    params.get("word"),
+                ],
+            )
+            self.connection.commit()
+        except Exception as e:
+            self.logger.error(f"Error updating database definition. Params:\n {params}")
+            self.logger.error(f"Error: {e}")
+
+    def get_all_definitions(self):
+        self.cursor.execute("SELECT * FROM dictionary")
+        words = self.cursor.fetchall()
+        return words
 
+    def get_all_completed_definitions(self):
         self.cursor.execute("SELECT * FROM dictionary WHERE definition IS NOT NULL")
-        raw_words = self.cursor.fetchall()
-
-        # pprint.pp(raw_words)
-        words = []
-        for row in raw_words:
-            word = {
-                "word_id": row[0],
-                "word": row[1],
-                "word_traditional": row[2],
-                "word_type": row[3],
-                "pinyin": row[4],
-                "pinyin_numbers": row[5],
-                "number_of_strokes": row[6],
-                "sub_components": row[7],
-                "frequency": row[8],
-                "hsk_level": row[9],
-                "top_level": row[10],
-                "audio_path": row[11],
-                "image_path": row[12],
-                "definition": row[13],
-            }
-            # print(word["word"])
-            # pprint.pp(word)
-            # words.append(word)
-            words.append(word)
-        # pprint.pp(words)
+        words = self.cursor.fetchall()
         return words
 
-    def unfinished_definitions(self) -> int:
-        self.cursor.execute("SELECT word FROM dictionary WHERE definition IS NULL")
+    def unfinished_definitions(self, column: str = "definition"):
+        self.cursor.execute(f"SELECT word FROM dictionary WHERE {column} IS NULL")
         unfinished_rows = self.cursor.fetchall()
-        return len(unfinished_rows)
+        return unfinished_rows
 
     @property
     def books(self):
         connection = sqlite3.connect(self.database_path)
         cursor = connection.cursor()
         cursor.execute("SELECT book_name FROM book_list")
         return_array = []
```

### Comparing `autoanki-1.2.0/src/autoanki/DatabaseManager/DatabaseManager.py` & `autoanki-1.2.1/src/autoanki/DatabaseManager/DatabaseManager.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,18 @@
         return True
 
     @staticmethod
     def create_database(database_path: str) -> bool:
         pass
 
     @abstractmethod
+    def get_columns(self) -> list:
+        pass
+
+    @abstractmethod
     def print_info(self):
         pass
 
     @abstractmethod
     def add_contents_to_database(self, contents: str, table_name: str):
         pass
 
@@ -56,13 +60,13 @@
         pass
 
     @abstractmethod
     def add_book_from_file(self, filepath: str, book_name: str) -> bool:
         pass
 
     @abstractmethod
-    def update_definition(self, params: list):
+    def update_definition(self, params: dict[str, str]):
         pass
 
     @abstractmethod
     def get_all_completed_definitions(self) -> list:
         pass
```

### Comparing `autoanki-1.2.0/src/autoanki/DatabaseManager/databases_init.sql` & `autoanki-1.2.1/src/autoanki/DatabaseManager/databases_init.sql`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,56 @@
+-- Here is all of the fields that a card could have:
+-- word
+-- word traditional 
+-- pinyin
+-- pinyin numbers
+-- zhuyin
+-- jyutping 
+-- part of speech
+-- number of strokes
+-- sub components
+-- definition
+-- frequency
+-- HSK level
+-- tocfl level
+-- audio path
+-- image path
+-- character graphic
+-- examples
+
 CREATE TABLE IF NOT EXISTS dictionary(
 	word_id INTEGER PRIMARY KEY AUTOINCREMENT,
 	word VARCHAR(255) NOT NULL UNIQUE,
 	word_traditional VARCHAR(255),
-	word_type VARCHAR(255),
 	pinyin VARCHAR(255),
 	pinyin_numbers VARCHAR(255),
+	zhuyin VARCHAR(255),
+	jyutping VARCHAR(255),
+	part_of_speech VARCHAR(255),
 	number_of_strokes INTEGER,
 	sub_components VARCHAR(255),
+	definition VARCHAR(255),
 	frequency FLOAT,
 	hsk_level VARCHAR(255),
-	top_level VARCHAR(255),
+	tocfl_level VARCHAR(255),
 	audio_path VARCHAR(255),
 	image_path VARCHAR(255),
-	definition VARCHAR(255)
+	character_graphic VARCHAR(255),
+	examples VARCHAR(255)
 );
 
+
 CREATE TABLE IF NOT EXISTS book_list(
     book_name VARCHAR(255),
     table_name VARCHAR(255),
     language VARCHAR(100)
 );
 
 
 --In the future make is so that BOTH have to be unique
 --ALTER TABLE definitions
 --ADD CONSTRAINT UQ_word_pinyin UNIQUE(word, pinyin)
 
 
 --Select b.dictionary_word_id, d.word, d.word_traditional, d.word_type, d.pinyin, d.pinyin_numbers, d.hsk_level, d.definition
 --FROM book_table b
---INNER JOIN dictionary d ON b.dictionary_word_id = d.word_id
+--INNER JOIN dictionary d ON b.dictionary_word_id = d.word_id
```

### Comparing `autoanki-1.2.0/src/autoanki/DeckManager/template_decks.py` & `autoanki-1.2.1/src/autoanki/DeckManager/template_decks.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,36 +13,62 @@
             "font": "Arial",
         },
         {
             "name": "pinyin",
             "font": "Arial",
         },
         {
+            "name": "audio",
+            "font": "Arial",
+        },
+        {
+            "name": "zhuyin",
+            "font": "Arial",
+        },
+        {
             "name": "part_of_speech",
             "font": "Arial",
             "color": "red",
         },
         {
             "name": "definition",
             "font": "Arial",
         },
     ],
     templates=[
         {
             "name": "Card 1",
             "qfmt": "{{word}}\n[{{word_traditional}}]",
-            "afmt": """{{FrontSide}}\n\n<hr id=answer>\n{{pinyin}}<br><br><span style="color:gray">{{part_of_speech}}</span>{{definition}}<br>""",
+            "afmt": """
+            {{FrontSide}}\n
+            \n
+            <hr id=answer>\n
+            {{pinyin}}
+            {{audio}}
+            {{zhuyin}}
+            <br>
+            <br>
+            <span style="color:gray">{{part_of_speech}}</span>
+            {{definition}}<br>
+            """,
         },
         # {
         # 'name': 'Card 2',
         # 'qfmt': '{{FrontSide}}\n\n<hr id=answer>\n{{Pinyin}}\n{{Back}}',
         # 'afmt': '{{Front}}',
         # },
     ],
-    css=".card {\n font-family: arial;\n font-size: 30px;\n text-align: center;\n color: black;\n background-color: white;\n}\n",
+    css="""
+    .card { \n 
+    font-family: arial; \n 
+    font-size: 30px;\n 
+    text-align: center;\n 
+    color: black;\n 
+    background-color: white;\n
+    }\n""",
 )
 
 # # All the resources for finding the
 #         CHINESE_CARD_MODEL = Model(
 #             1559383145,
 #             'Chinese Card (autoanki)',
 #             fields=[
```

### Comparing `autoanki-1.2.0/src/autoanki/Dictionary/.DS_Store` & `autoanki-1.2.1/src/autoanki/Dictionary/.DS_Store`

 * *Files identical despite different names*

### Comparing `autoanki-1.2.0/src/autoanki/Dictionary/CEDictionary.py` & `autoanki-1.2.1/src/autoanki/Dictionary/CEDictionary.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,22 +94,26 @@
                         "definition": "",
                         "pinyin": "",
                         "frequency": "",
                     }
 
                 # These only need to be done the first time the word is seen
                 if last_word != current_word:
-                    definitions[current_word]["trad_word"] = trad_word
+                    definitions[current_word]["traditional_word"] = trad_word
                     definitions[current_word]["pinyin"] = pinyin.get(current_word)
                     definitions[current_word]["pinyin_numbers"] = pinyin.get(
                         current_word, format="numerical"
                     )
                     definitions[current_word]["frequency"] = str(
                         100 * word_frequency(current_word, "zh")
                     )
+                    slice = next(pseg.cut(current_word))
+                    definitions[current_word][
+                        "part_of_speech"
+                    ] = self.get_part_of_speech(current_word, slice.flag)
 
                 definitions[current_word]["definition"] += "<br>" + definition
                 last_word = current_word
 
         for key, _ in definitions.items():
             definitions[key]["definition"].strip("\n")
             definitions[key]["definition"] = definitions[key]["definition"].lstrip(
@@ -118,51 +122,48 @@
             definitions[key]["definition"] = definitions[key]["definition"].lstrip("/")
 
             definitions[key]["definition"] = definitions[key]["definition"].rstrip("\n")
             definitions[key]["definition"] = definitions[key]["definition"].rstrip("/")
             # self.logger.info('[' + definitions[key]['definition'] + ']')
         return definitions
 
-    def find_word(self, word: str) -> None | list[str]:
+    def find_word(self, word: str) -> None | dict[str, str]:
         """
         Find a word in the dictionary. This can be simplified, or traditional
         `return` Paramaters that get passed to the database
         """
         # Convert the word to simplified if needed
+        # TODO: This should happen during load, not runtime
         word = chinese_converter.to_simplified(word)
         # self.logger.info(f"[{word}] [{word in self.dict}]")
-        if not word in self.dict:
+        word_found = self.dict.get(word)
+        if not word_found:
             return None
 
-        """
-        traditional_script = params[0]\n
-        word_type = params[1]\n
-        pinyin = params[2]\n
-        pinyin_numbers = params[3]\n
-        sub_components = params[4]\n
-        hsk_level = params[5]\n
-        top_level = params[6]\n
-        definition = params[7]\n
-        frequency = params[8]
-        word = params[9]
-        """
-        params = ["", "", "", "", "", "", "", "", "", ""]
+        params = {}
+
+        params["word"] = word
+        params["word_traditional"] = word_found["traditional_word"]
+        params["pinyin"] = word_found["pinyin"]
+        params["pinyin_numbers"] = word_found["pinyin_numbers"]
+        params["zhuyin"] = None
+        params["jyutping"] = None
+        params["part_of_speech"] = word_found["part_of_speech"]
+        params["number_of_strokes"] = None
+        params["sub_components"] = None
+        params["definition"] = word_found["definition"]
+        params["frequency"] = word_found["frequency"]
+        params["HSK_level"] = None
+        params["tocfl_level"] = None
+        params["audio_path"] = None
+        params["image_path"] = None
+        params["character_graphic"] = None
+        params["examples"] = None
 
-        slice = next(pseg.cut(word))
-        part_of_speech = self.get_part_of_speech(word, slice.flag)
-        if part_of_speech != None:
-            params[1] = part_of_speech
-
-        params[0] = self.dict[word]["trad_word"]
-        params[2] = self.dict[word]["pinyin"]
-        params[3] = self.dict[word]["pinyin_numbers"]
-        params[7] = self.dict[word]["definition"]
         # self.logger.debug(f"Word: {word}")
-        params[8] = self.dict[word]["frequency"]
-        params[9] = word
         return params
 
     def size(self):
         with open(PATH_TO_FILE, "r") as f:
             return len(f.readlines())
 
     def get_part_of_speech(self, word: str, code: str) -> str:
```

### Comparing `autoanki-1.2.0/src/autoanki/Dictionary/cedict_ts.u8` & `autoanki-1.2.1/src/autoanki/Dictionary/cedict_ts.u8`

 * *Files identical despite different names*

### Comparing `autoanki-1.2.0/src/autoanki/Tokenizer/ChineseTokenizer.py` & `autoanki-1.2.1/src/autoanki/Tokenizer/ChineseTokenizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from string import punctuation
 
 
 # TODO Is there a way to do this in a smarter way? Maybe check if the characters are in a certian UTF-8 block?
 PUNCTUATION = """
 +,;:'()[]{}&*^%$#@!◇♦•·■◎∞=™©×
 """
-CHINESE_PUNC = "！？｡。．.…、＂＃＄％＆＇（）＊＋，－／：；＜＝＞＠［＼］＾＿｀｛｜｝～｟｠｢｣､、〃《》「」『』【】〔〕〖〗〘〙〚〛〜〝〞〟〰〾〿–—‘’‛“”„‟…‧﹏  ① ② ③ ④ ⑽ "
+CHINESE_PUNC = "　！？｡。．.…、＂＃＄％＆＇（）＊＋，－／：；＜＝＞＠［＼］＾＿｀｛｜｝～｟｠｢｣､、〃《》「」『』【】〔〕〖〗〘〙〚〛〜〝〞〟〰〾〿–—‘’‛“”„‟…‧﹏  ① ② ③ ④ ⑽ "
 
 # TODO: This can be extened and implemented
 OTHER = "ｗ９ｌｉｔｂｎｅｐｈⅠ Ⅱ Ⅲ Ⅳ "
 
 # TODO Remove straight numbers and english words
 
 
@@ -55,15 +55,15 @@
                     continue
                 if word in OTHER:
                     continue
 
             # If there is a definition in the dictionary, skip any more processing
             if not word:
                 continue
-            if self.dictionary.find_word(word):
+            if self.dictionary.find_word(word).get("definition"):
                 clean_words.append(word)
                 continue
 
             # Try tokenizing again?
             subwords = jieba.lcut(word)
             if len(subwords) > 1:
                 for subword in subwords:
@@ -73,39 +73,39 @@
             # Remove all ascii
             new_word = "".join(i for i in word if ord(i) > 128)
             # if word != new_word:
             # self.logger.info(f"{word} -> {new_word}", )
             word = new_word
             if not word:
                 continue
-            if self.dictionary.find_word(word):
+            if self.dictionary.find_word(word).get("definition"):
                 clean_words.append(word)
                 continue
 
             word = self.remove_modifiers(word)
             if not word:
                 continue
-            if self.dictionary.find_word(word):
+            if self.dictionary.find_word(word).get("definition"):
                 clean_words.append(word)
                 continue
 
             word = self.remove_numbers(word)
             if not word:
                 continue
-            if self.dictionary.find_word(word):
+            if self.dictionary.find_word(word).get("definition"):
                 clean_words.append(word)
                 continue
 
             # Repeated characters (always?) contain the same meaning as one, just varied slightly
             # 人人 = everyone
             if len(word) == 2 and word[0] == word[1]:
                 word = word[0]
             if not word:
                 continue
-            if self.dictionary.find_word(word):
+            if self.dictionary.find_word(word).get("definition"):
                 clean_words.append(word)
                 continue
 
             # TODO 2 repeated, 1?
             #   点点头
             #   长长的
             # TODO 的 at the end?
@@ -122,21 +122,21 @@
             if len(word) == 3:
                 clean_words.append(word[0])
                 clean_words.append(word[1])
                 clean_words.append(word[2])
                 continue
 
             if len(word) == 4:
-                if self.dictionary.find_word(word[0:1]):
+                if self.dictionary.find_word(word[0:1]).get("definition"):
                     clean_words.append(word[0:1])
                 else:
                     clean_words.append(word[0])
                     clean_words.append(word[1])
 
-                if self.dictionary.find_word(word[2:3]):
+                if self.dictionary.find_word(word[2:3]).get("definition"):
                     clean_words.append(word[2:3])
                 else:
                     clean_words.append(word[2])
                     clean_words.append(word[3])
                 continue
 
             if len(word) == 5:
```

### Comparing `autoanki-1.2.0/src/autoanki.egg-info/PKG-INFO` & `autoanki-1.2.1/src/autoanki.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: autoanki
-Version: 1.2.0
+Version: 1.2.1
 Summary: Automatically make Anki Decks for Chinese text
 Home-page: https://github.com/timmy6figures/autoanki
 Author: Jarvis Coghlin
 Author-email: jarviscoghlin@gmail.com
 Project-URL: Bug Tracker, https://github.com/timmy6figures/autoanki/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: chinese-converter>=1.1.1
 Requires-Dist: beautifulsoup4~=4.12.2
+Requires-Dist: ebooklib
 Requires-Dist: genanki~=0.13.0
 Requires-Dist: jieba~=0.42.1
+Requires-Dist: pandas
+Requires-Dist: pdfplumber~=0.11.0
 Requires-Dist: pinyin~=0.4.0
+Requires-Dist: pydub
 Requires-Dist: requests~=2.31.0
 Requires-Dist: wordfreq
 
 # autoanki
 Tool for generating Chinese flashcards for Anki
 
 ![PyPI - Version](https://img.shields.io/pypi/v/autoanki)
```

### Comparing `autoanki-1.2.0/src/autoanki.egg-info/SOURCES.txt` & `autoanki-1.2.1/src/autoanki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autoanki-1.2.0/tests/test_AutoAnki.py` & `autoanki-1.2.1/tests/test_AutoAnki.py`

 * *Files identical despite different names*

