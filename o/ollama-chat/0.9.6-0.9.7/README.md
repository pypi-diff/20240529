# Comparing `tmp/ollama_chat-0.9.6.tar.gz` & `tmp/ollama_chat-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ollama_chat-0.9.6.tar", last modified: Sun May 26 20:28:31 2024, max compression
+gzip compressed data, was "ollama_chat-0.9.7.tar", last modified: Tue May 28 23:42:18 2024, max compression
```

## Comparing `ollama_chat-0.9.6.tar` & `ollama_chat-0.9.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-26 20:28:31.780307 ollama_chat-0.9.6/
--rw-r--r--   0 craighobbs   (501) staff       (20)     1081 2024-05-02 18:06:38.000000 ollama_chat-0.9.6/LICENSE
--rw-r--r--   0 craighobbs   (501) staff       (20)     3375 2024-05-26 20:28:31.780242 ollama_chat-0.9.6/PKG-INFO
--rw-r--r--   0 craighobbs   (501) staff       (20)     2517 2024-05-26 18:14:23.000000 ollama_chat-0.9.6/README.md
--rw-r--r--   0 craighobbs   (501) staff       (20)       50 2024-05-02 18:06:38.000000 ollama_chat-0.9.6/pyproject.toml
--rw-r--r--   0 craighobbs   (501) staff       (20)     1059 2024-05-26 20:28:31.780551 ollama_chat-0.9.6/setup.cfg
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-26 20:28:31.777771 ollama_chat-0.9.6/src/
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-26 20:28:31.778776 ollama_chat-0.9.6/src/ollama_chat/
--rw-r--r--   0 craighobbs   (501) staff       (20)        0 2024-05-02 18:06:38.000000 ollama_chat-0.9.6/src/ollama_chat/__init__.py
--rw-r--r--   0 craighobbs   (501) staff       (20)      229 2024-05-02 18:06:38.000000 ollama_chat-0.9.6/src/ollama_chat/__main__.py
--rw-r--r--   0 craighobbs   (501) staff       (20)    12030 2024-05-24 19:11:33.000000 ollama_chat-0.9.6/src/ollama_chat/app.py
--rw-r--r--   0 craighobbs   (501) staff       (20)     3113 2024-05-26 18:10:53.000000 ollama_chat-0.9.6/src/ollama_chat/main.py
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-26 20:28:31.779858 ollama_chat-0.9.6/src/ollama_chat/static/
--rw-r--r--   0 craighobbs   (501) staff       (20)        0 2024-05-26 20:10:13.000000 ollama_chat-0.9.6/src/ollama_chat/static/__init__.py
--rw-r--r--   0 craighobbs   (501) staff       (20)     3774 2024-05-09 17:20:22.000000 ollama_chat-0.9.6/src/ollama_chat/static/index.html
--rw-r--r--   0 craighobbs   (501) staff       (20)    17665 2024-05-24 18:38:01.000000 ollama_chat-0.9.6/src/ollama_chat/static/ollamaChat.bare
--rw-r--r--   0 craighobbs   (501) staff       (20)     3506 2024-05-23 17:06:52.000000 ollama_chat-0.9.6/src/ollama_chat/static/ollamaChat.smd
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-26 20:28:31.780015 ollama_chat-0.9.6/src/ollama_chat.egg-info/
--rw-r--r--   0 craighobbs   (501) staff       (20)     3375 2024-05-26 20:28:31.000000 ollama_chat-0.9.6/src/ollama_chat.egg-info/PKG-INFO
--rw-r--r--   0 craighobbs   (501) staff       (20)      527 2024-05-26 20:28:31.000000 ollama_chat-0.9.6/src/ollama_chat.egg-info/SOURCES.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)        1 2024-05-26 20:28:31.000000 ollama_chat-0.9.6/src/ollama_chat.egg-info/dependency_links.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       54 2024-05-26 20:28:31.000000 ollama_chat-0.9.6/src/ollama_chat.egg-info/entry_points.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       44 2024-05-26 20:28:31.000000 ollama_chat-0.9.6/src/ollama_chat.egg-info/requires.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       12 2024-05-26 20:28:31.000000 ollama_chat-0.9.6/src/ollama_chat.egg-info/top_level.txt
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-28 23:42:18.168810 ollama_chat-0.9.7/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     1081 2024-05-28 18:40:18.000000 ollama_chat-0.9.7/LICENSE
+-rw-r--r--   0 craighobbs   (501) staff       (20)     3636 2024-05-28 23:42:18.168748 ollama_chat-0.9.7/PKG-INFO
+-rw-r--r--   0 craighobbs   (501) staff       (20)     2778 2024-05-28 23:39:17.000000 ollama_chat-0.9.7/README.md
+-rw-r--r--   0 craighobbs   (501) staff       (20)       50 2024-05-28 18:40:18.000000 ollama_chat-0.9.7/pyproject.toml
+-rw-r--r--   0 craighobbs   (501) staff       (20)     1059 2024-05-28 23:42:18.169088 ollama_chat-0.9.7/setup.cfg
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-28 23:42:18.165510 ollama_chat-0.9.7/src/
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-28 23:42:18.166844 ollama_chat-0.9.7/src/ollama_chat/
+-rw-r--r--   0 craighobbs   (501) staff       (20)        0 2024-05-28 18:40:18.000000 ollama_chat-0.9.7/src/ollama_chat/__init__.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)      229 2024-05-28 18:40:18.000000 ollama_chat-0.9.7/src/ollama_chat/__main__.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)    12030 2024-05-28 18:40:18.000000 ollama_chat-0.9.7/src/ollama_chat/app.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)     3113 2024-05-28 18:40:18.000000 ollama_chat-0.9.7/src/ollama_chat/main.py
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-28 23:42:18.168276 ollama_chat-0.9.7/src/ollama_chat/static/
+-rw-r--r--   0 craighobbs   (501) staff       (20)        0 2024-05-28 18:40:18.000000 ollama_chat-0.9.7/src/ollama_chat/static/__init__.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)     3774 2024-05-28 18:40:18.000000 ollama_chat-0.9.7/src/ollama_chat/static/index.html
+-rw-r--r--   0 craighobbs   (501) staff       (20)    18572 2024-05-28 23:35:44.000000 ollama_chat-0.9.7/src/ollama_chat/static/ollamaChat.bare
+-rw-r--r--   0 craighobbs   (501) staff       (20)     3506 2024-05-28 19:22:28.000000 ollama_chat-0.9.7/src/ollama_chat/static/ollamaChat.smd
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-28 23:42:18.168430 ollama_chat-0.9.7/src/ollama_chat.egg-info/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     3636 2024-05-28 23:42:18.000000 ollama_chat-0.9.7/src/ollama_chat.egg-info/PKG-INFO
+-rw-r--r--   0 craighobbs   (501) staff       (20)      527 2024-05-28 23:42:18.000000 ollama_chat-0.9.7/src/ollama_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)        1 2024-05-28 23:42:18.000000 ollama_chat-0.9.7/src/ollama_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       54 2024-05-28 23:42:18.000000 ollama_chat-0.9.7/src/ollama_chat.egg-info/entry_points.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       44 2024-05-28 23:42:18.000000 ollama_chat-0.9.7/src/ollama_chat.egg-info/requires.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       12 2024-05-28 23:42:18.000000 ollama_chat-0.9.7/src/ollama_chat.egg-info/top_level.txt
```

### Comparing `ollama_chat-0.9.6/LICENSE` & `ollama_chat-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.6/PKG-INFO` & `ollama_chat-0.9.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ollama-chat
-Version: 0.9.6
+Version: 0.9.7
 Summary: ollama-chat
 Home-page: https://github.com/craigahobbs/ollama-chat
 Author: Craig A. Hobbs
 Author-email: craigahobbs@gmail.com
 License: MIT
 Keywords: ollama-chat
 Classifier: Development Status :: 5 - Production/Stable
@@ -76,32 +76,41 @@
 To start a conversation from the command line, use the `-m` argument:
 
 ~~~
 ollama-chat -m "Why is the sky blue?"
 ~~~
 
 
-## Future
+## File Format and API Documentation
 
-- Multi-line text input
+[Ollama Chat File Format](https://craigahobbs.github.io/ollama-chat/api.html#var.vName='OllamaChatConfig')
+
+[Ollama Chat API](https://craigahobbs.github.io/ollama-chat/api.html)
+
+
+## Future
 
 - Save conversation as Markdown file
   - Save link on index/conversation page
 
+- Markdown text view on conversation page
+
 - Auto-title task on start conversation
   - Update conversation title API
   - Update title link on index/conversation page
 
 - Prompts part 1
   - Prompts config collection (name, title, prompt)
   - Index links start new conversation with current model
   - `-t` command-line argument starts prompt by name
 
 - File / Directory / URL text inclusion in prompt
 
+- Multi-line text input
+
 - Prompts part 2
   - Prompt editor
   - Create link on index page
   - Delete links on index page
   - Index links open template editor if any template markers (e.g. "{Name}")
 
 - Local model management (pull, rm)
```

### Comparing `ollama_chat-0.9.6/README.md` & `ollama_chat-0.9.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -51,32 +51,41 @@
 To start a conversation from the command line, use the `-m` argument:
 
 ~~~
 ollama-chat -m "Why is the sky blue?"
 ~~~
 
 
-## Future
+## File Format and API Documentation
 
-- Multi-line text input
+[Ollama Chat File Format](https://craigahobbs.github.io/ollama-chat/api.html#var.vName='OllamaChatConfig')
+
+[Ollama Chat API](https://craigahobbs.github.io/ollama-chat/api.html)
+
+
+## Future
 
 - Save conversation as Markdown file
   - Save link on index/conversation page
 
+- Markdown text view on conversation page
+
 - Auto-title task on start conversation
   - Update conversation title API
   - Update title link on index/conversation page
 
 - Prompts part 1
   - Prompts config collection (name, title, prompt)
   - Index links start new conversation with current model
   - `-t` command-line argument starts prompt by name
 
 - File / Directory / URL text inclusion in prompt
 
+- Multi-line text input
+
 - Prompts part 2
   - Prompt editor
   - Create link on index page
   - Delete links on index page
   - Index links open template editor if any template markers (e.g. "{Name}")
 
 - Local model management (pull, rm)
```

### Comparing `ollama_chat-0.9.6/setup.cfg` & `ollama_chat-0.9.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ollama-chat
-version = 0.9.6
+version = 0.9.7
 url = https://github.com/craigahobbs/ollama-chat
 author = Craig A. Hobbs
 author_email = craigahobbs@gmail.com
 license = MIT
 description = ollama-chat
 long_description = file:README.md
 long_description_content_type = text/markdown
```

### Comparing `ollama_chat-0.9.6/src/ollama_chat/app.py` & `ollama_chat-0.9.7/src/ollama_chat/app.py`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.6/src/ollama_chat/main.py` & `ollama_chat-0.9.7/src/ollama_chat/main.py`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.6/src/ollama_chat/static/index.html` & `ollama_chat-0.9.7/src/ollama_chat/static/index.html`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.6/src/ollama_chat/static/ollamaChat.bare` & `ollama_chat-0.9.7/src/ollama_chat/static/ollamaChat.bare`

 * *Files 6% similar despite different names*

```diff
@@ -365,32 +365,44 @@
 endfunction
 
 
 # The Ollama chat pages floating controls element model
 function ollamaChatPageFloatingElements(id, generating):
     elements = arrayNew()
 
+    # Compute spacing
+    fontSizePx = documentFontSize()
+    topSpacePx = mathFloor(1.5 * fontSizePx)
+    borderRadiusPx = mathFloor(0.5 * fontSizePx)
+    menuPadPx = mathFloor(0.75 * fontSizePx)
+    inputPadPx = fontSizePx
+    textPadPx = mathFloor(0.5 * fontSizePx)
+    buttonLeftRightPx = mathFloor(0.5 * fontSizePx)
+    buttonTopBottomPx = fontSizePx
+    topBottomPx = fontSizePx
+    leftRightPx = 2 * fontSizePx
+
     # The top space
-    arrayPush(elements, objectNew('html', 'div', 'attr', objectNew('style', 'height: 20px')))
+    arrayPush(elements, objectNew('html', 'div', 'attr', objectNew('style', 'height: ' + topSpacePx + 'px')))
 
     # The menu controls
     separator = stringFromCharCode(160) + '|' + stringFromCharCode(160)
     arrayPush(elements, objectNew( \
         'html', 'div', \
         'attr', objectNew( \
             'style', arrayJoin(arrayNew( \
                 'align-items: left', \
                 'background-color: #e0e0e0', \
-                'border-radius: 5px', \
+                'border-radius: ' + borderRadiusPx + 'px', \
                 'color: black', \
                 'display: flex', \
-                'left: 10px', \
-                'padding: 10px', \
+                'left: ' + topBottomPx + 'px', \
+                'padding: ' + menuPadPx + 'px', \
                 'position: fixed', \
-                'top: 10px' \
+                'top: ' + topBottomPx + 'px' \
             ), '; ') \
         ), \
         'elem', arrayNew( \
             formsLinkElements('Back', argsURL(ollamaChatArguments, null, true)), \
             if(!generating, arrayNew( \
                 objectNew('text', separator), \
                 formsLinkElements('Top', argsURL(ollamaChatArguments, null, false, '_top')), \
@@ -403,85 +415,90 @@
     # The prompt controls
     arrayPush(elements, objectNew( \
         'html', 'div', \
         'attr', objectNew( \
             'style', arrayJoin(arrayNew( \
                 'align-items: center', \
                 'background-color: #c0c0c0', \
-                'border-radius: 10px', \
-                'bottom: 30px', \
+                'border-radius: ' + borderRadiusPx + 'px', \
+                'bottom: ' + topBottomPx + 'px', \
                 'display: flex', \
-                'left: 50px', \
-                'padding: 15px', \
+                'left: ' + leftRightPx + 'px', \
+                'padding: ' + inputPadPx + 'px', \
                 'position: fixed', \
-                'right: 50px' \
+                'right: ' + leftRightPx + 'px' \
             ), '; ') \
         ), \
         'elem', arrayNew( \
             objectNew( \
                 'html', 'input', \
                 'attr', objectNew( \
                     'type', 'text', \
                     'id', ollamaChatPromptInputID, \
                     'placeholder', 'Type your message...', \
                     'style', arrayJoin(arrayNew( \
                         'background-color: white', \
                         'border: none', \
                         'flex: 1', \
                         'font-size: inherit', \
-                        'margin-right: 10px', \
+                        'margin-right: ' + textPadPx + 'px', \
+                        'min-width: 0', \
                         'outline: none', \
-                        'padding: 10px' \
+                        'padding: ' + textPadPx + 'px' \
                     ), '; ') \
                 ), \
                 'callback', objectNew('keyup', systemPartial(formsTextOnKeyup, systemPartial(ollamaChatOnPrompt, id))) \
             ), \
             if(!generating, objectNew( \
                 'html', 'button', \
                 'attr', objectNew( \
                     'style', arrayJoin(arrayNew( \
                         'background-color: #4dff4d', \
-                        'border-radius: 4px', \
+                        'border-radius: ' + borderRadiusPx + 'px', \
                         'border: none', \
                         'color: black', \
                         'font-size: inherit', \
-                        'padding: 10px 20px' \
+                        'padding: ' + buttonLeftRightPx + 'px ' + buttonTopBottomPx + 'px' \
                     ), '; ') \
                 ), \
                 'elem', objectNew('text', 'Go'), \
                 'callback', objectNew('click', systemPartial(ollamaChatOnPrompt, id)) \
             )), \
             if(generating, objectNew( \
                 'html', 'button', \
                 'attr', objectNew( \
                     'style', arrayJoin(arrayNew( \
                         'background-color: #ff4d4d', \
-                        'border-radius: 4px', \
+                        'border-radius: ' + borderRadiusPx + 'px', \
                         'border: none', \
                         'color: white', \
                         'font-size: inherit', \
-                        'padding: 10px 20px' \
+                        'padding: ' + buttonLeftRightPx + 'px ' + buttonTopBottomPx + 'px' \
                     ), '; ') \
                 ), \
                 'elem', objectNew('text', 'Stop'), \
                 'callback', objectNew('click', systemPartial(ollamaChatOnConversationClick, id, 'stopConversation')) \
             )) \
         ) \
     ))
 
     return elements
 endfunction
 
 
-# The Ollama chat pages floating controls bottom-of-the-window space div element model
+# The Ollama Chat page's bottom-of-the-window space div element model
 function ollamaChatPageFloatingBottomElements():
     elements = arrayNew()
 
+    # Compute spacing
+    fontSizePx = documentFontSize()
+    bottomSpacePx = mathFloor(4.5 * fontSizePx)
+
     # Add the bottom space
-    arrayPush(elements, objectNew('html', 'div', 'attr', objectNew('style', 'height: 90px')))
+    arrayPush(elements, objectNew('html', 'div', 'attr', objectNew('style', 'height: ' + bottomSpacePx + 'px')))
 
     # Add the bottom document ID
     bottomElementId = stringSlice(argsURL(ollamaChatArguments, null, false, ollamaChatBottomID), 1)
     arrayPush(elements, objectNew('html', 'div', 'attr', objectNew('id', bottomElementId)))
 
     return elements
 endfunction
```

### Comparing `ollama_chat-0.9.6/src/ollama_chat/static/ollamaChat.smd` & `ollama_chat-0.9.7/src/ollama_chat/static/ollamaChat.smd`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,31 @@
 # Licensed under the MIT License
 # https://github.com/craigahobbs/ollama-chat/blob/main/LICENSE
 
 
-group "Ollama Chat JSON"
-
-
-# The Ollama Chat config file format
-struct OllamaChatConfig
-
-    # The current model name
-    optional string model
-
-    # The saved conversations
-    Conversation[] conversations
-
-    # If true, don't save the config file
-    optional bool noSave
-
-
 # The user-model conversation info
 struct ConversationInfo
 
     # The conversation identifier
     string id
 
     # The model name
     string model
 
     # The conversation title
     string title
 
 
+# Conversation information struct with generating state
+struct ConversationInfoEx (ConversationInfo)
+
+    # If True, the latest exchange is actively generating
+    bool generating
+
+
 # A user-model conversation
 struct Conversation (ConversationInfo)
 
     # The conversation's exchanges
     ConversationExchange[len > 0] exchanges
 
 
@@ -44,37 +35,53 @@
     # The user prompt
     string(len > 0) user
 
     # The model response
     string model
 
 
+# Model information struct
+struct ModelInfo
+
+    # The current model name
+    string model
+
+    # The model size, in bytes
+    int size
+
+
+group "Ollama Chat JSON"
+
+
+# The Ollama Chat config file format
+struct OllamaChatConfig
+
+    # The current model name
+    optional string model
+
+    # The saved conversations
+    Conversation[] conversations
+
+    # If true, don't save the config file
+    optional bool noSave
+
+
 group "Ollama Chat API"
 
 
 # Get the current model name
 action getModels
     urls
         GET
 
     output
         # The local models
         ModelInfo[] models
 
 
-# Model information struct
-struct ModelInfo
-
-    # The current model name
-    string model
-
-    # The model size, in bytes
-    int size
-
-
 # Get the current model name
 action getModel
     urls
         GET
 
     output
         # The current model name
@@ -97,21 +104,14 @@
         GET
 
     output
         # The conversations
         ConversationInfoEx[] conversations
 
 
-# Conversation information struct with generating state
-struct ConversationInfoEx (ConversationInfo)
-
-    # If True, the latest exchange is actively generating
-    bool generating
-
-
 # Start a conversation
 action startConversation
     urls
         POST
 
     input
         # The user prompt
```

### Comparing `ollama_chat-0.9.6/src/ollama_chat.egg-info/PKG-INFO` & `ollama_chat-0.9.7/src/ollama_chat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ollama-chat
-Version: 0.9.6
+Version: 0.9.7
 Summary: ollama-chat
 Home-page: https://github.com/craigahobbs/ollama-chat
 Author: Craig A. Hobbs
 Author-email: craigahobbs@gmail.com
 License: MIT
 Keywords: ollama-chat
 Classifier: Development Status :: 5 - Production/Stable
@@ -76,32 +76,41 @@
 To start a conversation from the command line, use the `-m` argument:
 
 ~~~
 ollama-chat -m "Why is the sky blue?"
 ~~~
 
 
-## Future
+## File Format and API Documentation
 
-- Multi-line text input
+[Ollama Chat File Format](https://craigahobbs.github.io/ollama-chat/api.html#var.vName='OllamaChatConfig')
+
+[Ollama Chat API](https://craigahobbs.github.io/ollama-chat/api.html)
+
+
+## Future
 
 - Save conversation as Markdown file
   - Save link on index/conversation page
 
+- Markdown text view on conversation page
+
 - Auto-title task on start conversation
   - Update conversation title API
   - Update title link on index/conversation page
 
 - Prompts part 1
   - Prompts config collection (name, title, prompt)
   - Index links start new conversation with current model
   - `-t` command-line argument starts prompt by name
 
 - File / Directory / URL text inclusion in prompt
 
+- Multi-line text input
+
 - Prompts part 2
   - Prompt editor
   - Create link on index page
   - Delete links on index page
   - Index links open template editor if any template markers (e.g. "{Name}")
 
 - Local model management (pull, rm)
```

### Comparing `ollama_chat-0.9.6/src/ollama_chat.egg-info/SOURCES.txt` & `ollama_chat-0.9.7/src/ollama_chat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

