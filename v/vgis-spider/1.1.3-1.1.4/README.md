# Comparing `tmp/vgis_spider-1.1.3.tar.gz` & `tmp/vgis_spider-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vgis_spider-1.1.3.tar", last modified: Wed Mar 20 04:03:59 2024, max compression
+gzip compressed data, was "dist\vgis_spider-1.1.4.tar", last modified: Wed May 29 03:26:43 2024, max compression
```

## Comparing `vgis_spider-1.1.3.tar` & `vgis_spider-1.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-20 04:03:59.324542 vgis_spider-1.1.3/
--rw-rw-rw-   0        0        0      992 2024-03-20 04:03:59.323541 vgis_spider-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      120 2023-11-02 06:05:38.000000 vgis_spider-1.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-03-20 04:03:59.324542 vgis_spider-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     2272 2024-03-20 04:03:55.000000 vgis_spider-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-20 04:03:59.312542 vgis_spider-1.1.3/vgis_spider/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_spider-1.1.3/vgis_spider/__init__.py
--rw-rw-rw-   0        0        0    37734 2024-03-20 04:03:13.000000 vgis_spider-1.1.3/vgis_spider/downloadTilesTools.py
--rw-rw-rw-   0        0        0    50776 2023-11-02 06:21:03.000000 vgis_spider-1.1.3/vgis_spider/htmlParse.py
--rw-rw-rw-   0        0        0      354 2021-01-08 02:20:43.000000 vgis_spider-1.1.3/vgis_spider/specialValue.py
--rw-rw-rw-   0        0        0     1721 2021-03-09 09:25:33.000000 vgis_spider-1.1.3/vgis_spider/spiderTest.py
--rw-rw-rw-   0        0        0    18982 2023-11-02 06:25:42.000000 vgis_spider-1.1.3/vgis_spider/weiboCrawler.py
--rw-rw-rw-   0        0        0      672 2021-01-26 04:16:49.000000 vgis_spider-1.1.3/vgis_spider/weiboSettings.py
--rw-rw-rw-   0        0        0    11904 2023-11-02 06:26:34.000000 vgis_spider-1.1.3/vgis_spider/weixinCrawler.py
-drwxrwxrwx   0        0        0        0 2024-03-20 04:03:59.322541 vgis_spider-1.1.3/vgis_spider.egg-info/
--rw-rw-rw-   0        0        0      992 2024-03-20 04:03:59.000000 vgis_spider-1.1.3/vgis_spider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      415 2024-03-20 04:03:59.000000 vgis_spider-1.1.3/vgis_spider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-20 04:03:59.000000 vgis_spider-1.1.3/vgis_spider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2024-03-20 04:03:59.000000 vgis_spider-1.1.3/vgis_spider.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-20 04:03:59.000000 vgis_spider-1.1.3/vgis_spider.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 03:26:43.198835 vgis_spider-1.1.4/
+-rw-rw-rw-   0        0        0      992 2024-05-29 03:26:43.197836 vgis_spider-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2023-11-02 06:05:38.000000 vgis_spider-1.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-29 03:26:43.198835 vgis_spider-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     2272 2024-05-29 03:26:24.000000 vgis_spider-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 03:26:43.167836 vgis_spider-1.1.4/vgis_spider/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_spider-1.1.4/vgis_spider/__init__.py
+-rw-rw-rw-   0        0        0    38169 2024-05-29 03:25:44.000000 vgis_spider-1.1.4/vgis_spider/downloadTilesTools.py
+-rw-rw-rw-   0        0        0    50776 2023-11-02 06:21:03.000000 vgis_spider-1.1.4/vgis_spider/htmlParse.py
+-rw-rw-rw-   0        0        0      354 2021-01-08 02:20:43.000000 vgis_spider-1.1.4/vgis_spider/specialValue.py
+-rw-rw-rw-   0        0        0     1721 2021-03-09 09:25:33.000000 vgis_spider-1.1.4/vgis_spider/spiderTest.py
+-rw-rw-rw-   0        0        0    18982 2023-11-02 06:25:42.000000 vgis_spider-1.1.4/vgis_spider/weiboCrawler.py
+-rw-rw-rw-   0        0        0      672 2021-01-26 04:16:49.000000 vgis_spider-1.1.4/vgis_spider/weiboSettings.py
+-rw-rw-rw-   0        0        0    11904 2023-11-02 06:26:34.000000 vgis_spider-1.1.4/vgis_spider/weixinCrawler.py
+drwxrwxrwx   0        0        0        0 2024-05-29 03:26:43.195837 vgis_spider-1.1.4/vgis_spider.egg-info/
+-rw-rw-rw-   0        0        0      992 2024-05-29 03:26:43.000000 vgis_spider-1.1.4/vgis_spider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2024-05-29 03:26:43.000000 vgis_spider-1.1.4/vgis_spider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 03:26:43.000000 vgis_spider-1.1.4/vgis_spider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2024-05-29 03:26:43.000000 vgis_spider-1.1.4/vgis_spider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-29 03:26:43.000000 vgis_spider-1.1.4/vgis_spider.egg-info/top_level.txt
```

### Comparing `vgis_spider-1.1.3/PKG-INFO` & `vgis_spider-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis_spider
-Version: 1.1.3
+Version: 1.1.4
 Summary: A libary for spider data
 Home-page: https://github.com/gisfanmachel/vgisSpider
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Keywords: spider,setuptools,development
 Platform: UNKNOWN
```

### Comparing `vgis_spider-1.1.3/setup.py` & `vgis_spider-1.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
 
     name="vgis_spider",  # Required 项目名称
-    version="1.1.3",  # Required 发布版本号
+    version="1.1.4",  # Required 发布版本号
     description="A libary for spider data",  # Optional 项目简单描述
     long_description=long_description,  # Optional 详细描述
     long_description_content_type="text/markdown",  # 内容类型
     url="https://github.com/gisfanmachel/vgisSpider",  # Optional github项目地址
     author="gisfanmachel",  # Optional 作者
     author_email="gisfanmachel@gmail.com",  # Optional 作者邮箱
     classifiers=[  # Optional 分类器通过对项目进行分类来帮助用户找到项目, 以下除了python版本其他的 不需要改动
```

### Comparing `vgis_spider-1.1.3/vgis_spider/downloadTilesTools.py` & `vgis_spider-1.1.4/vgis_spider/downloadTilesTools.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 @Date    :2023/11/2 13:52
 @Descr:  地图瓦片下载
 """
 import json
 import multiprocessing
 import os
 import shutil
+import uuid
 from datetime import datetime
 from math import floor, log, tan, cos, pi, atan, exp
 from multiprocessing.dummy import Pool as ThreadPool
 
 import cv2
 import numpy as np
 import requests as req
@@ -45,20 +46,26 @@
         # 要下载瓦片的影像服务类型，如wms,wmts,tms,xyz等
         self.image_service_type = image_service_type
         # 对于非wms服务，需要重新计算分辨率和瓦片像素大小，比如geoserver的wmts
         if image_service_type != "wms" and "geoserver" in image_service_info["service_type"]:
             self.resolution, self.tile_size, self.tile_coords = self.get_details_of_zoomlevel_in_geoserver(
                 self.image_service_info["zoom_level"], self.image_service_info["gridset_name"])
 
+        # 为每个用户线程创建一个临时目录
+        tem_dir_name = str(uuid.uuid4())
+
         # 瓦片存储路径
         self.tile_pic_path = tile_pic_path if tile_pic_path is not None else os.path.join(os.getcwd(), ".cache",
+                                                                                          tem_dir_name,
                                                                                           "allTiles")
         # 每列瓦片拼接的竖条图片存放路径
         self.vcontat_img_path = vcontat_img_path if vcontat_img_path is not None else os.path.join(os.getcwd(),
-                                                                                                   ".cache", "vMTiles")
+                                                                                                   ".cache",
+                                                                                                   tem_dir_name,
+                                                                                                   "vMTiles")
         # 所有瓦片合成大图存放路径
         self.out_image_path = out_image_path
         # 是否使用多线程
         self.is_multi_thread = is_multi_thread
         self.logger = logger
         self.retry_download_curent = 0
         self.retry_download_count = 5
@@ -280,15 +287,15 @@
                 try:
                     # 合成瓦片成大图
                     self.merge_tiles_to_image()
                     # 生成world文件需要的参数
                     # 根据坐标范围反算瓦片的行列号，最后拼成的瓦片大图，比输入的坐标范围要大些，因为需要重新计算左上角点的地图坐标
                     if self.image_service_type != "wms":
                         left_x, top_y = float(left_top_tile_bounds[0]), float(left_top_tile_bounds[3])
-                        if self.image_service_type == "xyz" or self.image_service_type=="quad":
+                        if self.image_service_type == "xyz" or self.image_service_type == "quad":
                             if self.image_service_info["epsg"] == 4326:
                                 self.resolution = 0.703125 * 2 / pow(2,
                                                                      self.image_service_info[
                                                                          "zoom_level"])
                             elif self.image_service_info["epsg"] == 3857:
                                 self.resolution = 78271.51696399994 * 2 / pow(2,
                                                                               self.image_service_info[
```

### Comparing `vgis_spider-1.1.3/vgis_spider/htmlParse.py` & `vgis_spider-1.1.4/vgis_spider/htmlParse.py`

 * *Files identical despite different names*

### Comparing `vgis_spider-1.1.3/vgis_spider/spiderTest.py` & `vgis_spider-1.1.4/vgis_spider/spiderTest.py`

 * *Files identical despite different names*

### Comparing `vgis_spider-1.1.3/vgis_spider/weiboCrawler.py` & `vgis_spider-1.1.4/vgis_spider/weiboCrawler.py`

 * *Files identical despite different names*

### Comparing `vgis_spider-1.1.3/vgis_spider/weiboSettings.py` & `vgis_spider-1.1.4/vgis_spider/weiboSettings.py`

 * *Files identical despite different names*

### Comparing `vgis_spider-1.1.3/vgis_spider/weixinCrawler.py` & `vgis_spider-1.1.4/vgis_spider/weixinCrawler.py`

 * *Files identical despite different names*

### Comparing `vgis_spider-1.1.3/vgis_spider.egg-info/PKG-INFO` & `vgis_spider-1.1.4/vgis_spider.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis-spider
-Version: 1.1.3
+Version: 1.1.4
 Summary: A libary for spider data
 Home-page: https://github.com/gisfanmachel/vgisSpider
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Keywords: spider,setuptools,development
 Platform: UNKNOWN
```

