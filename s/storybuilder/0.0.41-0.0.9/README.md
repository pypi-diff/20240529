# Comparing `tmp/storybuilder-0.0.41-py3-none-any.whl.zip` & `tmp/storybuilder-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,13 @@
-Zip file size: 22230 bytes, number of entries: 13
--rw-rw-r--  2.0 unx      112 b- defN 24-May-13 12:34 storybuilder/__init__.py
--rw-rw-r--  2.0 unx     4732 b- defN 24-May-13 12:34 storybuilder/characterpostures.py
--rw-rw-r--  2.0 unx     2974 b- defN 24-May-27 06:14 storybuilder/cosuploader.py
--rw-rw-r--  2.0 unx     5246 b- defN 24-May-22 11:48 storybuilder/speechsynthesizer.py
--rw-rw-r--  2.0 unx    79716 b- defN 24-May-29 02:43 storybuilder/storybuilder.py
--rw-rw-r--  2.0 unx     4599 b- defN 24-May-16 05:44 storybuilder/storyprofiles.py
--rw-rw-r--  2.0 unx     2640 b- defN 24-May-27 03:02 storybuilder/storyvoicebuilder.py
--rw-rw-r--  2.0 unx     4896 b- defN 24-May-27 03:02 storybuilder/utility.py
--rw-r--r--  2.0 unx     1062 b- defN 24-May-29 02:53 storybuilder-0.0.41.dist-info/LICENSE
--rw-rw-r--  2.0 unx      869 b- defN 24-May-29 02:53 storybuilder-0.0.41.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-29 02:53 storybuilder-0.0.41.dist-info/WHEEL
--rw-rw-r--  2.0 unx       13 b- defN 24-May-29 02:53 storybuilder-0.0.41.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1101 b- defN 24-May-29 02:53 storybuilder-0.0.41.dist-info/RECORD
-13 files, 108052 bytes uncompressed, 20382 bytes compressed:  81.1%
+Zip file size: 13537 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      112 b- defN 24-May-13 03:49 storybuilder/__init__.py
+-rw-r--r--  2.0 unx     1601 b- defN 24-May-13 03:38 storybuilder/cosuploader.py
+-rw-r--r--  2.0 unx     5305 b- defN 24-May-13 04:00 storybuilder/speechsynthesizer.py
+-rw-r--r--  2.0 unx    31502 b- defN 24-May-13 05:58 storybuilder/storybuilder.py
+-rw-r--r--  2.0 unx     4715 b- defN 24-May-12 15:23 storybuilder/storyprofiles.py
+-rw-r--r--  2.0 unx     2631 b- defN 24-May-13 04:01 storybuilder/storyvoicebuilder.py
+-rw-r--r--  2.0 unx     1062 b- defN 24-May-13 05:59 storybuilder-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      699 b- defN 24-May-13 05:59 storybuilder-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-13 05:59 storybuilder-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-May-13 05:59 storybuilder-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      926 b- defN 24-May-13 05:59 storybuilder-0.0.9.dist-info/RECORD
+11 files, 48658 bytes uncompressed, 11963 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -1,13 +1,10 @@
 Filename: storybuilder/__init__.py
 Comment: 
 
-Filename: storybuilder/characterpostures.py
-Comment: 
-
 Filename: storybuilder/cosuploader.py
 Comment: 
 
 Filename: storybuilder/speechsynthesizer.py
 Comment: 
 
 Filename: storybuilder/storybuilder.py
@@ -15,26 +12,23 @@
 
 Filename: storybuilder/storyprofiles.py
 Comment: 
 
 Filename: storybuilder/storyvoicebuilder.py
 Comment: 
 
-Filename: storybuilder/utility.py
-Comment: 
-
-Filename: storybuilder-0.0.41.dist-info/LICENSE
+Filename: storybuilder-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: storybuilder-0.0.41.dist-info/METADATA
+Filename: storybuilder-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: storybuilder-0.0.41.dist-info/WHEEL
+Filename: storybuilder-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: storybuilder-0.0.41.dist-info/top_level.txt
+Filename: storybuilder-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: storybuilder-0.0.41.dist-info/RECORD
+Filename: storybuilder-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## storybuilder/cosuploader.py

```diff
@@ -1,88 +1,39 @@
 from qcloud_cos import CosConfig
 from qcloud_cos import CosS3Client
-from qcloud_cos import CosServiceError
-from qcloud_cos import CosClientError
 
 import os
 import hashlib
 
-
 class CosUploader:
-    def __init__(
-        self,
-        service_root,
-        cos_region,
-        cos_secret_id,
-        cos_secret_key,
-        cos_bucket,
-        cos_token=None,
-        cos_scheme="https",
-    ):
+    def __init__(self, service_root, cos_region, cos_secret_id, cos_secret_key, cos_bucket, cos_token=None, cos_scheme="https"):
         self.service_root = service_root
-        self._config = CosConfig(
-            Region=cos_region,
-            SecretId=cos_secret_id,
-            SecretKey=cos_secret_key,
-            Token=cos_token,
-            Scheme=cos_scheme,
-        )
+        self._config = CosConfig(Region=cos_region, SecretId=cos_secret_id, SecretKey=cos_secret_key, Token=cos_token, Scheme=cos_scheme)
         self._client = CosS3Client(self._config)
         self._bucket = cos_bucket
-        self._region = cos_region
 
     def calculate_file_hash(self, file_path):
         hash_md5 = hashlib.md5()
         with open(file_path, "rb") as f:
             for chunk in iter(lambda: f.read(4096), b""):
                 hash_md5.update(chunk)
         return hash_md5.hexdigest()
 
     def get_file_name(self, file_path):
         filename, file_extension = os.path.splitext(os.path.basename(file_path))
-        if file_extension in [".svg", ".jpg", ".jpeg", ".png", ".gif"]:
-            return filename + "_" + self.calculate_file_hash(file_path) + file_extension
-        else:
-            return os.path.basename(file_path)
-
-    def local2cos(self, local_path, storyId, target_relative_path="test"):
-        if target_relative_path is None:
-            target_relative_path = ""
-        elif len(target_relative_path) > 0:
-            target_relative_path = (
-                target_relative_path
-                if target_relative_path[0] != "/"
-                else target_relative_path[1:]
-            )
+        return filename + "_" + self.calculate_file_hash(file_path) + file_extension
+        
+    def local2cos(self, local_path, storyId, target_relative_path='test'):
         try:
-            filename = os.path.join(
-                target_relative_path,
-                storyId,
-                self.get_file_name(local_path),
-            )
+            filename = os.path.join(self.site_root, 
+                                    target_relative_path if target_relative_path[0] !='/' else target_relative_path[1:], 
+                                    storyId, 
+                                    self.get_file_name(local_path))
         except:
-            print("file not found:", local_path)
+            print("file not found =========", local_path)
+
         response = self._client.upload_file(
-            Bucket=self._bucket, LocalFilePath=local_path, Key=filename
+            Bucket=self._bucket,
+            LocalFilePath=local_path,
+            Key=filename
         )
-        return "/"+filename
-    
-    def test2product(self, source):
-        source_file = source[1:] if source.startswith("/") else source
-        target_file = source_file
-        if source_file.startswith("test/audios/") or source_file.startswith("test/posters/"):
-            target_file = "story/" + source_file[len("test/"):]
-        if source_file != target_file:
-            try:
-                response = self._client.copy_object(
-                    Bucket=self._bucket,
-                    Key=target_file,
-                    CopySource={
-                        'Bucket': self._bucket, 
-                        'Key': source_file, 
-                        'Region': self._region
-                    }
-                )
-            except Exception as e:
-                print("copy test file to product path failed:", e)
-        return "/"+target_file
-
+        return filename
```

## storybuilder/speechsynthesizer.py

```diff
@@ -54,14 +54,15 @@
             ssml += "</voice></speak>"
             result = self.speech_synthesizer.speak_ssml_async(ssml).get()
         else:
             result = self.speech_synthesizer.speak_text_async(text).get()
             
         # Check result
         if result.reason == speechsdk.ResultReason.SynthesizingAudioCompleted:
+            print(f"Speech synthesized for text [{text}]")
             bytes = io.BytesIO(result.audio_data)
             sound = pydub.AudioSegment.from_file(bytes)
             
             if len(output_file_name) == 0:
                 id = uuid.uuid4()
                 file_name = f"voice-{id}.mp3"
             else:
```

## storybuilder/storybuilder.py

```diff
@@ -1,474 +1,220 @@
 import json
 import random
 import os
 import uuid
-import re
 import copy
+import re
 import xml.etree.ElementTree as ET
 from PIL import Image
-from typing import Dict, Union
-
-from .utility import *
 
 from .storyprofiles import CHARACTER_FIGURE_ACCESSORY_KEYS, STORY_SCENARIO_STYLES
-from .characterpostures import CHARACTER_FIGURES
-
-DEFAULT_LANGUAGE="zh-CN"
-LANGUAGE_ENG="en-US"
-DEFAULT_NARRATOR="M"
-VISIBLE_ACTORS=("boy", "girl", "eily")
-INVISIBLE_ACTORS=("", "M", "F")
-SCENARIO_ACTORS=("ending", "exam", "concentrak", "notes")
-LOCAL_DEFAULT_ROOT="./test"
-
-MText = Dict[str, str]
-
-def isMText(text: Union[str, MText]):
-    return isinstance(text, dict) and len(text) > 0
 
 class Story:
-
-    def test(self, localOutputPath=LOCAL_DEFAULT_ROOT, fileName="testStory.json", language=DEFAULT_LANGUAGE):
-        directory = os.path.join(localOutputPath, self.storyId)
-        if not os.path.exists(directory):
-            os.makedirs(directory)
-
-        language = DEFAULT_LANGUAGE if language == None else language
-        scripts = self.exportScripts()
-        if self._synthesizer != None:
-            try:
-                for script in scripts:
-                    for voice in script["voices"]:
-                        soundFileName = voice["sound"]
-                        if isinstance(soundFileName, str) and len(soundFileName) > 0:
-                            text = voice["subscript"][language] if isinstance(voice["subscript"], dict) else voice["subscript"]
-                            alternativeText = None if "alternative" not in voice \
-                                else (voice["alternative"][DEFAULT_LANGUAGE] \
-                                    if isinstance(voice["alternative"], dict) \
-                                    else voice["alternative"])
-                            narrator = voice["narrator"]
-                            text = text if alternativeText == None else alternativeText
-                            self._synthesizer.synthesizeFile(
-                                    narrator, remove_emojis(text), language, directory, os.path.basename(soundFileName)
-                                )
-                            localOutputFileName = os.path.join(directory, os.path.basename(soundFileName))
-                            if self._cosUploader != None:
-                                self._cosUploader.local2cos(localOutputFileName, self.storyId, self.audioPath)   
-            except Exception as e:
-                print(f"Story.test failed for {script}\n", e)
-
-        with open(os.path.join(localOutputPath, fileName), "w") as file:
-            json.dump(
-                self.export(), file, ensure_ascii=False, indent=4, sort_keys=False
-            )
     
-    def export(self):
-        voices = [{"sound": "/story/audios/OurMusicBox - 24 Hour Coverage - intro.mp3"}]
-        events = []
-        for page in self._pages:
-            pageObject = page.export(voiceOffset=len(voices), pageId=float(len(events)))
-            if pageObject != None and isinstance(pageObject, dict) \
-                and "voices" in pageObject and "events" in pageObject:
-                for entry in pageObject["voices"]:
-                    entryObject = {}
-                    for key in set(entry.keys()) & {"sound", "languages"}:
-                        if entry[key] != None:
-                            entryObject[key] = entry[key]
-                    if len(entryObject) > 0:
-                        voices.append(entryObject)
-                events = events + pageObject["events"]
-
-        return {"voices": voices, "events": events}
-
-    def exportScripts(self):
-        voices = []
-        for i, page in enumerate(self._pages):
-            pageObject = page.export(voiceOffset=len(voices))
-            pageVoices = []
-            for voice in pageObject["voices"]:
-                if (isinstance(voice["subscript"], str) or isinstance(voice["subscript"], dict)) and len(voice["subscript"]) > 0:
-                    pageVoices.append(voice)
-            if len(pageVoices) > 0:
-                voices = voices + [{"page": i, "voices": pageVoices}]
-
-        return voices
-
-    def exportAudios(self, localOutputPath=LOCAL_DEFAULT_ROOT, uploadToCos=True):
-        directory = os.path.join(localOutputPath, self.storyId)
-        if not os.path.exists(directory):
-            os.makedirs(directory)
-
-        if self._synthesizer:
-            voices = self.exportScripts()
-            for page in voices:
-                for i, voice in enumerate(page["voices"]):
-                    if not isinstance(voice["sound"], str) or voice["sound"].startswith("/story/"): # Ignore if production audio
-                        continue
-                    try:
-                        fileName = os.path.basename(voice["sound"])
-                        character = voice["narrator"]
-                        for language in voice["subscript"]:
-                                subscript = (
-                                    voice["alternative"][language]
-                                    if ("alternative" in voice) and (language in voice["alternative"]) and (voice["alternative"][language] != None)
-                                    else voice["subscript"][language]
-                                )
-                                print(f'Page {page["page"]}/Script {i}')
-                                self._synthesizer.synthesizeFile(
-                                    character, remove_emojis(subscript), language, directory, fileName
-                                )
-                                localOutputFileName = os.path.join(directory, fileName)
-
-                                if self._cosUploader != None and uploadToCos:
-                                    _ = self._cosUploader.local2cos(localOutputFileName, self.storyId, self.audioPath)
-                    except Exception as e:
-                        print(f"Synthesize & upload script failed for <{voice['subscript']}><{subscript}>\n", e)
-                        continue
-
-    def exportProduct(self, localOutputPath='./prod'):
-        if self._cosUploader == None:
-            print("Cos uploader is not available, exit.")
-            return
-
-        if not os.path.exists(localOutputPath):
-            os.makedirs(localOutputPath)
-
-        storyObject = self.export()
-        
-        # Copy audios to product path
-        for i, voice in enumerate(storyObject["voices"]):
-            storyObject["voices"][i]["sound"] = self._cosUploader.test2product(voice["sound"])
-
-        # Copy images to product path
-        for j, event in enumerate(storyObject["events"]):
-            if "board" in event and isinstance(event["board"], dict):
-                board = event["board"]
-                if "content" in board and isinstance(board["content"], dict) \
-                    and "image" in board["content"] and isinstance(board["content"]["image"], str) \
-                    and len(board["content"]["image"]) > 0:
-                    storyObject["events"][j]["board"]["content"]["image"] = self._cosUploader.test2product(board["content"]["image"])
-                if "contentList" in board and isinstance(board["contentList"], list) \
-                    and len(board["contentList"]) > 0:
-                    for k, contentEntry in enumerate(board["contentList"]):
-                        if "image" in contentEntry and isinstance(contentEntry["image"], str) \
-                            and len(contentEntry["image"]) > 0:
-                            storyObject["events"][j]["board"]["contentList"][k]["image"] = self._cosUploader.test2product(contentEntry["image"])
-
-        productFileName = os.path.join(localOutputPath, self.title + ".product.json")
-        with open(productFileName, "w") as file:
-            json.dump(
-                storyObject, file, ensure_ascii=False, indent=4, sort_keys=False
-            )
-        print(f"Story resource copied from test to production, product story generated as {productFileName}.")
-
-    @staticmethod
-    def buildStoryCollection(outputName, storyList):
-        storyCollection = {"collection": []}
-        for story in storyList:
-            storyTitle = story[:len(story)-5] if story.endswith(".json") else story
-            storyCollection["collection"].append(storyTitle)
-        with open(outputName, "w") as file:
-            json.dump(
-                storyCollection, file, ensure_ascii=False, indent=4, sort_keys=False
-            )
-
     @staticmethod
     def retrieveSvgSize(image_path):
         # Load the SVG file
-        tree = ET.parse(image_path)
+        tree = ET.parse(image_path) 
         root = tree.getroot()
-
+        
         # Extract attributes from the <svg> tag
-        width = root.get("width", 0)  # Get the width attribute
-        height = root.get("height", 0)  # Get the height attribute
-        viewBox = root.get("viewBox", "0, 0, 0, 0")  # Get the viewBox attribute
-
-        split_pattern = r"[ ,]+"
-
-        return [int(width), int(height)], [
-            int(float(num)) for num in re.split(split_pattern, viewBox)
-        ]
-
+        width = root.get('width', 0)  # Get the width attribute
+        height = root.get('height', 0)  # Get the height attribute
+        viewBox = root.get('viewBox', '0, 0, 0, 0')  # Get the viewBox attribute
+    
+        split_pattern = r'[ ,]+'
+        
+        return [int(width), int(height)], [int(num) for num in re.split(split_pattern, viewBox)]
+    
     @staticmethod
     def retrievePixelSize(image_path):
         # Open the image using the Python Imaging Library (PIL)
         image = Image.open(image_path)
-
+    
         # Get the width and height of the image in pixels
         width, height = image.size
-
+    
         # Return the width and height as a tuple
         return width, height
-
+    
     @staticmethod
     def getImageSize(file_path):
         width = height = 0
         try:
-            if ".svg" in file_path[-4:]:
+            if '.svg' in file_path[-4:]:
                 dim2, dim4 = Story.retrieveSvgSize(file_path)
-                if dim2 == [0, 0]:
+                if dim2 == [0,0]:
                     width = dim4[2]
                     height = dim4[3]
                 else:
                     width = dim2[0]
                     height = dim2[1]
-            elif (
-                ".jpg" in file_path[-4:]
-                or ".jpeg" in file_path[-5:]
-                or ".png" in file_path[-4:]
-                or ".gif" in file_path[-4:]
-            ):
+            elif '.jpg' in file_path[-4:] or '.jpeg' in file_path[-5:] or '.png' in file_path[-4:] or '.gif' in file_path[-4:]:
                 width, height = Story.retrievePixelSize(file_path)
         except:
-            print("Retrieve image size error for", file_path)
+                print('retrieve image file size error =========', file_path)
         return width, height
-    
-    @staticmethod
-    def loadFromFile(fileName, locale=DEFAULT_LANGUAGE, **kwargs):
-        story = None
-        storyId = None
-        try:
-            with open(fileName, 'r') as f:
-                object = json.load(f)
-            voices = object["voices"]
-            events = object["events"]
-            storyId = kwargs["storyId"] if "storyId" in kwargs else storyId
-            if len(voices) > 1:
-                for i in range(1, len(voices)):
-                    folder = voices[i].get("sound", "//").split("/")[-2]
-                    if len(folder) == 36: # length of uuid.uuid4()
-                        storyId = folder
-            storyStyle = None
-            validScene = None
-            for i in range(len(events)):
-                if events[i].get("scene", None) != None and len(events[i]["scene"]) > 0:
-                    validScene = events[i]["scene"]
-                    break
-            for styleKey in STORY_SCENARIO_STYLES.keys():
-                for key, value in STORY_SCENARIO_STYLES[styleKey]["scenarios"].items():
-                    if value == validScene \
-                        or (key == "notes" and value["scene"] == validScene):
-                        storyStyle = styleKey
-                        break
-            defaultNarrator = None
-            for event in events:
-                if defaultNarrator != None:
-                    break
-                if "objects" in event and isinstance(event["objects"], list):
-                    _, _, defaultNarrator, _, _, _ = get_actors(event["objects"])
-            kwargs["narrator"] = defaultNarrator if defaultNarrator != None else DEFAULT_NARRATOR
-            story = Story(title=os.path.basename(fileName).replace(".json", ""), 
-                        storyId=storyId, 
-                        style=storyStyle, 
-                        locale=locale, 
-                        **kwargs)
-
-            pageScenario = None
-            for event in events:
-                # 获取页面类型
-                if "board" in event \
-                    and ((event["board"].get("type", None) != None and len(event["board"]["type"]) > 0) \
-                         or (isinstance(event["board"].get("content", None), dict) \
-                             and event["board"]["content"].get("type", None) != None)):
-                    pageScenario = event["board"]["type"] if event["board"].get("type", None) != None else event["board"]["content"]["type"]
-                else:
-                    sceneObject = event.get("scene", None)
-                    if isinstance(sceneObject, str) and len(sceneObject) > 0:
-                        for key, value in STORY_SCENARIO_STYLES[storyStyle]["scenarios"].items():
-                            if isinstance(value, str) and value == sceneObject:
-                                pageScenario = key
-                    elif "index" in sceneObject and sceneObject["index"] == STORY_SCENARIO_STYLES[storyStyle]["scenarios"]["concentrak"]["index"]:
-                        pageScenario = "concentrak"
-                    elif "bgColor" in sceneObject and len(sceneObject["bgColor"]) > 0:
-                        pageScenario = "blackboard"
-                pageScenario = "cover" if pageScenario == None else pageScenario # 没有样式匹配，设为CoverPage
-
-
-                # 创建对应页面
-                print(f"Loading page as {pageScenario}")
-                # CoverPage
-                if pageScenario == "cover":
-                    story.createPage(
-                        sceneType = pageScenario,
-                        source = "",
-                        voices = voices,
-                        board = event["board"],
-                        objects = event["objects"],
-                        interactions = event["interactions"]
-                        )
-                # ClassroomPage
-                elif pageScenario == "classroom":
-                    story.createPage(
-                        sceneType = pageScenario,
-                        actor = "",
-                        voices = copy.deepcopy(voices),
-                        board = event["board"],
-                        objects = event["objects"],
-                        interactions = event["interactions"]
-                        )
-                # BlackboardPage
-                elif pageScenario == "blackboard":
-                    story.createPage(
-                        sceneType = pageScenario,
-                        source = "",
-                        voices = copy.deepcopy(voices),
-                        board = event["board"],
-                        objects = event["objects"],
-                        interactions = event["interactions"]
-                        )
-
-                # ConcentrakPage
-                elif pageScenario == "concentrak":
-                    story.createPage(
-                        sceneType = pageScenario,
-                        text = "",
-                        voices = copy.deepcopy(voices),
-                        board = event["board"],
-                        objects = event["objects"],
-                        interactions = event["interactions"]
-                        )
-                # ExamPage
-                elif pageScenario == "exam":
-                    story.createPage(
-                        sceneType = pageScenario,
-                        actor = "", 
-                        voices = copy.deepcopy(voices),
-                        board = event["board"],
-                        objects = event["objects"],
-                        interactions = event["interactions"]
-                    )
-
-                # NotesPage
-                elif pageScenario == "notes":
-                    story.createPage(
-                        sceneType = pageScenario,
-                        actor = "", 
-                        voices = copy.deepcopy(voices),
-                        board = event["board"],
-                        objects = event["objects"],
-                        interactions = event["interactions"]
-                    )
 
-                else:
-                    pass            
-            
-        except Exception as e:
-            print("Load story from file exception:\n", e)
-            return None
-            
-        return story
+    def _loadStoryDataDefaults(self, filename, key='defaultCharacters'):
+        with open(filename) as f:
+            data = f.read()
+    
+        pattern = r'export const (\w+) = (.*?)(;)'
+        flags = re.DOTALL | re.MULTILINE
+    
+        matches = re.finditer(pattern, data, flags=flags)
+    
+        # Replace export const with key:
+        matched = {key:None}
+        for one_match in matches:
+            if one_match.group(1) == key:
+                cleaned_string = one_match.group(2).strip().replace('\n', '').replace(',]', ']')
+                matched[key] = json.loads(cleaned_string)
+        
+        return matched
 
+    
     def __init__(self, title, storyId=None, style="shinkai_makoto", **kwargs):
         self.title = title
-        self.storyId = storyId if storyId != None else uuid.uuid4()
+        self.storyId = storyId if storyId!=None else uuid.uuid4()
         self.styles = STORY_SCENARIO_STYLES[style]
-        self.locale = kwargs["locale"] if "locale" in kwargs else DEFAULT_LANGUAGE
-        self.narrator = kwargs["narrator"] if "narrator" in kwargs else DEFAULT_NARRATOR
-        self._pages = []
-        self.posterPath = 'test/posters/'
-        self.audioPath = 'test/audios/'
+        self.locale = kwargs["locale"] if "locale" in kwargs else "cn"
+        self.narrator = kwargs["narrator"] if "narrator" in kwargs else "M"
+        self.pages = []
 
         self._cosUploader = kwargs["uploader"] if "uploader" in kwargs else None
         self._synthesizer = kwargs["synthesizer"] if "synthesizer" in kwargs else None
+        
+        self._defaultCharacters = None
+        # 需要提供defaultdata.tsx源文件所在项目根路径
+        figureSource = kwargs["figureSource"] if "figureSource" in kwargs else None
+        if figureSource != None:
+            print("Load default character figure info at", figureSource)
 
-        self._defaultCharacters = CHARACTER_FIGURES
-
-        print(f"Create a new story title: {title}, Id:", self.storyId)
+            self._defaultCharacters = self._loadStoryDataDefaults(figureSource, key='defaultCharacters')['defaultCharacters']
+        else:
+            print("No source file for default character figure loaded, please input number for posture variable.")
 
-    def getAudioPath(self, fileName):
-        return os.path.join("/", self.audioPath, self.storyId, fileName)
+        print("New story Id", self.storyId)
 
-    def getUserPostureId(
-        self, actor, postures, keyScenario="stand", excludeAccessories=True
-    ):
+    def getUserPostureId(self, actor, postures, keyScenario = 'stand', excludeAccessories=True):
         if type(postures) is int:
             return postures
         if type(postures) is list and type(postures[0]) is int:
             return postures[0]
         if self._defaultCharacters == None:
             return 0
 
-        currentActorFigures = self._defaultCharacters[actor]
+        currentActorFigures = self._defaultCharacters[actor]['figure']
         availableFigures = []
         for j, figure in enumerate(currentActorFigures):
+            fullFigure = figure['source'].split('/')[-1]
             skip = False
             if excludeAccessories:
                 for accessory in CHARACTER_FIGURE_ACCESSORY_KEYS:
-                    if accessory in figure:
+                    if accessory in fullFigure:
                         skip = True
             if skip:
                 continue
-            if keyScenario in figure and all(keyWord in figure for keyWord in postures):
-                availableFigures.append({"index": j, "figure": figure})
+            if keyScenario in fullFigure and all(keyWord in fullFigure for keyWord in postures):
+                availableFigures.append({'index':j, 'figure':fullFigure.split('.')[0]})
         if len(availableFigures) > 0:
-            return random.choice(availableFigures)["index"]
+            return random.choice(availableFigures)['index']
         else:
             return 0
 
-    def _NewPage(self, sceneType, **kwargs):
-        try:
-            scene = sceneType.lower()
-        except Exception as e:
-            print(f"problematic sceneType in type {type(sceneType)}: {sceneType}")
+    def appendPage(self, page):
+        self.pages.append(page)
+
+    def insertPage(self, pos, page):
+        self.pages.insert(pos, page)
+
+    def createPage(self, sceneType, **kwargs):
+        if sceneType.lower() not in ("exam", "notes", "cover", "blackboard", "concentrak", "classroom"):
+            raise Exception(f"Invalid scenario type {sceneType}, must be one of ('exam', 'notes', 'cover', 'blackboard', 'concentrak', 'classroom')")
+        
         newPage = None
-        if scene == "classroom":
+
+        if sceneType.lower() == "classroom":
             if "actor" not in kwargs:
                 raise Exception(f'argument "actor" is required')
-            newPage = ClassroomPage(self, **kwargs)
-        elif scene == "exam":
+            if "postures" in kwargs:
+                newPage = ClassroomPage(self, kwargs["actor"], postures=kwargs["postures"])
+            else:
+                newPage = ClassroomPage(self, kwargs["actor"])
+        elif sceneType.lower() == "blackboard":
+            if "source" not in kwargs:
+                raise Exception(f'argument "source" is required')
+            if "rect" in kwargs:
+                newPage = BlackboardPage(self, kwargs["source"], rect=kwargs["rect"])
+            else:
+                newPage = BlackboardPage(self, kwargs["source"])
+        elif sceneType.lower() == "exam":
             if "actor" not in kwargs:
                 raise Exception(f'argument "actor" is required')
-            newPage = ExamPage(self, **kwargs)
-        elif scene == "concentrak":
+            if "postures" in kwargs:
+                newPage = ExamPage(self, kwargs["actor"], postures=kwargs["postures"])
+            else:
+                newPage = ExamPage(self, kwargs["actor"])
+        elif sceneType.lower() == "concentrak":
             if "text" not in kwargs:
                 raise Exception(f'argument "text" is required')
-            newPage = ConcentrakPage(self, **kwargs)
-        elif scene == "blackboard":
-            if "source" not in kwargs:
-                raise Exception(f'argument "source" is required')
-            newPage = BlackboardPage(self, **kwargs)
-        elif scene == "cover":
+            newPage = ConcentrakPage(self, kwargs["text"])
+        elif sceneType.lower() == "cover":
             if "source" not in kwargs:
                 raise Exception(f'argument "source" is required')
-            newPage = CoverPage(self, **kwargs)
-        elif scene == "notes":
+            if "rect" in kwargs:
+                newPage = CoverPage(self, kwargs["source"], rect=kwargs["rect"])
+            else:
+                newPage = CoverPage(self, kwargs["source"])
+        elif sceneType.lower() == "notes":
             if "actor" not in kwargs:
                 raise Exception(f'argument "actor" is required')
-            newPage = NotesPage(self, **kwargs)
-        else:
-            print(f"Invalid scenario type {sceneType}, must be one of ('exam', 'notes', 'cover', 'blackboard', 'concentrak', 'classroom')")
-
-        return newPage        
-
-    def createPage(self, sceneType, **kwargs):
-        newPage = self._NewPage(sceneType, **kwargs)
+            if "postures" in kwargs:
+                newPage = NotesPage(self, kwargs["actor"], postures=kwargs["postures"])
+            else:
+                newPage = NotesPage(self, kwargs["actor"])
 
         if newPage != None:
-            self._pages.append(newPage)
+            self.pages.append(newPage)
 
         return newPage
 
-    def createPageAtPos(self, pos, sceneType, **kwargs):
-        if pos >= 0 and pos < len(self._pages):
-            newPage = self._NewPage(sceneType, **kwargs)
-            if newPage != None:
-                self._pages.insert(pos, newPage)
-        else:
-            print("Input pos is out of boundary.")
-            newPage = None
+    def export(self):
+        voices = [{"sound": "/story/audios/OurMusicBox - 24 Hour Coverage - intro.mp3"}]
+        events = []
+        for page in self.pages:
+            pageObject = page.export(voiceOffset=len(voices), pageId=float(len(events)))
+            voices = voices + [{"sound": entry["sound"]} for entry in pageObject["voices"]]
+            events = events + pageObject["events"]
 
-        return newPage
-    
-    def removePageAtPos(self, pos):
-        if pos >= 0  and pos < len(self._pages):
-            self._pages.pop(pos)
+        return {"voices": voices, "events": events}
+
+    def exportScripts(self):
+        voices = []
+        for page in self.pages:
+            pageObject = page.export(voiceOffset=len(voices))
+            voices = voices + pageObject["voices"]
 
-    def getPage(self, pos):
-        return self._pages[pos] if (pos >= 0  and pos < len(self._pages)) else None
+        return voices
+    
+    def exportAudios(self, outputPath):
+        if self._synthesizer:
+            voices = self.exportScripts()
+            for voice in voices:
+                fileName = voice["sound"]
+                character = voice["narrator"]
+                for language in voice["subscript"]:
+                    subscript = voice["alternative"][language] if "alternative" in voice else voice["subscript"][language]
+                    self._synthesizer.synthesizeFile(character, 
+                                                     subscript, 
+                                                     language, 
+                                                     outputPath, 
+                                                     fileName)
 
 class Page:
     def __init__(self, type, storyInstance):
         self.story = storyInstance
         self.narrator = storyInstance.narrator
         self.locale = storyInstance.locale
         self.type = type
@@ -479,1160 +225,562 @@
         self.subscripts = []
         self.narrations = []
         self.actor = ""
 
     def _getUserId(self, actor):
         userId = -1
         for i, object in enumerate(self.objects):
-            if object["name"].lower() == actor.lower():
+            if object["name"].upper() == actor.upper():
                 userId = i
-
+    
         if userId == -1:
-            self.objects.append({"name": actor})
+            self.objects.append({"name":actor})
             userId = len(self.objects) - 1
         return userId
 
-    def test(self, localOutputPath=LOCAL_DEFAULT_ROOT, fileName="testPage.json", language=DEFAULT_LANGUAGE):
-        directory = os.path.join(localOutputPath, self.story.storyId)
-        if not os.path.exists(directory):
-            os.makedirs(directory)
-
-        language = DEFAULT_LANGUAGE if language == None else language
-        scripts = self.exportScripts()
-        if self.story._synthesizer != None:
-            try:
-                for script in scripts:
-                    soundFileName = script["sound"]
-                    if isinstance(soundFileName, str) and len(soundFileName) > 0:
-                        text = script["subscript"][language] if isinstance(script["subscript"], dict) else script["subscript"]
-                        alternativeText = None if "alternative" not in script else \
-                            (script["alternative"][language] \
-                                if isinstance(script["alternative"], dict) \
-                                else script["alternative"])
-                        narrator = script["narrator"]
-                        text = alternativeText if isinstance(alternativeText, str) else text
-                        self.story._synthesizer.synthesizeFile(
-                                narrator, remove_emojis(text), language, directory, os.path.basename(soundFileName)
-                            )
-                        localOutputFileName = os.path.join(directory, os.path.basename(soundFileName))
-
-                        if self.story._cosUploader != None:
-                            self.story._cosUploader.local2cos(localOutputFileName, self.story.storyId, self.story.audioPath)
-            except Exception as e:
-                print(f"Page.test failed for {script}\n", e)
-
-        with open(os.path.join(localOutputPath, fileName), "w") as file:
-            json.dump(
-                self.export(), file, ensure_ascii=False, indent=4, sort_keys=False
-            )
-
-    def updateScript(self, pos, text=None, actor=None, alternativeText=None):
-        if self.type in ("blackboard", "concentrak", "cover", "classroom"):
-            self.updateNarration(pos, text=text, narrator=actor, alternativeText=alternativeText)
+    def updateScript(self, scriptId: int, text=None, actor=None, alternativeText=None, locale=None):
+        locale = self.locale if locale == None else locale
+        if len(self.subscripts) > 0 and scriptId < len(self.subscripts):
+            if text != None:
+                self.subscripts[scriptId]['subscript'][locale] = text 
+            if actor != None:
+                self.subscripts[scriptId]['narrator'] = actor
+            if alternativeText != None:
+                self.subscripts[scriptId]['alternative'][locale] = alternativeText 
+        else:
+            scriptId = scriptId - len(self.subscript)
+            if len(self.narrations) > 0 and scriptId < len(self.narrations):
+                if text != None:
+                    self.narrations[scriptId]['subscript'][locale] = text 
+                if actor != None:
+                    self.narrations[scriptId]['narrator'] = actor
+                if alternativeText != None:
+                    self.narrations[scriptId]['alternative'][locale] = alternativeText             
 
-    def export(self, voiceOffset, pageId):
+    def export(self, voiceOffset=0, pageId=0.0):
         raise NotImplementedError("Subclasses must implement export()")
 
-    def exportScripts(self):
-        return self.export()["voices"]
-
 ##### 问答页面 #####
 class ExamPage(Page):
-    def __init__(self, storyInstance, actor, postures=["smilesay"], audio=None, **kwargs):
+    def __init__(self, storyInstance, actor, postures=["smilesay"]):
         super().__init__("exam", storyInstance)
         self.scene = self.story.styles["scenarios"]["exam"]
-        self.defaultObject = "exam"
-        self.questionSubscripts = [{}]
-        self.questionInteractions = []
-
-        if all(key in kwargs for key in ("voices", "board", "objects", "interactions")):
-            voices = kwargs["voices"]
-            self.board = kwargs["board"]
-            if "content" in self.board and isinstance(self.board["content"], dict):
-                boardContent = self.board["content"]
-                if "options" in boardContent:
-                    for option in (boardContent["options"] if isinstance(boardContent["options"], list) else boardContent["options"][DEFAULT_LANGUAGE]):
-                        if has_chinese_char(option):
-                            self.subscripts.append(
-                                {
-                                    "sound": None,
-                                    "subscript": option,
-                                    "narrator": None
-                                }
-                            )
-            self.objects = kwargs["objects"]
-            self.questionInteractions = kwargs["interactions"]
-            self.actor, _, _, _, _, _ = get_actors(self.objects)
-            for i, interaction in enumerate(self.questionInteractions):
-                if isinstance(interaction, dict):
-                    if "content" in interaction and \
-                        "onResult" in interaction and (interaction["onResult"][0] if isinstance(interaction["onResult"], list) else interaction["onResult"]) == -2:
-                        content = interaction["content"]
-                        if isinstance(content, dict) and "voice" in content:
-                            value = content["voice"]
-                            self.questionSubscripts[0]["sound"] = self.soundFile = voices[value]["sound"]
-                            self.questionSubscripts[0]["subscript"] = self.board["content"]["question"] if ("content" in self.board and isinstance(self.board["content"], dict) and "question" in self.board["content"]) else ""
-                            self.questionSubscripts[0]["narrator"] = self.actor
-                            self.questionSubscripts[0]["languages"] = voices[value]["languages"] if "languages" in voices[value] else None
-                            self.questionInteractions[i]["content"]["voice"] = 0
-                    elif "onResult" in interaction:
-                        value = (interaction["onResult"][0] if isinstance(interaction["onResult"], list) else interaction["onResult"])
-                        if value > -1:
-                            self.correctAnswerId = value
-                        if "content" in interaction and isinstance(interaction["content"].get("text", None), str):
-                            self.subscripts.append(
-                                {
-                                    "sound": None,
-                                    "subscript": interaction["content"]["text"],
-                                    "narrator": None
-                                }
-                            )
-                    elif "type" in interaction and interaction["type"] == "motion" and "figure" in interaction:
-                        postures = interaction["figure"]
-
-        else:
-            self.actor = actor
-            self.soundFile = self.story.getAudioPath(f"voice-{uuid.uuid4()}.mp3" if audio == None else audio)
-            posture_list = (
-                [postures]
-                if (isinstance(postures, str) or isinstance(postures, int))
-                else postures
-            )
-            self.interactions.append(
-                {
-                    "start": "",
-                    "duration": "",
-                    "position": self.story.styles["positions"]["right-bottom"],
-                    "transform": "scale(1.5, 1.5)",
-                    "figure": self.story.getUserPostureId(
-                        actor, posture_list, keyScenario="half"
-                    ),
-                    "type": "motion",
-                    "actor": self._getUserId(self.actor),
-                }
-            )
-
-    def setQuestion(self, question, options, answers=None, **kwargs):
-        assert isinstance(question, str) or isinstance(question, dict)
+        self.actor = actor
 
-        hasChinese = False
-        for option in (options if isinstance(options, list) else options[DEFAULT_LANGUAGE]):
-            if has_chinese_char(option):
-                self.subscripts.append(
-                    {
-                        "sound": None,
-                        "subscript": option,
-                        "narrator": None
-                    }
-                )
-                hasChinese = True
-
-        answer_list = None
-        if hasChinese:
-            if isinstance(answers, dict):
-                answer_list = {}
-                for locale in answers.keys():
-                    answer_list[locale] = [answers[locale]] if not isinstance(answers[locale], list) else answers[locale]
-            else:
-                answer_list = {DEFAULT_LANGUAGE: [answers] if not isinstance(answers, list) else answers}
-            options = options if isinstance(options, dict) else {DEFAULT_LANGUAGE: options}
-        else:
-            answer_list = [] if answers == None else ([answers] if not isinstance(answers, list) else answers)
-            options = options if isinstance(options, list) else options[DEFAULT_LANGUAGE]
+        posture_list = [postures] if (isinstance(postures, str) or isinstance(postures, int)) else postures      
+        self.interactions.append({
+          "start": "",
+          "duration": "",
+          "position": self.story.styles["positions"]["right-bottom"],
+          "transform": "scale(1.5, 1.5)",
+          "figure": self.story.getUserPostureId(actor, posture_list, keyScenario='half'),
+          "type": "motion",
+          "actor": self._getUserId(self.actor)
+        })
+        self.questionInteractions = []
+        self.questionSubscripts = []
 
+    def setQuestion(self, question, options, answers=[], **kwargs):
+        assert isinstance(options, list)
+        answer_list = list(answers) if not isinstance(answers, list) else answers
+        
         self.board = {
-            "content": {
-                "fontSize": kwargs["fontSize"] if "fontSize" in kwargs else 20,
-                "fontColor": kwargs["fontColor"] if "fontColor" in kwargs else "white",
-                "question": question if isinstance(question, dict) else {self.locale: question},
-                "options": options,
-                "answer": answer_list,
-                "colsPerRow": kwargs["colsPerRow"] if "colsPerRow" in kwargs else 1,
-            },
-            "type": "exam",
-            "rect": kwargs["rect"] if "rect" in kwargs else [0, 0, 1, 1],
+          "content": {
+          "fontSize": kwargs["fontSize"] if "fontSize" in kwargs else 20,
+          "fontColor": "white",
+          "question": {self.locale: question},
+          "options": {self.locale: options},
+          "answer": {self.locale: answer_list},
+          "colsPerRow": kwargs["colsPerRow"] if "colsPerRow" in kwargs else 1
+        },
+        "type": "exam",
+        "rect": kwargs["rect"] if "rect" in kwargs else [0, 0, 1, 1]
         }
 
         self.correctAnswerId = 0
-        language = next(iter(options), None) if isinstance(options, dict) else None
-        if (isinstance(answer_list, list) and len(answer_list) > 0) or (isinstance(answer_list, dict) and len(answer_list[language]) > 0):
-            for i, option in enumerate(options[language] if isinstance(options, dict) else options):
-                for entry in (answer_list[language] if (isinstance(options, dict) and isinstance(answer_list, dict)) else answer_list):
-                    if entry == option:
-                        self.correctAnswerId += 2**i
+        for i, option in enumerate(options):
+            for entry in answer_list:
+                if entry == option:
+                    self.correctAnswerId += 2**i
 
         self.questionInteractions = []
+        self.questionSubscripts = []
+        # 错误答案提示行为 onResult: -1
+        self.questionInteractions.append({
+          "start": "",
+          "duration": "",
+          "onResult": -1,
+          "content": {
+            "popup": 4,
+            "voice": -1,
+            "text": {self.locale: kwargs["alwaysTruePrompt"]} if "alwaysTruePrompt" in kwargs else {"cn":"再想想", "en": "Try again"}
+          },
+          "actor": self._getUserId("exam"),
+          "type": "talk"
+        })
 
         # 添加初始化问题语音
-        inputSubscript = {
-            "sound": self.soundFile,
-            "subscript": question if isinstance(question, dict) else {self.locale: question},
-            "narrator": self.actor
-        }
-
-        # 如果新内容与原内容不同。则需先生成test内容，下一步再更新production上内容
-        if self.questionSubscripts[0].get("subscript", None) != (question if isinstance(question, dict) else {self.locale: question}):
-            self.questionSubscripts[0]["subscript"] = (question if isinstance(question, dict) else {self.locale: question})
-            if isinstance(self.questionSubscripts[0].get("sound", None), str) and (self.questionSubscripts[0]["sound"]) > 0:
-                self.questionSubscripts[0]["sound"] = switch_to_test_path(self.questionSubscripts[0]["sound"])
-            else:
-                self.questionSubscripts[0]["sound"] = self.story.getAudioPath(f"voice-{uuid.uuid4()}.mp3")
-            self.questionSubscripts[0]["narrator"] = self.actor
-            self.questionSubscripts[0].pop("languages", None)
-
+        self.questionSubscripts.append({"sound": f"voice-{uuid.uuid4()}.mp3", "subscript":question, "narrator": self.actor})
         # 初始化页面行为 onResult: -2
-        self.questionInteractions.append(
-            {
-                "start": "",
-                "duration": "",
-                "onResult": -2,
-                "content": {
-                    "popup": 4,
-                    "voice": 0,
-                    "text": "",
-                },
-                "actor": self._getUserId(self.defaultObject),
-                "type": "talk",
-            }
-        )
-
-        # 错误答案提示行为 onResult: -1
-        self.questionInteractions.append(
-            {
-                "start": "",
-                "duration": "",
-                "onResult": -1,
-                "content": {
-                    "popup": 4,
-                    "voice": -1,
-                    "text": {DEFAULT_LANGUAGE: "再想想", LANGUAGE_ENG: "Try again"} if "alwaysTruePrompt" not in kwargs
-                        else kwargs["alwaysTruePrompt"] if isinstance(kwargs["alwaysTruePrompt"], dict)
-                        else {self.locale: kwargs["alwaysTruePrompt"]},
-                },
-                "actor": self._getUserId(self.defaultObject),
-                "type": "talk",
-            }
-        )
+        self.questionInteractions.append({
+          "start": "",
+          "duration": "auto",
+          "onResult": -2,
+          "content": {
+            "popup": 4,
+            "voice": len(self.questionSubscripts)-1,
+            "text": ""
+          },
+          "actor": self._getUserId("exam"),
+          "type": "talk"
+        })
 
         # 正确答案行为 onResult: 由所有正确答案id计算所得
-        if self.correctAnswerId > 0:
-            self.questionInteractions.append(
-                {
-                    "start": "",
-                    "duration": "",
-                    "onResult": self.correctAnswerId,
-                    "content": {"popup": 2, "text": ""},
-                    "actor": self._getUserId(self.defaultObject),
-                    "type": "talk",
-                }
-            )
-
+        if self.answerId > 0:
+            self.questionInteractions.append({
+              "start": "",
+              "duration": "",
+              "onResult": self.correctAnswerId,
+              "content": {
+                "popup": 2,
+                "text": ""
+              },
+              "actor": self._getUserId("exam"),
+              "type": "talk"
+            })            
+    
     def setFontSize(self, size):
-        if "content" in self.board and isinstance(self.board["content"], dict):
-            self.board["content"]["fontSize"] = size
-
+        self.board["fontSize"] = size
+    
     def setColsPerRow(self, colsPerRow):
-        if "content" in self.board and isinstance(self.board["content"], dict):
-            self.board["content"]["colsPerRow"] = colsPerRow
+        self.board["colsPerRow"] = colsPerRow
 
     def setRect(self, rect):
-        if isinstance(self.board, dict):
-            self.board["rect"] = rect
+        self.board["rect"] = rect
 
     def setFontColor(self, color):
-        if "content" in self.board and isinstance(self.board["content"], dict):
-            self.board["content"]["fontColor"] = color
-
-    def addImage(self, source, rect=[0, 0, 1, 1], autoFit=True, uploadToCos=True, caption=None):
-        assert len(rect) >= 4 and type(rect) is list
-        width, height = Story.getImageSize(next(iter(source.values()), None) if isinstance(source, dict) else source)
-        assert width > 0 and height > 0
-        assert rect[2] > 0 and rect[3] > 0
-
-        if autoFit:
-            # image is wider in ratio
-            if width / height > (rect[2] if rect[2] > 1.0 else rect[2]*960) / (rect[3] if rect[3] > 1.0 else rect[3]*540):
-                height = round((rect[2] if rect[2] > 1.0 else rect[2]*960) * height / width / (1.0 if rect[3] > 1.0 else 540.0), 3)
-                width = rect[2] * 1.0
-            # vice versa, rect is wider in ratio
-            else:
-                width = round((rect[3] if rect[3] > 1.0 else rect[3]*540) * width / height / (1.0 if rect[2] > 1.0 else 960.0), 3)
-                height = rect[3] * 1.0
-            rect[2] = width
-            rect[3] = height
+        self.board["fontColor"] = color
 
+    def addImage(self, source, rect=[0,0,1,1], **kwargs):
+        assert len(rect)>=4 and type(rect) is list
         if "contentList" not in self.board:
-            self.board["contentList"] = []
-        if  self.story._cosUploader != None and uploadToCos:
-            if isinstance(source, dict):
-                for key in source:
-                    source[key] = self.story._cosUploader.local2cos(source[key], self.story.storyId, self.story.posterPath)
-            else:
-                source = self.story._cosUploader.local2cos(source, self.story.storyId, self.story.posterPath)
-        self.board["contentList"].append(
-            {
-                "image": source,
-                "rect": rect,
-                "caption": ""
-            }
-        )
-        if caption != None and len(caption) > 0:
-            self.board["contentList"][-1]["caption"] = caption if isinstance(caption, dict) else {self.locale: caption}
-
-    def updateImage(self, pos, source, rect=[0, 0, 1, 1], autoFit=True, uploadToCos=True, caption=None):
-        if pos < len(self.board["contentList"]) and pos >= 0:
-            assert len(rect) >= 4 and type(rect) is list
-            width, height = Story.getImageSize(next(iter(source.values()), None) if isinstance(source, dict) else source)
-            assert width > 0 and height > 0
-            assert rect[2] > 0 and rect[3] > 0
-
-            if autoFit:
-                # image is wider in ratio
-                if width / height > (rect[2] if rect[2] > 1.0 else rect[2]*960) / (rect[3] if rect[3] > 1.0 else rect[3]*540):
-                    height = round((rect[2] if rect[2] > 1.0 else rect[2]*960) * height / width / (1.0 if rect[3] > 1.0 else 540.0), 3)
-                    width = rect[2] * 1.0
-                # vice versa, rect is wider in ratio
-                else:
-                    width = round((rect[3] if rect[3] > 1.0 else rect[3]*540) * width / height / (1.0 if rect[2] > 1.0 else 960.0), 3)
-                    height = rect[3] * 1.0
-                rect[2] = width
-                rect[3] = height
-
-            if  self.story._cosUploader != None and uploadToCos:
-                if isinstance(source, dict):
-                    for key in source:
-                        source[key] = self.story._cosUploader.local2cos(source[key], self.story.storyId, self.story.posterPath)
-                else:
-                    source = self.story._cosUploader.local2cos(source, self.story.storyId, self.story.posterPath)
-
-            self.board["contentList"][pos] = {
-                    "image": update_object(self.board["contentList"][pos]["image"], source, self.locale),
-                    "rect": rect,
-                    "caption": ""
-                }
+            self.board["contentList"] = []    
             
-            if caption != None and len(caption) > 0:
-                self.board["contentList"][pos]["caption"] = caption if isinstance(caption, dict) else {self.locale: caption}
-
-    def removeImage(self, pos):
-        if pos < len(self.board["contentList"]) and pos >= 0:
-            self.board["contentList"].pop(pos)
+        if  self.story._cosUploader != None:
+            target_path = kwargs["targetPath"] if "targetPath" in kwargs else None
+            source = self.story._cosUploader.local2cos(source, self.story.storyId, target_path)    
+        
+        self.board["contentList"].append({
+            "caption": {self.locale: kwargs["caption"]} if "caption" in kwargs else "",
+            "rect": rect,
+            "image": {"cn" : source}
+          })
 
     def export(self, voiceOffset=0, pageId=0.0):
-        outInteractions = copy.deepcopy(self.interactions + self.questionInteractions)
-        tempSubscripts = copy.deepcopy(self.subscripts + self.questionSubscripts)
-        outSubscripts = []
-        for subscript in [d for d in tempSubscripts if any(value is not None for value in d.values())]:
-            outSubscripts.append(subscript)
+        outSubscripts = self.subscripts + self.questionSubscripts
+        outInteractions = self.interactions + self.questionInteractions
 
+        interactionOffset = len(self.interactions)
         for i, interaction in enumerate(outInteractions):
-            if isinstance(interaction, dict) and "content" in interaction:
-                content = interaction["content"]
-                if isinstance(content, dict) and "voice" in content:
-                    value = content["voice"]
-                    if value > -1:
-                        outInteractions[i]["content"]["voice"] = value + voiceOffset
-
+            if "content" in interaction and interaction["content"].get("voice", -1) >= 0:
+                outInteractions[i]["content"]["voice"] += voiceOffset + (0 if i < interactionOffset else interactionOffset)
+        
         return {
             "voices": outSubscripts,
             "events": [
                 {
-                    "id": pageId,
-                    "scene": self.scene if isinstance(self.scene, str) else copy.deepcopy(self.scene),
-                    "board": copy.deepcopy(self.board),
-                    "objects": copy.deepcopy(self.objects),
-                    "interactions": outInteractions,
+                "id": pageId,
+                "scene": self.scene,
+                "board": self.board,
+                "objects": self.objects,
+                "interactions": outInteractions
                 }
-            ],
+            ]
         }
 
 ##### 总结页面 #####
 class NotesPage(Page):
-    def __init__(self, storyInstance, actor, postures=["smilesay"], endingEffect=True, audio=None, **kwargs):
+    RESERVED_VOICE = -999
+    def __init__(self, storyInstance, actor, postures=["smilesay"]):
         super().__init__("notes", storyInstance)
         self.scene = self.story.styles["scenarios"]["notes"]["scene"]
         self.board = self.story.styles["scenarios"]["notes"]["board"]
         self.bullets = []
-        self.defaultObject = "notes"
-
-        if all(key in kwargs for key in ("voices", "board", "objects", "interactions")):
-            voices = kwargs["voices"]
-            self.board = kwargs["board"]
-            self.objects = kwargs["objects"]
-            self.interactions = kwargs["interactions"]
-            self.actor, actorId, _, _, defaultObject, _ = get_actors(self.objects)
-            self.defaultObject = defaultObject if defaultObject != None else self.defaultObject
-            html = self.board["content"].get("html", None)
-            self.soundFile = self.story.getAudioPath(f"voice-{uuid.uuid4()}.mp3" if audio == None else audio)
-            self.soundFileLanguages = None
-            self.endingEffect = False
-            if isinstance(html, dict):
-                bullets = {}
-                for key in html.keys():
-                    bullets[key] = get_bullets_from_html(html[key])
-                for i in range(len(bullets[DEFAULT_LANGUAGE])):
-                    self.bullets.append({key: bullets[key][i] for key in bullets.keys()})
-            elif isinstance(html, str):
-                self.bullets = get_bullets_from_html(html)
-            endingPos = -1
-            for i, interaction in enumerate(self.interactions):
-                if isinstance(interaction, dict):
-                    if "content" in interaction:
-                        content = interaction["content"]
-                        if isinstance(content, dict) and "voice" in content:
-                            value = content["voice"]
-                            if value == 0:
-                                self.endingEffect = True
-                                endingPos = i
-                            elif value > 0:
-                                self.soundFile = voices[value]["sound"]
-                                self.soundFileLanguages = voices[value]["languages"] if "languages" in voices[value] else None
-                                self.interactions[i]["content"]["voice"] = 0
-                    elif "type" in interaction and "figure" in interaction:
-                        value = interaction["figure"]
-                        if interaction["type"] == "motion":
-                            postures = value
-                        elif interaction["type"] == "talk":
-                            if interaction["actor"] == actorId and value > -1: 
-                                postures = value
-            if endingPos > -1:
-                self.interactions.pop(endingPos)
-
-            # Remove content from board, leave template only
-            if isinstance(self.board["content"]["html"], dict):
-                key = self.board["content"]["html"].keys()[0]
-                self.board["content"]["html"] = self.board["content"]["html"][key]
-                pattern = r"<ul>(.*?)</ul>"
-                text = self.board["content"]["html"]\
-                    .replace("</ul><ul>", "")\
-                    .replace("</li><li>", "")\
-                    .replace("<li>", "")\
-                    .replace("</li>", "")
-                matches = re.findall(pattern, text, flags=re.DOTALL)
-                for match in matches:
-                    text = text.replace(match, "{}")
-                self.board["content"]["html"] = text
-
-        else:
-            self.actor = actor
-            self.soundFile = self.story.getAudioPath(f"voice-{uuid.uuid4()}.mp3" if audio == None else audio)
-            self.endingEffect = endingEffect
-            self.soundFileLanguages = kwargs["languages"] if ("languages" in kwargs and isinstance(kwargs["languages"], list)) else None
-
-            posture_list = (
-                [postures]
-                if (isinstance(postures, str) or isinstance(postures, int))
-                else postures
-            )
-            self.interactions.insert(
-                0,
-                {
-                    "start": "",
-                    "duration": "",
-                    "position": self.story.styles["positions"]["right-bottom"],
-                    "transform": "scale(1.5, 1.5)",
-                    "figure": self.story.getUserPostureId(
-                        actor, posture_list, keyScenario="half"
-                    ),
-                    "type": "motion",
-                    "actor": self._getUserId(actor),
-                },
-            )
-
-        self.endingInteraction = {
+        self.interactions.append({
             "start": "",
             "duration": "",
-            "content": {"text": "", "voice": 0},
+            "content": {
+                "text": "",
+                "voice": self.RESERVED_VOICE
+            },
             "type": "talk",
-            "actor": self._getUserId(self.defaultObject),
-        }
+            "actor": self._getUserId("ending")
+        })
 
-    def addBullet(self, text):
-        self.bullets.append(text if isinstance(text, dict) else {self.locale: text})
-        self.soundFileLanguages = None
-        if isinstance(self.soundFile, str):
-            self.soundFile = switch_to_test_path(self.soundFile)
-
-    def updateBullet(self, pos, text):
-        if pos < len(self.bullets) and pos >= 0:
-            self.bullets[pos] = update_object(self.bullets[pos], text, self.locale)
-        self.soundFileLanguages = None
-        if isinstance(self.soundFile, str):
-            self.soundFile = switch_to_test_path(self.soundFile)
-
-    def removeBullet(self, pos):
-        if pos < len(self.bullets) and pos >= 0:
-            self.bullets.pop(pos)
-        self.soundFileLanguages = None
-        if isinstance(self.soundFile, str):
-            self.soundFile = switch_to_test_path(self.soundFile)
+        posture_list = [postures] if (isinstance(postures, str) or isinstance(postures, int)) else postures
+        self.interactions.insert(0, {
+            "start": "",
+            "duration": "",
+            "position": self.story.styles["positions"]["right-bottom"],
+            "transform": "scale(1.5, 1.5)",
+            "figure": self.story.getUserPostureId(actor, posture_list, keyScenario='half'),
+            "type": "motion",
+            "actor": self._getUserId(actor)
+        })
+        self.actor = actor
 
-    def setEndingEffect(self, on: bool):
-        self.endingEffect = on
+    def addBullet(self, text):
+        self.bullets.append(text)
 
     def export(self, voiceOffset=0, pageId=0.0):
-        bullets_strings = {}
-        bullets_subscripts = {}
+        bullets_string = subscript = ""
         for bullet in self.bullets:
-            if isinstance(bullet, dict):
-                for key in bullet.keys():
-                    bullets_strings[key] = f"<li>{bullet[key]}</li>" \
-                        if (key not in bullets_strings or bullets_strings[key] == None) \
-                        else bullets_strings[key] + f"<li>{bullet[key]}</li>"
-                    bullets_subscripts[key] = bullet[key] \
-                        if (key not in bullets_subscripts or bullets_subscripts[key] == None) \
-                        else bullets_subscripts[key] + "<break time=\"1500ms\"/>" + bullet[key]
-            else:
-                if self.locale not in bullets_strings:
-                    bullets_strings[self.locale] = ""
-                if self.locale not in bullets_subscripts:
-                    bullets_subscripts[self.locale] = ""
-                bullets_strings[self.locale] = f"<li>{bullet}</li>" \
-                    if bullets_strings[self.locale] in (None, "") \
-                    else bullets_strings[self.locale] + f"<li>{bullet}</li>"
-                bullets_subscripts[self.locale] = bullet \
-                    if bullets_subscripts[self.locale] in (None, "") \
-                    else bullets_subscripts[self.locale] + "<break time=\"1500ms\"/>" + bullet
+            bullets_string += f"<li>{bullet}</li>"
+            subscript += f"{bullet}..."
 
         outBoard = copy.deepcopy(self.board)
-        formatString = outBoard["content"]["html"]
-        outBoard["content"]["html"] = {}
-        for key in bullets_strings:
-            outBoard["content"]["html"][key] = formatString.format(bullets_strings[key])
-
-        tempSubscripts = copy.deepcopy(self.subscripts)
-        tempSubscripts.append(
-            {
-                "sound": self.soundFile,
-                "subscript": bullets_subscripts,
-                "narrator": self.actor,
-            }
-        )
-        if isinstance(self.soundFileLanguages, list):
-            tempSubscripts[-1]["languages"] = self.soundFileLanguages
-        outSubscripts = []
-        for subscript in [d for d in tempSubscripts if any(value is not None for value in d.values())]:
-            outSubscripts.append(subscript)
+        outBoard["content"]["html"] = {self.locale: outBoard["content"]["html"].format(bullets_string)}
+
+        outSubscripts = copy.deepcopy(self.subscripts)
+        outSubscripts.append({"sound": f"voice-{uuid.uuid4()}.mp3", "subscript":{self.locale:subscript}, "narrator": self.actor})
 
         outInteractions = copy.deepcopy(self.interactions)
-        outInteractions.insert(
-            len(outInteractions) - 1,
-            {
-                "start": "",
-                "duration": "",
-                "content": {"popup": 4, "voice": len(outSubscripts) - 1, "text": ""},
-                "type": "talk",
-                "actor": self._getUserId(self.defaultObject),
-            },
-        )
+        outInteractions.insert(len(outInteractions)-1, {
+            "start": "",
+            "duration": "",
+            "content": {"popup": 4, "voice": len(outSubscripts)-1, "text": ""},
+            "type": "talk",
+            "actor": self._getUserId(self.actor)
+        })
         for i, interaction in enumerate(outInteractions):
-            if isinstance(interaction, dict) and "content" in interaction:
-                content = interaction["content"]
-                if isinstance(content, dict) and "voice" in content:
-                    if content["voice"] > -1:
-                        outInteractions[i]["content"]["voice"] += voiceOffset
+            if "content" in interaction:
+                if interaction["content"].get("voice", -1) >= 0:
+                    outInteractions[i]["content"]["voice"] += voiceOffset
+                elif interaction["content"].get("voice", -1) == self.RESERVED_VOICE:
+                    outInteractions[i]["content"]["voice"] = 0
 
         return {
             "voices": outSubscripts,
             "events": [
                 {
-                    "id": pageId,
-                    "scene": self.scene if isinstance(self.scene, str) else copy.deepcopy(self.scene),
-                    "board": outBoard,
-                    "objects": copy.deepcopy(self.objects),
-                    "interactions": outInteractions + [copy.deepcopy(self.endingInteraction)] \
-                        if self.endingEffect \
-                        else outInteractions
+                "id": pageId,
+                "scene": self.scene,
+                "board": outBoard,
+                "objects": self.objects,
+                "interactions": outInteractions
                 }
-            ],
+            ]
         }
 
+##### 黑板页面 #####
+class BlackboardPage(Page):
+    def __init__(self, storyInstance, source, rect=[0,0,1,1]):
+        assert len(rect)>=4 and type(rect) is list
+        super().__init__("blackboard", storyInstance)
+        self.scene = self.story.styles["scenarios"]["blackboard"]
+        self.board = {
+            "content": {"image": source},
+            "rect": rect
+        }
 
-##### 概念页面 #####
-class ConcentrakPage(Page):
-    def __init__(self, storyInstance, text, **kwargs):
-        super().__init__("concentrak", storyInstance)
-        self.scene = self.story.styles["scenarios"]["concentrak"]
-        self.defaultObject = "concentrak"
+    def addNarration(self, text, narrator=None, alternativeText=None):
+        if alternativeText != None:          
+            self.subscripts.append({"sound": f"voice-{uuid.uuid4()}.mp3", 
+                                "subscript":{self.locale: text}, 
+                                "narrator": narrator if narrator!=None else self.narrator
+                                })
+        else:
+            self.subscripts.append({"sound": f"voice-{uuid.uuid4()}.mp3", 
+                                "subscript":{self.locale: text}, 
+                                "narrator": narrator if narrator!=None else self.narrator,
+                                "alternative": {self.locale: alternativeText}})
+        self.interactions.append({
+            "start": "",
+            "duration": "",
+            "content": {
+                "popup": 4,
+                "voice": len(self.subscripts)-1,
+                "text": {self.locale: text}
+            },
+            "actor": self._getUserId(narrator if narrator!=None else self.narrator),
+            "type": "talk"
+        })
 
-        if all(key in kwargs for key in ("voices", "board", "objects", "interactions")):
-            voices = kwargs["voices"]
-            self.objects = kwargs["objects"]
-            self.board = kwargs["board"]
-            self.interactions = kwargs["interactions"]
-            validSubscriptsOffset = 0
-            for i, interaction in enumerate(self.interactions):
-                if isinstance(interaction, dict):
-                    if "content" in interaction:
-                        content = interaction["content"]
-                        if isinstance(content, dict):
-                            if "popup" in content and "text" in content:
-                                text = content["text"]
-                                if content["popup"] == 6:
-                                    self.subscripts.append(
-                                        {
-                                            "sound": None,
-                                            "subscript": text,
-                                            "narrator": None
-                                        }
-                                    )
-                                    validSubscriptsOffset += 1
-                                elif content["popup"] == 4 and "voice" in content and content["voice"] > 0:
-                                    voice = content["voice"]
-                                    if "type" in interaction and interaction["type"] == "talk" and "actor" in interaction:
-                                        actor = interaction["actor"]
-                                        self.subscripts.append(
-                                            {
-                                                "sound": voices[voice]["sound"],
-                                                "subscript": text,
-                                                "narrator": self.objects[actor]["name"]
-                                            }
-                                        )
-                                        if "languages" in voices[voice] and isinstance(voices[voice]["languages"], list):
-                                            self.subscripts[-1]["languages"] = voices[voice]["languages"]
-                                        self.interactions[i]["content"]["voice"] = len(self.subscripts) - 1 - validSubscriptsOffset
-        else:
-            self.interactions.append(
+    def export(self, voiceOffset=0, pageId=0.0):
+        outInteractions = copy.deepcopy(self.interactions)
+        for i, interaction in enumerate(outInteractions):
+            if "content" in interaction and interaction["content"].get("voice", -1) >= 0:
+                outInteractions[i]["content"]["voice"] += voiceOffset
+        return {
+            "voices": self.subscripts,
+            "events": [
                 {
-                    "start": "",
-                    "duration": "",
-                    "actor": self._getUserId(self.defaultObject),
-                    "content": {"popup": 6, "text": text if isinstance(text, dict) else {self.locale: text}},
+                "id": pageId,
+                "scene": self.scene,
+                "board": self.board,
+                "objects": self.objects,
+                "interactions": outInteractions
                 }
-            )
-        self.offset = len(self.interactions)
+            ]
+        }
 
-    def addNarration(self, text, narrator=None, alternativeText=None, audio=None, **kwargs):
-        if alternativeText != None:
-            self.subscripts.append(
-                {
-                    "sound": self.story.getAudioPath(f"voice-{uuid.uuid4()}.mp3" if audio == None else audio),
-                    "subscript": text if isinstance(text, dict) else {self.locale: text},
-                    "narrator": narrator if narrator != None else self.narrator,
-                    "alternative": {self.locale: alternativeText},
-                }
-            )
-            if "languages" in kwargs and isinstance(kwargs["languages"], list):
-                self.subscripts[-1]["languages"] = kwargs["languages"]           
-        else:
-            self.subscripts.append(
-                {
-                    "sound": self.story.getAudioPath(f"voice-{uuid.uuid4()}.mp3" if audio == None else audio),
-                    "subscript": text if isinstance(text, dict) else {self.locale: text},
-                    "narrator": narrator if narrator != None else self.narrator,
-                }
-            )
-            if "languages" in kwargs and isinstance(kwargs["languages"], list):
-                self.subscripts[-1]["languages"] = kwargs["languages"]           
-        self.interactions.append(
-            {
-                "start": "",
-                "duration": "auto",
-                "content": {
-                    "popup": 4,
-                    "voice": len(self.subscripts) - 1,
-                    "text": text if isinstance(text, dict) else {self.locale: text},
-                },
-                "actor": self._getUserId(
-                    narrator if narrator != None else self.narrator
-                ),
-                "type": "talk",
+##### 概念页面 #####
+class ConcentrakPage(Page):
+    def __init__(self, storyInstance, text):
+        super().__init__("concentrak", storyInstance)
+        self.scene = self.story.styles["scenarios"]["concentrak"]
+        self.narrator = ""
+        self.interactions.append({
+            "start": "",
+            "duration": "",
+            "actor": self._getUserId("concentrak"),
+            "content": {
+                "popup": 6,
+                "voice": -1,
+                "text": {self.locale: text}
             }
-        )
-
-    def updateNarration(self, pos, text, narrator=None, alternativeText=None):
-        if pos < len(self.subscripts) and pos >= 0:
-            self.subscripts[pos]["subscript"] = update_object(self.subscripts[pos]["subscript"], text, self.locale)
-            self.interactions[pos+self.offset]["content"]["text"] = update_object(self.interactions[pos+self.offset]["content"]["text"], text, self.locale)
-            if alternativeText != None:
-                self.subscripts[pos]["alternative"] = update_object(self.subscripts[pos]["alternative"], alternativeText, self.locale)
-            self.subscripts[pos]["sound"] = switch_to_test_path(self.subscripts[pos]["sound"])
-            
-            if narrator != None:
-                self.subscripts[pos]["narrator"] = narrator
-                self.interactions[pos+self.offset]["actor"] = self._getUserId(narrator)
-            self.subscripts[pos].pop("languages", None)
-
-    def removeNarration(self, pos):
-        if pos < len(self.subscripts) and pos >= 0:
-            self.subscripts.pop(pos)
-            self.interactions.pop(pos+self.offset)
-            if pos+self.offset < len(self.interactions):
-                for i, interaction in enumerate(self.interactions[pos+self.offset:]):
-                    self.interactions[i]["content"]["voice"] = interaction["content"]["voice"] - 1
+        })
+    
+    def addNarration(self, text, narrator=None, alternativeText=None):            
+        if alternativeText != None:
+            self.subscripts.append({"sound": f"voice-{uuid.uuid4()}.mp3", 
+                                    "subscript":{self.locale: text}, 
+                                    "narrator": narrator if narrator!=None else self.narrator})
+        else:
+            self.subscripts.append({"sound": f"voice-{uuid.uuid4()}.mp3", 
+                                "subscript":{self.locale: text}, 
+                                "narrator": narrator if narrator!=None else self.narrator,
+                                "alternative": {self.locale: alternativeText}})
+        self.interactions.append({
+            "start": "",
+            "duration": "",
+            "content": {
+                "popup": 4,
+                "voice": len(self.subscripts)-1,
+                "text": {self.locale: text}
+            },
+            "actor": self._getUserId(narrator if narrator!=None else self.narrator),
+            "type": "talk"
+        })
 
     def export(self, voiceOffset=0, pageId=0.0):
         outInteractions = copy.deepcopy(self.interactions)
         for i, interaction in enumerate(outInteractions):
-            if (
-                "content" in interaction
-                and interaction["content"].get("voice", -1) >= 0
-            ):
+            if "content" in interaction and interaction["content"].get("voice", -1) >= 0:
                 outInteractions[i]["content"]["voice"] += voiceOffset
-
-        tempSubscripts = copy.deepcopy(self.subscripts)
-        outSubscripts = []
-        for subscript in [d for d in tempSubscripts if any(value is not None for value in d.values())]:
-            outSubscripts.append(subscript)
-
         return {
-            "voices": outSubscripts,
+            "voices": self.subscripts,
             "events": [
                 {
-                    "id": pageId,
-                    "scene": self.scene if isinstance(self.scene, str) else copy.deepcopy(self.scene),
-                    "board": copy.deepcopy(self.board),
-                    "objects": copy.deepcopy(self.objects),
-                    "interactions": outInteractions,
+                "id": pageId,
+                "scene": self.scene,
+                "board": self.board,
+                "objects": self.objects,
+                "interactions": outInteractions
                 }
-            ],
+            ]
         }
 
-
-##### 黑板页面 #####
-class BoardPage(Page):
-    def __init__(self, pageType, storyInstance, source, rect=[0, 0, 1, 1], uploadToCos=True, **kwargs):
-        assert len(rect) >= 4 and type(rect) is list
-        assert pageType in ("cover", "blackboard")
-        super().__init__(pageType, storyInstance)
-        self.scene = self.story.styles["scenarios"][pageType]
-        self.narrator = self.story.narrator
-        self.narratorId = -1
-
-        if all(key in kwargs for key in ("voices", "board", "objects", "interactions")):
-            voices = kwargs["voices"]
-            self.objects = kwargs["objects"]
-            self.board = kwargs["board"]
-            self.interactions = kwargs["interactions"]
-            self.actor, self.actorId, self.narrator, self.narratorId, _, _ = get_actors(self.objects)
-            for i, interaction in enumerate(self.interactions):
-                if isinstance(interaction, dict):
-                    if "content" in interaction:
-                        content = interaction["content"]
-                        if isinstance(content, dict) and "popup" in content and content["popup"] == 4 and "text" in content and "voice" in content:
-                            text = content["text"]
-                            voice = content["voice"]
-                            if "type" in interaction and interaction["type"] == "talk" and "actor" in interaction and voice > 0:
-                                self.subscripts.append(
-                                    {
-                                        "sound": voices[voice]["sound"],
-                                        "subscript": text,
-                                        "narrator": self.narrator if self.narrator != None else self.actor if self.actor != None else self.story.narrator
-                                    }
-                                )
-                                if "languages" in voices[voice] and isinstance(voices[voice]["languages"], list):
-                                    self.subscripts[-1]["languages"] = voices[voice]["languages"]                  
-                                self.interactions[i]["content"]["voice"] = len(self.subscripts) - 1              
-
-        else:
-            if self.story._cosUploader != None and uploadToCos:
-                if isinstance(source, dict):
-                    for key in source.keys():
-                        source[key] = self.story._cosUploader.local2cos(source[key], self.story.storyId, self.story.posterPath)
-                else:
-                    source = self.story._cosUploader.local2cos(source, self.story.storyId, self.story.posterPath)
-
-            self.board = {"content": {"image": source}, "rect": rect}
-
-    def addNarration(self, text, narrator=None, alternativeText=None, audio=None, **kwargs):
+##### 首页页面 #####
+class CoverPage(Page):
+    def __init__(self, storyInstance, source, rect=[0,0,1,1]):
+        assert len(rect)>=4 and type(rect) is list
+        super().__init__("cover", storyInstance)
+        self.scene = self.story.styles["scenarios"]["cover"]
+        self.board = {
+            "content": {"image": source},
+            "rect": rect
+        }
+    
+    def addNarration(self, text, narrator=None, alternativeText=None):            
         if alternativeText != None:
-            self.subscripts.append(
-                {
-                    "sound": self.story.getAudioPath(f"voice-{uuid.uuid4()}.mp3" if audio == None else audio),
-                    "subscript": text if isinstance(text, dict) else {self.locale: text},
-                    "narrator": narrator if narrator != None else self.narrator,
-                    "alternative": {self.locale: alternativeText},
-                }
-            )
-            if "languages" in kwargs and isinstance(kwargs["languages"], list):
-                self.subscripts[-1]["languages"] = kwargs["languages"]           
-        else:
-            self.subscripts.append(
-                {
-                    "sound": self.story.getAudioPath(f"voice-{uuid.uuid4()}.mp3" if audio == None else audio),
-                    "subscript": text if isinstance(text, dict) else {self.locale: text},
-                    "narrator": narrator if narrator != None else self.narrator,
-                }
-            )
-            if "languages" in kwargs and isinstance(kwargs["languages"], list):
-                self.subscripts[-1]["languages"] = kwargs["languages"]           
-        self.interactions.append(
-            {
-                "start": "",
-                "duration": "auto",
-                "content": {
-                    "popup": 4,
-                    "voice": len(self.subscripts) - 1,
-                    "text": text if isinstance(text, dict) else {self.locale: text},
-                },
-                "actor": self._getUserId(
-                    narrator if narrator != None else self.narrator
-                ),
-                "type": "talk",
-            }
-        )
-
-    def updateNarration(self, pos, text, narrator=None, alternativeText=None):
-        if pos < len(self.subscripts) and pos >= 0:
-            self.subscripts[pos]["subscript"] = update_object(self.subscripts[pos]["subscript"], text, self.locale)
-            self.interactions[pos]["content"]["text"] = update_object(self.interactions[pos]["content"]["text"], text, self.locale)
-            self.subscripts[pos]["sound"] = switch_to_test_path(self.subscripts[pos]["sound"])
-            if alternativeText != None:
-                self.subscripts[pos]["alternative"] = update_object(self.subscripts[pos]["alternative"], alternativeText, self.locale)
-            if narrator != None:
-                self.subscripts[pos]["narrator"] = narrator
-                self.interactions[pos]["actor"] = self._getUserId(narrator)
-            self.subscripts[pos].pop("languages", None)
-
-    def removeNarration(self, pos):
-        if pos < len(self.subscripts) and pos >= 0:
-            self.subscripts.pop(pos)
-            self.interactions.pop(pos)
-            if pos < len(self.interactions):
-                for i, interaction in enumerate(self.interactions[pos:]):
-                    self.interactions[i]["content"]["voice"] = interaction["content"]["voice"] - 1
-
-    def updateImage(self, source=None, rect=None, autoFit=False, uploadToCos=True):
-        if source != None:
-            width, height = Story.getImageSize(next(iter(source.values()), None) if isinstance(source, dict) else source)
-            assert width > 0 and height > 0
-            if  self.story._cosUploader != None and uploadToCos:
-                if isinstance(source, dict):
-                    for key in source.keys():
-                        source[key] = self.story._cosUploader.local2cos(source[key], self.story.storyId, self.story.posterPath)
-                else:
-                    source = self.story._cosUploader.local2cos(source, self.story.storyId, self.story.posterPath)
-                
-            self.board["content"]["image"] = update_object(self.board["content"]["image"], source, self.locale)
-            if rect != None:
-                assert rect[2] > 0 and rect[3] > 0
-
-                if autoFit:
-                    # image is wider in ratio
-                    if width / height > (rect[2] if rect[2] > 1.0 else rect[2]*960) / (rect[3] if rect[3] > 1.0 else rect[3]*540):
-                        height = round((rect[2] if rect[2] > 1.0 else rect[2]*960) * height / width / (1.0 if rect[3] > 1.0 else 540.0), 3)
-                        width = rect[2] * 1.0
-                    # vice versa, rect is wider in ratio
-                    else:
-                        width = round((rect[3] if rect[3] > 1.0 else rect[3]*540) * width / height / (1.0 if rect[2] > 1.0 else 960.0), 3)
-                        height = rect[3] * 1.0
-                    rect[2] = width
-                    rect[3] = height
-                self.board["rect"] = rect
+            self.subscripts.append({"sound": f"voice-{uuid.uuid4()}.mp3", 
+                                    "subscript":{self.locale: text}, 
+                                    "narrator": narrator if narrator!=None else self.narrator})
+        else:
+            self.subscripts.append({"sound": f"voice-{uuid.uuid4()}.mp3", 
+                                "subscript":{self.locale: text}, 
+                                "narrator": narrator if narrator!=None else self.narrator,
+                                "alternative": {self.locale: alternativeText}})
+        self.interactions.append({
+            "start": "",
+            "duration": "",
+            "content": {
+                "popup": 4,
+                "voice": len(self.subscripts)-1,
+                "text": {self.locale: text}
+            },
+            "actor": self._getUserId(narrator if narrator!=None else self.narrator),
+            "type": "talk"
+        })
 
     def export(self, voiceOffset=0, pageId=0.0):
         outInteractions = copy.deepcopy(self.interactions)
         for i, interaction in enumerate(outInteractions):
-            if isinstance(interaction, dict) and "content" in interaction:
-                content = interaction["content"]
-                if isinstance(content, dict) and "voice" in content:
-                    value = content.get("voice", -1)
-                    if value > -1:
-                        outInteractions[i]["content"]["voice"] = value + voiceOffset
-
-        tempSubscripts = copy.deepcopy(self.subscripts)
-        outSubscripts = []
-        for subscript in [d for d in tempSubscripts if any(value is not None for value in d.values())]:
-            outSubscripts.append(subscript)
-
+            if "content" in interaction and interaction["content"].get("voice", -1) >= 0:
+                outInteractions[i]["content"]["voice"] += voiceOffset
         return {
-            "voices": outSubscripts,
+            "voices": self.subscripts,
             "events": [
                 {
-                    "id": pageId,
-                    "scene": self.scene if isinstance(self.scene, str) else copy.deepcopy(self.scene),
-                    "board": copy.deepcopy(self.board),
-                    "objects": copy.deepcopy(self.objects),
-                    "interactions": outInteractions,
+                "id": pageId,
+                "scene": self.scene,
+                "board": self.board,
+                "objects": self.objects,
+                "interactions": self.interactions
                 }
-            ],
+            ]
         }
 
-
-##### 黑板页面 #####
-class BlackboardPage(BoardPage):
-    def __init__(self, storyInstance, source, rect=[0, 0, 1, 1], uploadToCos=True, **kwargs):
-        pageType = "blackboard"
-        super().__init__(pageType, storyInstance, source, rect, uploadToCos, **kwargs)
-
-
-##### 封面页面 #####
-class CoverPage(BoardPage):
-    def __init__(self, storyInstance, source, rect=[0, 0, 1, 1], uploadToCos=True, **kwargs):
-        pageType = "cover"
-        super().__init__(pageType, storyInstance, source, rect, uploadToCos, **kwargs)
-
-
 ##### 教室页面 #####
 class ClassroomPage(Page):
-    def __init__(self, storyInstance, actor, postures=["smilesay"], **kwargs):
+    def __init__(self, storyInstance, actor, postures=["smilesay"]):
         super().__init__("classroom", storyInstance)
         self.scene = self.story.styles["scenarios"]["classroom"]
-        self.narrations = {"subscripts": [], "interactions": []}
+        self.narrations = {"subscripts":[], "interactions":[]}
+
+        posture_list = [postures] if (isinstance(postures, str) or isinstance(postures, int)) else postures
+        self.subscripts.insert(0, {
+            "sound": f"voice-{uuid.uuid4()}.mp3", 
+            "subscript":{self.locale: ""}, 
+            "narrator": actor
+        })
+        self.interactions.insert(0, {
+            "start": "",
+            "duration": "",
+            "content": {
+                "popup": self.story.styles["popup"],
+                "voice": 0,
+                "text": {self.locale: ""}
+            },
+            "figure": self.story.getUserPostureId(actor, posture_list, keyScenario='-stand-'),
+            "position": self.story.styles["positions"]["left" if actor == "boy" else "right"],
+            "transform": f'scale({self.story.styles["scale"]}, {self.story.styles["scale"]})',
+            "type": "talk",
+            "actor": self._getUserId(actor)
+        })
+        self.actor = actor
         self.hasImage = False
 
-        if all(key in kwargs for key in ("voices", "board", "objects", "interactions")):
-            voices = kwargs["voices"]
-            self.objects = kwargs["objects"]
-            self.board = kwargs["board"]
-            if "rect" in self.board and isinstance(self.board["rect"], list):
-                self.hasImage = True
-            for i, interaction in enumerate(kwargs["interactions"]):
-                if isinstance(interaction, dict):
-                    if (("onResult" in interaction and (interaction["onResult"][0] if isinstance(interaction["onResult"], list) else interaction["onResult"]) == 1) \
-                        or ("onPoster" in interaction and (interaction["onPoster"][0] if isinstance(interaction["onPoster"], list) else interaction["onPoster"]) == 1)) \
-                        and "type" in interaction and interaction["type"] == "talk" and "actor" in interaction and "content" in interaction:
-                        actor = interaction["actor"]
-                        content = interaction["content"]
-                        if isinstance(content, dict) and "text" in content and "voice" in content and content["voice"] > 0:
-                            text = content["text"]
-                            voice = content["voice"]
-                            self.narrations["subscripts"].append(
-                                {
-                                    "sound": voices[voice]["sound"],
-                                    "subscript": text,
-                                    "narrator": self.objects[actor]["name"]
-                                }
-                            )
-                            if "languages" in voices[voice] and isinstance(voices[voice]["languages"], list):
-                                self.narrations["subscripts"][-1]["languages"] = voices[voice]["languages"]
-                            interaction["content"]["voice"] = len(self.narrations["subscripts"]) - 1
-                            self.narrations["interactions"].append(interaction)
-                    elif "type" in interaction and interaction["type"] == "talk" and "actor" in interaction and "content" in interaction:
-                        actor = interaction["actor"]                        
-                        content = interaction["content"]
-                        if isinstance(content, dict) and "text" in content and "voice" in content and content["voice"] > 0:
-                            text = content["text"]
-                            voice = content["voice"]   
-                            self.interactions.append(interaction)
-                            self.subscripts.append({
-                                "sound": voices[voice]["sound"],
-                                "subscript": text,
-                                "narrator": self.objects[actor]["name"]
-                            })
-                            if "languages" in voices[voice] and isinstance(voices[voice]["languages"], list):
-                                self.subscripts[0]["languages"] = voices[voice]["languages"]
-                            self.interactions[-1]["content"]["voice"] = len(self.subscripts) - 1
-        else:
-            posture_list = (
-                [postures]
-                if (isinstance(postures, str) or isinstance(postures, int))
-                else postures
-            )
-            self.subscripts.append({
-                "sound": "",
-                "subscript": None,
-                "narrator": actor,
-            }),
-            self.interactions.append({
-            
-                "start": "",
-                "duration": "",
-                "content": {
-                    "popup": self.story.styles["popup"],
-                    "voice": 0,
-                    "text": {self.locale: ""},
-                },
-                "figure": self.story.getUserPostureId(
-                    actor, posture_list, keyScenario="-stand-"
-                ),
-                "position": self.story.styles["positions"][
-                    "left" if actor == "boy" else "right"
-                ],
-                "transform": f'scale({self.story.styles["scale"]}, {self.story.styles["scale"]})',
-                "type": "talk",
-                "actor": self._getUserId(actor),
-            })
-            self.actor = actor
-
-    def setDialog(self, text, alternativeText=None, **kwargs):
-        self.subscripts[0]["subscript"] = text if isinstance(text, dict) else {self.locale: text}
-        if isinstance(self.subscripts[0]["sound"], str) and len(self.subscripts[0]["sound"]) > 0:
-            self.subscripts[0]["sound"] = switch_to_test_path(self.subscripts[0]["sound"])
-        else:
-            self.subscripts[0]["sound"] = self.story.getAudioPath(f"voice-{uuid.uuid4()}.mp3")
-        if "languages" in kwargs and isinstance(kwargs["languages"], list):
-            self.subscripts[0]["languages"] = kwargs["languages"]
-        else:
-            self.subscripts[0].pop("languages", None)     
+    def setVoice(self, text, alternativeText=None):
+        self.subscripts[0]["subscript"][self.locale] = text
         if alternativeText != None:
-            self.subscripts[0]["alternativeText"] = alternativeText if isinstance(alternativeText, dict) else {self.locale: alternativeText}
-        self.interactions[0]["content"]["text"] = text if isinstance(text, dict) else {self.locale: text}
+            self.subscripts[0]["alternativeText"][self.locale] = alternativeText
+        self.interactions[0]["content"]["text"][self.locale] = text
 
-    def setImage(self, source, rect=[0.2, 0.2, 400, 400], autoFit=True, uploadToCos=True, **kwargs):
-        assert len(rect) >= 4 and type(rect) is list
-        width, height = Story.getImageSize(next(iter(source.values()), None) if isinstance(source, dict) else source)
+    def setImage(self, source, autoFit=True, rect=[0.2,0.2,400,400], **kwargs):
+        assert len(rect)>=4 and type(rect) is list
+        width, height = Story.getImageSize(source)
         assert width > 0 and height > 0
         assert rect[2] > 0 and rect[3] > 0
 
         if autoFit:
-            # image is wider in ratio
-            if width / height > (rect[2] if rect[2] > 1.0 else rect[2]*960) / (rect[3] if rect[3] > 1.0 else rect[3]*540):
-                height = round((rect[2] if rect[2] > 1.0 else rect[2]*960) * height / width / (1.0 if rect[3] > 1.0 else 540.0), 3)
-                width = rect[2] * 1.0
+            #image is wider in ratio
+            if width/height > rect[2]/rect[3]:
+                height = rect[2]*height/width
+                width = rect[2]
             # vice versa, rect is wider in ratio
             else:
-                width = round((rect[3] if rect[3] > 1.0 else rect[3]*540) * width / height / (1.0 if rect[2] > 1.0 else 960.0), 3)
-                height = rect[3] * 1.0
-            rect[2] = width
-            rect[3] = height
-
-            if self.actor == "boy":
-                if rect[2] > 1.0:
-                    rect[0] = round(((1 - rect[0]) if rect[0] <= 1.0 else rect[0]/960.0) - rect[2]/960.0, 3)
-                elif rect[2] < 1.0:
-                    rect[0] = ((1 - rect[0]) if rect[0] <= 1.0 else rect[0]/960.0) - rect[2]
-
-        if self.story._cosUploader != None and uploadToCos:
-            if isinstance(source, dict):
-                for key in source.keys():
-                    source[key] = self.story._cosUploader.local2cos(source[key], self.story.storyId, self.story.posterPath)
-            else:
-                source = self.story._cosUploader.local2cos(source, self.story.storyId, self.story.posterPath)
+                width = rect[3]*width/height
+                height = rect[3]
+
+        if autoFit and self.actor == "girl":
+            if rect[3] > 1.0:
+                rect[0] = 960 * 0.9 - rect[3]
+            elif rect[3] < 1.0:
+                rect[0] = 0.9 - rect[3]
+
+        if self.story._cosUploader != None:
+            target_path = kwargs["targetPath"] if "targetPath" in kwargs else None
+            source = self.story._cosUploader.local2cos(source, self.story.storyId, target_path)
 
         self.board = {
             "content": {
                 "caption": kwargs["caption"] if "caption" in kwargs else "",
                 "fontSize": kwargs["fontSize"] if "fontSize" in kwargs else "24px",
                 "fontColor": kwargs["fontColor"] if "fontColor" in kwargs else "white",
-                "image": source,
+                "image": {"cn" : source},
                 "magnify": True,
-                "border": self.story.styles["frame"],
+                "border": self.story.styles["frame"]
             },
-            "rect": rect,
+            "rect": rect
         }
         self.hasImage = True
 
-    def setVideo(self, source, autoFit=True, rect=[0.1, 0.1, 640, 360], **kwargs):
-        assert len(rect) >= 4 and type(rect) is list
-
-        if autoFit and self.actor == "boy":
-            if rect[2] > 1.0:
-                rect[0] = round(0.9 - rect[2]/0.9, 3)
-            elif rect[2] < 1.0:
-                rect[0] = 0.9 - rect[2]
+    def setVideo(self, source, autoFit=True, rect=[0.1,0.1,640,360], **kwargs):
+        assert len(rect)>=4 and type(rect) is list
 
+        if autoFit and self.actor == "girl":
+            if rect[3] > 1.0:
+                rect[0] = 960 * 0.9 - rect[3]
+            elif rect[3] < 1.0:
+                rect[0] = 0.9 - rect[3]
+            
         self.board = {
             "content": {
                 "caption": kwargs["caption"] if "caption" in kwargs else "",
                 "fontSize": kwargs["fontSize"] if "fontSize" in kwargs else "24px",
                 "fontColor": kwargs["fontColor"] if "fontColor" in kwargs else "white",
                 "src": source,
-                "border": self.story.styles["frame"],
+                "border": self.story.styles["frame"]
             },
-            "rect": rect,
+            "rect": rect
         }
         if "videoType" in kwargs:
             self.board["content"]["videoType"] = kwargs["videoType"].lower()
         self.hasImage = True
 
-    def addNarration(self, text, narrator=None, alternativeText=None, audio=None, **kwargs):
-        if alternativeText != None:
-            self.narrations["subscripts"].append(
-                {
-                    "sound": self.story.getAudioPath(f"voice-{uuid.uuid4()}.mp3" if audio == None else audio),
-                    "subscript": text if isinstance(text, dict) else {self.locale: text},
-                    "narrator": narrator if narrator != None else self.narrator,
-                    "alternative": alternativeText if isinstance(alternativeText, dict) else {self.locale: alternativeText},
-                }
-            )
-            if "languages" in kwargs and isinstance(kwargs["languages"], list):
-                self.subscripts[-1]["languages"] = kwargs["languages"]           
-        else:
-            self.narrations["subscripts"].append(
-                {
-                    "sound": self.story.getAudioPath(f"voice-{uuid.uuid4()}.mp3" if audio == None else audio),
-                    "subscript": text if isinstance(text, dict) else {self.locale: text},
-                    "narrator": narrator if narrator != None else self.narrator,
-                }
-            )
-            if "languages" in kwargs and isinstance(kwargs["languages"], list):
-                self.subscripts[-1]["languages"] = kwargs["languages"]           
-        self.narrations["interactions"].append(
-            {
-                "start": "",
-                "duration": "auto",
-                "content": {
-                    "popup": 4,
-                    "voice": len(self.narrations["subscripts"]) - 1,
-                    "text": text if isinstance(text, dict) else {self.locale: text},
-                },
-                "onPoster": 1,
-                "actor": self._getUserId(
-                    narrator if narrator != None else self.narrator
-                ),
-                "type": "talk",
-            }
-        )
-
-    def updateDialog(self, text=None, alternativeText=None):
-        if text != None:
-            self.subscripts[0]["subscript"] = update_object(self.subscripts[0]["subscript"], text, self.locale)
+    def addNarration(self, text, narrator=None, alternativeText=None):
         if alternativeText != None:
-            self.subscripts[0]["alternative"] = update_object(self.subscripts[0]["alternative"] \
-                                                                if "alternative" in self.subscripts[0] \
-                                                                else {}, \
-                                                                alternativeText, self.locale)
-        self.subscripts[0]["sound"] = switch_to_test_path(self.subscripts[0]["sound"])
-        self.subscripts[0].pop("languages", None)
-
-    def updateNarration(self, pos, text, narrator=None, alternativeText=None):
-        if pos < len(self.narrations["subscripts"]) and pos >= 0:
-            self.narrations["subscripts"][pos]["subscript"] = update_object(self.narrations["subscripts"][pos]["subscript"], text, self.locale)
-            self.narrations["interactions"][pos]["content"]["text"] = update_object(self.narrations["interactions"][pos]["content"]["text"], text, self.locale)
-            if alternativeText != None:
-                self.narrations["subscripts"][pos]["alternative"] = update_object(self.narrations["subscripts"][pos]["alternative"], alternativeText, self.locale)
-            
-            if narrator != None:
-                self.narrations["subscripts"][pos]["narrator"] = narrator
-                self.narrations["interactions"][pos]["actor"] = self._getUserId(narrator)
-            self.narrations["subscripts"][pos]["sound"] = switch_to_test_path(self.narrations["subscripts"][pos]["sound"])
-            self.narrations["subscripts"][pos].pop("languages", None)
-
-    def removeNarration(self, pos):
-        if pos < len(self.narrations["subscripts"]) and pos > 0:
-            self.narrations["subscripts"].pop(pos)
-            self.narrations["interactions"].pop(pos)
-            if pos < len(self.narrations["interactions"]):
-                for i, interaction in enumerate(self.narrations["interactions"][pos:]):
-                    self.narrations["interactions"][i]["content"]["voice"] = interaction["content"]["voice"] - 1
+            self.narrations["subscripts"].append({"sound": f"voice-{uuid.uuid4()}.mp3", 
+                                                  "subscript":{self.locale: text}, 
+                                                  "narrator": narrator if narrator!=None else self.narrator})
+        else:
+            self.subscripts.append({"sound": f"voice-{uuid.uuid4()}.mp3", 
+                                "subscript":{self.locale: text}, 
+                                "narrator": narrator if narrator!=None else self.narrator,
+                                "alternative": {self.locale: alternativeText}})
+        self.narrations["interactions"].append({
+            "start": "",
+            "duration": "auto",
+            "content": {
+                "popup": 4,
+                "voice": len(self.narrations["subscripts"])-1,
+                "text": {self.locale: text}
+            },
+            "onPoster": 1,
+            "actor": self._getUserId(narrator if narrator!=None else self.narrator),
+            "type": "talk"
+        })
 
     def export(self, voiceOffset=0, pageId=0.0):
-        tempSubscripts = copy.deepcopy(self.subscripts)
+        outSubscripts = copy.deepcopy(self.subscripts)
         outInteractions = copy.deepcopy(self.interactions)
         outNarrations = copy.deepcopy(self.narrations)
 
         if self.hasImage:
             for i, interaction in enumerate(outInteractions):
                 if interaction["type"] != "motion":
                     outInteractions[i]["duration"] = "auto"
                     outInteractions[i]["content"]["popup"] = 4
 
-        narrationOffset = len(tempSubscripts)
-        tempSubscripts = tempSubscripts + outNarrations["subscripts"]
-
-        outSubscripts = []
-        for subscript in [d for d in tempSubscripts if any(value is not None for value in d.values())]:
-            outSubscripts.append(subscript)
-
+        outSubscripts = outSubscripts + outNarrations["subscripts"]
+        narrationOffset = len(outSubscripts)
         for i, interaction in enumerate(outNarrations["interactions"]):
-            outNarrations["interactions"][i]["content"]["voice"] = outNarrations["interactions"][i]["content"]["voice"] + narrationOffset
+            outNarrations["interactions"][i]["content"]["voice"] += narrationOffset
             outInteractions.append(outNarrations["interactions"][i])
 
         for j, interaction in enumerate(outInteractions):
-            if (
-                "content" in interaction
-                and interaction["content"].get("voice", -1) >= 0
-            ):
-                outInteractions[j]["content"]["voice"] = outInteractions[j]["content"]["voice"] + voiceOffset
+            if "content" in interaction and interaction["content"].get("voice", -1) >= 0:
+                outInteractions[j]["content"]["voice"] += voiceOffset
         return {
             "voices": outSubscripts,
             "events": [
                 {
-                    "id": pageId,
-                    "scene": self.scene if isinstance(self.scene, str) else copy.deepcopy(self.scene),
-                    "board": copy.deepcopy(self.board),
-                    "objects": copy.deepcopy(self.objects),
-                    "interactions": outInteractions,
+                "id": pageId,
+                "scene": self.scene,
+                "board": self.board,
+                "objects": self.objects,
+                "interactions": outInteractions
                 }
-            ],
-        }
+            ]
+        }
```

## storybuilder/storyprofiles.py

```diff
@@ -90,28 +90,34 @@
         '数数': '暑shù',
         '∠': '角',
         '°': '度',
         '<ul>': '',
         '</ul>': '',
         '<li>': '',
         '</li>': '。',
+        '😳': '',
+        '😄': '',
+        '💡': '',
         '·': '-',
         '>': '大于',
         '<': '小于',
         '>=': '大于等于',
         '<=': '小于等于',
         'WHO': 'WH欧',
         'elif': 'L-If',
         'for': 'four',
     },
     "en-US": {
         '<ul>': '',
         '</ul>': '',
         '<li>': '',
         '</li>': '。',
+        '😳': '',
+        '😄': '',
+        '💡': '',
     }
 }
 
 CHARACTER_FIGURE_ACCESSORY_KEYS = ['mask', 'cap']
 
 STORY_SCENARIO_STYLES = {
     "shinkai_makoto": {
@@ -120,52 +126,52 @@
             "classroom": "475dc094-e147-478e-a1cf-770df5efa081",
             "notes": {
                 "scene":"ce3ae229-7e6b-4e10-9d0a-e5e53d923d61",
                 "board":{
                     "content":{
                         "rect": [0.2, 0.2, 0.6, 0.8], 
                         "type": "notes", 
-                        "html":"<h2 style=\'color:white\'><br/><ul>{}</ul></h2>"
+                        "html":"<h2 style='color:white'><br/><ul>{}</ul></h2>"
                     }
                 }
             },
             "exam": "a65ed1dc-9e27-4c3d-a5f7-090fc2af4917",
             "blackboard": {"bgColor": "#98A698"},
             "concentrak": {"index": "0bd6c33e-31eb-4083-8dd8-ee07837bc975", "bgColor": "#C1D0BA"},
         },
         "frame": "10px solid #843C0C",
         "positions": {
             "left": [0.2, 0.05],
             "right": [0.8, 0.05],
-            "right-bottom": [0.85, -0.05],
+            "right_bottom": [0.85, -0.05],
         },
         "popup": 11,
         "scale": 1
     },
     "close_up": {
         "scenarios": {
             "cover": "5cdab8ba-c028-45ea-87cc-b0d75dd81e10",
             "classroom": "b99b0dc2-0387-4a4f-9c61-308b362cb8f6",
             "notes": {
                 "scene": "6c5c45c3-070f-439a-a6f7-a366a04c357c",
                 "board":{
                     "content":{
                         "rect": [0.1, 0.28, 0.7, 0.5], 
                         "type": "notes", 
-                        "html":"<p><ul style=\'color: white\' size='5'>{}</ul></p>"
+                        "html":"<p><ul style='color: white' size='5'>{}</ul></p>"
                     }
                 }
             },
             "exam": "ea874992-c7a9-44c4-8bef-13cad8cee917",
             "blackboard": "e183c517-cbb7-4831-bcf6-efd310ee8790",
             "concentrak": {"index": "0bd6c33e-31eb-4083-8dd8-ee07837bc975", "bgColor": "#9BB9BF"},
         },
         "frame": "10px solid #843C0C",
         "positions": {
             "left": [0.2, -0.25],
             "right": [0.8, -0.25],
-            "right-bottom": [0.8, 0.05],
+            "right_bottom": [0.8, 0.05],
         },
         "popup": 10,
         "scale": 2
     }
 }
```

## storybuilder/storyvoicebuilder.py

```diff
@@ -37,20 +37,21 @@
         synthesizer = speech_synthesizer(speech_key=self.subscription, service_region=self.region)
 
         character = character if character != '' else 'M'
         synthesizer.set_voice(
             language,
             CHARACTER_VOICE_PROFILES[character][language]['voiceName'],
             **CHARACTER_VOICE_PROFILES[character][language]['kwargs'])
-        if fileName == None or len(fileName) < 1:
+
+        if fileName == None:
             fileName = self._newAudioFileName(language)
             print(f'No input file_name, generate new file name as: {fileName}')
         elif language.lower() not in ('cn', 'zh-cn'):
             fileName = self._fixAudioFileName(fileName, language)
-            print(f'Filename with language code: {fileName}')
+            print(f'Adjust file_name with language code as: {fileName}')
 
         print('Original:', text)
         newText = text
         for symbol in stopSymbols:
             newText = newText.split(symbol)[0]
         print('Corrected:', newText)
```

## Comparing `storybuilder-0.0.41.dist-info/LICENSE` & `storybuilder-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `storybuilder-0.0.41.dist-info/METADATA` & `storybuilder-0.0.9.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 Metadata-Version: 2.1
 Name: storybuilder
-Version: 0.0.41
+Version: 0.0.9
 Summary: A Python toolkit to build story meta.
 Author-email: Kelvin Xu <xxk59@hotmail.com>
 Project-URL: Homepage, https://github.com/xxk59/StoryBuilder
 Project-URL: Issues, https://github.com/xxk59/StoryBuilder/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Pillow
-Requires-Dist: azure-cognitiveservices-speech
-Requires-Dist: cos-python-sdk-v5
-Requires-Dist: pydub
-Requires-Dist: pyperclip
-Requires-Dist: ffmpeg
 
 # StoryBuilder
 
 Toolkit to build a story meta
 
 # Pre-requisites
```

