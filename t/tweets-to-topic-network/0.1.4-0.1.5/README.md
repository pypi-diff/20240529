# Comparing `tmp/tweets_to_topic_network-0.1.4.tar.gz` & `tmp/tweets_to_topic_network-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweets_to_topic_network-0.1.4.tar", max compression
+gzip compressed data, was "tweets_to_topic_network-0.1.5.tar", max compression
```

## Comparing `tweets_to_topic_network-0.1.4.tar` & `tweets_to_topic_network-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2024-04-11 12:12:13.477841 tweets_to_topic_network-0.1.4/LICENSE
--rw-r--r--   0        0        0    13380 2024-05-09 17:14:43.252015 tweets_to_topic_network-0.1.4/README.md
--rw-r--r--   0        0        0      799 2024-05-09 17:14:53.182988 tweets_to_topic_network-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       21 2024-04-16 17:41:11.397030 tweets_to_topic_network-0.1.4/tweets_to_topic_network/__init__.py
--rw-r--r--   0        0        0     7924 2024-04-18 11:53:20.230781 tweets_to_topic_network-0.1.4/tweets_to_topic_network/data.py
--rw-r--r--   0        0        0    10831 2024-04-11 12:12:13.484495 tweets_to_topic_network-0.1.4/tweets_to_topic_network/network.py
--rw-r--r--   0        0        0     9952 2024-05-09 17:13:26.067271 tweets_to_topic_network-0.1.4/tweets_to_topic_network/topic.py
--rw-r--r--   0        0        0    14428 1970-01-01 00:00:00.000000 tweets_to_topic_network-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-11 12:12:13.477841 tweets_to_topic_network-0.1.5/LICENSE
+-rw-r--r--   0        0        0    13380 2024-05-09 17:14:43.252015 tweets_to_topic_network-0.1.5/README.md
+-rw-r--r--   0        0        0      819 2024-05-29 12:01:39.453762 tweets_to_topic_network-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-04-16 17:41:11.397030 tweets_to_topic_network-0.1.5/tweets_to_topic_network/__init__.py
+-rw-r--r--   0        0        0     7924 2024-04-18 11:53:20.230781 tweets_to_topic_network-0.1.5/tweets_to_topic_network/data.py
+-rw-r--r--   0        0        0    10831 2024-04-11 12:12:13.484495 tweets_to_topic_network-0.1.5/tweets_to_topic_network/network.py
+-rw-r--r--   0        0        0     9876 2024-05-29 11:48:28.646422 tweets_to_topic_network-0.1.5/tweets_to_topic_network/topic.py
+-rw-r--r--   0        0        0    14469 1970-01-01 00:00:00.000000 tweets_to_topic_network-0.1.5/PKG-INFO
```

### Comparing `tweets_to_topic_network-0.1.4/LICENSE` & `tweets_to_topic_network-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tweets_to_topic_network-0.1.4/README.md` & `tweets_to_topic_network-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tweets_to_topic_network-0.1.4/pyproject.toml` & `tweets_to_topic_network-0.1.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [tool.poetry]
 name = "tweets-to-topic-network"
-version = "0.1.4"
+version = "0.1.5"
 description = "start from a set of tweets and create a multilayer network where each layer is a topic"
 authors = ["alessiogandelli <alessiogandelli99@gmail.com>"]
 readme = "README.md"
 packages = [{include = "tweets_to_topic_network"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 jsonlines = "^4.0.0"
-pandas = "^2.2.2"
+pandas = "^2.2.1"
 sentence-transformers = "^2.6.1"
 bertopic = "^0.16.0"
 openai = "^1.17.0"
 typing-extensions = "^4.11.0"
 qdrant-client = "^1.8.2"
 uunet = "^2.1.1"
 networkx = "^3.3"
 igraph = "^0.11.4"
 fastembed = "^0.2.6"
 umap-learn = "^0.5.6"
 langchain = "^0.1.16"
 flask = "^3.0.3"
+tiktoken = "^0.6.0"
 
 
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 
 [build-system]
```

### Comparing `tweets_to_topic_network-0.1.4/tweets_to_topic_network/data.py` & `tweets_to_topic_network-0.1.5/tweets_to_topic_network/data.py`

 * *Files identical despite different names*

### Comparing `tweets_to_topic_network-0.1.4/tweets_to_topic_network/network.py` & `tweets_to_topic_network-0.1.5/tweets_to_topic_network/network.py`

 * *Files identical despite different names*

### Comparing `tweets_to_topic_network-0.1.4/tweets_to_topic_network/topic.py` & `tweets_to_topic_network-0.1.5/tweets_to_topic_network/topic.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,14 @@
         # add topics label to the originaldataframe and for the not original tweet put the reference of the original tweet in that field 
 
     def _preprocess(self):
 
         self.df['new_text'] = self.df['text']
         self.df['new_text'] =  self.df['new_text'].str.replace(r"http\S+", "")
         self.df['new_text'] =  self.df['new_text'].str.replace(r"@\S+", "")
-        self.df['new_text'] =  self.df['new_text'].str.replace(r"#\S+", "")
         self.df['new_text'] =  self.df['new_text'].str.replace(r"\n", "")
         self.df['new_text'] =  self.df['new_text'].str.strip()
 
         # if new text is empty delete the row
         self.df = self.df[self.df['new_text'] != '']
 
         docs = self.df['new_text'].tolist()
```

### Comparing `tweets_to_topic_network-0.1.4/PKG-INFO` & `tweets_to_topic_network-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweets-to-topic-network
-Version: 0.1.4
+Version: 0.1.5
 Summary: start from a set of tweets and create a multilayer network where each layer is a topic
 Author: alessiogandelli
 Author-email: alessiogandelli99@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,17 +12,18 @@
 Requires-Dist: fastembed (>=0.2.6,<0.3.0)
 Requires-Dist: flask (>=3.0.3,<4.0.0)
 Requires-Dist: igraph (>=0.11.4,<0.12.0)
 Requires-Dist: jsonlines (>=4.0.0,<5.0.0)
 Requires-Dist: langchain (>=0.1.16,<0.2.0)
 Requires-Dist: networkx (>=3.3,<4.0)
 Requires-Dist: openai (>=1.17.0,<2.0.0)
-Requires-Dist: pandas (>=2.2.2,<3.0.0)
+Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: qdrant-client (>=1.8.2,<2.0.0)
 Requires-Dist: sentence-transformers (>=2.6.1,<3.0.0)
+Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
 Requires-Dist: umap-learn (>=0.5.6,<0.6.0)
 Requires-Dist: uunet (>=2.1.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # tweets-to-network
 ```bash
```

