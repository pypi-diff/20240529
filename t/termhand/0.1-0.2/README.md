# Comparing `tmp/termhand-0.1.tar.gz` & `tmp/termhand-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termhand-0.1.tar", last modified: Wed May 29 17:19:23 2024, max compression
+gzip compressed data, was "termhand-0.2.tar", last modified: Wed May 29 17:41:25 2024, max compression
```

## Comparing `termhand-0.1.tar` & `termhand-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 adarsh    (1000) adarsh    (1000)        0 2024-05-29 17:19:23.915138 termhand-0.1/
--rw-r--r--   0 adarsh    (1000) adarsh    (1000)       85 2024-05-29 17:19:23.915138 termhand-0.1/PKG-INFO
-drwxr-xr-x   0 adarsh    (1000) adarsh    (1000)        0 2024-05-29 17:19:23.915138 termhand-0.1/TermHand.egg-info/
--rw-r--r--   0 adarsh    (1000) adarsh    (1000)       85 2024-05-29 17:19:23.000000 termhand-0.1/TermHand.egg-info/PKG-INFO
--rw-r--r--   0 adarsh    (1000) adarsh    (1000)      208 2024-05-29 17:19:23.000000 termhand-0.1/TermHand.egg-info/SOURCES.txt
--rw-r--r--   0 adarsh    (1000) adarsh    (1000)        1 2024-05-29 17:19:23.000000 termhand-0.1/TermHand.egg-info/dependency_links.txt
--rw-r--r--   0 adarsh    (1000) adarsh    (1000)       31 2024-05-29 17:19:23.000000 termhand-0.1/TermHand.egg-info/entry_points.txt
--rw-r--r--   0 adarsh    (1000) adarsh    (1000)       20 2024-05-29 17:19:23.000000 termhand-0.1/TermHand.egg-info/requires.txt
--rw-r--r--   0 adarsh    (1000) adarsh    (1000)        3 2024-05-29 17:19:23.000000 termhand-0.1/TermHand.egg-info/top_level.txt
--rw-r--r--   0 adarsh    (1000) adarsh    (1000)       38 2024-05-29 17:19:23.915138 termhand-0.1/setup.cfg
--rw-r--r--   0 adarsh    (1000) adarsh    (1000)      238 2024-05-29 17:19:01.000000 termhand-0.1/setup.py
--rwxr-xr-x   0 adarsh    (1000) adarsh    (1000)     2247 2024-05-29 14:10:50.000000 termhand-0.1/th.py
+drwxr-xr-x   0 adarsh    (1000) adarsh    (1000)        0 2024-05-29 17:41:25.414958 termhand-0.2/
+-rw-r--r--   0 adarsh    (1000) adarsh    (1000)       85 2024-05-29 17:41:25.414958 termhand-0.2/PKG-INFO
+drwxr-xr-x   0 adarsh    (1000) adarsh    (1000)        0 2024-05-29 17:41:25.414958 termhand-0.2/TermHand.egg-info/
+-rw-r--r--   0 adarsh    (1000) adarsh    (1000)       85 2024-05-29 17:41:25.000000 termhand-0.2/TermHand.egg-info/PKG-INFO
+-rw-r--r--   0 adarsh    (1000) adarsh    (1000)      208 2024-05-29 17:41:25.000000 termhand-0.2/TermHand.egg-info/SOURCES.txt
+-rw-r--r--   0 adarsh    (1000) adarsh    (1000)        1 2024-05-29 17:41:25.000000 termhand-0.2/TermHand.egg-info/dependency_links.txt
+-rw-r--r--   0 adarsh    (1000) adarsh    (1000)       31 2024-05-29 17:41:25.000000 termhand-0.2/TermHand.egg-info/entry_points.txt
+-rw-r--r--   0 adarsh    (1000) adarsh    (1000)       20 2024-05-29 17:41:25.000000 termhand-0.2/TermHand.egg-info/requires.txt
+-rw-r--r--   0 adarsh    (1000) adarsh    (1000)        3 2024-05-29 17:41:25.000000 termhand-0.2/TermHand.egg-info/top_level.txt
+-rw-r--r--   0 adarsh    (1000) adarsh    (1000)       38 2024-05-29 17:41:25.414958 termhand-0.2/setup.cfg
+-rw-r--r--   0 adarsh    (1000) adarsh    (1000)      238 2024-05-29 17:41:04.000000 termhand-0.2/setup.py
+-rwxr-xr-x   0 adarsh    (1000) adarsh    (1000)     2825 2024-05-29 17:36:36.000000 termhand-0.2/th.py
```

### Comparing `termhand-0.1/th.py` & `termhand-0.2/th.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 #!/usr/bin/env python3
 
+import os
+import configparser
 import argparse
 import google.generativeai as genai
 import subprocess
 
 
 def main():
     prompt = get_prompt()
-    message = f'You have to send the exact command for me to directly copy paste in my linux terminal and use it based on the given request. Don\'t even format with backticks of markdown like syntax. Simply return the command in response. Given request is: "{prompt}"'
 
-    chat = get_chat()
+    api_key = get_api_key()
+    if not api_key:
+        print(
+            "Error: API Key not found. Please make sure it is configured in the configuration file."
+        )
+        return
+
+    chat = get_chat(api_key)
+    message = f'You have to send the exact command for me to directly copy paste in my linux terminal and use it based on the given request. Don\'t even format with backticks of markdown like syntax. Simply return the command in response. Given request is: "{prompt}"'
     response = chat.send_message(message)
     command = response.parts[0].text.rstrip()
 
     print(f"Generated command: {command}")
     confirm = input("Do you want to execute the command? (Y/n): ").strip().lower()
 
     if confirm == "y" or confirm == "":
@@ -30,16 +39,16 @@
         description="Generate terminal command from natural language prompt"
     )
     parser.add_argument("prompt", type=str, help="The natural language prompt")
     args = parser.parse_args()
     return args.prompt
 
 
-def get_chat():
-    genai.configure(api_key="AIzaSyBNJUJE-wyez78Aj3aoTZNX281GJrI948A")
+def get_chat(key):
+    genai.configure(api_key=key)
 
     generation_config = {
         "temperature": 1,
         "top_p": 0.95,
         "top_k": 64,
         "max_output_tokens": 8192,
         "response_mime_type": "text/plain",
@@ -70,9 +79,22 @@
         generation_config=generation_config,
     )
 
     chat = model.start_chat()
     return chat
 
 
+def get_api_key():
+    config_file_path = os.path.expanduser("~/.config/termhand/termhand_config.ini")
+    if not os.path.exists(config_file_path):
+        return None
+
+    config = configparser.ConfigParser()
+    config.read(config_file_path)
+    if "termhand" in config and "api_key" in config["termhand"]:
+        return config["termhand"]["api_key"]
+    else:
+        return None
+
+
 if __name__ == "__main__":
     main()
```

