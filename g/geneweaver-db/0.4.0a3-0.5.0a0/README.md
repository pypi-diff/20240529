# Comparing `tmp/geneweaver_db-0.4.0a3.tar.gz` & `tmp/geneweaver_db-0.5.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneweaver_db-0.4.0a3.tar", max compression
+gzip compressed data, was "geneweaver_db-0.5.0a0.tar", max compression
```

## Comparing `geneweaver_db-0.4.0a3.tar` & `geneweaver_db-0.5.0a0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    11356 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/LICENSE
--rw-r--r--   0        0        0     2162 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/README.md
--rw-r--r--   0        0        0      955 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/pyproject.toml
--rw-r--r--   0        0        0      156 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/__init__.py
--rw-r--r--   0        0        0      132 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/aio/__init__.py
--rw-r--r--   0        0        0     3134 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/aio/gene.py
--rw-r--r--   0        0        0     5163 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/aio/geneset.py
--rw-r--r--   0        0        0     2189 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/aio/publication.py
--rw-r--r--   0        0        0     1310 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/aio/species.py
--rw-r--r--   0        0        0      809 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/aio/threshold.py
--rw-r--r--   0        0        0       56 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/core/__init__.py
--rw-r--r--   0        0        0      845 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/core/cursor.py
--rw-r--r--   0        0        0      145 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/core/settings.py
--rw-r--r--   0        0        0     1769 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/core/settings_class.py
--rw-r--r--   0        0        0      438 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/exceptions.py
--rw-r--r--   0        0        0    10316 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/gene.py
--rw-r--r--   0        0        0     8981 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/geneset.py
--rw-r--r--   0        0        0     7887 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/geneset_value.py
--rw-r--r--   0        0        0     2063 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/publication.py
--rw-r--r--   0        0        0       42 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/__init__.py
--rw-r--r--   0        0        0     5410 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/gene.py
--rw-r--r--   0        0        0      364 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/geneset/__init__.py
--rw-r--r--   0        0        0     1351 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/geneset/const.py
--rw-r--r--   0        0        0     5492 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/geneset/read.py
--rw-r--r--   0        0        0     4824 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/geneset/utils.py
--rw-r--r--   0        0        0     4014 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/geneset/write.py
--rw-r--r--   0        0        0      982 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/project.py
--rw-r--r--   0        0        0     4683 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/publication.py
--rw-r--r--   0        0        0       60 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/search/__init__.py
--rw-r--r--   0        0        0       50 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/search/search.py
--rw-r--r--   0        0        0     1572 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/search/utils.py
--rw-r--r--   0        0        0     1603 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/species.py
--rw-r--r--   0        0        0     2900 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/threshold.py
--rw-r--r--   0        0        0     1782 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/utils.py
--rw-r--r--   0        0        0     1249 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/species.py
--rw-r--r--   0        0        0      775 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/threshold.py
--rw-r--r--   0        0        0     6887 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/user.py
--rw-r--r--   0        0        0     3201 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/utils.py
--rw-r--r--   0        0        0     2984 1970-01-01 00:00:00.000000 geneweaver_db-0.4.0a3/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-29 14:33:54.663021 geneweaver_db-0.5.0a0/LICENSE
+-rw-r--r--   0        0        0     2162 2024-05-29 14:33:54.663021 geneweaver_db-0.5.0a0/README.md
+-rw-r--r--   0        0        0      955 2024-05-29 14:33:54.663021 geneweaver_db-0.5.0a0/pyproject.toml
+-rw-r--r--   0        0        0      156 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/__init__.py
+-rw-r--r--   0        0        0      132 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/aio/__init__.py
+-rw-r--r--   0        0        0     3134 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/aio/gene.py
+-rw-r--r--   0        0        0     5163 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/aio/geneset.py
+-rw-r--r--   0        0        0     4062 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/aio/publication.py
+-rw-r--r--   0        0        0     1310 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/aio/species.py
+-rw-r--r--   0        0        0      809 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/aio/threshold.py
+-rw-r--r--   0        0        0       56 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/core/__init__.py
+-rw-r--r--   0        0        0      845 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/core/cursor.py
+-rw-r--r--   0        0        0      145 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/core/settings.py
+-rw-r--r--   0        0        0     1769 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/core/settings_class.py
+-rw-r--r--   0        0        0      438 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/exceptions.py
+-rw-r--r--   0        0        0    10316 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/gene.py
+-rw-r--r--   0        0        0     8981 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/geneset.py
+-rw-r--r--   0        0        0     7887 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/geneset_value.py
+-rw-r--r--   0        0        0     3913 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/publication.py
+-rw-r--r--   0        0        0       42 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/__init__.py
+-rw-r--r--   0        0        0     5410 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/gene.py
+-rw-r--r--   0        0        0      364 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/geneset/__init__.py
+-rw-r--r--   0        0        0     1351 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/geneset/const.py
+-rw-r--r--   0        0        0     5492 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/geneset/read.py
+-rw-r--r--   0        0        0     4824 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/geneset/utils.py
+-rw-r--r--   0        0        0     4014 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/geneset/write.py
+-rw-r--r--   0        0        0      982 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/project.py
+-rw-r--r--   0        0        0     6984 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/publication.py
+-rw-r--r--   0        0        0       60 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/search/__init__.py
+-rw-r--r--   0        0        0       50 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/search/search.py
+-rw-r--r--   0        0        0     1572 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/search/utils.py
+-rw-r--r--   0        0        0     1603 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/species.py
+-rw-r--r--   0        0        0     2900 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/threshold.py
+-rw-r--r--   0        0        0     1782 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/query/utils.py
+-rw-r--r--   0        0        0     1249 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/species.py
+-rw-r--r--   0        0        0      775 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/threshold.py
+-rw-r--r--   0        0        0     6887 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/user.py
+-rw-r--r--   0        0        0     3201 2024-05-29 14:33:54.667021 geneweaver_db-0.5.0a0/src/geneweaver/db/utils.py
+-rw-r--r--   0        0        0     2984 1970-01-01 00:00:00.000000 geneweaver_db-0.5.0a0/PKG-INFO
```

### Comparing `geneweaver_db-0.4.0a3/LICENSE` & `geneweaver_db-0.5.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/README.md` & `geneweaver_db-0.5.0a0/README.md`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/pyproject.toml` & `geneweaver_db-0.5.0a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geneweaver-db"
-version = "0.4.0a3"
+version = "0.5.0a0"
 description = "Database Interaction Services for GeneWeaver"
 authors = ["Jax Computational Sciences <cssc@jax.org>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://thejacksonlaboratory.github.io/geneweaver-docs/"
 repository = "https://github.com/TheJacksonLaboratory/geneweaver-db"
 packages = [
```

### Comparing `geneweaver_db-0.4.0a3/src/geneweaver/db/aio/gene.py` & `geneweaver_db-0.5.0a0/src/geneweaver/db/aio/gene.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/src/geneweaver/db/aio/geneset.py` & `geneweaver_db-0.5.0a0/src/geneweaver/db/aio/geneset.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/src/geneweaver/db/aio/species.py` & `geneweaver_db-0.5.0a0/src/geneweaver/db/aio/species.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/src/geneweaver/db/aio/threshold.py` & `geneweaver_db-0.5.0a0/src/geneweaver/db/aio/threshold.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/src/geneweaver/db/core/cursor.py` & `geneweaver_db-0.5.0a0/src/geneweaver/db/core/cursor.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/src/geneweaver/db/core/settings_class.py` & `geneweaver_db-0.5.0a0/src/geneweaver/db/core/settings_class.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/src/geneweaver/db/gene.py` & `geneweaver_db-0.5.0a0/src/geneweaver/db/gene.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/src/geneweaver/db/geneset.py` & `geneweaver_db-0.5.0a0/src/geneweaver/db/geneset.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/src/geneweaver/db/geneset_value.py` & `geneweaver_db-0.5.0a0/src/geneweaver/db/geneset_value.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/src/geneweaver/db/query/gene.py` & `geneweaver_db-0.5.0a0/src/geneweaver/db/query/gene.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/src/geneweaver/db/query/geneset/const.py` & `geneweaver_db-0.5.0a0/src/geneweaver/db/query/geneset/const.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/src/geneweaver/db/query/geneset/read.py` & `geneweaver_db-0.5.0a0/src/geneweaver/db/query/geneset/read.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/src/geneweaver/db/query/geneset/utils.py` & `geneweaver_db-0.5.0a0/src/geneweaver/db/query/geneset/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/src/geneweaver/db/query/geneset/write.py` & `geneweaver_db-0.5.0a0/src/geneweaver/db/query/geneset/write.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/src/geneweaver/db/query/project.py` & `geneweaver_db-0.5.0a0/src/geneweaver/db/query/project.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/src/geneweaver/db/query/publication.py` & `geneweaver_db-0.5.0a0/src/geneweaver/db/publication.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,159 +1,124 @@
-"""Generate SQL queries for publications."""
+"""Database code for interacting with Publication table."""
 
-from typing import Iterable, Optional, Tuple
+from typing import Iterable, List, Optional
 
-from geneweaver.db.utils import format_sql_fields
-from psycopg import rows
-from psycopg.sql import SQL, Composed, Identifier, Placeholder
-
-PUB_FIELD_MAP = {
-    "pub_id": "id",
-    "pub_authors": "authors",
-    "pub_title": "title",
-    "pub_abstract": "abstract",
-    "pub_journal": "journal",
-    "pub_volume": "volume",
-    "pub_pages": "pages",
-    "pub_month": "month",
-    "pub_year": "year",
-    "pub_pubmed": "pubmed_id",
-}
-
-PUB_FIELDS = format_sql_fields(PUB_FIELD_MAP, query_table="publication")
-
-PUB_QUERY = SQL("SELECT") + SQL(",").join(PUB_FIELDS) + SQL("FROM publication")
-
-PUB_INSERT_COLS = SQL(",").join(
-    [Identifier(k) for k in PUB_FIELD_MAP.keys() if k != "pub_id"]
-)
-PUB_INSERT_VALS = SQL(",").join(
-    [Placeholder(k) for k in PUB_FIELD_MAP.keys() if k != "pub_id"]
-)
+from geneweaver.core.schema.publication import PublicationInfo
+from geneweaver.db.query import publication as publication_query
+from psycopg import Cursor, rows
+from psycopg.rows import Row
 
 
-def get(
-    pub_id: Optional[int] = None,
-    authors: Optional[str] = None,
-    title: Optional[str] = None,
-    abstract: Optional[str] = None,
-    journal: Optional[str] = None,
-    volume: Optional[str] = None,
-    pages: Optional[str] = None,
-    month: Optional[str] = None,
-    year: Optional[str] = None,
-    pubmed: Optional[str] = None,
-    search_text: Optional[str] = None,
-    limit: Optional[int] = None,
-    offset: Optional[int] = None,
-) -> Tuple[Composed, dict]:
-    """Get publications by some criteria.
+def by_pubmed_id(cursor: Cursor, pubmed_id: int) -> Optional[rows.Row]:
+    """Get a publication by PubMed ID.
 
-    NOTE: NOT IMPLEMENTED
+    :param cursor: The database cursor.
+    :param pubmed_id: The PubMed ID to search for.
+
+    :return: optional row using `.fetchone()`
     """
-    raise NotImplementedError()
+    cursor.execute(*publication_query.by_pubmed_id(pubmed_id))
+    return cursor.fetchone()
 
 
-def by_id(pub_id: int) -> Optional[rows.Row]:
-    """Create a psycopg query to get a publication by ID.
+def by_pubmed_ids(cursor: Cursor, pubmed_ids: Iterable[int]) -> List[rows.Row]:
+    """Get publications by a list of PubMed IDs.
 
-    :param pub_id: The publication ID (geneweaver internal) to search for.
+    :param cursor: The database cursor.
+    :param pubmed_ids: The PubMed IDs to search for.
 
-    :return: A query (and params) that can be executed on a cursor.
+    :return: list of results using `.fetchall()`
     """
-    query = (PUB_QUERY + SQL("WHERE pub_id = %(pub_id)s")).join(" ")
-    params = {"pub_id": pub_id}
-    return query, params
+    cursor.execute(*publication_query.by_pubmed_ids(pubmed_ids))
+    return cursor.fetchall()
 
 
-def by_geneset_id(geneset_id: int) -> Tuple[Composed, dict]:
-    """Create a psycopg query to get a publication by geneset ID.
+def by_id(cursor: Cursor, pub_id: int) -> Optional[rows.Row]:
+    """Get a publication by ID.
 
-    :param geneset_id: The geneset ID to search for.
+    :param cursor: The database cursor.
+    :param pub_id: The publication ID (geneweaver internal) to search for.
 
-    :return: A query (and params) that can be executed on a cursor.
+    :return: optional row using `.fetchone()`
     """
-    query = (
-        PUB_QUERY
-        + SQL("JOIN geneset ON publication.pub_id = geneset.pub_id")
-        + SQL("WHERE gs_id = %(geneset_id)s")
-    ).join(" ")
-
-    params = {"geneset_id": geneset_id}
-    return query, params
+    cursor.execute(*publication_query.by_id(pub_id))
+    return cursor.fetchone()
 
 
-def by_pubmed_id(pubmed_id: int) -> Tuple[Composed, dict]:
-    """Create a psycopg query to get a publication by PubMed ID.
+def by_geneset_id(cursor: Cursor, geneset_id: int) -> Optional[rows.Row]:
+    """Get a publication by geneset ID.
 
-    :param pubmed_id: The PubMed ID to search for.
+    :param cursor: The database cursor.
+    :param geneset_id: The geneset ID to search for.
 
-    :return: A query (and params) that can be executed on a cursor.
+    :return: optional row using `.fetchone()`
     """
-    query = (PUB_QUERY + SQL("WHERE pub_pubmed = %(pmid)s")).join(" ")
-    # PubMed IDs are integers, but are stored as strings in the database.
-    params = {"pmid": str(pubmed_id)}
-    return query, params
+    cursor.execute(*publication_query.by_geneset_id(geneset_id))
+    return cursor.fetchone()
 
 
-def by_pubmed_ids(pubmed_ids: Iterable[int]) -> Tuple[Composed, dict]:
-    """Create a psycopg query to get publications by a list of PubMed IDs.
+def add(cursor: Cursor, publication: PublicationInfo) -> Optional[rows.Row]:
+    """Add a publication to the database.
 
-    :param pubmed_ids: The PubMed IDs to search for.
+    :param cursor: The database cursor.
+    :param publication: The publication to add.
 
-    :return: A query (and params) that can be executed on a cursor.
+    :return: optional row using `.fetchone()`
     """
-    query = (PUB_QUERY + SQL("WHERE pub_pubmed = ANY(%(pubmed_ids)s)")).join(" ")
-    params = {"pubmed_ids": list(pubmed_ids)}
-    return query, params
+    cursor.execute(*publication_query.add(**publication.dict()))
+    return cursor.fetchone()
 
 
-def add(
-    authors: str,
-    title: str,
-    abstract: str,
-    journal: str,
-    pubmed_id: str,
+def get(
+    cursor: Cursor,
+    pub_id: Optional[int] = None,
+    authors: Optional[str] = None,
+    title: Optional[str] = None,
+    abstract: Optional[str] = None,
+    journal: Optional[str] = None,
     volume: Optional[str] = None,
     pages: Optional[str] = None,
     month: Optional[str] = None,
-    year: Optional[int] = None,
-) -> Tuple[Composed, dict]:
-    """Create a psycopg query to add a publication to the database.
-
-    :param authors: The authors of the publication.
-    :param title: The title of the publication.
-    :param abstract: The abstract of the publication.
-    :param journal: The journal of the publication.
-    :param volume: The volume of the publication.
-    :param pages: The pages of the publication.
-    :param month: The month of the publication.
-    :param year: The year of the publication.
-    :param pubmed_id: The PubMed ID of the publication.
-
-    :return: A query (and params) that can be executed on a cursor.
-    """
-    query = (
-        SQL("INSERT INTO publication")
-        + SQL("(")
-        + PUB_INSERT_COLS
-        + SQL(")")
-        + SQL("VALUES")
-        + SQL("(")
-        + PUB_INSERT_VALS
-        + SQL(")")
-        + SQL("RETURNING pub_id")
-    ).join(" ")
-
-    params = {
-        "pub_authors": authors,
-        "pub_title": title,
-        "pub_abstract": abstract,
-        "pub_journal": journal,
-        "pub_volume": volume,
-        "pub_pages": pages,
-        "pub_month": month,
-        "pub_year": year,
-        "pub_pubmed": pubmed_id,
-    }
+    year: Optional[str] = None,
+    pubmed: Optional[str] = None,
+    search_text: Optional[str] = None,
+    limit: Optional[int] = None,
+    offset: Optional[int] = None,
+) -> List[Row]:
+    """Get publications by some criteria.
+
+    :param cursor: An async database cursor.
+    :param pub_id: Show only results with this publication id
+    :param authors: Show only results with these authors
+    :param title: Show only results with this title
+    :param abstract: Show only results with this abstract
+    :param journal: Show only results with this journal
+    :param volume: Show only results with volume
+    :param pages: Show only results with these pages
+    :param month: Show only results with this publication month
+    :param year: Show only results with publication year
+    :param pubmed: Show only results with pubmed id
+    :param search_text: Show only results that match this search text (using PostgreSQL
+                        full-text search).
+    :param limit: Limit the number of results.
+    :param offset: Offset the results.
+
+    """
+    cursor.execute(
+        *publication_query.get(
+            pub_id=pub_id,
+            authors=authors,
+            title=title,
+            abstract=abstract,
+            journal=journal,
+            volume=volume,
+            pages=pages,
+            month=month,
+            year=year,
+            pubmed=pubmed,
+            search_text=search_text,
+            limit=limit,
+            offset=offset,
+        )
+    )
 
-    return query, params
+    return cursor.fetchall()
```

### Comparing `geneweaver_db-0.4.0a3/src/geneweaver/db/query/search/utils.py` & `geneweaver_db-0.5.0a0/src/geneweaver/db/query/search/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/src/geneweaver/db/query/species.py` & `geneweaver_db-0.5.0a0/src/geneweaver/db/query/species.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/src/geneweaver/db/query/threshold.py` & `geneweaver_db-0.5.0a0/src/geneweaver/db/query/threshold.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/src/geneweaver/db/query/utils.py` & `geneweaver_db-0.5.0a0/src/geneweaver/db/query/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/src/geneweaver/db/species.py` & `geneweaver_db-0.5.0a0/src/geneweaver/db/species.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/src/geneweaver/db/threshold.py` & `geneweaver_db-0.5.0a0/src/geneweaver/db/threshold.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/src/geneweaver/db/user.py` & `geneweaver_db-0.5.0a0/src/geneweaver/db/user.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/src/geneweaver/db/utils.py` & `geneweaver_db-0.5.0a0/src/geneweaver/db/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a3/PKG-INFO` & `geneweaver_db-0.5.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneweaver-db
-Version: 0.4.0a3
+Version: 0.5.0a0
 Summary: Database Interaction Services for GeneWeaver
 Home-page: https://thejacksonlaboratory.github.io/geneweaver-docs/
 License: Apache-2.0
 Author: Jax Computational Sciences
 Author-email: cssc@jax.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

