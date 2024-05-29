# Comparing `tmp/simpleaug-0.0.1.tar.gz` & `tmp/simpleaug-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleaug-0.0.1.tar", last modified: Wed May 29 08:51:53 2024, max compression
+gzip compressed data, was "simpleaug-0.0.2.tar", last modified: Wed May 29 09:00:20 2024, max compression
```

## Comparing `simpleaug-0.0.1.tar` & `simpleaug-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 08:51:53.871720 simpleaug-0.0.1/
--rw-rw-rw-   0        0        0     1086 2024-05-29 07:23:30.000000 simpleaug-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1811 2024-05-29 08:51:53.870722 simpleaug-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1425 2024-05-29 08:50:29.000000 simpleaug-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 08:51:53.860263 simpleaug-0.0.1/SimpleAUG.egg-info/
--rw-rw-rw-   0        0        0     1811 2024-05-29 08:51:53.000000 simpleaug-0.0.1/SimpleAUG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2024-05-29 08:51:53.000000 simpleaug-0.0.1/SimpleAUG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 08:51:53.000000 simpleaug-0.0.1/SimpleAUG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-29 08:51:53.000000 simpleaug-0.0.1/SimpleAUG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2024-05-29 07:55:09.000000 simpleaug-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-29 08:51:53.871720 simpleaug-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1034 2024-05-29 08:49:15.000000 simpleaug-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-29 08:51:53.859262 simpleaug-0.0.1/simpleaug/
--rw-rw-rw-   0        0        0        0 2024-05-29 06:10:34.000000 simpleaug-0.0.1/simpleaug/__init__.py
--rw-rw-rw-   0        0        0     2755 2024-05-29 08:06:20.000000 simpleaug-0.0.1/simpleaug/aug.py
--rw-rw-rw-   0        0        0      220 2024-05-29 06:53:52.000000 simpleaug-0.0.1/simpleaug/temp.py
--rw-rw-rw-   0        0        0     2587 2024-05-29 06:29:04.000000 simpleaug-0.0.1/simpleaug/tool.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:00:20.151780 simpleaug-0.0.2/
+-rw-rw-rw-   0        0        0     1086 2024-05-29 07:23:30.000000 simpleaug-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1841 2024-05-29 09:00:20.150779 simpleaug-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1455 2024-05-29 08:56:40.000000 simpleaug-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 09:00:20.149780 simpleaug-0.0.2/SimpleAUG.egg-info/
+-rw-rw-rw-   0        0        0     1841 2024-05-29 09:00:20.000000 simpleaug-0.0.2/SimpleAUG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2024-05-29 09:00:20.000000 simpleaug-0.0.2/SimpleAUG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 09:00:20.000000 simpleaug-0.0.2/SimpleAUG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-29 09:00:20.000000 simpleaug-0.0.2/SimpleAUG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2024-05-29 07:55:09.000000 simpleaug-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-29 09:00:20.151780 simpleaug-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1034 2024-05-29 09:00:07.000000 simpleaug-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:00:20.148780 simpleaug-0.0.2/simpleaug/
+-rw-rw-rw-   0        0        0        0 2024-05-29 06:10:34.000000 simpleaug-0.0.2/simpleaug/__init__.py
+-rw-rw-rw-   0        0        0     2756 2024-05-29 08:59:48.000000 simpleaug-0.0.2/simpleaug/aug.py
+-rw-rw-rw-   0        0        0      220 2024-05-29 06:53:52.000000 simpleaug-0.0.2/simpleaug/temp.py
+-rw-rw-rw-   0        0        0     2587 2024-05-29 06:29:04.000000 simpleaug-0.0.2/simpleaug/tool.py
```

### Comparing `simpleaug-0.0.1/LICENSE.txt` & `simpleaug-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simpleaug-0.0.1/PKG-INFO` & `simpleaug-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: SimpleAUG
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simpler imgaug tool
 Author: Duyuxuan
 Author-email: g2702922146@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # SimpleAUG 更加简单的数据增强库
 ## 使用示例
 
+pip install SimpleAUG==0.0.1
 数据增强的具体配置可以到[overview_of_augmenters.html](https://imgaug.readthedocs.io/en/latest/source/overview_of_augmenters.html)查阅
 
     from imgaug import augmenters as iaa
     from simpleaug import aug
     
     # 输入VOC数据集的路径
     XML_DIR = "/demo/VOC_MASK/Annotations/"
```

### Comparing `simpleaug-0.0.1/README.md` & `simpleaug-0.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SimpleAUG 更加简单的数据增强库
 ## 使用示例
 
+pip install SimpleAUG==0.0.1
 数据增强的具体配置可以到[overview_of_augmenters.html](https://imgaug.readthedocs.io/en/latest/source/overview_of_augmenters.html)查阅
 
     from imgaug import augmenters as iaa
     from simpleaug import aug
     
     # 输入VOC数据集的路径
     XML_DIR = "/demo/VOC_MASK/Annotations/"
```

### Comparing `simpleaug-0.0.1/SimpleAUG.egg-info/PKG-INFO` & `simpleaug-0.0.2/SimpleAUG.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: SimpleAUG
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simpler imgaug tool
 Author: Duyuxuan
 Author-email: g2702922146@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # SimpleAUG 更加简单的数据增强库
 ## 使用示例
 
+pip install SimpleAUG==0.0.1
 数据增强的具体配置可以到[overview_of_augmenters.html](https://imgaug.readthedocs.io/en/latest/source/overview_of_augmenters.html)查阅
 
     from imgaug import augmenters as iaa
     from simpleaug import aug
     
     # 输入VOC数据集的路径
     XML_DIR = "/demo/VOC_MASK/Annotations/"
```

### Comparing `simpleaug-0.0.1/setup.py` & `simpleaug-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SimpleAUG",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.0.1",  # 包版本号，便于维护版本
+    version="0.0.2",  # 包版本号，便于维护版本
     author="Duyuxuan",  # 作者，可以写自己的姓名
     author_email="g2702922146@gmail.com",  # 作者联系方式，可写自己的邮箱地址
     description="A simpler imgaug tool",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     # url="https://github.com/pypa/sampleproject",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

### Comparing `simpleaug-0.0.1/simpleaug/aug.py` & `simpleaug-0.0.2/simpleaug/aug.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tool import *
+from .tool import *
 import imgaug as ia
 import numpy as np
 import shutil
 from tqdm import tqdm
 from PIL import Image
 from imgaug import augmenters as iaa
```

### Comparing `simpleaug-0.0.1/simpleaug/tool.py` & `simpleaug-0.0.2/simpleaug/tool.py`

 * *Files identical despite different names*

