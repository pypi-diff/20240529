# Comparing `tmp/stream-chat-4.8.0.tar.gz` & `tmp/stream-chat-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stream-chat-4.8.0.tar", last modified: Wed May  3 11:44:51 2023, max compression
+gzip compressed data, was "stream-chat-4.9.0.tar", last modified: Fri Jul 21 15:24:00 2023, max compression
```

## Comparing `stream-chat-4.8.0.tar` & `stream-chat-4.9.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:44:51.773857 stream-chat-4.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    14424 2023-05-03 11:44:41.000000 stream-chat-4.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 11:44:41.000000 stream-chat-4.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-05-03 11:44:51.769857 stream-chat-4.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-05-03 11:44:41.000000 stream-chat-4.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-03 11:44:41.000000 stream-chat-4.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 11:44:51.773857 stream-chat-4.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-03 11:44:41.000000 stream-chat-4.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:44:51.765857 stream-chat-4.8.0/stream_chat/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-03 11:44:41.000000 stream-chat-4.8.0/stream_chat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-03 11:44:41.000000 stream-chat-4.8.0/stream_chat/__pkg__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:44:51.769857 stream-chat-4.8.0/stream_chat/async_chat/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-03 11:44:41.000000 stream-chat-4.8.0/stream_chat/async_chat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-05-03 11:44:41.000000 stream-chat-4.8.0/stream_chat/async_chat/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    26000 2023-05-03 11:44:41.000000 stream-chat-4.8.0/stream_chat/async_chat/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:44:51.769857 stream-chat-4.8.0/stream_chat/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 11:44:41.000000 stream-chat-4.8.0/stream_chat/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13788 2023-05-03 11:44:41.000000 stream-chat-4.8.0/stream_chat/base/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    37384 2023-05-03 11:44:41.000000 stream-chat-4.8.0/stream_chat/base/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-03 11:44:41.000000 stream-chat-4.8.0/stream_chat/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-05-03 11:44:41.000000 stream-chat-4.8.0/stream_chat/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    23816 2023-05-03 11:44:41.000000 stream-chat-4.8.0/stream_chat/client.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 11:44:41.000000 stream-chat-4.8.0/stream_chat/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:44:51.769857 stream-chat-4.8.0/stream_chat/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 11:44:41.000000 stream-chat-4.8.0/stream_chat/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-03 11:44:41.000000 stream-chat-4.8.0/stream_chat/types/rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-03 11:44:41.000000 stream-chat-4.8.0/stream_chat/types/stream_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:44:51.769857 stream-chat-4.8.0/stream_chat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-05-03 11:44:51.000000 stream-chat-4.8.0/stream_chat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-03 11:44:51.000000 stream-chat-4.8.0/stream_chat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 11:44:51.000000 stream-chat-4.8.0/stream_chat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 11:44:51.000000 stream-chat-4.8.0/stream_chat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-03 11:44:51.000000 stream-chat-4.8.0/stream_chat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 11:44:51.000000 stream-chat-4.8.0/stream_chat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:24:00.064748 stream-chat-4.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    14424 2023-07-21 15:23:48.000000 stream-chat-4.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-21 15:23:48.000000 stream-chat-4.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-07-21 15:24:00.064748 stream-chat-4.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-21 15:23:48.000000 stream-chat-4.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-21 15:23:48.000000 stream-chat-4.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 15:24:00.064748 stream-chat-4.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-21 15:23:48.000000 stream-chat-4.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:24:00.060748 stream-chat-4.9.0/stream_chat/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-21 15:23:48.000000 stream-chat-4.9.0/stream_chat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-21 15:23:48.000000 stream-chat-4.9.0/stream_chat/__pkg__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:24:00.064748 stream-chat-4.9.0/stream_chat/async_chat/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-21 15:23:48.000000 stream-chat-4.9.0/stream_chat/async_chat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-21 15:23:48.000000 stream-chat-4.9.0/stream_chat/async_chat/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26000 2023-07-21 15:23:48.000000 stream-chat-4.9.0/stream_chat/async_chat/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:24:00.064748 stream-chat-4.9.0/stream_chat/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:48.000000 stream-chat-4.9.0/stream_chat/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13788 2023-07-21 15:23:48.000000 stream-chat-4.9.0/stream_chat/base/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37384 2023-07-21 15:23:48.000000 stream-chat-4.9.0/stream_chat/base/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-21 15:23:48.000000 stream-chat-4.9.0/stream_chat/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-07-21 15:23:48.000000 stream-chat-4.9.0/stream_chat/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-07-21 15:23:48.000000 stream-chat-4.9.0/stream_chat/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:48.000000 stream-chat-4.9.0/stream_chat/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:24:00.064748 stream-chat-4.9.0/stream_chat/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:48.000000 stream-chat-4.9.0/stream_chat/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-21 15:23:48.000000 stream-chat-4.9.0/stream_chat/types/rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-21 15:23:48.000000 stream-chat-4.9.0/stream_chat/types/stream_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:24:00.064748 stream-chat-4.9.0/stream_chat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-07-21 15:24:00.000000 stream-chat-4.9.0/stream_chat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-21 15:24:00.000000 stream-chat-4.9.0/stream_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:24:00.000000 stream-chat-4.9.0/stream_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:24:00.000000 stream-chat-4.9.0/stream_chat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-21 15:24:00.000000 stream-chat-4.9.0/stream_chat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 15:24:00.000000 stream-chat-4.9.0/stream_chat.egg-info/top_level.txt
```

### Comparing `stream-chat-4.8.0/LICENSE` & `stream-chat-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stream-chat-4.8.0/PKG-INFO` & `stream-chat-4.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: stream-chat
-Version: 4.8.0
+Version: 4.9.0
 Summary: Client for Stream Chat.
 Home-page: https://github.com/GetStream/stream-chat-python
 Author: Tommaso Barbugli
 Author-email: support@getstream.io
 Project-URL: Bug Tracker, https://github.com/GetStream/stream-chat-python/issues
 Project-URL: Documentation, https://getstream.io/activity-feeds/docs/python/?language=python
-Project-URL: Release Notes, https://github.com/GetStream/stream-chat-python/releases/tag/v4.8.0
+Project-URL: Release Notes, https://github.com/GetStream/stream-chat-python/releases/tag/v4.9.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: stream-chat Version: 4.8.0 Summary: Client for
+Metadata-Version: 2.1 Name: stream-chat Version: 4.9.0 Summary: Client for
 Stream Chat. Home-page: https://github.com/GetStream/stream-chat-python Author:
 Tommaso Barbugli Author-email: support@getstream.io Project-URL: Bug Tracker,
 https://github.com/GetStream/stream-chat-python/issues Project-URL:
 Documentation, https://getstream.io/activity-feeds/docs/python/?language=python
 Project-URL: Release Notes, https://github.com/GetStream/stream-chat-python/
-releases/tag/v4.8.0 Classifier: Intended Audience :: Developers Classifier:
+releases/tag/v4.9.0 Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: System Administrators Classifier: Operating System :: OS
 Independent Classifier: Topic :: Software Development Classifier: Development
 Status :: 5 - Production/Stable Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Topic :: Software Development ::
```

### Comparing `stream-chat-4.8.0/README.md` & `stream-chat-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `stream-chat-4.8.0/pyproject.toml` & `stream-chat-4.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stream-chat-4.8.0/setup.py` & `stream-chat-4.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `stream-chat-4.8.0/stream_chat/async_chat/channel.py` & `stream-chat-4.9.0/stream_chat/async_chat/channel.py`

 * *Files identical despite different names*

### Comparing `stream-chat-4.8.0/stream_chat/async_chat/client.py` & `stream-chat-4.9.0/stream_chat/async_chat/client.py`

 * *Files identical despite different names*

### Comparing `stream-chat-4.8.0/stream_chat/base/channel.py` & `stream-chat-4.9.0/stream_chat/base/channel.py`

 * *Files identical despite different names*

### Comparing `stream-chat-4.8.0/stream_chat/base/client.py` & `stream-chat-4.9.0/stream_chat/base/client.py`

 * *Files identical despite different names*

### Comparing `stream-chat-4.8.0/stream_chat/base/exceptions.py` & `stream-chat-4.9.0/stream_chat/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `stream-chat-4.8.0/stream_chat/channel.py` & `stream-chat-4.9.0/stream_chat/channel.py`

 * *Files identical despite different names*

### Comparing `stream-chat-4.8.0/stream_chat/client.py` & `stream-chat-4.9.0/stream_chat/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,14 +268,17 @@
         return self.post("channels/read", data={"user": {"id": user_id}})
 
     def translate_message(self, message_id: str, language: str) -> StreamResponse:
         return self.post(
             f"messages/{message_id}/translate", data={"language": language}
         )
 
+    def commit_message(self, message_id: str) -> StreamResponse:
+        return self.post(f"messages/{message_id}/commit")
+
     def pin_message(
         self, message_id: str, user_id: str, expiration: int = None
     ) -> StreamResponse:
         updates = {
             "set": {
                 "pinned": True,
                 "pin_expires": expiration,
```

### Comparing `stream-chat-4.8.0/stream_chat/types/stream_response.py` & `stream-chat-4.9.0/stream_chat/types/stream_response.py`

 * *Files identical despite different names*

### Comparing `stream-chat-4.8.0/stream_chat.egg-info/PKG-INFO` & `stream-chat-4.9.0/stream_chat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: stream-chat
-Version: 4.8.0
+Version: 4.9.0
 Summary: Client for Stream Chat.
 Home-page: https://github.com/GetStream/stream-chat-python
 Author: Tommaso Barbugli
 Author-email: support@getstream.io
 Project-URL: Bug Tracker, https://github.com/GetStream/stream-chat-python/issues
 Project-URL: Documentation, https://getstream.io/activity-feeds/docs/python/?language=python
-Project-URL: Release Notes, https://github.com/GetStream/stream-chat-python/releases/tag/v4.8.0
+Project-URL: Release Notes, https://github.com/GetStream/stream-chat-python/releases/tag/v4.9.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: stream-chat Version: 4.8.0 Summary: Client for
+Metadata-Version: 2.1 Name: stream-chat Version: 4.9.0 Summary: Client for
 Stream Chat. Home-page: https://github.com/GetStream/stream-chat-python Author:
 Tommaso Barbugli Author-email: support@getstream.io Project-URL: Bug Tracker,
 https://github.com/GetStream/stream-chat-python/issues Project-URL:
 Documentation, https://getstream.io/activity-feeds/docs/python/?language=python
 Project-URL: Release Notes, https://github.com/GetStream/stream-chat-python/
-releases/tag/v4.8.0 Classifier: Intended Audience :: Developers Classifier:
+releases/tag/v4.9.0 Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: System Administrators Classifier: Operating System :: OS
 Independent Classifier: Topic :: Software Development Classifier: Development
 Status :: 5 - Production/Stable Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Topic :: Software Development ::
```

### Comparing `stream-chat-4.8.0/stream_chat.egg-info/SOURCES.txt` & `stream-chat-4.9.0/stream_chat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

