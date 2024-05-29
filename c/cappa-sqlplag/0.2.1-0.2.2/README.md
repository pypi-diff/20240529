# Comparing `tmp/cappa_sqlplag-0.2.1.tar.gz` & `tmp/cappa_sqlplag-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cappa_sqlplag-0.2.1.tar", last modified: Sun May 26 09:57:38 2024, max compression
+gzip compressed data, was "cappa_sqlplag-0.2.2.tar", last modified: Wed May 29 05:20:56 2024, max compression
```

## Comparing `cappa_sqlplag-0.2.1.tar` & `cappa_sqlplag-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 09:57:38.137605 cappa_sqlplag-0.2.1/
--rw-rw-rw-   0        0        0     1090 2024-05-26 09:15:34.000000 cappa_sqlplag-0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1918 2024-05-26 09:57:38.135604 cappa_sqlplag-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      803 2024-05-26 09:55:32.000000 cappa_sqlplag-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 09:57:38.110715 cappa_sqlplag-0.2.1/cappa_sqlplag/
--rw-rw-rw-   0        0        0       51 2024-05-26 09:56:08.000000 cappa_sqlplag-0.2.1/cappa_sqlplag/__init__.py
--rw-rw-rw-   0        0        0     2566 2024-05-26 09:09:05.000000 cappa_sqlplag-0.2.1/cappa_sqlplag/sqlplag.py
-drwxrwxrwx   0        0        0        0 2024-05-26 09:57:38.134604 cappa_sqlplag-0.2.1/cappa_sqlplag.egg-info/
--rw-rw-rw-   0        0        0     1918 2024-05-26 09:57:38.000000 cappa_sqlplag-0.2.1/cappa_sqlplag.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2024-05-26 09:57:38.000000 cappa_sqlplag-0.2.1/cappa_sqlplag.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 09:57:38.000000 cappa_sqlplag-0.2.1/cappa_sqlplag.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-26 09:57:38.000000 cappa_sqlplag-0.2.1/cappa_sqlplag.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 09:57:38.137605 cappa_sqlplag-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      845 2024-05-26 09:56:18.000000 cappa_sqlplag-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:20:56.289292 cappa_sqlplag-0.2.2/
+-rw-rw-rw-   0        0        0     1090 2024-05-26 09:15:34.000000 cappa_sqlplag-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     1325 2024-05-29 05:20:56.287294 cappa_sqlplag-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      806 2024-05-26 09:58:56.000000 cappa_sqlplag-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 05:20:56.262288 cappa_sqlplag-0.2.2/cappa_sqlplag/
+-rw-rw-rw-   0        0        0       51 2024-05-29 05:20:29.000000 cappa_sqlplag-0.2.2/cappa_sqlplag/__init__.py
+-rw-rw-rw-   0        0        0     2568 2024-05-29 05:20:33.000000 cappa_sqlplag-0.2.2/cappa_sqlplag/sqlplag.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:20:56.286293 cappa_sqlplag-0.2.2/cappa_sqlplag.egg-info/
+-rw-rw-rw-   0        0        0     1325 2024-05-29 05:20:56.000000 cappa_sqlplag-0.2.2/cappa_sqlplag.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-05-29 05:20:56.000000 cappa_sqlplag-0.2.2/cappa_sqlplag.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 05:20:56.000000 cappa_sqlplag-0.2.2/cappa_sqlplag.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-29 05:20:56.000000 cappa_sqlplag-0.2.2/cappa_sqlplag.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 05:20:56.289292 cappa_sqlplag-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      889 2024-05-29 05:20:51.000000 cappa_sqlplag-0.2.2/setup.py
```

### Comparing `cappa_sqlplag-0.2.1/LICENSE.txt` & `cappa_sqlplag-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cappa_sqlplag-0.2.1/README.md` & `cappa_sqlplag-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Moss CAPPA
+# CAPPA SQLPlag
 SQL-детектор, предназначенный для использования в комплексе автоматической проверки программ [CAPPA](http://cappa.csu.ru/).
 
 ### Установка
  
 ```shell
 pip install cappa_sqlplag
 ```
```

### Comparing `cappa_sqlplag-0.2.1/cappa_sqlplag/sqlplag.py` & `cappa_sqlplag-0.2.2/cappa_sqlplag/sqlplag.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         where_body = where_match.group(1).strip() if where_match else ''
 
         statements = [columns, tables_and_conditions, where_body]
 
         return statements   
     
     
-    def levenshtein_distance(self, s1: str, s2: str) -> list:
+    def levenshtein_distance(self, s1: str, s2: str) -> int:
         if len(s1) < len(s2):
             return self.levenshtein_distance(s2, s1)
 
         if len(s2) == 0:
             return len(s1)
 
         previous_row = range(len(s2) + 1)
@@ -55,21 +55,21 @@
                 deletions = current_row[j] + 1
                 substitutions = previous_row[j] + (c1 != c2)
                 current_row.append(min(insertions, deletions, substitutions))
             previous_row = current_row
 
         return previous_row[-1]
 
-    def similarity_percentage(self) -> float:
+    def similarity_percentage(self) -> int:
 
         query1 = self.ref_code.lower()
         query2 = self.candidate_code.lower()
 
         if query1.startswith('select') and query2.startswith('select'):
             parsed_query1 = self.split_sql_statement(query1)
             parsed_query2 = self.split_sql_statement(query2) 
                 
         distance = self.levenshtein_distance(parsed_query1, parsed_query2)
         max_length = max(len(parsed_query1), len(parsed_query2))
         
         similarity = 1 - distance / max_length
-        return similarity * 100
+        return int(similarity * 100)
```

### Comparing `cappa_sqlplag-0.2.1/setup.py` & `cappa_sqlplag-0.2.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 
 try:
    import pypandoc
    long_description = pypandoc.convert_file('README.md', 'rst')
    long_description = long_description.replace("\r","")  
 except(IOError, ImportError):
-    long_description = open('README.md').read()
+    with open('README.md', 'r', encoding='utf-8') as f:
+        long_description = f.read()
 
 setup(
     name='cappa_sqlplag',
-    version='0.2.1',
+    version='0.2.2',
     description='SQL-детектор плагиата, предназначенный для использования в комплексе автоматической проверки программ CAPPA',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='vrilad',
     url='https://github.com/vrilad/cappa_sqlplag',
     download_url='https://github.com/vrilad/cappa_sqlplag/releases',
     keywords=['cappa', 'sql', 'plagiarism'],
```

