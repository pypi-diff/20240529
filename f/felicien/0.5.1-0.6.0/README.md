# Comparing `tmp/felicien-0.5.1.tar.gz` & `tmp/felicien-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "felicien-0.5.1.tar", max compression
+gzip compressed data, was "felicien-0.6.0.tar", max compression
```

## Comparing `felicien-0.5.1.tar` & `felicien-0.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1095 2024-05-28 13:20:00.022959 felicien-0.5.1/LICENSE
--rw-r--r--   0        0        0     2599 2024-05-28 13:20:00.023959 felicien-0.5.1/README.md
--rw-r--r--   0        0        0      142 2024-05-28 13:20:00.028959 felicien-0.5.1/felicien/__init__.py
--rw-r--r--   0        0        0     6505 2024-05-28 13:20:00.029959 felicien-0.5.1/felicien/feliconnector.py
--rw-r--r--   0        0        0    13044 2024-05-28 13:20:00.029959 felicien-0.5.1/felicien/felits.py
--rw-r--r--   0        0        0     1067 2024-05-28 13:20:00.030959 felicien-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     3398 1970-01-01 00:00:00.000000 felicien-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-05-29 08:06:42.368491 felicien-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2599 2024-05-29 08:06:42.368491 felicien-0.6.0/README.md
+-rw-r--r--   0        0        0      142 2024-05-29 08:06:42.373491 felicien-0.6.0/felicien/__init__.py
+-rw-r--r--   0        0        0     6506 2024-05-29 08:06:42.374491 felicien-0.6.0/felicien/feliconnector.py
+-rw-r--r--   0        0        0    13239 2024-05-29 08:06:42.374491 felicien-0.6.0/felicien/felits.py
+-rw-r--r--   0        0        0     1067 2024-05-29 08:06:42.375491 felicien-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3398 1970-01-01 00:00:00.000000 felicien-0.6.0/PKG-INFO
```

### Comparing `felicien-0.5.1/LICENSE` & `felicien-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `felicien-0.5.1/README.md` & `felicien-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `felicien-0.5.1/felicien/feliconnector.py` & `felicien-0.6.0/felicien/feliconnector.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
             ConnectionError if query status code is not HTTP/204
         """
         payload = {"match[]": metric}
         method = "GET" if self.tsdb == "victoriametrics" else "POST"
 
         r = requests.request(
             method=method,
-            url=f"{self.base_url}/{API_TSDB_QUERY[self.tsdb]}",
+            url=f"{self.base_url}/{API_TSDB_DELETE[self.tsdb]}",
             params=payload,
             **self._options,  # type: ignore
             timeout=60,
         )
         if not r.status_code == 204:
             raise ConnectionError(
                 f"unable to delete timeserie: {r.status_code}"
```

### Comparing `felicien-0.5.1/felicien/felits.py` & `felicien-0.6.0/felicien/felits.py`

 * *Files 3% similar despite different names*

```diff
@@ -188,31 +188,40 @@
     def as_prometheus(self) -> str:
         """Object representation based on Prometheus API format
 
         Returns:
             str: JSON representation of the object, as you could push it
                 to Prometheus
         """
+        return json.dumps(self.as_dict())
+
+    def as_dict(self) -> dict:
+        """Object representation as a Dictionary
+
+        Returns:
+            dict: representation of the object
+        """
         result = dict()
 
         result["metric"] = {"__name__": self.name}
 
         for k, v in self.labels.items():
             result["metric"][k] = v
 
         result["values"] = self.data.to_list()  # type: ignore
         result["timestamps"] = (
-            (pd.Series(data=self.data.index) - dt.datetime(1970, 1, 1))
+            (
+                pd.Series(data=self.data.index) - dt.datetime(1970, 1, 1)
+            )  # type: ignore
             .dt.total_seconds()
-            .apply(lambda x: x * 1000)
             .astype(int)
             .to_list()
         )
 
-        return json.dumps(result)
+        return result
 
     def as_dataframe(self, name: str = "") -> pd.DataFrame:
         """self.data representation as a pandas.DataFrame
 
         Args:
             name (str, optional): Name of the column for the Serie in the
                 resulting DataFrame. Defaults to self.name.
```

### Comparing `felicien-0.5.1/pyproject.toml` & `felicien-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "felicien"
-version = "0.5.1"
+version = "0.6.0"
 description = "Felicien is you companion to retrieve timeseries from a TSDB, to transform it in various format and to push it to a TSDB."
 authors = ["Julien Andrieux <chilladx@pm.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "felicien" },
 ]
```

### Comparing `felicien-0.5.1/PKG-INFO` & `felicien-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felicien
-Version: 0.5.1
+Version: 0.6.0
 Summary: Felicien is you companion to retrieve timeseries from a TSDB, to transform it in various format and to push it to a TSDB.
 License: MIT
 Author: Julien Andrieux
 Author-email: chilladx@pm.me
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

