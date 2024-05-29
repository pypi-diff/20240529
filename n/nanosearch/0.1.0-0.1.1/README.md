# Comparing `tmp/nanosearch-0.1.0.tar.gz` & `tmp/nanosearch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanosearch-0.1.0.tar", last modified: Wed May 29 10:12:32 2024, max compression
+gzip compressed data, was "nanosearch-0.1.1.tar", last modified: Wed May 29 12:06:29 2024, max compression
```

## Comparing `nanosearch-0.1.0.tar` & `nanosearch-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-29 10:12:32.604449 nanosearch-0.1.0/
--rw-r--r--   0 james      (501) staff       (20)     1062 2024-05-28 23:01:54.000000 nanosearch-0.1.0/LICENSE
--rw-r--r--   0 james      (501) staff       (20)     2349 2024-05-29 10:12:32.604061 nanosearch-0.1.0/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     1401 2024-05-29 10:09:41.000000 nanosearch-0.1.0/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-29 10:12:32.601777 nanosearch-0.1.0/nanosearch/
--rw-r--r--   0 james      (501) staff       (20)       86 2024-05-29 10:11:32.000000 nanosearch-0.1.0/nanosearch/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     7336 2024-05-29 10:11:57.000000 nanosearch-0.1.0/nanosearch/engine.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-29 10:12:32.603120 nanosearch-0.1.0/nanosearch.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     2349 2024-05-29 10:12:32.000000 nanosearch-0.1.0/nanosearch.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      239 2024-05-29 10:12:32.000000 nanosearch-0.1.0/nanosearch.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2024-05-29 10:12:32.000000 nanosearch-0.1.0/nanosearch.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)      140 2024-05-29 10:12:32.000000 nanosearch-0.1.0/nanosearch.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       11 2024-05-29 10:12:32.000000 nanosearch-0.1.0/nanosearch.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2024-05-29 10:12:32.604566 nanosearch-0.1.0/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1423 2024-05-29 10:11:28.000000 nanosearch-0.1.0/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-29 12:06:29.602698 nanosearch-0.1.1/
+-rw-r--r--   0 james      (501) staff       (20)     1062 2024-05-28 23:01:54.000000 nanosearch-0.1.1/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)     2349 2024-05-29 12:06:29.602177 nanosearch-0.1.1/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1401 2024-05-29 10:09:41.000000 nanosearch-0.1.1/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-29 12:06:29.599174 nanosearch-0.1.1/nanosearch/
+-rw-r--r--   0 james      (501) staff       (20)      109 2024-05-29 12:06:20.000000 nanosearch-0.1.1/nanosearch/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1095 2024-05-29 11:40:20.000000 nanosearch-0.1.1/nanosearch/cli.py
+-rw-r--r--   0 james      (501) staff       (20)     8432 2024-05-29 11:39:59.000000 nanosearch-0.1.1/nanosearch/engine.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-29 12:06:29.600845 nanosearch-0.1.1/nanosearch.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     2349 2024-05-29 12:06:29.000000 nanosearch-0.1.1/nanosearch.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      294 2024-05-29 12:06:29.000000 nanosearch-0.1.1/nanosearch.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2024-05-29 12:06:29.000000 nanosearch-0.1.1/nanosearch.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       50 2024-05-29 12:06:29.000000 nanosearch-0.1.1/nanosearch.egg-info/entry_points.txt
+-rw-r--r--   0 james      (501) staff       (20)      140 2024-05-29 12:06:29.000000 nanosearch-0.1.1/nanosearch.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       11 2024-05-29 12:06:29.000000 nanosearch-0.1.1/nanosearch.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2024-05-29 12:06:29.602784 nanosearch-0.1.1/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1457 2024-05-29 11:24:46.000000 nanosearch-0.1.1/setup.py
```

### Comparing `nanosearch-0.1.0/LICENSE` & `nanosearch-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nanosearch-0.1.0/PKG-INFO` & `nanosearch-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanosearch
-Version: 0.1.0
+Version: 0.1.1
 Summary: Build a search engine from a website sitemap.
 Home-page: https://github.com/capjamesg/nanosearch
 Author: capjamesg
 Author-email: readers@jamesg.blog
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `nanosearch-0.1.0/README.md` & `nanosearch-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nanosearch-0.1.0/nanosearch/engine.py` & `nanosearch-0.1.1/nanosearch/engine.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import concurrent.futures
 import json
 import re
 from abc import ABC
-from typing import List
+from typing import List, Union
 
 import getsitemap
 import numpy as np
 import requests
 from bs4 import BeautifulSoup
 from rank_bm25 import BM25Okapi
 from sklearn.feature_extraction.text import TfidfVectorizer
 from urllib.parse import urlparse, urljoin
 import math
 
+REMOVE_ALL_SEPARATORS = [
+    lambda x: x.split(" | ")[0],
+    lambda x: x.split(" - ")[0],
+]
+
 def retrieve_page_text(url: str) -> str:
     try:
         page = requests.get(url).text
     except requests.exceptions.RequestException as e:
         return "", "", None
 
     content = BeautifulSoup(page, "html.parser")
@@ -31,49 +36,86 @@
 
     return content.get_text().replace("\n", " ").lower(), content.title.text, content
 
 def get_links(content: BeautifulSoup, site: str) -> List[str]:
     """
     Retrieve all inlinks to the site on a given page.
     """
+    if not content:
+        return []
+    
     links = content.find_all("a")
     links = [link["href"] for link in links if link.get("href")]
     links = [link.split("#")[0].split("?")[0] for link in links]
     links = [link for link in links if urlparse(link).netloc == urlparse(site).netloc or link.startswith("/")]
     links = [urljoin(site, link) for link in links]
     return links
 
+def get_description(content: BeautifulSoup) -> str:
+    """
+    Retrieve the description of a page.
+    """
+    options = [
+        content.find("meta", attrs={"name": "description"}),
+        content.find("meta", attrs={"property": "og:description"}),
+        content.find("meta", attrs={"name": "twitter:description"}),
+    ]
+    
+    for option in options:
+        if option:
+            return option["content"]
+        
+    return ""
+
 class NanoSearch(ABC):
     def __init__(self) -> None:
        pass
 
     @classmethod
-    def from_sitemap(cls, sitemap_url: str, includes: List[str] = [], excludes: List[str] = [], title_transforms: List[callable] = []) -> None:
+    def from_sitemap(cls, sitemap_url: Union[str, List[str]],
+                     includes: List[str] = [], excludes: List[str] = [], title_transforms: List[callable] = []) -> None:
         """
         Create an index from a sitemap.
         """
         instance = cls()
-        urls = getsitemap.get_individual_sitemap(sitemap_url)
-        if not urls:
-            print("No sitemap found")
-            return None
         
-        urls = urls[sitemap_url]
+        if isinstance(sitemap_url, str):
+            sitemap_url = [sitemap_url]
+
+        all_urls = []
+        sitemap_domains = {}
+
+        for su in sitemap_url:
+            urls = getsitemap.get_individual_sitemap(su)
+
+            if not urls:
+                print("No sitemap found")
+                return None
+            
+            urls = urls[su]
+
+            all_urls.extend(urls)
+
+            site = urlparse(su).netloc
+            for u in urls:
+                sitemap_domains[u] = "https://" + site
+
+        urls = list(set(all_urls))
+        
         urls.sort()
 
         if includes:
             urls = [url for url in urls if any(re.match(include, url) for include in includes)]
 
         if excludes:
             urls = [url for url in urls if not any(re.match(exclude, url) for exclude in excludes)]
         
         print("Indexing", len(urls), "URLs")
-        instance.sitemap_domain = urlparse(sitemap_url).netloc
-        instance.sitemap_domain = "https://" + instance.sitemap_domain
         instance.title_transforms = title_transforms
+        instance.sitemap_domains = sitemap_domains
         instance.create_index(urls=urls)
         return instance
 
     @classmethod
     def from_nanosearch_json(cls, file_path: str) -> None:
         """
         Create an index from a plain text file.
@@ -128,15 +170,17 @@
 
             title = titles[i]
 
             if self.title_transforms:
                 for transform in self.title_transforms:
                     title = transform(title)
 
-            self.url2data[url] = {"text": results[i], "title": title, "url": url}
+            description = get_description(content[i])
+
+            self.url2data[url] = {"text": results[i], "title": title, "url": url, "description": description}
 
         self.urls = list(self.url2data.keys())
         self.create_index_object([data["text"] for data in self.url2data.values()])
 
     def create_index_object(self, data: str) -> None:
         self.inference = self.vectorizer.fit_transform(data)
 
@@ -185,17 +229,19 @@
 
             title = titles[i]
 
             if self.title_transforms:
                 for transform in self.title_transforms:
                     title = transform(title)
 
-            self.url2data[url] = {"text": text, "title": title, "url": url}
+            description = get_description(content[i])
+
+            self.url2data[url] = {"text": text, "title": title, "url": url, "description": description}
             
-            for link in get_links(content[i], site=self.sitemap_domain):
+            for link in get_links(content[i], site=self.sitemap_domains[url]):
                 self.link_graph[link] = self.link_graph.get(link, []) + [url]
 
         for url, linked_from in self.link_graph.items():
             if url in self.url2data:
                 self.url2data[url]["linked_from"] = len(linked_from)
 
         self.create_index_object([data["text"] for data in self.url2data.values()])
```

### Comparing `nanosearch-0.1.0/nanosearch.egg-info/PKG-INFO` & `nanosearch-0.1.1/nanosearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanosearch
-Version: 0.1.0
+Version: 0.1.1
 Summary: Build a search engine from a website sitemap.
 Home-page: https://github.com/capjamesg/nanosearch
 Author: capjamesg
 Author-email: readers@jamesg.blog
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `nanosearch-0.1.0/setup.py` & `nanosearch-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,16 +24,16 @@
         "getsitemap",
         "numpy",
         "requests",
         "beautifulsoup4",
         "rank-bm25",
         "scikit-learn",
     ],
+    entry_points={"console_scripts": ["nanosearch=nanosearch.cli:cli"]},
     include_package_data=True,
-    package_data={"": ["models.csv"]},
     packages=find_packages(exclude=("tests",)),
     extras_require={
         "dev": [
             "flake8",
             "black==22.3.0",
             "isort",
             "twine",
```

