# Comparing `tmp/arcdlnexus-0.1.2.tar.gz` & `tmp/arcdlnexus-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcdlnexus-0.1.2.tar", last modified: Wed May 29 10:33:51 2024, max compression
+gzip compressed data, was "arcdlnexus-0.1.3.tar", last modified: Wed May 29 11:22:39 2024, max compression
```

## Comparing `arcdlnexus-0.1.2.tar` & `arcdlnexus-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 10:33:51.306396 arcdlnexus-0.1.2/
-drwxrwxrwx   0        0        0        0 2024-05-29 10:33:51.288444 arcdlnexus-0.1.2/ArcDLNexus/
--rw-rw-rw-   0        0        0       46 2024-05-29 10:33:49.000000 arcdlnexus-0.1.2/ArcDLNexus/__init__.py
--rw-rw-rw-   0        0        0     6814 2024-05-29 10:04:20.000000 arcdlnexus-0.1.2/ArcDLNexus/main.py
-drwxrwxrwx   0        0        0        0 2024-05-29 10:33:51.304402 arcdlnexus-0.1.2/ArcDLNexus.egg-info/
--rw-rw-rw-   0        0        0     6134 2024-05-29 10:33:51.000000 arcdlnexus-0.1.2/ArcDLNexus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-05-29 10:33:51.000000 arcdlnexus-0.1.2/ArcDLNexus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 10:33:51.000000 arcdlnexus-0.1.2/ArcDLNexus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-29 10:33:51.000000 arcdlnexus-0.1.2/ArcDLNexus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-29 10:33:51.000000 arcdlnexus-0.1.2/ArcDLNexus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1324 2024-05-28 13:09:40.000000 arcdlnexus-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     6134 2024-05-29 10:33:51.305399 arcdlnexus-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4892 2024-05-29 10:33:49.000000 arcdlnexus-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-29 10:33:51.306396 arcdlnexus-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2186 2024-05-29 10:16:04.000000 arcdlnexus-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:22:39.445900 arcdlnexus-0.1.3/
+drwxrwxrwx   0        0        0        0 2024-05-29 11:22:39.416977 arcdlnexus-0.1.3/ArcDLNexus/
+-rw-rw-rw-   0        0        0       46 2024-05-29 11:22:35.000000 arcdlnexus-0.1.3/ArcDLNexus/__init__.py
+-rw-rw-rw-   0        0        0     8290 2024-05-29 11:19:20.000000 arcdlnexus-0.1.3/ArcDLNexus/main.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:22:39.443923 arcdlnexus-0.1.3/ArcDLNexus.egg-info/
+-rw-rw-rw-   0        0        0     6134 2024-05-29 11:22:39.000000 arcdlnexus-0.1.3/ArcDLNexus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2024-05-29 11:22:39.000000 arcdlnexus-0.1.3/ArcDLNexus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 11:22:39.000000 arcdlnexus-0.1.3/ArcDLNexus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-29 11:22:39.000000 arcdlnexus-0.1.3/ArcDLNexus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-29 11:22:39.000000 arcdlnexus-0.1.3/ArcDLNexus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1324 2024-05-28 13:09:40.000000 arcdlnexus-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     6134 2024-05-29 11:22:39.444903 arcdlnexus-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4892 2024-05-29 10:33:49.000000 arcdlnexus-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-29 11:22:39.445900 arcdlnexus-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     2186 2024-05-29 10:16:04.000000 arcdlnexus-0.1.3/setup.py
```

### Comparing `arcdlnexus-0.1.2/ArcDLNexus/main.py` & `arcdlnexus-0.1.3/ArcDLNexus/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,30 +22,47 @@
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE."""
 import os.path
 import random
 import re
 import time
-
 import requests
 
+headers = {
+    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36",
+    "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8",
+    "Accept-Language": "en-US,en;q=0.5",
+    "Accept-Encoding": "gzip, deflate, br",
+    "Connection": "keep-alive",
+    "Upgrade-Insecure-Requests": "1",
+    "Cache-Control": "max-age=0"
+}
+
 
 def download(url, path="./archive_download", mode=0):
-    r = requests.get(url)
+    html_path = path
+    if not path[-1] == "/":
+        path += "/"
+    html_path += "index.html"
+    tmp_path = ""
+    for tmp in html_path.split("/"):
+        tmp_path += tmp + "/"
+        if not os.path.exists(tmp_path) and not "." in tmp:
+            os.mkdir(tmp_path)
+    session = requests.session()
+    while True:
+        try:
+            r = session.get(url, headers=headers)
+            break
+        except Exception:
+            print("レート制限のため数秒後再試行します")
+            time.sleep(random.uniform(5, 15))
+
     if r.ok:
-        html_path = path
-        if not path[-1] == "/":
-            path += "/"
-        html_path += "index.html"
-        tmp_path = ""
-        for tmp in html_path.split("/"):
-            tmp_path += tmp + "/"
-            if not os.path.exists(tmp_path) and not "." in tmp:
-                os.mkdir(tmp_path)
         # HTMLをファイルに保存
         with open(html_path, "w", encoding="utf-8") as f:
             f.write(r.text)
     else:
         print(r.status_code)
         raise
 
@@ -59,23 +76,24 @@
     soup = BeautifulSoup(html_content, 'html.parser')
 
     f_pth = path + "index_files/"
     datas = {}
 
     def download_file(url):
         print(url)
-        for tmp in range(5):
+        while True:
             try:
-                if url.startswith("//web.archive.org/web/"):
-                    r = requests.get(f"https:{url}")
+                if url.startswith("//"):
+                    r = session.get(f"https:{url}", headers=headers)
                 else:
-                    r = requests.get(url)
+                    r = session.get(url, headers=headers)
                 print("OK")
                 break
-            except Exception:
+            except Exception as e:
+                print(e)
                 print("レート制限のため数秒後再試行します")
                 time.sleep(random.uniform(1, 15))
         if r.ok:
             try:
                 if not os.path.exists(f_pth):
                     os.mkdir(f_pth)
                 ch_tmp = url.split('/')[-1].split('?')[0]
@@ -89,16 +107,17 @@
                     r.encoding = 'utf-8'
                     with open(f"{f_pth}{url_tmp}", "w", encoding="utf-8") as f:
                         f.write(r.text)
                 else:
                     with open(f"{f_pth}{url_tmp}", "wb") as f:
                         f.write(r.content)
                 datas[url] = f"index_files/{url_tmp}"
-            except Exception:
-                pass
+                print("File Save")
+            except Exception as e:
+                print(e)
 
     if not mode == 0:
         # 全ての<script>タグと<link>タグを取得
         script_tags = soup.find_all('script')
         link_tags = soup.find_all('link')
 
         # URLを抽出するための正規表現パターン
@@ -115,14 +134,33 @@
         # 各<link>タグのhref属性の値を抽出
         for link in link_tags:
             href = link.get('href')
             if href:
                 urls = re.findall(url_pattern, href)
                 for url in urls:
                     download_file(url)
+        # すべてのdivタグを取得
+        div_tags = soup.find_all('div', class_=True)
+
+        # URLを格納するリスト
+        urls = []
+
+        # divタグごとにループ
+        for div_tag in div_tags:
+            # data-bg属性を取得
+            data_bg = div_tag.get('data-bg')
+
+            # data-bg属性が存在し、その値がURLを含むか確認
+            if data_bg and re.match(r"url\('.*?'\)", data_bg):
+                # URLを正規表現で抽出
+                match = re.search(r"url\('(.*?)'\)", data_bg)
+                if match and not url in urls:
+                    url = match.group(1)
+                    urls.append(url)
+                    download_file(url)
 
     # 特定の<div>要素を削除
     div_to_remove = soup.find("div", id="wm-ipp-inside")
     if div_to_remove:
         div_to_remove.decompose()
 
     # 特定の<div>要素を削除
```

### Comparing `arcdlnexus-0.1.2/ArcDLNexus.egg-info/PKG-INFO` & `arcdlnexus-0.1.3/ArcDLNexus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArcDLNexus
-Version: 0.1.2
+Version: 0.1.3
 Summary: ArcDLNexus: PythonからWayback Machineのアーカイブ（サイト）をダウンロードするモジュールです。
 Home-page: https://github.com/harumaki4649/ArcDLNexus
 Download-URL: https://github.com/harumaki4649/ArcDLNexus
 Author: ArcDLNexus
 Author-email: support@disnana.com
 Maintainer: ArcDLNexus
 Maintainer-email: support@disnana.com
```

### Comparing `arcdlnexus-0.1.2/LICENSE` & `arcdlnexus-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arcdlnexus-0.1.2/PKG-INFO` & `arcdlnexus-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArcDLNexus
-Version: 0.1.2
+Version: 0.1.3
 Summary: ArcDLNexus: PythonからWayback Machineのアーカイブ（サイト）をダウンロードするモジュールです。
 Home-page: https://github.com/harumaki4649/ArcDLNexus
 Download-URL: https://github.com/harumaki4649/ArcDLNexus
 Author: ArcDLNexus
 Author-email: support@disnana.com
 Maintainer: ArcDLNexus
 Maintainer-email: support@disnana.com
```

### Comparing `arcdlnexus-0.1.2/README.md` & `arcdlnexus-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `arcdlnexus-0.1.2/setup.py` & `arcdlnexus-0.1.3/setup.py`

 * *Files identical despite different names*

