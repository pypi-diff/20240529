# Comparing `tmp/alg_library-0.0.tar.gz` & `tmp/alg_library-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alg_library-0.0.tar", last modified: Wed May 29 14:06:22 2024, max compression
+gzip compressed data, was "alg_library-0.1.tar", last modified: Wed May 29 19:24:23 2024, max compression
```

## Comparing `alg_library-0.0.tar` & `alg_library-0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 14:06:22.824018 alg_library-0.0/
--rw-rw-rw-   0        0        0      117 2024-05-29 14:06:22.824018 alg_library-0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-29 14:06:22.824018 alg_library-0.0/alg_library/
--rw-rw-rw-   0        0        0     4483 2024-05-29 13:34:22.000000 alg_library-0.0/alg_library/alg_library.py
-drwxrwxrwx   0        0        0        0 2024-05-29 14:06:22.824018 alg_library-0.0/alg_library.egg-info/
--rw-rw-rw-   0        0        0      117 2024-05-29 14:06:22.000000 alg_library-0.0/alg_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2024-05-29 14:06:22.000000 alg_library-0.0/alg_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 14:06:22.000000 alg_library-0.0/alg_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-29 13:56:29.000000 alg_library-0.0/alg_library.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-05-29 14:06:22.000000 alg_library-0.0/alg_library.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 14:06:22.824018 alg_library-0.0/setup.cfg
--rw-rw-rw-   0        0        0      216 2024-05-29 14:05:12.000000 alg_library-0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 19:24:23.525897 alg_library-0.1/
+-rw-rw-rw-   0        0        0      117 2024-05-29 19:24:23.525897 alg_library-0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-29 19:24:23.510054 alg_library-0.1/alg_library/
+-rw-rw-rw-   0        0        0     5352 2024-05-29 19:23:30.000000 alg_library-0.1/alg_library/alg_library.py
+drwxrwxrwx   0        0        0        0 2024-05-29 19:24:23.525897 alg_library-0.1/alg_library.egg-info/
+-rw-rw-rw-   0        0        0      117 2024-05-29 19:24:23.000000 alg_library-0.1/alg_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2024-05-29 19:24:23.000000 alg_library-0.1/alg_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 19:24:23.000000 alg_library-0.1/alg_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-29 13:56:29.000000 alg_library-0.1/alg_library.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-05-29 19:24:23.000000 alg_library-0.1/alg_library.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 19:24:23.530118 alg_library-0.1/setup.cfg
+-rw-rw-rw-   0        0        0      216 2024-05-29 19:23:53.000000 alg_library-0.1/setup.py
```

### Comparing `alg_library-0.0/alg_library/alg_library.py` & `alg_library-0.1/alg_library/alg_library.py`

 * *Files 18% similar despite different names*

```diff
@@ -190,8 +190,36 @@
         a[j] = elem_now
 
     new_d = {i: d[i] for i in a}
     return new_d
 
 
 sort_1()
-sort_2()"""
+sort_2()
+
+# Класс с книгой
+class Book:
+    def __init__(self, author, title, year):
+        self.author = author
+        self.title = title
+        self.year = year
+
+
+def quick_sort(list_1, key):
+    if len(list_1) <= 1:
+        return list_1
+
+    elem = getattr(list_1[0], key)
+    left = [i for i in list_1 if getattr(i, key) < elem]
+    center = [i for i in list_1 if getattr(i, key) == elem]
+    right = [i for i in list_1 if getattr(i, key) > elem]
+
+    return quick_sort(left, key) + center + quick_sort(right, key)
+
+
+books = [("Pushlin", "dw", "1989"), ("Dostoyevsky", "po", "1400"), ("Fet", "fd", "1221"), ("Tutchev", "fs", "1333")]
+list_books = []
+for i in books:
+    author, title, year = i[0], i[1], i[2]
+    list_books.append(Book(author, title, year))
+
+[[i.author, i.title, i.year] for i in quick_sort(list_books, 'author')]"""
```

