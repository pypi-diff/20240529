# Comparing `tmp/p-template-generator-0.1.99.tar.gz` & `tmp/p_template_generator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p-template-generator-0.1.99.tar", last modified: Thu Dec 28 05:10:56 2023, max compression
+gzip compressed data, was "p_template_generator-0.2.0.tar", last modified: Tue May 28 12:31:24 2024, max compression
```

## Comparing `p-template-generator-0.1.99.tar` & `p_template_generator-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-12-28 05:10:56.369647 p-template-generator-0.1.99/
--rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-template-generator-0.1.99/LICENSE
--rw-rw-rw-   0        0        0      406 2023-12-28 05:10:56.369647 p-template-generator-0.1.99/PKG-INFO
--rw-rw-rw-   0        0        0       20 2023-03-14 06:24:47.000000 p-template-generator-0.1.99/README.md
-drwxrwxrwx   0        0        0        0 2023-12-28 05:10:56.344969 p-template-generator-0.1.99/p_template_generator.egg-info/
--rw-rw-rw-   0        0        0      406 2023-12-28 05:10:56.000000 p-template-generator-0.1.99/p_template_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      868 2023-12-28 05:10:56.000000 p-template-generator-0.1.99/p_template_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-28 05:10:56.000000 p-template-generator-0.1.99/p_template_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-12-28 05:10:56.000000 p-template-generator-0.1.99/p_template_generator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-12-28 05:10:56.000000 p-template-generator-0.1.99/p_template_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-12-28 05:10:56.000000 p-template-generator-0.1.99/p_template_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-28 05:10:56.370643 p-template-generator-0.1.99/setup.cfg
--rw-rw-rw-   0        0        0      993 2023-12-28 05:10:46.000000 p-template-generator-0.1.99/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-28 05:10:56.353426 p-template-generator-0.1.99/template_generator/
--rw-rw-rw-   0        0        0        0 2023-12-28 02:03:28.000000 p-template-generator-0.1.99/template_generator/__init__.py
--rw-rw-rw-   0        0        0     6065 2023-11-30 12:32:15.000000 p-template-generator-0.1.99/template_generator/aigc_input.py
-drwxrwxrwx   0        0        0        0 2023-12-28 05:10:56.355114 p-template-generator-0.1.99/template_generator/bin/
--rw-rw-rw-   0        0        0        0 2023-12-28 02:03:28.000000 p-template-generator-0.1.99/template_generator/bin/__init__.py
--rw-rw-rw-   0        0        0      709 2023-11-30 12:32:25.000000 p-template-generator-0.1.99/template_generator/bin/print_md5.py
--rw-rw-rw-   0        0        0     4875 2023-12-28 05:10:29.000000 p-template-generator-0.1.99/template_generator/binary.py
-drwxrwxrwx   0        0        0        0 2023-12-28 05:10:56.359125 p-template-generator-0.1.99/template_generator/convertor/
--rw-rw-rw-   0        0        0        0 2023-12-28 02:03:28.000000 p-template-generator-0.1.99/template_generator/convertor/__init__.py
--rw-rw-rw-   0        0        0     8692 2023-11-21 09:36:44.000000 p-template-generator-0.1.99/template_generator/convertor/convertor.py
--rw-rw-rw-   0        0        0    55927 2023-11-10 11:06:14.000000 p-template-generator-0.1.99/template_generator/convertor/of_to_skymedia.py
--rw-rw-rw-   0        0        0     4269 2023-11-28 10:25:30.000000 p-template-generator-0.1.99/template_generator/ffmpeg.py
--rw-rw-rw-   0        0        0     9455 2023-11-30 12:31:34.000000 p-template-generator-0.1.99/template_generator/main.py
--rw-rw-rw-   0        0        0     8693 2023-12-02 09:28:58.000000 p-template-generator-0.1.99/template_generator/server_generator.py
--rw-rw-rw-   0        0        0    15537 2023-12-04 05:39:09.000000 p-template-generator-0.1.99/template_generator/template.py
--rw-rw-rw-   0        0        0     3822 2023-11-30 09:02:49.000000 p-template-generator-0.1.99/template_generator/template_service.py
--rw-rw-rw-   0        0        0    10941 2023-12-27 07:06:17.000000 p-template-generator-0.1.99/template_generator/template_test.py
-drwxrwxrwx   0        0        0        0 2023-12-28 05:10:56.360125 p-template-generator-0.1.99/template_generator/test/
--rw-rw-rw-   0        0        0        0 2023-12-28 02:03:28.000000 p-template-generator-0.1.99/template_generator/test/__init__.py
--rw-rw-rw-   0        0        0  9341185 2023-11-21 10:17:45.000000 p-template-generator-0.1.99/template_generator/test/tp_2023112102.zip.py
+drwxrwxrwx   0        0        0        0 2024-05-28 12:31:24.968364 p_template_generator-0.2.0/
+-rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p_template_generator-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      610 2024-05-28 12:31:24.967365 p_template_generator-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       20 2023-03-14 06:24:47.000000 p_template_generator-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 12:31:24.966364 p_template_generator-0.2.0/p_template_generator.egg-info/
+-rw-rw-rw-   0        0        0      610 2024-05-28 12:31:24.000000 p_template_generator-0.2.0/p_template_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      868 2024-05-28 12:31:24.000000 p_template_generator-0.2.0/p_template_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 12:31:24.000000 p_template_generator-0.2.0/p_template_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-28 12:31:24.000000 p_template_generator-0.2.0/p_template_generator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       77 2024-05-28 12:31:24.000000 p_template_generator-0.2.0/p_template_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-28 12:31:24.000000 p_template_generator-0.2.0/p_template_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 12:31:24.968364 p_template_generator-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      977 2024-05-28 12:31:05.000000 p_template_generator-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 12:31:24.952846 p_template_generator-0.2.0/template_generator/
+-rw-rw-rw-   0        0        0        0 2024-05-25 03:39:47.000000 p_template_generator-0.2.0/template_generator/__init__.py
+-rw-rw-rw-   0        0        0     6065 2023-11-30 12:32:15.000000 p_template_generator-0.2.0/template_generator/aigc_input.py
+drwxrwxrwx   0        0        0        0 2024-05-28 12:31:24.953847 p_template_generator-0.2.0/template_generator/bin/
+-rw-rw-rw-   0        0        0        0 2024-05-25 03:39:47.000000 p_template_generator-0.2.0/template_generator/bin/__init__.py
+-rw-rw-rw-   0        0        0      709 2023-11-30 12:32:25.000000 p_template_generator-0.2.0/template_generator/bin/print_md5.py
+-rw-rw-rw-   0        0        0     8171 2024-05-28 12:29:21.000000 p_template_generator-0.2.0/template_generator/binary.py
+drwxrwxrwx   0        0        0        0 2024-05-28 12:31:24.957848 p_template_generator-0.2.0/template_generator/convertor/
+-rw-rw-rw-   0        0        0        0 2024-05-25 03:39:47.000000 p_template_generator-0.2.0/template_generator/convertor/__init__.py
+-rw-rw-rw-   0        0        0     8692 2023-11-21 09:36:44.000000 p_template_generator-0.2.0/template_generator/convertor/convertor.py
+-rw-rw-rw-   0        0        0    55822 2023-12-28 10:41:57.000000 p_template_generator-0.2.0/template_generator/convertor/of_to_skymedia.py
+-rw-rw-rw-   0        0        0     6075 2024-04-29 13:07:26.000000 p_template_generator-0.2.0/template_generator/ffmpeg.py
+-rw-rw-rw-   0        0        0     9455 2023-11-30 12:31:34.000000 p_template_generator-0.2.0/template_generator/main.py
+-rw-rw-rw-   0        0        0     8693 2024-02-26 04:09:02.000000 p_template_generator-0.2.0/template_generator/server_generator.py
+-rw-rw-rw-   0        0        0    16123 2024-04-21 14:16:48.000000 p_template_generator-0.2.0/template_generator/template.py
+-rw-rw-rw-   0        0        0     3826 2024-01-29 06:20:08.000000 p_template_generator-0.2.0/template_generator/template_service.py
+-rw-rw-rw-   0        0        0    11945 2024-04-29 13:07:26.000000 p_template_generator-0.2.0/template_generator/template_test.py
+drwxrwxrwx   0        0        0        0 2024-05-28 12:31:24.959847 p_template_generator-0.2.0/template_generator/test/
+-rw-rw-rw-   0        0        0        0 2024-05-25 03:39:47.000000 p_template_generator-0.2.0/template_generator/test/__init__.py
+-rw-rw-rw-   0        0        0  9341185 2023-11-21 10:17:45.000000 p_template_generator-0.2.0/template_generator/test/tp_2023112102.zip.py
```

### Comparing `p-template-generator-0.1.99/LICENSE` & `p_template_generator-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `p-template-generator-0.1.99/p_template_generator.egg-info/SOURCES.txt` & `p_template_generator-0.2.0/p_template_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `p-template-generator-0.1.99/setup.py` & `p_template_generator-0.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="p-template-generator",
-    version="0.1.99",
+    version="0.2.0",
     author="pengjun",
     author_email="mr_lonely@foxmail.com",
     description="temple tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
@@ -20,16 +20,16 @@
     install_requires=[
         'requests',
         'Image',
         'protobuf',
         'imagesize',
         'urlparser',
         'Pillow',
-        'mecord-cli>=0.4.10',
-        'p-template-res>=0.2.5',
+        'mecord-cli',
+        'p-template-res',
     ],
     dependency_links=[],
     entry_points={
         'console_scripts':[
             'template = template_generator.main:main'
         ]
     },
```

### Comparing `p-template-generator-0.1.99/template_generator/aigc_input.py` & `p_template_generator-0.2.0/template_generator/aigc_input.py`

 * *Files identical despite different names*

### Comparing `p-template-generator-0.1.99/template_generator/bin/print_md5.py` & `p_template_generator-0.2.0/template_generator/bin/print_md5.py`

 * *Files identical despite different names*

### Comparing `p-template-generator-0.1.99/template_generator/convertor/convertor.py` & `p_template_generator-0.2.0/template_generator/convertor/convertor.py`

 * *Files identical despite different names*

### Comparing `p-template-generator-0.1.99/template_generator/convertor/of_to_skymedia.py` & `p_template_generator-0.2.0/template_generator/convertor/of_to_skymedia.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import cv2
 import os
 import json
 import uuid
 import random
+from template_generator import ffmpeg
 
 def json_get(json_data, key, val = None):
     if key in json_data:
         return json_data[key]
     else:
         return val
 
@@ -770,21 +770,18 @@
 def getVolume(volume):
     return 1 if volume is None else max(0, min(1, volume))
 
 def generateUUID():
     return ''.join(str(uuid.uuid4()).split('-'))
 
 def getMediaInfo(mp4):
-    try:
-        cap = cv2.VideoCapture(mp4)
-        mp4_width = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
-        mp4_height = int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
-        frame_rate = int(cap.get(cv2.CAP_PROP_FPS))
+    mp4_width,mp4_height,bitrate,frame_rate = ffmpeg.videoInfo(mp4)
+    if mp4_width > 0:
         return frame_rate, mp4_width, mp4_height
-    except:
+    else:
         return 30, 544, 960
 
 class VideoInputBean(object):
     def __init__(self, videoPath=None, videoEffect=None, multiVideoEffect=None, videoMusic=None):
         self.videoPath = videoPath
         self.videoEffect = videoEffect
         self.multiVideoEffect = multiVideoEffect
```

### Comparing `p-template-generator-0.1.99/template_generator/ffmpeg.py` & `p_template_generator-0.2.0/template_generator/ffmpeg.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,11 @@
 import sys
 import os
-import subprocess
-import json
-import random
-from pathlib import Path
-import shutil
-import zipfile
-import stat
-import requests
+import subprocess, re
 import platform
-import logging
 
 from template_generator import binary
 
 def ffmpegBinary(searchPath):        
     binaryFile = ""
     if sys.platform == "win32":
         binaryFile = os.path.join(binary.ffmpegPath(searchPath), "win", "ffmpeg.exe")
@@ -27,35 +19,41 @@
     elif sys.platform == "darwin":
         binaryFile = os.path.join(binary.ffmpegPath(searchPath), "darwin", "ffmpeg")
     
     if len(binaryFile) > 0 and sys.platform != "win32":
         cmd = subprocess.Popen(f"chmod 755 {binaryFile}", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
         while cmd.poll() is None:
             print(cmd.stdout.readline().rstrip().decode('utf-8'))
-    return binaryFile
+            
+    if os.path.exists(binaryFile):
+        return os.path.dirname(binaryFile), os.path.basename(binaryFile)
+    else:
+        return "", ""
 
 def realCommand(cmd):
-    if sys.platform != "win32":
+    if sys.platform == "linux":
+        return "./" + " ".join(cmd)
+    if sys.platform == "darwin":
         return "./" + " ".join(cmd)
     else:
         return cmd
     
 def videoInfo(file,searchPath):
     w = 0
     h = 0
     bitrate = 0
     fps = 0
     duration = 0
 
-    ffmpeg = ffmpegBinary(searchPath)
-    command = [ffmpeg,"-i",file]
+    binary_dir, binary_file = ffmpegBinary(searchPath)
+    command = [binary_file,"-i",file]
     command = realCommand(command)
     try:
         result = subprocess.run(command, stdout=subprocess.PIPE,
-                                stderr=subprocess.PIPE, shell=True)
+                                stderr=subprocess.PIPE, shell=True, cwd=binary_dir)
         str = ""
         if result.returncode == 0:
             str = result.stdout.decode(encoding="utf8", errors="ignore")
         else:
             str = result.stderr.decode(encoding="utf8", errors="ignore")
         if str.find("yuv420p") > 0 and str.find("fps") > 0:
             s1 = str[str.find("yuv420p"):str.find("fps")+3].replace(' ', "")
@@ -85,21 +83,63 @@
                 duration = hour*3600 + min*60 + second
     except subprocess.CalledProcessError as e:
         print("====================== process error ======================")
         print(e)
         print("======================      end      ======================")
     return float(w),float(h),float(bitrate),float(fps),float(duration)
 
+def audioInfo(file,searchPath=""):
+    sample = 0
+    duration = 0
+    bitrate = 0
+
+    binary_dir, binary_file = ffmpegBinary(searchPath)
+    command = [binary_file,"-i",file]
+    command = realCommand(command)
+    try:
+        result = subprocess.run(command, stdout=subprocess.PIPE,
+                                stderr=subprocess.PIPE, shell=True, cwd=binary_dir)
+        str = ""
+        if result.returncode == 0:
+            str = result.stdout.decode(encoding="utf8", errors="ignore")
+        else:
+            str = result.stderr.decode(encoding="utf8", errors="ignore")
+            
+        duration_match = re.search(r"Duration: (\d{2}:\d{2}:\d{2}\.\d{2})", str)
+        if duration_match:
+            s2 = duration_match.group(1)
+            s2_split = s2.split(":")
+            if len(s2_split) > 2:
+                hour = float(s2_split[0])
+                min = float(s2_split[1])
+                second  = float(s2_split[2])
+                duration = hour*3600 + min*60 + second
+
+        # Extract sample rate
+        sample_rate_match = re.search(r"(\d+) Hz", str)
+        if sample_rate_match:
+            sample = int(sample_rate_match.group(1))
+
+        # Extract bitrate
+        bitrate_match = re.search(r"bitrate: (\d+) kb/s", str)
+        if bitrate_match:
+            bitrate = int(bitrate_match.group(1))
+    except subprocess.CalledProcessError as e:
+        print("====================== process error ======================")
+        print(e)
+        print("======================      end      ======================")
+    return float(sample),float(bitrate),float(duration)
+
 def process(args, searchPath):
-    binary = ffmpegBinary(searchPath)
-    command = [binary] + args
+    binary_dir, binary_file = ffmpegBinary(searchPath)
+    command = [binary_file] + args
     command = realCommand(command)
     try:
         result = subprocess.run(command, stdout=subprocess.PIPE,
-                                stderr=subprocess.PIPE, shell=True)
+                                stderr=subprocess.PIPE, shell=True, cwd=binary_dir)
         if result.returncode == 0:
             print(result.stdout.decode(encoding="utf8", errors="ignore"))
             return True
         # else:
         #     print("====================== ffmpeg error ======================")
         #     print(result.stderr.decode(encoding="utf8", errors="ignore"))
         #     print("======================     end      ======================")
```

### Comparing `p-template-generator-0.1.99/template_generator/main.py` & `p_template_generator-0.2.0/template_generator/main.py`

 * *Files identical despite different names*

### Comparing `p-template-generator-0.1.99/template_generator/server_generator.py` & `p_template_generator-0.2.0/template_generator/server_generator.py`

 * *Files identical despite different names*

### Comparing `p-template-generator-0.1.99/template_generator/template.py` & `p_template_generator-0.2.0/template_generator/template.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from template_generator import binary
 from template_generator import aigc_input
 from template_generator.convertor import convertor
 from template_res import template as template_res_search
 
 def getCommandResult(cmd):
     try:
-        result = subprocess.run(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
+        result = subprocess.run(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, timeout=300)
         if result.returncode == 0:
             return result.stdout.decode(encoding="utf8", errors="ignore").replace("\n","").strip()
         else:
             return ""
     except subprocess.CalledProcessError as e:
         logging.info(f"getCommandResult fail {e}")
         return ""
@@ -47,15 +47,20 @@
             #no x11 or wayland , check Xvfb
             displayShell = os.path.join(binary.skymediaPath(searchPath), "linux", "display.sh")
             if os.path.exists(displayShell):
                 print(f"=== sh {displayShell}")
                 cmd1 = subprocess.Popen(f"sh {displayShell}", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
                 while cmd1.poll() is None:
                     print(cmd1.stdout.readline().rstrip().decode('utf-8'))
-
+    elif sys.platform == "darwin":
+        binaryPath = os.path.join(os.path.join(binary.skymediaPath(searchPath), "darwin"), "TemplateProcess")
+        if os.path.exists(binaryPath):
+            cmd = subprocess.Popen(f"chmod 755 {binaryPath}", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
+            while cmd.poll() is None:
+                print(cmd.stdout.readline().rstrip().decode('utf-8'))
             
     if os.path.exists(binaryPath):
         return os.path.dirname(binaryPath), os.path.basename(binaryPath)
     else:
         return "", ""
     
 # def transcode(f):
@@ -212,27 +217,30 @@
             return False
         else:
             return True
     else:
         return True
     
 def realCommand(cmd):
-    if sys.platform != "win32":
+    if sys.platform == "linux":
+        return "./" + " ".join(cmd)
+    if sys.platform == "darwin":
         return "./" + " ".join(cmd)
     else:
         return cmd
     
 def executeTemplate(data, searchPath="", useAdaptiveSize=False, useAdaptiveDuration=False, useHardware=False, printLog=True):
     binary_dir, binary_file = getBinary(searchPath, useHardware)
     if len(binary_dir) <= 0:
         raise Exception("binary not found")
 
     tmp_file_cache = []
     tmp_dir_cache = []
     output_path = ""
+    output_cnt = 1
     if isinstance(data, (dict)):
         output_path = data["output"]
         # resetInput(data, tmp_file_cache)
         resetTemplate(data, searchPath)
         useAdaptiveSize = useAdaptiveSize or isAdaptiveSize(data)
         useAdaptiveDuration = useAdaptiveDuration or isAdaptiveDuration(data)
         aigc_input.preProcessAIGC(data,tmp_file_cache,tmp_dir_cache)
@@ -240,14 +248,15 @@
         for it in data:
             output_path = it["output"]
             # resetInput(it, tmp_file_cache)
             resetTemplate(it, searchPath)
             useAdaptiveSize = useAdaptiveSize or isAdaptiveSize(it)
             useAdaptiveDuration = useAdaptiveDuration or isAdaptiveDuration(it)
             aigc_input.preProcessAIGC(it,tmp_file_cache,tmp_dir_cache)
+            output_cnt+=1
 
     tempDir = os.path.dirname(os.path.abspath(__file__))
     if os.path.exists(tempDir) == False:
         os.makedirs(tempDir)
     inputArgs = os.path.join(tempDir, f"{random.randint(100,99999999)}.in")
     tmp_file_cache.append(inputArgs)
     if os.path.exists(inputArgs):
@@ -276,15 +285,15 @@
     if sys.platform == "linux" and maybeSoftWare(useHardware):
         extArgs += ["--call_software"]
 
     command = [binary_file, "--config", inputArgs] + extArgs
     command = realCommand(command)
     if printLog:
         print(f"=== executeTemplate => {command}")
-    result = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, cwd=binary_dir)
+    result = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, cwd=binary_dir, timeout=120*output_cnt)
     if result.returncode == 0:
         for t in tmp_file_cache:
             os.remove(t)
         for t in tmp_dir_cache:
             shutil.rmtree(t)
         if printLog:
             print(result.stdout.decode(encoding="utf8", errors="ignore"))
@@ -314,15 +323,15 @@
     if os.path.exists(output) == False:
         os.makedirs(output)
 
     command = [binary_file, "--project", config ,"-y", output]
     command = realCommand(command)
     if printLog:
         print(f"=== generateTemplate => {command}")
-    result = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, cwd=binary_dir)
+    result = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, cwd=binary_dir, timeout=120)
     if result.returncode != 0:
         err_msg = result.stdout.decode(encoding="utf8", errors="ignore")
         logging.info(f"generateTemplate err {err_msg}")
         if printLog:
             print(err_msg)
         raise Exception(f"generate template exception!")
```

### Comparing `p-template-generator-0.1.99/template_generator/template_service.py` & `p_template_generator-0.2.0/template_generator/template_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,16 @@
             cpu_count = psutil.cpu_count(logical=False)
             cpu_percentages = psutil.cpu_percent(percpu=True)
             average_cpu_percentage = sum(cpu_percentages) / cpu_count
             self.queue.append(average_cpu_percentage)
             time.sleep(1)
             if random.randint(0, 10) == 3:
                 print(self.getCurrentPerformance())
-a = aaaaaaaaaaaa()
-a.join()
+# a = aaaaaaaaaaaa()
+# a.join()
     
     
 
 # class KeepTemplateProcessThread(Thread):
 #     pipin = None
 #     pipout = None
 #     process = None
```

### Comparing `p-template-generator-0.1.99/template_generator/template_test.py` & `p_template_generator-0.2.0/template_generator/template_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -150,26 +150,28 @@
             print(f"your device performance is very low")
     else:
         print(f"test fail")
     for s in tmp_file:
         os.remove(s)
     shutil.rmtree(tp_dir)
 
-def testAigc(cnt):
-    for i in range(0,cnt):
-        try:
-            inputs = []
-            output_width = 100
-            output_height = 100
-            fn_name = "aicamera"
-            params = {"batch_count":1,"batch_size":1,"cfg_scale":7,"creative_strength":1,"denoising_strength":1,"era":"spaceSuit","face_index":1,"fn_name":"aicamera","func":"d849eff2cfb2d09a0bb7ae573e69b1cc.png","height":1536,"musicUrl":"","negative_prompt":"","package_url":"https://m-beta-yesdesktop.2tianxin.com/upload/beta/undefined/6079/2763/607947D9CFD52763.zip","prompt":"","restore_faces":True,"sampler_index":"DPM++ SDE Karras","scratch":1,"seed":-1,"steps":25,"text_mark_url":"","type":"image","user_file_name":"d59e9302-f17f-4468-aa23-5b3fd3d44685.png","user_url":"","width":1152}
-            server_generator.MecordAIGC().testTask(378 , inputs, fn_name, params, output_width, output_height)
-            print("pushed one!")
-        except:
-            print("")
+if __name__ == '__main__':
+    test("")
+# def testAigc(cnt):
+#     for i in range(0,cnt):
+#         try:
+#             inputs = []
+#             output_width = 100
+#             output_height = 100
+#             fn_name = "aicamera"
+#             params = {"batch_count":1,"batch_size":1,"cfg_scale":7,"creative_strength":1,"denoising_strength":1,"era":"spaceSuit","face_index":1,"fn_name":"aicamera","func":"d849eff2cfb2d09a0bb7ae573e69b1cc.png","height":1536,"musicUrl":"","negative_prompt":"","package_url":"https://m-beta-yesdesktop.2tianxin.com/upload/beta/undefined/6079/2763/607947D9CFD52763.zip","prompt":"","restore_faces":True,"sampler_index":"DPM++ SDE Karras","scratch":1,"seed":-1,"steps":25,"text_mark_url":"","type":"image","user_file_name":"d59e9302-f17f-4468-aa23-5b3fd3d44685.png","user_url":"","width":1152}
+#             server_generator.MecordAIGC().testTask(378 , inputs, fn_name, params, output_width, output_height)
+#             print("pushed one!")
+#         except:
+#             print("")
 
 # server_generator.MecordAIGC().testTask(386 , [], "test fnname", {}, 100, 100)
             
 # testAigc(1)
 # def testToon():
 #     try:
 #         inputs = []
@@ -237,8 +239,31 @@
 #                              "C:\\Users\\123\\Downloads\\3333\\mohu.jpg")
 # print(f"================== SSIM分数为：{ssim_score:.2f}")
 # ssim_score = calculate_ssim("C:\\Users\\123\\Downloads\\3333\\heidao-shu_video-cover.jpg",
 #                              "E:\\template\\111111111111111111111111111111111111111111package\\test\\out.png")
 # print(f"================== SSIM分数为：{ssim_score:.2f}")
 # ssim_score = calculate_ssim("C:\\Users\\123\\Downloads\\3333\\heidao-shu_video-cover.jpg",
 #                              "E:\\template\\111111111111111111111111111111111111111111package\\test\\out_stb.png")
-# print(f"================== SSIM分数为：{ssim_score:.2f}")
+# print(f"================== SSIM分数为：{ssim_score:.2f}")
+
+
+# from facebook_scraper import get_posts
+# #credentials=("dajidali.dev@gmail.com","dajidalidajidali"), 
+# for post in get_posts('nintendo',start_url="https://mbasic.facebook.com/nintendo?v=timeline", pages=10, cookies='/Users/pengjun/Desktop/template_python/template_generator/template_generator/cookie.txt'):
+#     print(post)
+#     exit(-1)
+
+# #import Facebook_scraper class from facebook_page_scraper
+# from facebook_page_scraper import Facebook_scraper
+
+# #instantiate the Facebook_scraper class
+
+# page_or_group_name = "Meta"
+# posts_count = 10
+# browser = "chrome"
+# proxy = "IP:PORT" #if proxy requires authentication then user:password@IP:PORT
+# timeout = 600
+# headless = True
+# fb_password = "dajidalidajidali"
+# fb_email = "dajidali.dev@gmail.com"
+# isGroup= False
+# meta_ai = Facebook_scraper(page_or_group_name, posts_count, browser, proxy=proxy, timeout=timeout, headless=headless, isGroup=isGroup)
```

### Comparing `p-template-generator-0.1.99/template_generator/test/tp_2023112102.zip.py` & `p_template_generator-0.2.0/template_generator/test/tp_2023112102.zip.py`

 * *Files identical despite different names*

