# Comparing `tmp/django_openai_assistant-0.5.2.tar.gz` & `tmp/django_openai_assistant-0.5.3.tar.gz`

## Comparing `django_openai_assistant-0.5.2.tar` & `django_openai_assistant-0.5.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.2/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.2/src/django_openai_assistant/__init__.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.2/src/django_openai_assistant/apps.py
--rw-r--r--   0        0        0    18912 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.2/src/django_openai_assistant/assistant.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.2/src/django_openai_assistant/models.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.2/src/django_openai_assistant/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.2/src/django_openai_assistant/migrations/__init__.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.2/LICENSE
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.2/README.md
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.3/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.3/src/django_openai_assistant/__init__.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.3/src/django_openai_assistant/apps.py
+-rw-r--r--   0        0        0    20016 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.3/src/django_openai_assistant/assistant.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.3/src/django_openai_assistant/models.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.3/src/django_openai_assistant/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.3/src/django_openai_assistant/migrations/__init__.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.3/LICENSE
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.3/README.md
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 django_openai_assistant-0.5.3/PKG-INFO
```

### Comparing `django_openai_assistant-0.5.2/src/django_openai_assistant/assistant.py` & `django_openai_assistant-0.5.3/src/django_openai_assistant/assistant.py`

 * *Files 6% similar despite different names*

```diff
@@ -295,30 +295,45 @@
             return self._metadata
     
     @metadata.setter
     def metadata(self, value):
         self._metadata = value
         
     @prompt.setter
-    def prompt(self, message):
-        att = [
-            {
+    def prompt(self, message:str):
+        att = []
+        visions = []
+        for file in self._fileids:
+            if file['vision']:
+                visions.append(file['id'])
+                continue
+            elif file['retrieval']:
+                tools = [{'type': 'file_search'}]
+            else:
+                tools = [{'type': 'code_interpreter'}]            
+            att.append( {
                 'file_id': file['id'],
-                'tools': [{'type': 'file_search'}] if file['retrieval'] else [{'type': 'code_interpreter'}]
-            }
-            for file in self._fileids
-        ]        
+                'tools': tools  }  ) 
         self._startPrompt = message
         self.threadObject = self.client.beta.threads.create(messages=[] )
         self._message_id = self.client.beta.threads.messages.create(
         thread_id=self.thread_id,
         content=message,
         attachments= att,
         role="user"
             )
+        #for v in visions:
+        #    self.client.beta.threads.messages.create(
+        #        thread_id=self.thread_id,
+        #        content= [{
+        #        'type' : "image_file",
+        #        'image_file' : {"file_id": v ,'detail':'high'}},
+        #         role="user"]
+        #    )
+        
     
     def __init__(self, **kwargs ):
         ''' Create an assistant task
         
         Two modes: create a new task or retrieve an existing (probably completed) task from the database
         
         if run_id is provided it will retrieve the task from the database. If not it will create a new task.
@@ -430,28 +445,29 @@
             *** Note addToAssistant is not currently supported due to the V2 changes. 
             
             filename - the name of the file. If not provided will use the name of the file object
             All uploaded files will automatically be provided in the message to the assistant with both search and code interpreter enabled.
         '''
         if fileContent == None:
             fileContent = file.read()
-        uploadFile = self.client.files.create( file=(filename,fileContent),purpose='assistants')
         # Determine file extension
         file_extension = filename.split('.')[-1].lower()
         
         # Determine if the file is an image
         image_extensions = ['jpg', 'jpeg', 'png', 'gif', 'bmp', 'tiff']
         vision = file_extension in image_extensions
-        
         # Determine if the file is for retrieval
         retrieval_extensions = [
             'c', 'cs', 'cpp', 'doc', 'docx', 'html', 'java', 'json', 'md', 'pdf', 'php',
             'pptx', 'py', 'rb', 'tex', 'txt', 'css', 'js', 'sh', 'ts'
         ]
         retrieval = file_extension in retrieval_extensions
+        
+        #uploadFile = self.client.files.create( file=(filename,fileContent),purpose=('vision' if vision else 'assistants'))
+        uploadFile = self.client.files.create( file=(filename,fileContent),purpose='assistants')
 
         # Append the file information to self._fileids
         self._fileids.append({
             'id': uploadFile.id,
             'filename': filename,
             'vision': vision,
             'retrieval': retrieval
@@ -461,11 +477,23 @@
         
     def getlastresponse(self):
         ''' Get the last response from the assistant, returns the data[] portion of the response
         '''
         messages = self.client.beta.threads.messages.list( thread_id=self.thread_id)
         return messages.data[0]
     
+    def getfullresponse(self):
+        ''' Get the full text response from the assistant (concatenated text type messages)
+        '''
+        messages = self.client.beta.threads.messages.list( thread_id=self.thread_id)
+        res = ''
+        for m in reversed(messages.data):
+            if m.role == 'assistant':
+                for t in m.content:
+                    if t.type == 'text':
+                        res += t.text.value
+        return res
+    
     def retrieveFile(self,file_id):
         ''' Retrieve the FILE CONTENT of a file from OpenAI
         '''
         return self.client.files.content(file_id=file_id)
```

### Comparing `django_openai_assistant-0.5.2/src/django_openai_assistant/models.py` & `django_openai_assistant-0.5.3/src/django_openai_assistant/models.py`

 * *Files identical despite different names*

### Comparing `django_openai_assistant-0.5.2/src/django_openai_assistant/migrations/0001_initial.py` & `django_openai_assistant-0.5.3/src/django_openai_assistant/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_openai_assistant-0.5.2/LICENSE` & `django_openai_assistant-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_openai_assistant-0.5.2/README.md` & `django_openai_assistant-0.5.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,17 @@
         print(task.markdownresponse())
     else:
         print('run failed')
 ```
 See https://medium.com/@jlvalorvc/building-a-scalable-openai-assistant-processor-in-django-with-celery-a61a1af722e0
 
 ## Version history:
+0.5.3
+- Added getfullresponse() that comiles all Assistant repsonses in one message
+- still waiting for the openai Python library to support vision.
 0.5.2
 - Updated the file upload mechanism to determine file types (retrieval yes/no and prepare for vision support (image yes/no))
 - When attachments are added to a thread they will always have 'tools' enabled and retrieval will only be enabled for the supported file types https://platform.openai.com/docs/assistants/tools/file-search/supported-files
 
 0.5.1
 - Remove getopenaiclient() instead use OpenAI() everywhere
 - Fix getAssistant() that could fail if retrieving an Assistant by name from an org with more than 20 Assistants.
```

### Comparing `django_openai_assistant-0.5.2/pyproject.toml` & `django_openai_assistant-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "django-openai-assistant"
-version = "0.5.2"
+version = "0.5.3"
 dependencies = ["openai", "markdown"]
 readme = "README.md"
 authors = [{name = "Jean-Luc Vanhulst", email = "jl@valor.vc"}]
 maintainers = [{name = "Jean-Luc Vanhulst", email = "jl@valor.vc"}]
 classifiers = ["License :: OSI Approved :: MIT License"]
 urls = {Homepage = "https://github.com/jlvanhulst/django-openai"}
 keywords = ["django", "celery", "openai", "assistants"]
```

### Comparing `django_openai_assistant-0.5.2/PKG-INFO` & `django_openai_assistant-0.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-openai-assistant
-Version: 0.5.2
+Version: 0.5.3
 Summary: Django OpenAI Assistant
 Project-URL: Homepage, https://github.com/jlvanhulst/django-openai
 Author-email: Jean-Luc Vanhulst <jl@valor.vc>
 Maintainer-email: Jean-Luc Vanhulst <jl@valor.vc>
 License-File: LICENSE
 Keywords: assistants,celery,django,openai
 Classifier: License :: OSI Approved :: MIT License
@@ -56,14 +56,17 @@
         print(task.markdownresponse())
     else:
         print('run failed')
 ```
 See https://medium.com/@jlvalorvc/building-a-scalable-openai-assistant-processor-in-django-with-celery-a61a1af722e0
 
 ## Version history:
+0.5.3
+- Added getfullresponse() that comiles all Assistant repsonses in one message
+- still waiting for the openai Python library to support vision.
 0.5.2
 - Updated the file upload mechanism to determine file types (retrieval yes/no and prepare for vision support (image yes/no))
 - When attachments are added to a thread they will always have 'tools' enabled and retrieval will only be enabled for the supported file types https://platform.openai.com/docs/assistants/tools/file-search/supported-files
 
 0.5.1
 - Remove getopenaiclient() instead use OpenAI() everywhere
 - Fix getAssistant() that could fail if retrieving an Assistant by name from an org with more than 20 Assistants.
```

