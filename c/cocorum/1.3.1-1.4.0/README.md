# Comparing `tmp/cocorum-1.3.1.tar.gz` & `tmp/cocorum-1.4.0.tar.gz`

## Comparing `cocorum-1.3.1.tar` & `cocorum-1.4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0   343002 2020-02-02 00:00:00.000000 cocorum-1.3.1/cocorum_icon.png
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cocorum-1.3.1/requirements.txt
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 cocorum-1.3.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    21108 2020-02-02 00:00:00.000000 cocorum-1.3.1/src/cocorum/__init__.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 cocorum-1.3.1/src/cocorum/localvars.py
--rw-r--r--   0        0        0    13591 2020-02-02 00:00:00.000000 cocorum-1.3.1/src/cocorum/ssechat.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 cocorum-1.3.1/src/cocorum/utils.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cocorum-1.3.1/LICENSE.txt
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 cocorum-1.3.1/README.md
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 cocorum-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 cocorum-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0   343002 2020-02-02 00:00:00.000000 cocorum-1.4.0/cocorum_icon.png
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cocorum-1.4.0/requirements.txt
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 cocorum-1.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    21108 2020-02-02 00:00:00.000000 cocorum-1.4.0/src/cocorum/__init__.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 cocorum-1.4.0/src/cocorum/localvars.py
+-rw-r--r--   0        0        0    14382 2020-02-02 00:00:00.000000 cocorum-1.4.0/src/cocorum/ssechat.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 cocorum-1.4.0/src/cocorum/utils.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cocorum-1.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 cocorum-1.4.0/README.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 cocorum-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 cocorum-1.4.0/PKG-INFO
```

### Comparing `cocorum-1.3.1/cocorum_icon.png` & `cocorum-1.4.0/cocorum_icon.png`

 * *Files identical despite different names*

### Comparing `cocorum-1.3.1/.github/workflows/python-publish.yml` & `cocorum-1.4.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cocorum-1.3.1/src/cocorum/__init__.py` & `cocorum-1.4.0/src/cocorum/__init__.py`

 * *Files identical despite different names*

### Comparing `cocorum-1.3.1/src/cocorum/localvars.py` & `cocorum-1.4.0/src/cocorum/localvars.py`

 * *Files 23% similar despite different names*

```diff
@@ -47,7 +47,21 @@
 BADGE_ICON_SIZE = "48"
 
 #How long to wait before giving up on a network request, in seconds
 DEFAULT_TIMEOUT = 20
 
 #How long to reuse old data from the API, in seconds
 DEFAULT_REFRESH_RATE = 10
+
+#Dictionary of badge slugs mapped to UTF-8 glyphs
+BADGES_AS_GLYPHS = {
+    "verified" : "✅",
+    "admin" : "👑",
+    "moderator" : "🛡",
+    "premium" : "🗲",
+    "locals" : "♖",
+    "recurring_subscription" : "♖",
+    "locals_supporter" : "⛋",
+    "whale-grey" : "🐳",
+    "whale-yellow" : "🐳",
+    "whale-blue" : "🐳",
+    }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cocorum-1.3.1/src/cocorum/ssechat.py` & `cocorum-1.4.0/src/cocorum/ssechat.py`

 * *Files 6% similar despite different names*

```diff
@@ -162,18 +162,26 @@
         if isinstance(other, str):
             return self.text == other
 
         #Check if the other object's text matches our own, if it has such
         if hasattr(other, "text"):
             #Check if the other object's user ID matches our own, if it has one
             if hasattr(other, "user_id"):
+                #Check if the other object is a raid notification, if it says
+                if hasattr(other, "raid_notification"):
+                    return (self.user_id, self.text, self.raid_notification) == (other.user_id, other.text, other.raid_notification)
+
                 return (self.user_id, self.text) == (other.user_id, other.text)
 
             #Check if the other object's username matches our own, if it has one
             if hasattr(other, "username"):
+                #Check if the other object is a raid notification, if it says
+                if hasattr(other, "raid_notification"):
+                    return (self.user_id, self.text, self.raid_notification) == (other.user_id, other.text, other.raid_notification)
+
                 return (self.user.username, self.text) == (other.username, other.text)
 
             #No user identifying attributes, but the text does match
             return self.text == other.text
 
     def __str__(self):
         """The chat message in string form"""
@@ -219,15 +227,15 @@
             return None
 
         return self.chat.channels[self.channel_id]
 
     @property
     def is_rant(self):
         """Is this message a rant?"""
-        return "rant" in self._jsondata.keys()
+        return "rant" in self._jsondata
 
     @property
     def rant_price_cents(self):
         """The price of the rant, returns 0 if message is not a rant"""
         if not self.is_rant:
             return 0
         return self["rant"]["price_cents"]
@@ -242,14 +250,22 @@
     @property
     def rant_expires_on(self):
         """When the rant expires, returns message creation time if message is not a rant"""
         if not self.is_rant:
             return self.time
         return utils.parse_timestamp(self["rant"]["expires_on"])
 
+    @property
+    def raid_notification(self):
+        """Are we a raid notification? Returns associated JSON data if yes, False if no"""
+        if "raid_notification" in self._jsondata:
+            return self["raid_notification"]
+
+        return False
+
 class SSEChat():
     """Access the Rumble SSE chat api"""
     def __init__(self, stream_id):
         self.stream_id = utils.stream_id_ensure_b36(stream_id)
 
         self.__mailbox = [] #A mailbox if you will
         self.deleted_message_ids = [] #IDs of messages that were deleted, as reported by the client
@@ -359,15 +375,15 @@
 
             #Re-initialize (could contain new messages)
             elif jsondata["type"] == "init":
                 self.parse_init_data(jsondata)
 
             #Pinned message
             elif jsondata["type"] == "pin_message":
-                self.pinned_message = SSEChatMessage(jsondata["data"]["message"])
+                self.pinned_message = SSEChatMessage(jsondata["data"]["message"], self)
 
             #New messages
             elif jsondata["type"] == "messages":
                 #Parse messages, users, and channels
                 self.update_mailbox(jsondata)
                 self.update_users(jsondata)
                 self.update_channels(jsondata)
```

### Comparing `cocorum-1.3.1/src/cocorum/utils.py` & `cocorum-1.4.0/src/cocorum/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -53,7 +53,18 @@
     """No matter wether a stream ID is base 36 or 10, return 10"""
     #It is base 10
     if isinstance(stream_id, int) or (isinstance(stream_id, str) and stream_id.isnumeric()):
         return int(stream_id)
 
     #It is base 36:
     return stream_id_36_to_10(stream_id)
+
+def badges_to_glyph_string(badges):
+    """Convert a list of badges into a string of glyphs"""
+    out = ""
+    for badge in badges:
+        badge = str(badge)
+        if badge in BADGES_AS_GLYPHS:
+            out += BADGES_AS_GLYPHS[badge]
+        else:
+            out += "?"
+    return out
```

### Comparing `cocorum-1.3.1/LICENSE.txt` & `cocorum-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cocorum-1.3.1/README.md` & `cocorum-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cocorum-1.3.1/pyproject.toml` & `cocorum-1.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cocorum"
-version = "1.3.1"
+version = "1.4.0"
 keywords = ["rumble", "api", "wrapper", "livestream"]
 authors = [
   { name="Wilbur Jaywright", email="zargulthewizard@outlook.com" },
 ]
 description = "An unofficial Python wrapper for the Rumble Live Stream API v1.0 (beta)"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `cocorum-1.3.1/PKG-INFO` & `cocorum-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cocorum
-Version: 1.3.1
+Version: 1.4.0
 Summary: An unofficial Python wrapper for the Rumble Live Stream API v1.0 (beta)
 Project-URL: Homepage, https://github.com/thelabcat/rumble-api-wrapper-py
 Project-URL: Issues, https://github.com/thelabcat/rumble-api-wrapper-py/issues
 Project-URL: Rumble Live Stream API docs, https://rumblefaq.groovehq.com/help/how-to-use-rumble-s-live-stream-api
 Author-email: Wilbur Jaywright <zargulthewizard@outlook.com>
 License-File: LICENSE.txt
 Keywords: api,livestream,rumble,wrapper
```

