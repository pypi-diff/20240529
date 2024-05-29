# Comparing `tmp/askvideos-0.1.2.tar.gz` & `tmp/askvideos-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "askvideos-0.1.2.tar", last modified: Wed May 29 01:19:13 2024, max compression
+gzip compressed data, was "askvideos-0.1.3.tar", last modified: Wed May 29 01:22:26 2024, max compression
```

## Comparing `askvideos-0.1.2.tar` & `askvideos-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 bhavashok  (1000) bhavashok  (1000)        0 2024-05-29 01:19:12.997670 askvideos-0.1.2/
--rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)     1050 2024-05-29 01:19:12.997670 askvideos-0.1.2/PKG-INFO
--rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)      790 2024-05-29 00:55:03.000000 askvideos-0.1.2/README.md
-drwxrwxr-x   0 bhavashok  (1000) bhavashok  (1000)        0 2024-05-29 01:19:12.997670 askvideos-0.1.2/askvideos/
--rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)        0 2024-05-29 01:18:17.000000 askvideos-0.1.2/askvideos/__init__.py
--rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)    11411 2024-05-29 00:43:29.000000 askvideos-0.1.2/askvideos/client.py
-drwxrwxr-x   0 bhavashok  (1000) bhavashok  (1000)        0 2024-05-29 01:19:12.997670 askvideos-0.1.2/askvideos.egg-info/
--rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)     1050 2024-05-29 01:19:12.000000 askvideos-0.1.2/askvideos.egg-info/PKG-INFO
--rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)      224 2024-05-29 01:19:12.000000 askvideos-0.1.2/askvideos.egg-info/SOURCES.txt
--rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)        1 2024-05-29 01:19:12.000000 askvideos-0.1.2/askvideos.egg-info/dependency_links.txt
--rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)        9 2024-05-29 01:19:12.000000 askvideos-0.1.2/askvideos.egg-info/requires.txt
--rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)       10 2024-05-29 01:19:12.000000 askvideos-0.1.2/askvideos.egg-info/top_level.txt
--rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)       38 2024-05-29 01:19:12.997670 askvideos-0.1.2/setup.cfg
--rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)     1298 2024-05-29 01:18:36.000000 askvideos-0.1.2/setup.py
+drwxrwxr-x   0 bhavashok  (1000) bhavashok  (1000)        0 2024-05-29 01:22:26.587466 askvideos-0.1.3/
+-rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)     1050 2024-05-29 01:22:26.587466 askvideos-0.1.3/PKG-INFO
+-rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)      790 2024-05-29 00:55:03.000000 askvideos-0.1.3/README.md
+drwxrwxr-x   0 bhavashok  (1000) bhavashok  (1000)        0 2024-05-29 01:22:26.583466 askvideos-0.1.3/askvideos/
+-rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)       22 2024-05-29 01:21:17.000000 askvideos-0.1.3/askvideos/__init__.py
+-rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)    10573 2024-05-29 01:21:45.000000 askvideos-0.1.3/askvideos/client.py
+drwxrwxr-x   0 bhavashok  (1000) bhavashok  (1000)        0 2024-05-29 01:22:26.587466 askvideos-0.1.3/askvideos.egg-info/
+-rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)     1050 2024-05-29 01:22:26.000000 askvideos-0.1.3/askvideos.egg-info/PKG-INFO
+-rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)      224 2024-05-29 01:22:26.000000 askvideos-0.1.3/askvideos.egg-info/SOURCES.txt
+-rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)        1 2024-05-29 01:22:26.000000 askvideos-0.1.3/askvideos.egg-info/dependency_links.txt
+-rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)        9 2024-05-29 01:22:26.000000 askvideos-0.1.3/askvideos.egg-info/requires.txt
+-rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)       10 2024-05-29 01:22:26.000000 askvideos-0.1.3/askvideos.egg-info/top_level.txt
+-rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)       38 2024-05-29 01:22:26.587466 askvideos-0.1.3/setup.cfg
+-rw-rw-r--   0 bhavashok  (1000) bhavashok  (1000)     1298 2024-05-29 01:22:20.000000 askvideos-0.1.3/setup.py
```

### Comparing `askvideos-0.1.2/PKG-INFO` & `askvideos-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: askvideos
-Version: 0.1.2
+Version: 0.1.3
 Summary: AskVideos python library
 Home-page: https://github.com/AskYoutubeAI/askvideos-py
 Author: AskVideos
 Author-email: askutubeai@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `askvideos-0.1.2/README.md` & `askvideos-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `askvideos-0.1.2/askvideos/client.py` & `askvideos-0.1.3/askvideos/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -254,38 +254,7 @@
         Returns:
         dict: JSON that lists all videos in index.
         """
         url = f"{self.api_url}/index/{index_name}/videos"
         response = requests.get(url, headers=self.headers)
         response.raise_for_status()
         return response.json()
-
-if __name__ == '__main__':
-    api_url = "http://127.0.0.1:8123"#"http://73.202.138.16:8888"
-    api_key = "example_api_key"
-
-    client = AskVideosClient(api_url, api_key)
-
-    # Create an index
-    #index_name = "coffee"
-    index_name = "cinematic"
-    #client.create_index(index_name)
-
-    vid = client.index_video(
-            index_name,
-            video_url='https://videos.pexels.com/video-files/6060027/6060027-hd_1080_1920_25fps.mp4')
-    print(vid)
-    exit()
-
-    # Index videos from a YouTube search
-    search_term = "coffee brewing"
-    client.index_from_youtube_search(index_name, search_term)
-
-    # Search for videos
-    query = "how do I make cold brew"
-    results = client.search_videos(index_name, query)
-    print(results)
-
-    # List indexed videos
-    videos = client.list_videos(index_name)
-    print(videos)
-
```

### Comparing `askvideos-0.1.2/askvideos.egg-info/PKG-INFO` & `askvideos-0.1.3/askvideos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: askvideos
-Version: 0.1.2
+Version: 0.1.3
 Summary: AskVideos python library
 Home-page: https://github.com/AskYoutubeAI/askvideos-py
 Author: AskVideos
 Author-email: askutubeai@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `askvideos-0.1.2/setup.py` & `askvideos-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='askvideos',  # Replace 'your_package_name' with the name of your package
-    version='0.1.2',  # Version number for your package
+    version='0.1.3',  # Version number for your package
     author='AskVideos',  # Your name or your organization's name
     author_email='askutubeai@gmail.com',  # Your email or your organization's contact email
     description='AskVideos python library',  # A brief description of your package
     long_description=open('README.md').read(),  # A long description from your README.md
     long_description_content_type='text/markdown',  # Specifies that the long description is in Markdown
     url='https://github.com/AskYoutubeAI/askvideos-py',  # URL to your package's repository
     #packages=find_packages(exclude=('tests', 'docs')),  # Automatically find all packages in your project
```

