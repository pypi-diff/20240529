# Comparing `tmp/tgnlp-0.0.1.tar.gz` & `tmp/tgnlp-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgnlp-0.0.1.tar", last modified: Mon May 27 16:14:12 2024, max compression
+gzip compressed data, was "tgnlp-1.0.0.tar", last modified: Tue May 28 21:38:02 2024, max compression
```

## Comparing `tgnlp-0.0.1.tar` & `tgnlp-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0 prim      (1000) prim      (1000)        0 2024-05-27 16:14:12.695453 tgnlp-0.0.1/
--rwxrwxrwx   0 prim      (1000) prim      (1000)     7213 2024-05-27 16:14:12.686811 tgnlp-0.0.1/PKG-INFO
--rwxrwxrwx   0 prim      (1000) prim      (1000)     6518 2024-05-17 00:12:21.000000 tgnlp-0.0.1/README.md
-drwxrwxrwx   0 prim      (1000) prim      (1000)        0 2024-05-27 16:14:12.504032 tgnlp-0.0.1/TGNLP/
--rwxrwxrwx   0 prim      (1000) prim      (1000)    24473 2024-05-27 16:11:15.000000 tgnlp-0.0.1/TGNLP/__init__.py
-drwxrwxrwx   0 prim      (1000) prim      (1000)        0 2024-05-27 16:14:12.668181 tgnlp-0.0.1/TGNLP.egg-info/
--rwxrwxrwx   0 prim      (1000) prim      (1000)     7213 2024-05-27 16:14:12.000000 tgnlp-0.0.1/TGNLP.egg-info/PKG-INFO
--rwxrwxrwx   0 prim      (1000) prim      (1000)      186 2024-05-27 16:14:12.000000 tgnlp-0.0.1/TGNLP.egg-info/SOURCES.txt
--rwxrwxrwx   0 prim      (1000) prim      (1000)        1 2024-05-27 16:14:12.000000 tgnlp-0.0.1/TGNLP.egg-info/dependency_links.txt
--rwxrwxrwx   0 prim      (1000) prim      (1000)       88 2024-05-27 16:14:12.000000 tgnlp-0.0.1/TGNLP.egg-info/requires.txt
--rwxrwxrwx   0 prim      (1000) prim      (1000)        6 2024-05-27 16:14:12.000000 tgnlp-0.0.1/TGNLP.egg-info/top_level.txt
--rwxrwxrwx   0 prim      (1000) prim      (1000)      904 2024-05-26 00:17:17.000000 tgnlp-0.0.1/pyproject.toml
--rwxrwxrwx   0 prim      (1000) prim      (1000)       38 2024-05-27 16:14:12.700462 tgnlp-0.0.1/setup.cfg
+drwxrwxrwx   0 prim      (1000) prim      (1000)        0 2024-05-28 21:38:03.608955 tgnlp-1.0.0/
+-rwxrwxrwx   0 prim      (1000) prim      (1000)     1107 2024-05-27 22:50:29.000000 tgnlp-1.0.0/LICENSE
+-rwxrwxrwx   0 prim      (1000) prim      (1000)    15162 2024-05-28 21:38:03.597440 tgnlp-1.0.0/PKG-INFO
+-rwxrwxrwx   0 prim      (1000) prim      (1000)    14339 2024-05-28 21:32:31.000000 tgnlp-1.0.0/README.md
+drwxrwxrwx   0 prim      (1000) prim      (1000)        0 2024-05-28 21:38:03.414466 tgnlp-1.0.0/TGNLP/
+-rwxrwxrwx   0 prim      (1000) prim      (1000)    24564 2024-05-27 22:38:55.000000 tgnlp-1.0.0/TGNLP/__init__.py
+drwxrwxrwx   0 prim      (1000) prim      (1000)        0 2024-05-28 21:38:03.587943 tgnlp-1.0.0/TGNLP.egg-info/
+-rwxrwxrwx   0 prim      (1000) prim      (1000)    15162 2024-05-28 21:38:03.000000 tgnlp-1.0.0/TGNLP.egg-info/PKG-INFO
+-rwxrwxrwx   0 prim      (1000) prim      (1000)      194 2024-05-28 21:38:03.000000 tgnlp-1.0.0/TGNLP.egg-info/SOURCES.txt
+-rwxrwxrwx   0 prim      (1000) prim      (1000)        1 2024-05-28 21:38:03.000000 tgnlp-1.0.0/TGNLP.egg-info/dependency_links.txt
+-rwxrwxrwx   0 prim      (1000) prim      (1000)       88 2024-05-28 21:38:03.000000 tgnlp-1.0.0/TGNLP.egg-info/requires.txt
+-rwxrwxrwx   0 prim      (1000) prim      (1000)        6 2024-05-28 21:38:03.000000 tgnlp-1.0.0/TGNLP.egg-info/top_level.txt
+-rwxrwxrwx   0 prim      (1000) prim      (1000)      955 2024-05-28 21:37:13.000000 tgnlp-1.0.0/pyproject.toml
+-rwxrwxrwx   0 prim      (1000) prim      (1000)       38 2024-05-28 21:38:03.609960 tgnlp-1.0.0/setup.cfg
```

### Comparing `tgnlp-0.0.1/TGNLP/__init__.py` & `tgnlp-1.0.0/TGNLP/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
             #for each sentence remove stopwords/lemmatize if necissary
             for sentence in sentences:
                 words = sentence.split()
                 if remove_stopwords== True:
                     words = [word for word in words if word not in stop_words]
                 if lemmatization == True:
                     tagged_words = pos_tag(words)
-                    words = [lemmatizer.lemmatize(word,pos_dict.get(tag[0], 'n')) for word, tag in tagged_words]
+                    words = [lemmatizer.lemmatize(word, pos_dict.get(tag[0])) if pos_dict.get(tag[0]) else word for word, tag in tagged_words]
                 cleaned_sentence = ' '.join(words)
                 cleaned_sentences.append(cleaned_sentence)
             return [re.sub("[^A-Za-z ]", "", sentence) for sentence in cleaned_sentences]
         else:
             return [re.sub("[^A-Za-z ]", "", sentence) for sentence in sentences]
     elif corpus_type == 'word':
         #split into list of words
@@ -163,15 +163,15 @@
             stop_words = set(stopwords.words('english'))
             words = [word for word in words if word not in stop_words]
         #lemmatize
         if lemmatization == True:
             lemmatizer = WordNetLemmatizer()
             tagged_words = pos_tag(words)
             #if word is unknown default to noun tag
-            words = [lemmatizer.lemmatize(word,pos_dict.get(tag[0], 'n')) for word, tag in tagged_words]
+            words = [lemmatizer.lemmatize(word, pos_dict.get(tag[0])) if pos_dict.get(tag[0]) else word for word, tag in tagged_words]
         return words
     
 
 #due to how this function is used, it assumes what is passed to it is a list
 #helper function for load_data, used to make sure a list only has strings in it
 def check_type(data):
   if not isinstance(data, list):
@@ -213,15 +213,15 @@
   if lemmatization == True:
     pos_dict = {"J": nltk.corpus.wordnet.ADJ,
           "N": nltk.corpus.wordnet.NOUN,
           "V": nltk.corpus.wordnet.VERB,
           "R": nltk.corpus.wordnet.ADV}
     lemmatizer = WordNetLemmatizer()
     tagged_words = pos_tag(text)
-    text= [lemmatizer.lemmatize(word,pos_dict.get(tag[0], 'n')) for word, tag in tagged_words]
+    text = [lemmatizer.lemmatize(word, pos_dict.get(tag[0])) if pos_dict.get(tag[0]) else word for word, tag in tagged_words]
   
   return text
      
 #turn a dataframe into preprocessed list of documents with each document containing list of words
 def dataframe_to_tokens_labels(df, text_column_name, label_column_name, lower_case=True, remove_stopwords=True, lemmatization = False):
   #checking if valid dataframe
   if not isinstance(df, pd.DataFrame):
```

### Comparing `tgnlp-0.0.1/pyproject.toml` & `tgnlp-1.0.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TGNLP"
-version = "0.0.1"
+version = "1.0.0"
 authors = [
   { name="Jesse Coulson",   email="jesseccoulson@gmail.com" },
   { name="Primrose Johns",  email= "primrose.johns.1@gmail.com"}
 ]
 description = "A text analysis/feature generation tool for english text, or text corpuses"
 readme = "README.md"
 requires-python = ">=3.9.2"
 classifiers = [
     "Programming Language :: Python :: 3",
-    #"License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
+    "Development Status :: 5 - Production/Stable",
 ]
 
 #package dependencies
 dependencies = [
   "pandas",
   "networkx",
   "gensim",
```

