# Comparing `tmp/pyeventengine-0.3.0.post1.tar.gz` & `tmp/pyeventengine-0.3.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeventengine-0.3.0.post1.tar", last modified: Tue May 28 10:43:55 2024, max compression
+gzip compressed data, was "pyeventengine-0.3.0.post2.tar", last modified: Tue May 28 11:03:38 2024, max compression
```

## Comparing `pyeventengine-0.3.0.post1.tar` & `pyeventengine-0.3.0.post2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 10:43:55.460847 pyeventengine-0.3.0.post1/
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 10:43:54.999170 pyeventengine-0.3.0.post1/EventEngine/
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 10:43:55.152214 pyeventengine-0.3.0.post1/EventEngine/Core/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3227 2024-05-28 10:24:33.000000 pyeventengine-0.3.0.post1/EventEngine/Core/__init__.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    13778 2024-05-28 10:17:54.000000 pyeventengine-0.3.0.post1/EventEngine/Core/_event.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     4525 2024-05-28 10:21:19.000000 pyeventengine-0.3.0.post1/EventEngine/Core/_topic.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3001 2024-05-28 06:54:14.000000 pyeventengine-0.3.0.post1/EventEngine/Core/_topic_c.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       49 2024-05-28 10:43:18.000000 pyeventengine-0.3.0.post1/EventEngine/__init__.py
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 10:43:55.224277 pyeventengine-0.3.0.post1/EventEngine/cpp/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     9271 2024-05-28 06:20:25.000000 pyeventengine-0.3.0.post1/EventEngine/cpp/topic_api.cpp
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1066 2024-05-28 06:20:25.000000 pyeventengine-0.3.0.post1/LICENSE
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     2109 2024-05-28 10:43:55.455847 pyeventengine-0.3.0.post1/PKG-INFO
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 10:43:55.430847 pyeventengine-0.3.0.post1/PyEventEngine.egg-info/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     2109 2024-05-28 10:43:54.000000 pyeventengine-0.3.0.post1/PyEventEngine.egg-info/PKG-INFO
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      350 2024-05-28 10:43:54.000000 pyeventengine-0.3.0.post1/PyEventEngine.egg-info/SOURCES.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2024-05-28 10:43:54.000000 pyeventengine-0.3.0.post1/PyEventEngine.egg-info/dependency_links.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       12 2024-05-28 10:43:54.000000 pyeventengine-0.3.0.post1/PyEventEngine.egg-info/top_level.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1507 2024-05-28 06:20:25.000000 pyeventengine-0.3.0.post1/README.md
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       79 2024-05-28 10:43:55.463847 pyeventengine-0.3.0.post1/setup.cfg
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1733 2024-05-28 10:24:33.000000 pyeventengine-0.3.0.post1/setup.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 11:03:38.758236 pyeventengine-0.3.0.post2/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1066 2024-05-28 06:20:25.000000 pyeventengine-0.3.0.post2/LICENSE
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     2112 2024-05-28 11:03:38.755233 pyeventengine-0.3.0.post2/PKG-INFO
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 11:03:38.734233 pyeventengine-0.3.0.post2/PyEventEngine.egg-info/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     2112 2024-05-28 11:03:38.000000 pyeventengine-0.3.0.post2/PyEventEngine.egg-info/PKG-INFO
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      364 2024-05-28 11:03:38.000000 pyeventengine-0.3.0.post2/PyEventEngine.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2024-05-28 11:03:38.000000 pyeventengine-0.3.0.post2/PyEventEngine.egg-info/dependency_links.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       13 2024-05-28 11:03:38.000000 pyeventengine-0.3.0.post2/PyEventEngine.egg-info/top_level.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1510 2024-05-28 11:01:21.000000 pyeventengine-0.3.0.post2/README.md
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 11:03:38.493878 pyeventengine-0.3.0.post2/event_engine/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       51 2024-05-28 11:03:19.000000 pyeventengine-0.3.0.post2/event_engine/__init__.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 11:03:38.507881 pyeventengine-0.3.0.post2/event_engine/cpp/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     9271 2024-05-28 06:20:25.000000 pyeventengine-0.3.0.post2/event_engine/cpp/topic_api.cpp
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 11:03:38.615981 pyeventengine-0.3.0.post2/event_engine/native/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3227 2024-05-28 10:24:33.000000 pyeventengine-0.3.0.post2/event_engine/native/__init__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    13778 2024-05-28 10:17:54.000000 pyeventengine-0.3.0.post2/event_engine/native/_event.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     4525 2024-05-28 10:21:19.000000 pyeventengine-0.3.0.post2/event_engine/native/_topic.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3001 2024-05-28 06:54:14.000000 pyeventengine-0.3.0.post2/event_engine/native/_topic_c.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       79 2024-05-28 11:03:38.760236 pyeventengine-0.3.0.post2/setup.cfg
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1736 2024-05-28 11:01:21.000000 pyeventengine-0.3.0.post2/setup.py
```

### Comparing `pyeventengine-0.3.0.post1/EventEngine/Core/__init__.py` & `pyeventengine-0.3.0.post2/event_engine/native/__init__.py`

 * *Files identical despite different names*

### Comparing `pyeventengine-0.3.0.post1/EventEngine/Core/_event.py` & `pyeventengine-0.3.0.post2/event_engine/native/_event.py`

 * *Files identical despite different names*

### Comparing `pyeventengine-0.3.0.post1/EventEngine/Core/_topic.py` & `pyeventengine-0.3.0.post2/event_engine/native/_topic.py`

 * *Files identical despite different names*

### Comparing `pyeventengine-0.3.0.post1/EventEngine/Core/_topic_c.py` & `pyeventengine-0.3.0.post2/event_engine/native/_topic_c.py`

 * *Files identical despite different names*

### Comparing `pyeventengine-0.3.0.post1/EventEngine/cpp/topic_api.cpp` & `pyeventengine-0.3.0.post2/event_engine/cpp/topic_api.cpp`

 * *Files identical despite different names*

### Comparing `pyeventengine-0.3.0.post1/LICENSE` & `pyeventengine-0.3.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyeventengine-0.3.0.post1/PKG-INFO` & `pyeventengine-0.3.0.post2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyEventEngine
-Version: 0.3.0.post1
+Version: 0.3.0.post2
 Summary: Basic event engine
 Home-page: https://github.com/BolunHan/PyEventEngine.git
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -35,15 +35,15 @@
 # Use
 
 ## basic usage
 
 ```python
 # init event engine
 import time
-from EventEngine import EventEngine, Topic
+from event_engine import EventEngine, Topic
 
 EVENT_ENGINE = EventEngine()
 EVENT_ENGINE.start()
 
 
 # register handler
 def test_handler(msg, **kwargs):
@@ -59,15 +59,15 @@
 ```
 
 ## regular topic
 
 ```python
 # init event engine
 import time
-from EventEngine import EventEngine, Topic, RegularTopic
+from event_engine import EventEngine, Topic, RegularTopic
 
 EVENT_ENGINE = EventEngine()
 EVENT_ENGINE.start()
 
 
 # register handler
 def test_handler(msg, **kwargs):
@@ -83,15 +83,15 @@
 ```
 
 ## timer topic
 
 ```python
 # init event engine
 import time
-from EventEngine import EventEngine, Topic, RegularTopic
+from event_engine import EventEngine, Topic, RegularTopic
 
 EVENT_ENGINE = EventEngine()
 EVENT_ENGINE.start()
 
 
 # register handler
 def test_handler(**kwargs):
```

### Comparing `pyeventengine-0.3.0.post1/PyEventEngine.egg-info/PKG-INFO` & `pyeventengine-0.3.0.post2/PyEventEngine.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyEventEngine
-Version: 0.3.0.post1
+Version: 0.3.0.post2
 Summary: Basic event engine
 Home-page: https://github.com/BolunHan/PyEventEngine.git
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -35,15 +35,15 @@
 # Use
 
 ## basic usage
 
 ```python
 # init event engine
 import time
-from EventEngine import EventEngine, Topic
+from event_engine import EventEngine, Topic
 
 EVENT_ENGINE = EventEngine()
 EVENT_ENGINE.start()
 
 
 # register handler
 def test_handler(msg, **kwargs):
@@ -59,15 +59,15 @@
 ```
 
 ## regular topic
 
 ```python
 # init event engine
 import time
-from EventEngine import EventEngine, Topic, RegularTopic
+from event_engine import EventEngine, Topic, RegularTopic
 
 EVENT_ENGINE = EventEngine()
 EVENT_ENGINE.start()
 
 
 # register handler
 def test_handler(msg, **kwargs):
@@ -83,15 +83,15 @@
 ```
 
 ## timer topic
 
 ```python
 # init event engine
 import time
-from EventEngine import EventEngine, Topic, RegularTopic
+from event_engine import EventEngine, Topic, RegularTopic
 
 EVENT_ENGINE = EventEngine()
 EVENT_ENGINE.start()
 
 
 # register handler
 def test_handler(**kwargs):
```

### Comparing `pyeventengine-0.3.0.post1/README.md` & `pyeventengine-0.3.0.post2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # Use
 
 ## basic usage
 
 ```python
 # init event engine
 import time
-from EventEngine import EventEngine, Topic
+from event_engine import EventEngine, Topic
 
 EVENT_ENGINE = EventEngine()
 EVENT_ENGINE.start()
 
 
 # register handler
 def test_handler(msg, **kwargs):
@@ -41,15 +41,15 @@
 ```
 
 ## regular topic
 
 ```python
 # init event engine
 import time
-from EventEngine import EventEngine, Topic, RegularTopic
+from event_engine import EventEngine, Topic, RegularTopic
 
 EVENT_ENGINE = EventEngine()
 EVENT_ENGINE.start()
 
 
 # register handler
 def test_handler(msg, **kwargs):
@@ -65,15 +65,15 @@
 ```
 
 ## timer topic
 
 ```python
 # init event engine
 import time
-from EventEngine import EventEngine, Topic, RegularTopic
+from event_engine import EventEngine, Topic, RegularTopic
 
 EVENT_ENGINE = EventEngine()
 EVENT_ENGINE.start()
 
 
 # register handler
 def test_handler(**kwargs):
```

### Comparing `pyeventengine-0.3.0.post1/setup.py` & `pyeventengine-0.3.0.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     raise RuntimeError("Unable to find version string.")
 
 
 long_description = read("README.md")
 
 setuptools.setup(
     name="PyEventEngine",
-    version=get_version(os.path.join('EventEngine', '__init__.py')),
+    version=get_version(os.path.join('event_engine', '__init__.py')),
     author="Bolun.Han",
     author_email="Bolun.Han@outlook.com",
     description="Basic event engine",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BolunHan/PyEventEngine.git",
     packages=setuptools.find_packages(),
@@ -44,10 +44,10 @@
         "Programming Language :: Python :: 3.12",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8',
     license='MIT',
     install_requires=[],
     ext_modules=[
-        setuptools.extension.Extension(r'EventEngine.topic_api', sources=[r'EventEngine/cpp/topic_api.cpp'], include_dirs=[], language='c++', optional=True),
+        setuptools.extension.Extension(r'event_engine.topic_api', sources=[r'event_engine/cpp/topic_api.cpp'], include_dirs=[], language='c++', optional=True),
     ],
 )
```

