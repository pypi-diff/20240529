# Comparing `tmp/pyktok-0.0.8.tar.gz` & `tmp/pyktok-0.0.9.tar.gz`

## Comparing `pyktok-0.0.8.tar` & `pyktok-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pyktok-0.0.8/.gitattributes
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pyktok-0.0.8/src/pyktok/__init__.py
--rw-r--r--   0        0        0     9394 2020-02-02 00:00:00.000000 pyktok-0.0.8/src/pyktok/pyktok.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 pyktok-0.0.8/LICENSE
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 pyktok-0.0.8/README.md
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pyktok-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 pyktok-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pyktok-0.0.9/.gitattributes
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pyktok-0.0.9/src/pyktok/__init__.py
+-rw-r--r--   0        0        0    12398 2020-02-02 00:00:00.000000 pyktok-0.0.9/src/pyktok/pyktok.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 pyktok-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 pyktok-0.0.9/README.md
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pyktok-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 pyktok-0.0.9/PKG-INFO
```

### Comparing `pyktok-0.0.8/src/pyktok/pyktok.py` & `pyktok-0.0.9/src/pyktok/pyktok.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,68 +13,79 @@
 import os
 import pandas as pd
 import random
 import re
 import requests
 import time
 
-headers = {
-    'Accept-Encoding': 'gzip, deflate, sdch',
-    'Accept-Language': 'en-US,en;q=0.8',
-    'Upgrade-Insecure-Requests': '1',
-    'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/56.0.2924.87 Safari/537.36',
-    'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8',
-    'Cache-Control': 'max-age=0',
-    'Connection': 'keep-alive',
-}
+headers = {'Accept-Encoding': 'gzip, deflate, sdch',
+           'Accept-Language': 'en-US,en;q=0.8',
+           'Upgrade-Insecure-Requests': '1',
+           'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/56.0.2924.87 Safari/537.36',
+           'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8',
+           'Cache-Control': 'max-age=0',
+           'Connection': 'keep-alive'}
 
 def get_account_video_urls(user_url):
     tt_json = get_tiktok_json(user_url)
     video_ids = tt_json['ItemList']['user-post']['list']
     tt_account = tt_json['UserPage']['uniqueId']
     url_seg_1 = 'https://www.tiktok.com/@'
     url_seg_2 = '/video/'
     video_urls = [url_seg_1 + tt_account + url_seg_2 + u for u in video_ids]
     return video_urls
 
 def get_tiktok_json(video_url):
-    cookies = browser_cookie3.chrome(domain_name='.tiktok.com')
+    cookies = browser_cookie3.load()
     tt = requests.get(video_url,
                       headers=headers,
                       cookies=cookies,
                       timeout=20)
     soup = BeautifulSoup(tt.text, "html.parser")
     tt_script = soup.find('script', attrs={'id':"SIGI_STATE"})
-    tt_json = json.loads(tt_script.string)
+    try:
+        tt_json = json.loads(tt_script.string)
+    except AttributeError:
+        print("The function encountered a downstream error and did not deliver any data, which happens periodically (not sure why). Please try again later.")
+        return
     return tt_json
 
 def save_tiktok(video_url,
                 save_video=True,
                 metadata_fn=''):
     if save_video == False and metadata_fn == '':
         print('Since save_video and metadata_fn are both False/blank, the program did nothing.')
         return
 
     tt_json = get_tiktok_json(video_url)
     regex_url = re.findall('(?<=@)(.+?)(?=\?|$)',video_url)[0]
     video_fn = regex_url.replace('/','_') + '.mp4'
     video_id = list(tt_json['ItemModule'].keys())[0]
     
+    if save_video == True:
+        tt_video_url = tt_json['ItemList']['video']['preloadList'][0]['url']
+        tt_video = requests.get(tt_video_url,allow_redirects=True)
+    
+        with open(video_fn, 'wb') as fn:
+            fn.write(tt_video.content)
+        print("Saved video\n",video_url,"\nto\n",os.getcwd())
+    
     if metadata_fn != '':
         data_header = ['video_id',
                        'video_timestamp',
                        'video_length',
                        'video_title',
                        'video_locationcreated',
                        'video_diggcount',
                        'video_sharecount',
                        'video_commentcount',
                        'video_playcount',
                        'video_description',                       
                        'video_is_ad',
+                       'video_stickers',
                        'video_fn',
                        'author_username',
                        'author_name',
                        'author_followercount',
                        'author_followingcount',
                        'author_heartcount',
                        'author_videocount',
@@ -117,14 +128,22 @@
         except Exception:
             video_description = ''
         try:
             video_is_ad = tt_json['ItemModule'][video_id]['isAd']
         except Exception:
             video_is_ad = ''
         try:
+            video_stickers = []
+            for sticker in tt_json['ItemModule'][video_id]['stickersOnItem']:
+                for text in sticker['stickerText']:
+                    video_stickers.append(text)
+            video_stickers = ';'.join(video_stickers)
+        except Exception:
+            video_stickers = ''
+        try:
             author_username = tt_json['ItemModule'][video_id]['author']
         except Exception:
             author_username = ''
         try:
             author_name = tt_json['ItemModule'][video_id]['authorName']
         except Exception:
             try:
@@ -158,14 +177,15 @@
                      video_locationcreated,
                      video_diggcount,
                      video_sharecount,
                      video_commentcount,
                      video_playcount,
                      video_description,
                      video_is_ad,
+                     video_stickers,
                      video_fn,
                      author_username,
                      author_name,
                      author_followercount,
                      author_followingcount,
                      author_heartcount,
                      author_videocount,
@@ -174,64 +194,106 @@
         if os.path.exists(metadata_fn):
             metadata = pd.read_csv(metadata_fn,keep_default_na=False)
             new_data = pd.concat([metadata,data_line])
         else:
             new_data = data_line
         new_data.to_csv(metadata_fn,index=False)
         print("Saved metadata for video\n",video_url,"\nto\n",os.getcwd())
-        
-    if save_video == True:
-        tt_video_url = tt_json['ItemList']['video']['preloadList'][0]['url']
-        tt_video = requests.get(tt_video_url,allow_redirects=True)
-    
-        with open(video_fn, 'wb') as fn:
-            fn.write(tt_video.content)
-        print("Saved video\n",video_url,"\nto\n",os.getcwd())
 
 def save_tiktok_multi(video_urls,
                       save_video=True,
                       metadata_fn='',
                       sleep=4):
     if type(video_urls) is str:
         tt_urls = open(video_urls).read().splitlines()
     else:
         tt_urls = video_urls
     for u in tt_urls:
         save_tiktok(u,save_video,metadata_fn)
         time.sleep(random.randint(1, sleep))
 
 def save_video_comments(video_url,
-                        comments_file,
+                        comments_file=None,
                         cursor_resume=0,
                         max_comments=np.inf,
                         sleep=4):
     cursor = cursor_resume
     headers["referer"] = video_url
     video_id = re.findall('(?<=/video/)(.+?)(?=\?|$)',video_url)[0]
-    cookies = browser_cookie3.chrome(domain_name='.tiktok.com')
+    if comments_file == None:
+        comments_file = video_id + 'tiktok_comments.csv'
+    cookies = browser_cookie3.load()
     while cursor < max_comments:
         params = {'aweme_id': video_id,
                   'count': '20',
-                  'cursor': str(cursor)
-                 }
+                  'cursor': str(cursor)}
         try:
             response = requests.get('https://www.tiktok.com/api/comment/list/',
                                     headers=headers,
                                     params=params,
-                                    cookies=cookies
-                                    )
+                                    cookies=cookies)
             data = response.json()
             old_cursor = cursor
             cursor = cursor + len(data['comments'])
-            print("Comments",old_cursor,"through",cursor,"downloaded (max "+ str(max_comments) +")")
+            print("Comments",old_cursor,"through",cursor,"downloaded (max " + str(max_comments) + ")")
             if os.path.exists(comments_file):
                 pd.DataFrame(data['comments']).to_csv(comments_file,
                                                       mode='a',
                                                       header=False,
                                                       index=False)
             else:
-                pd.DataFrame(data['comments']).to_csv(comments_file,index=False)
+                pd.DataFrame(data['comments']).to_csv(comments_file,index=False,header=['comment'])
             if data["has_more"] != 1:
                 break
             time.sleep(random.randint(1, sleep))
         except Exception as e:
             print(e)
+
+def save_hashtag_video_urls(hashtag,
+                            urls_file=None,
+                            cursor_resume=0,
+                            max_videos=np.inf,
+                            sleep=4):
+    if urls_file == None:
+        urls_file = '#' + hashtag + '_tiktok.csv'
+    cursor = cursor_resume
+    tagurl = "https://www.tiktok.com/tag/" + hashtag
+    tagjson = get_tiktok_json(tagurl)
+    al_ios = tagjson['SharingMeta']['value']['al:ios:url']
+    tag_id = re.findall('(?<=/detail/)(.+?)(?=\?|$)',al_ios)[0]
+    headers["referer"] = tagurl
+    cookies = browser_cookie3.load()
+    while cursor < max_videos:
+        params = {'challengeID': tag_id,
+                  'count': '20',
+                  'cursor': str(cursor),
+                  'aid': '1988'}
+        try:
+            response = requests.get('https://www.tiktok.com/api/challenge/item_list/',
+                                    headers=headers,
+                                    params=params,
+                                    cookies=cookies)
+            data = response.json()
+            urllist = []
+            for video in data['itemList']:
+                urllist.append('https://tiktok.com/@' + video['author']['uniqueId'] + '/video/' + video['id'])
+            if os.path.exists(urls_file):
+                pd.DataFrame(urllist).to_csv(urls_file,
+                                             mode='a',
+                                             header=False,
+                                             index=False)
+            else:
+               pd.DataFrame(urllist).to_csv(urls_file,index=False,header=['url'])
+            old_cursor = cursor
+            cursor = cursor + len(data['itemList'])
+            print("Video urls", old_cursor, "through", cursor, "downloaded (max " + str(max_videos) + ")")
+            if data["hasMore"] != 1:
+                break
+            time.sleep(random.randint(1, sleep))
+        except Exception as e:
+            print(e)
+    finalurls = pd.read_csv(urls_file)
+    old_count = len(finalurls.index)
+    finalurls.drop_duplicates(subset=None, inplace=True)
+    count = len(finalurls.index)
+    finalurls.to_csv(urls_file, index=False)
+    print("Dropped", str(old_count - count), "duplicate urls. Total number of urls in file:", count)
```

### Comparing `pyktok-0.0.8/LICENSE` & `pyktok-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyktok-0.0.8/README.md` & `pyktok-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 ## Pyktok
-**A simple module to collect video, text, and metadata from Tiktok.**
+**A simple module to collect video, text, and metadata from Tiktok, with no authentication required.**
 
 I developed Pyktok ("pick-tock") because none of the existing TikTok data collection utilities I could find worked for me. Pyktok pulls its data directly from the JSON object embedded in every Tiktok video and user page (except for `save_video_comments`, which uses the TikTok API). Here are its major features, most of which require the URL(s) of the content you wish to collect:
 
  - Download TikTok videos
  - Download video metadata
  - Download ~~up to 20 most recent~~ **all available video comments** (special thanks to **[@pkreissel](https://github.com/pkreissel)** for drafting the code for this!!!)
  - Download up to 30 most recent user video URLs
  - Download full TikTok JSON data objects (in case you want to extract data from parts of the object not included in the above functions)
  
 This program may stop working suddenly if TikTok changes how it stores its data ([see Freelon, 2018](https://osf.io/preprints/socarxiv/56f4q/)).
 
+R users, check out [traktok](https://github.com/JBGruber/traktok), an R port of Pyktok.
+
 **Installation**
 
 ```pip install pyktok```
 
 **Requirements**
 
 Pyktok relies on the following packages:
```

### Comparing `pyktok-0.0.8/pyproject.toml` & `pyktok-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
             "numpy",
             "pandas",
             "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyktok"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Deen Freelon", email="dfreelon@gmail.com"},
 ]
 description = "A package for collecting TikTok videos and metadata."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `pyktok-0.0.8/PKG-INFO` & `pyktok-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyktok
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for collecting TikTok videos and metadata.
 Project-URL: Homepage, https://github.com/dfreelon/pyktok
 Author-email: Deen Freelon <dfreelon@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Deen Freelon
         All rights reserved.
@@ -29,33 +29,36 @@
         DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## Pyktok
-**A simple module to collect video, text, and metadata from Tiktok.**
+**A simple module to collect video, text, and metadata from Tiktok, with no authentication required.**
 
 I developed Pyktok ("pick-tock") because none of the existing TikTok data collection utilities I could find worked for me. Pyktok pulls its data directly from the JSON object embedded in every Tiktok video and user page (except for `save_video_comments`, which uses the TikTok API). Here are its major features, most of which require the URL(s) of the content you wish to collect:
 
  - Download TikTok videos
  - Download video metadata
  - Download ~~up to 20 most recent~~ **all available video comments** (special thanks to **[@pkreissel](https://github.com/pkreissel)** for drafting the code for this!!!)
  - Download up to 30 most recent user video URLs
  - Download full TikTok JSON data objects (in case you want to extract data from parts of the object not included in the above functions)
  
 This program may stop working suddenly if TikTok changes how it stores its data ([see Freelon, 2018](https://osf.io/preprints/socarxiv/56f4q/)).
 
+R users, check out [traktok](https://github.com/JBGruber/traktok), an R port of Pyktok.
+
 **Installation**
 
 ```pip install pyktok```
 
 **Requirements**
 
 Pyktok relies on the following packages:
```

