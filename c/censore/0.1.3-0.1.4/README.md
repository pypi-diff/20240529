# Comparing `tmp/censore-0.1.3.tar.gz` & `tmp/censore-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censore-0.1.3.tar", last modified: Tue May 21 05:52:28 2024, max compression
+gzip compressed data, was "censore-0.1.4.tar", last modified: Wed May 29 13:41:28 2024, max compression
```

## Comparing `censore-0.1.3.tar` & `censore-0.1.4.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:28.902911 censore-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 05:52:23.000000 censore-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-21 05:52:23.000000 censore-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-21 05:52:28.902911 censore-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 05:52:23.000000 censore-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:28.898911 censore-0.1.3/censore/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-21 05:52:23.000000 censore-0.1.3/censore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-05-21 05:52:23.000000 censore-0.1.3/censore/censor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:28.894911 censore-0.1.3/censore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:28.902911 censore-0.1.3/censore/data/list/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/ar.txt
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/cs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/da.txt
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/de.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20314 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/en.txt
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/eo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/es.txt
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/fa.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/fi.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/fil.txt
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/fr.txt
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/hi.txt
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/hu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/it.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/ja.txt
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/ko.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/nl.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/no.txt
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/pl.txt
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/pt.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/ru.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/sv.txt
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/th.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/tr.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/uk.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-21 05:52:24.000000 censore-0.1.3/censore/data/list/zh.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:28.902911 censore-0.1.3/censore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-21 05:52:28.000000 censore-0.1.3/censore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-21 05:52:28.000000 censore-0.1.3/censore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 05:52:28.000000 censore-0.1.3/censore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 05:52:28.000000 censore-0.1.3/censore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-21 05:52:28.902911 censore-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-21 05:52:23.000000 censore-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:41:28.907460 censore-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-29 13:41:21.000000 censore-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-29 13:41:21.000000 censore-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-29 13:41:28.907460 censore-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 13:41:21.000000 censore-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:41:28.903460 censore-0.1.4/censore/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-29 13:41:21.000000 censore-0.1.4/censore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-05-29 13:41:21.000000 censore-0.1.4/censore/censor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:41:28.899460 censore-0.1.4/censore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:41:28.907460 censore-0.1.4/censore/data/list/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/ar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/cs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/da.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/de.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20314 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/en.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/eo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/es.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/fa.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/fi.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/fil.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/fr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/hi.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/hu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/it.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/ja.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/ko.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/nl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/no.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/pl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/pt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/ru.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/sv.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/th.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/tr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/uk.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-29 13:41:21.000000 censore-0.1.4/censore/data/list/zh.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:41:28.907460 censore-0.1.4/censore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-29 13:41:28.000000 censore-0.1.4/censore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-29 13:41:28.000000 censore-0.1.4/censore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:41:28.000000 censore-0.1.4/censore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 13:41:28.000000 censore-0.1.4/censore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-29 13:41:28.907460 censore-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-29 13:41:21.000000 censore-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:41:28.907460 censore-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:41:21.000000 censore-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-29 13:41:21.000000 censore-0.1.4/tests/test.py
```

### Comparing `censore-0.1.3/LICENSE` & `censore-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `censore-0.1.3/censore/censor.py` & `censore-0.1.4/censore/censor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,119 +1,221 @@
 import os
 from typing import List, Dict, Optional
 
 
 class Censor:
-    def __init__(self, languages: List[str] = ["en"]) -> None:
+    # Substitution table for normalizing words
+
+    substitution_table = str.maketrans(
+        {
+            "0": "o",
+            "1": "i",
+            "@": "a",
+            "$": "s",
+            "3": "e",
+            "5": "s",
+            "7": "t",
+            "8": "b",
+        }
+    )
+
+    data_folder = os.path.join(os.path.dirname(__file__), "data/list")
+
+    def __init__(
+        self, languages: List[str] = ["en"], custom_words: Optional[List[str]] = None
+    ) -> None:
         """
         Initializes the Censor object by loading the appropriate profanity lists
         for the specified languages.
 
         :param languages: List of languages to load for censorship. If "all", loads all available languages.
         """
         self.languages: List[str] = []
         self.profanity_list: Dict[str, List[str]] = {}
-        self.data_folder = "data/list"
-
-        # Substitution table for normalizing words
-        self.substitution_table = str.maketrans(
-            {
-                "0": "o",
-                "1": "i",
-                "@": "a",
-                "$": "s",
-                "3": "e",
-                "5": "s",
-                "7": "t",
-                "8": "b",
-            }
-        )
 
         # Load profanity lists for each language
         self._load_languages(languages)
 
-    def _load_languages(self, languages: List[str]) -> None:
+        if custom_words:
+            self.add_custom_words(custom_words)
+
+    def _load_languages(
+        self, languages: List[str], is_additional: bool = False
+    ) -> None:
         """
         Loads the list of profane words for the specified language(s) from files.
 
         :param languages: A list of languages to load for censorship. If "all", loads all available languages.
         :return: None
         """
         languages_for_loading = []
 
         # Load languages
         if "all" in languages:
             for filename in os.listdir(self.data_folder):
                 if filename.endswith(".txt"):
                     languages_for_loading.append(os.path.splitext(filename)[0])
-
         else:
             languages_for_loading = languages
 
         for language in languages_for_loading:
-            self._load_language(language)
+            self._load_language(language, is_additional)
 
-    def _load_language(self, language: str) -> None:
+    def _load_language(self, language: str, is_additional: bool = False) -> None:
         """
         Loads the list of profane words for the specified language from a file.
 
         :param language: The language for which to load the profanity list.
         """
 
         if language not in self.languages:
             path_to_list = os.path.join(self.data_folder, f"{language}.txt")
 
             with open(path_to_list, "r", encoding="utf-8") as file:
                 profanities = file.read().split()
 
             self.profanity_list[language] = profanities
+
+            if not is_additional:
+                self.languages.append(language)
+
+    def add_custom_words(
+        self, custom_words: List[str], language: str = "custom"
+    ) -> None:
+        """
+        Adds custom words to the profanity list.
+
+        :param custom_words: A list of custom words to add to the profanity list.
+        """
+
+        self.add_custom_lang(language, custom_words)
+
+    def add_custom_lang(self, language: str, custom_words: List[str]) -> None:
+        """
+        Adds custom words to the profanity list for the specified language.
+
+        :param language: The language for which to add the custom words.
+        :param custom_words: A list of custom words to add to the profanity list for the specified language.
+        """
+
+        if language not in self.profanity_list:
+            self.profanity_list[language] = []
+
+        self.profanity_list[language] = custom_words
+
+        if language not in self.languages:
             self.languages.append(language)
 
-    def _normalize_word(self, word: str) -> str:
+    @staticmethod
+    def _normalize_word(word: str) -> str:
         """
         Normalizes a word by substituting characters according to the substitution table
         and removing punctuation.
 
         :param word: The word to normalize.
         :return: The normalized word.
         """
-        return self._strip(word.translate(self.substitution_table)).lower()
+        return Censor._strip(word.translate(Censor.substitution_table)).lower()
 
-    def _strip(self, word: str) -> str:
+    @staticmethod
+    def _strip(word: str) -> str:
         """
         Strips punctuation from the beginning and end of a word.
 
         :param word: The word to strip.
         :return: The stripped word.
         """
         return word.strip(".,!?:;/()[]{}-")
 
     def contains_profanity(
-        self, string: str, languages: Optional[List[str]] = None
+        self,
+        text: str,
+        languages: Optional[List[str]] = None,
+        additional_languages: Optional[List[str]] = None,
+        custom_words: List[str] = [],
     ) -> bool:
         """
         Checks if the input string contains any profanity from the specified languages.
 
-        :param string: The input string to check for profanity.
+        :param text: The input string to check for profanity.
         :param languages: A list of languages to check for profanity. If "all", checks all available languages.
         :return: True if the string contains profanity, False otherwise.
         """
+
+        # Ensure all specified languages are loaded
+        active_languages = list(self.languages)  # Clone the current languages
+
+        if languages:
+            self._load_languages(languages)
+
+            if "all" in languages:
+                active_languages = self.languages
+            else:
+                active_languages = languages
+
+        if additional_languages:
+            self._load_languages(additional_languages, is_additional=True)
+            active_languages += additional_languages
+
+        lines = text.split("\n")
+
         # Ensure all specified languages are loaded
         if languages:
             self._load_languages(languages)
 
-            if languages == ["all"]:
+            if "all" in languages:
                 languages = self.languages
         else:
             languages = self.languages
 
-        for language in languages:
-            for profanity in self.profanity_list[language]:
-                if profanity in string:
-                    return True
+        for line in lines:
+            words = line.split(" ")
+
+            for language in active_languages:
+                for word in words:
+                    normalized_word = self._normalize_word(word)
+
+                    if (
+                        normalized_word in self.profanity_list.get(language, [])
+                        or normalized_word in custom_words
+                    ):
+                        return True
+
+        return False
+
+    def is_profane(
+        self,
+        word: str,
+        languages: Optional[List[str]] = None,
+        additional_languages: Optional[List[str]] = None,
+        custom_words: List[str] = [],
+    ) -> bool:
+        # Ensure all specified languages are loaded
+        active_languages = list(self.languages)  # Clone the current languages
+
+        if languages:
+            self._load_languages(languages)
+
+            if "all" in languages:
+                active_languages = self.languages
+            else:
+                active_languages = languages
+
+        if additional_languages:
+            self._load_languages(additional_languages, is_additional=True)
+            active_languages += additional_languages
+
+        for language in active_languages:
+            normalized_word = self._normalize_word(word)
+
+            if (
+                normalized_word in self.profanity_list.get(language, [])
+                or normalized_word in custom_words
+            ):
+                return True
 
         return False
 
     def censor_word(
         self, word: str, partial_censor: bool = False, censoring_char: str = "#"
     ) -> str:
         """
@@ -132,55 +234,61 @@
         else:
             return censoring_char * len(word)
 
     def censor_text(
         self,
         text: str,
         languages: Optional[List[str]] = None,
+        additional_languages: Optional[List[str]] = None,
+        custom_words: List[str] = [],
         partial_censor: bool = False,
         censoring_char: str = "#",
     ) -> str:
         """
         Censors an entire text, replacing profane words according to the specified languages.
 
         :param text: The text to censor.
         :param languages: The list of languages to use for censorship.
         :param partial_censor: Whether to partially censor the words.
         :param censoring_char: The character to use for censorship.
         :return: The censored text.
         """
 
-        # Split the text into lines to process each line separately
         lines = text.split("\n")
         censored_lines = []
 
+        active_languages = list(self.languages)  # Clone the current languages
+
         if languages:
-            # Ensure all specified languages are loaded
             self._load_languages(languages)
 
-            if languages == ["all"]:
-                languages = self.languages
-        else:
-            languages = self.languages
+            if "all" in languages:
+                active_languages = self.languages
+            else:
+                active_languages = languages
+
+        if additional_languages:
+            self._load_languages(additional_languages, is_additional=True)
+            active_languages += additional_languages
 
         for line in lines:
             words = line.split(" ")
 
-            for language in languages:
+            for language in active_languages:
                 for i, word in enumerate(words):
                     normalized_word = self._normalize_word(word)
 
-                    if normalized_word in self.profanity_list[language]:
-                        # Replace the entire word if it matches the profanity
+                    if (
+                        normalized_word in self.profanity_list.get(language, [])
+                        or normalized_word in custom_words
+                    ):
                         words[i] = words[i].replace(
                             self._strip(word),
                             self.censor_word(
                                 self._strip(word), partial_censor, censoring_char
                             ),
                         )
 
-            # Reassemble the line with censored words
             censored_line = " ".join(words)
             censored_lines.append(censored_line)
 
-        # Reassemble the text with censored lines
         return "\n".join(censored_lines)
```

### Comparing `censore-0.1.3/censore/data/list/de.txt` & `censore-0.1.4/censore/data/list/de.txt`

 * *Files identical despite different names*

### Comparing `censore-0.1.3/censore/data/list/en.txt` & `censore-0.1.4/censore/data/list/en.txt`

 * *Files identical despite different names*

### Comparing `censore-0.1.3/censore/data/list/fi.txt` & `censore-0.1.4/censore/data/list/fi.txt`

 * *Files identical despite different names*

### Comparing `censore-0.1.3/censore/data/list/fr.txt` & `censore-0.1.4/censore/data/list/fr.txt`

 * *Files identical despite different names*

### Comparing `censore-0.1.3/censore/data/list/hi.txt` & `censore-0.1.4/censore/data/list/hi.txt`

 * *Files identical despite different names*

### Comparing `censore-0.1.3/censore/data/list/hu.txt` & `censore-0.1.4/censore/data/list/hu.txt`

 * *Files identical despite different names*

### Comparing `censore-0.1.3/censore/data/list/it.txt` & `censore-0.1.4/censore/data/list/it.txt`

 * *Files identical despite different names*

### Comparing `censore-0.1.3/censore/data/list/ja.txt` & `censore-0.1.4/censore/data/list/ja.txt`

 * *Files identical despite different names*

### Comparing `censore-0.1.3/censore/data/list/ko.txt` & `censore-0.1.4/censore/data/list/ko.txt`

 * *Files identical despite different names*

### Comparing `censore-0.1.3/censore/data/list/nl.txt` & `censore-0.1.4/censore/data/list/nl.txt`

 * *Files identical despite different names*

### Comparing `censore-0.1.3/censore/data/list/ru.txt` & `censore-0.1.4/censore/data/list/ru.txt`

 * *Files identical despite different names*

### Comparing `censore-0.1.3/censore/data/list/tr.txt` & `censore-0.1.4/censore/data/list/tr.txt`

 * *Files identical despite different names*

### Comparing `censore-0.1.3/censore/data/list/uk.txt` & `censore-0.1.4/censore/data/list/uk.txt`

 * *Files identical despite different names*

### Comparing `censore-0.1.3/censore/data/list/zh.txt` & `censore-0.1.4/censore/data/list/zh.txt`

 * *Files identical despite different names*

### Comparing `censore-0.1.3/censore.egg-info/SOURCES.txt` & `censore-0.1.4/censore.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -30,8 +30,10 @@
 censore/data/list/pl.txt
 censore/data/list/pt.txt
 censore/data/list/ru.txt
 censore/data/list/sv.txt
 censore/data/list/th.txt
 censore/data/list/tr.txt
 censore/data/list/uk.txt
-censore/data/list/zh.txt
+censore/data/list/zh.txt
+tests/__init__.py
+tests/test.py
```

### Comparing `censore-0.1.3/setup.py` & `censore-0.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name="censore",
     # noqa
-    version="0.1.3",
+    version="0.1.4",
     description="A package for censoring profanity in text",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Okinea Dev",
     url="https://github.com/okineadev/censore",
     packages=find_packages(),
-    package_data={'' :['data/list/*.txt']},
+    package_data={"": ["data/list/*.txt"]},
     include_package_data=True,
     install_requires=[],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

