# Comparing `tmp/easyofd-0.1.1.5.tar.gz` & `tmp/easyofd-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyofd-0.1.1.5.tar", last modified: Thu Apr 11 03:20:39 2024, max compression
+gzip compressed data, was "easyofd-0.3.0.tar", last modified: Wed May 29 03:57:03 2024, max compression
```

## Comparing `easyofd-0.1.1.5.tar` & `easyofd-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 03:20:39.624474 easyofd-0.1.1.5/
--rw-rw-rw-   0        0        0    11550 2023-10-07 08:01:17.000000 easyofd-0.1.1.5/LICENSE
--rw-rw-rw-   0        0        0     1875 2024-04-11 03:20:39.623472 easyofd-0.1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1439 2024-03-14 10:29:52.000000 easyofd-0.1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 03:20:39.381949 easyofd-0.1.1.5/easyofd/
--rw-rw-rw-   0        0        0       41 2023-10-23 03:28:51.000000 easyofd-0.1.1.5/easyofd/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 03:20:39.495237 easyofd-0.1.1.5/easyofd/draw/
--rw-rw-rw-   0        0        0      492 2023-10-31 09:09:18.000000 easyofd-0.1.1.5/easyofd/draw/__init__.py
--rw-rw-rw-   0        0        0     4746 2023-12-06 06:05:56.000000 easyofd-0.1.1.5/easyofd/draw/draw_ofd.py
--rw-rw-rw-   0        0        0    16450 2024-04-11 03:18:54.000000 easyofd-0.1.1.5/easyofd/draw/draw_pdf.py
--rw-rw-rw-   0        0        0     2974 2023-10-26 07:49:17.000000 easyofd-0.1.1.5/easyofd/draw/font_tools.py
--rw-rw-rw-   0        0        0    11957 2023-12-05 08:02:52.000000 easyofd-0.1.1.5/easyofd/draw/ofdtemplate.py
--rw-rw-rw-   0        0        0    33496 2023-10-31 09:01:30.000000 easyofd-0.1.1.5/easyofd/draw/pdf_parse.py
--rw-rw-rw-   0        0        0     3904 2023-11-17 02:43:10.000000 easyofd-0.1.1.5/easyofd/ofd.py
-drwxrwxrwx   0        0        0        0 2024-04-11 03:20:39.599536 easyofd-0.1.1.5/easyofd/parser_ofd/
--rw-rw-rw-   0        0        0     1021 2023-10-21 09:56:30.000000 easyofd-0.1.1.5/easyofd/parser_ofd/__init__.py
--rw-rw-rw-   0        0        0     2963 2023-11-09 02:42:47.000000 easyofd-0.1.1.5/easyofd/parser_ofd/file_deal.py
--rw-rw-rw-   0        0        0    10238 2023-12-06 08:37:56.000000 easyofd-0.1.1.5/easyofd/parser_ofd/file_parser.py
--rw-rw-rw-   0        0        0    11119 2024-03-19 05:59:26.000000 easyofd-0.1.1.5/easyofd/parser_ofd/ofd_parser.py
-drwxrwxrwx   0        0        0        0 2024-04-11 03:20:39.398907 easyofd-0.1.1.5/easyofd.egg-info/
--rw-rw-rw-   0        0        0     1875 2024-04-11 03:20:39.000000 easyofd-0.1.1.5/easyofd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      532 2024-04-11 03:20:39.000000 easyofd-0.1.1.5/easyofd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 03:20:39.000000 easyofd-0.1.1.5/easyofd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-11 03:20:39.000000 easyofd-0.1.1.5/easyofd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-11 03:20:39.000000 easyofd-0.1.1.5/easyofd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 03:20:39.624474 easyofd-0.1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1008 2024-04-11 03:19:40.000000 easyofd-0.1.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 03:20:39.613500 easyofd-0.1.1.5/test/
--rw-rw-rw-   0        0        0      815 2023-10-26 06:35:50.000000 easyofd-0.1.1.5/test/test.py
--rw-rw-rw-   0        0        0     1282 2023-10-26 06:23:17.000000 easyofd-0.1.1.5/test/test_muty.py
+drwxrwxrwx   0        0        0        0 2024-05-29 03:57:03.267630 easyofd-0.3.0/
+-rw-rw-rw-   0        0        0    11550 2023-10-07 08:01:17.000000 easyofd-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     2096 2024-05-29 03:57:03.267630 easyofd-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1662 2024-04-26 02:47:22.000000 easyofd-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 03:57:03.215682 easyofd-0.3.0/easyofd/
+-rw-rw-rw-   0        0        0       62 2024-05-29 03:53:19.000000 easyofd-0.3.0/easyofd/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 03:57:03.239859 easyofd-0.3.0/easyofd/draw/
+-rw-rw-rw-   0        0        0      492 2023-10-31 09:09:18.000000 easyofd-0.3.0/easyofd/draw/__init__.py
+-rw-rw-rw-   0        0        0    10696 2024-05-21 07:47:47.000000 easyofd-0.3.0/easyofd/draw/draw_ofd.py
+-rw-rw-rw-   0        0        0    18213 2024-05-29 03:52:57.000000 easyofd-0.3.0/easyofd/draw/draw_pdf.py
+-rw-rw-rw-   0        0        0     3707 2024-05-29 03:52:41.000000 easyofd-0.3.0/easyofd/draw/find_seal_img.py
+-rw-rw-rw-   0        0        0     2960 2024-05-20 02:31:57.000000 easyofd-0.3.0/easyofd/draw/font_tools.py
+-rw-rw-rw-   0        0        0    22428 2024-05-22 01:57:42.000000 easyofd-0.3.0/easyofd/draw/ofdtemplate.py
+-rw-rw-rw-   0        0        0    39152 2024-05-20 10:42:45.000000 easyofd-0.3.0/easyofd/draw/pdf_parse.py
+-rw-rw-rw-   0        0        0     4020 2024-05-17 09:42:44.000000 easyofd-0.3.0/easyofd/ofd.py
+drwxrwxrwx   0        0        0        0 2024-05-29 03:57:03.242121 easyofd-0.3.0/easyofd/parser_ofd/
+-rw-rw-rw-   0        0        0     1021 2023-10-21 09:56:30.000000 easyofd-0.3.0/easyofd/parser_ofd/__init__.py
+-rw-rw-rw-   0        0        0     3003 2024-05-28 09:37:29.000000 easyofd-0.3.0/easyofd/parser_ofd/file_deal.py
+-rw-rw-rw-   0        0        0    12443 2024-05-29 03:31:45.000000 easyofd-0.3.0/easyofd/parser_ofd/file_parser.py
+-rw-rw-rw-   0        0        0     3403 2024-05-28 08:06:54.000000 easyofd-0.3.0/easyofd/parser_ofd/find_seal_img.py
+-rw-rw-rw-   0        0        0    13831 2024-05-29 03:51:31.000000 easyofd-0.3.0/easyofd/parser_ofd/ofd_parser.py
+drwxrwxrwx   0        0        0        0 2024-05-29 03:57:03.217677 easyofd-0.3.0/easyofd.egg-info/
+-rw-rw-rw-   0        0        0     2096 2024-05-29 03:57:03.000000 easyofd-0.3.0/easyofd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      598 2024-05-29 03:57:03.000000 easyofd-0.3.0/easyofd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 03:57:03.000000 easyofd-0.3.0/easyofd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2024-05-29 03:57:03.000000 easyofd-0.3.0/easyofd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-29 03:57:03.000000 easyofd-0.3.0/easyofd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 03:57:03.267630 easyofd-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2024-05-29 03:54:43.000000 easyofd-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 03:57:03.257823 easyofd-0.3.0/test/
+-rw-rw-rw-   0        0        0      815 2023-10-26 06:35:50.000000 easyofd-0.3.0/test/test.py
+-rw-rw-rw-   0        0        0     1282 2023-10-26 06:23:17.000000 easyofd-0.3.0/test/test_muty.py
```

### Comparing `easyofd-0.1.1.5/LICENSE` & `easyofd-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easyofd-0.1.1.5/PKG-INFO` & `easyofd-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyofd
-Version: 0.1.1.5
+Version: 0.3.0
 Summary: easy operate OFD
 Home-page: https://github.com/renoyuan/easyofd
 Author: renoyuan
 Author-email: renoyuan@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -29,21 +29,22 @@
 
 5 添加gui 工具实现上述功能
 
 
 
 
 
-
-
 关于 jb2格式图片解析 
 使用了第三方库 jbig2dec 去读取jb2格式图片 参考下面链接安装使用jbig2dec 
 https://github.com/rillian/jbig2dec 
 
 
+:hand: 有疑问或者建议需求等等，优先看看文档和demo代码，没有的请提交issues，不要直接发邮件，不要直接发邮件。
+
+:hand: 有啥问题在 github 上提 issues，有空的时候会尽力解答以及优化。邮箱只接受问题文件不做回复。
 
 ​	
 
 :hand:[参考文档实现](https://openstd.samr.gov.cn/bzgk/gb/newGbInfo?hcno=3AF6682D939116B6F5EED53D01A9DB5D )
 
 项目链接： https://github.com/renoyuan/easyofd
 
@@ -75,13 +76,13 @@
 
 3 本库对你有所帮助可以star 支持一下作者，或者fork。
 
 
 
 ### 版本规划:
 
-3月有时间会可能重构下代码并添加相应的注释。
+
 因为ofd本质上就是国产的pdf所以对于pdf的解析也会考虑单独封装一个模块，这块还要考虑一下。
```

### Comparing `easyofd-0.1.1.5/easyofd/draw/draw_pdf.py` & `easyofd-0.3.0/easyofd/draw/draw_pdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,28 +22,30 @@
 from reportlab.lib.utils import ImageReader
 from reportlab.pdfgen import canvas
 from reportlab.pdfbase import pdfmetrics
 from reportlab.pdfbase.cidfonts import UnicodeCIDFont
 from reportlab.pdfbase.ttfonts import TTFont
 from reportlab.lib import fonts as reportlab_fonts
 
+from .find_seal_img import SealExtract
 from easyofd.draw.font_tools import FontTool
 from loguru import logger
 
 # print(reportlab_fonts)
 class DrawPDF():
     """
     ofd 解析结果 绘制pdf
     OP ofd 单位转换
     """
     def __init__(self, data, *args, **kwargs):
         assert data, "未输入ofd解析结果"
         self.data = data
         self.author = "renoyuan"
         self.OP = 200/25.4
+        # self.OP = 1
         self.pdf_uuid_name = self.data[0]["pdf_name"]
         self.pdf_io = BytesIO() 
         self.SupportImgType = ("JPG", "IPEG", "PNG")
         self.init_font = "宋体"
         self.font_tool = FontTool()
     
    
@@ -190,15 +192,15 @@
                     # 按字符写入
                     else:
                         for cahr_id, _cahr_ in enumerate(text):
                             # print("char wtite")
                             c.setFont(font, line_dict["size"] * self.OP *resizeX)
                             _cahr_x = float(x_list[cahr_id])*self.OP
                             _cahr_y = (float(page_size[3])-(float(y_list[cahr_id])))*self.OP
-                            print(_cahr_x,  _cahr_y, _cahr_)
+                            # print(_cahr_x,  _cahr_y, _cahr_)
                             c.drawString(_cahr_x,  _cahr_y, _cahr_, mode=0)  # mode=3 文字不可见 0可見
                         
                             # text_write.append((_cahr_x,  _cahr_y, _cahr_))
                     
                 except Exception as e:
                     logger.error(f"{e}")
                     traceback.print_exc()     
@@ -223,15 +225,59 @@
             y = (page_size[3] - (img_d.get('pos')[1]+y_offset))*self.OP
             if wrap_pos:
                 x = x+(wrap_pos[0]*self.OP)
                 y = y-(wrap_pos[1]*self.OP)
             w = img_d.get('pos')[2]*self.OP
             h = -img_d.get('pos')[3]*self.OP
             c.drawImage(imgReade,x,y ,w, h, 'auto')
-                    
+
+    def draw_signature(self, canvas, signatures_page_list, page_size):
+        """
+        写入签章
+            {
+            "sing_page_no": sing_page_no,
+            "PageRef": PageRef,
+            "Boundary": Boundary,
+            "SignedValue": self.file_tree(SignedValue),
+                            }
+        """
+        c = canvas
+        try:
+            if signatures_page_list:
+                # print("signatures_page_list",signatures_page_list)
+                for signature_info in signatures_page_list:
+                    image = SealExtract()(b64=signature_info.get("SignedValue"))
+                    if not image:
+                        logger.info(f"提取不到签章图片")
+                        continue
+                    else:
+                        image_pil = image[0]
+
+                    pos = [float(i) for i in signature_info.get("Boundary").split(" ")]
+
+
+
+                    imgReade = ImageReader(image_pil)
+
+
+                    x = pos[0] * self.OP
+                    y = (page_size[3] -pos[1]) * self.OP
+
+                    w = pos[2] * self.OP
+                    h = -pos[3] * self.OP
+                    c.drawImage(imgReade, x, y, w, h, 'auto')
+                    print(f"签章写入成功")
+            else:
+                # 无签章
+                pass
+        except Exception as e:
+            print(f"签章写入失败 {e}")
+            traceback.print_exc()
+
+
     def draw_line(self,canvas,line_list,page_size):
         """绘制线条"""
         # print("绘制",line_list)
         for line in line_list:
             Abbr = line.get("AbbreviatedData").split(" ")  # AbbreviatedData 
             color = line.get("FillColor",[0,0,0])
             
@@ -334,46 +380,59 @@
         c = canvas.Canvas(self.pdf_io)
         c.setAuthor(self.author)
 
         for doc_id, doc in enumerate(self.data, start=0):
             fonts = doc.get("fonts")
             images = doc.get("images")
             page_size = doc.get("page_size")
-            
+            signatures_page_id = doc.get("signatures_page_id")  # 签证信息
+
+
             # 注册字体
             for font_id, font_v in fonts.items():
                 file_name = font_v.get("FontFile")
                 font_b64 = font_v.get("font_b64")
                 if font_b64:
                     self.font_tool.register_font(os.path.split(file_name)[1], font_v.get("@FontName"),font_b64)
             # text_write = []
             # print("doc.get(page_info)", len(doc.get("page_info")))
-            for page_id,page in doc.get("page_info").items():     
+            for page_id, page in doc.get("page_info").items():
+                logger.info(f"page_id {page_id}")
                 text_list = page.get("text_list")
                 img_list = page.get("img_list")
                 line_list = page.get("line_list")
                 # print("img_list",img_list)
               
                 c.setPageSize((page_size[2]*self.OP, page_size[3]*self.OP))
 
                 # 写入图片
                 self.draw_img(c, img_list, images, page_size)
 
+
+
                 # 写入文本
                 self.draw_chars(c, text_list, fonts, page_size)
 
                 # 绘制线条
                 self.draw_line(c, line_list, page_size)
+
+                # 绘制签章
+                self.draw_signature(c, signatures_page_id.get(page_id), page_size)
+
+
+
+
                 # print("去写入")
                 # print(doc_id,len(self.data))
                 # 页码判断逻辑
-                if page_id != len(doc.get("page_info"))-1  and doc_id != len(self.data):
+                if page_id != len(doc.get("page_info"))-1 and doc_id != len(self.data):
                     # print("写入")
                     c.showPage()  
             # json.dump(text_write,open("text_write.json","w",encoding="utf-8"),ensure_ascii=False)
+
         c.save()
         
     def __call__(self):
         try:
             self.draw_pdf()
             pdfbytes  = self.pdf_io.getvalue()
         except Exception as e:
```

### Comparing `easyofd-0.1.1.5/easyofd/draw/font_tools.py` & `easyofd-0.3.0/easyofd/draw/font_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,22 +76,22 @@
     def register_font(self,file_name,FontName,font_b64):
         
         if font_b64:
             
             file_name = os.path.split(file_name)
             # logger.error(f"file_name:{file_name}")
             # logger.info(f"file_name:{file_name}")
-            if isinstance(file_name,(tuple,list)):
+            if isinstance(file_name, (tuple, list)):
                     file_name = file_name[1]
             if not FontName:
                 FontName =  file_name.split(".")[0]
             try:
-                with open(file_name,"wb") as f: 
+                with open(file_name, "wb") as f:
                     f.write(base64.b64decode(font_b64))
-                
+
                 pdfmetrics.registerFont(TTFont(FontName, file_name))
                 self.FONTS.append(FontName)
                 
             except Exception as e:
                 traceback.print_exc()
                 logger.error(f"register_font_error:\n{e}")
```

### Comparing `easyofd-0.1.1.5/easyofd/draw/ofdtemplate.py` & `easyofd-0.3.0/easyofd/draw/draw_ofd.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,326 +1,271 @@
 #!/usr/bin/env python
 #-*- coding: utf-8 -*-
 #PROJECT_NAME: F:\code\easyofd\easyofd\draw
-#CREATE_TIME: 2023-10-30 
+#CREATE_TIME: 2023-10-26 
 #E_MAIL: renoyuan@foxmail.com
 #AUTHOR: reno 
-#note:  ofd 基础结构模板
-import tempfile
-import os
-import abc
-import copy
+#note:  写入 xml 目录并打包成ofd 文件
+import time
+from io import BytesIO
+from datetime import datetime
 
 import xmltodict
-import zipfile
+import cv2
+from PIL import Image
+from loguru import logger
 
-__all__ = ["OFDTemplate","DocumentTemplate","DocumentResTemplate","PulicResTemplate","ContentTemplate","OFDStructure"]
+from .pdf_parse import DPFParser
+from .ofdtemplate import CurId, OFDTemplate,DocumentTemplate,DocumentResTemplate,PublicResTemplate,ContentTemplate,OFDStructure
 
-class TemplateBase(object):
-    """模板基类"""
-    key_map = {}
-    def __init__(self,*args,**kwargs):
-        self.assemble(*args,**kwargs)
-        
-  
-    def assemble(self,*args,**kwargs):
-        """对ofdjson组装"""
-        self.final_json = copy.deepcopy(self.ofdjson)
-
-        if kwargs:
-            for k,v in kwargs.items():
-                if k in self.key_map :
-                    self.modify(self.final_json,self.key_map[k],v)
-                    
-    def modify(self,ofdjson,key,value):
-        """对指定key的值更改 多个会统一改"""
-        
-        for k,v in ofdjson.items():
-            if k == key:
-                ofdjson[k] = value
-            elif isinstance(v,dict):
-                self.modify(v,key,value)
-            elif isinstance(v,list):
-                for v_cell in v:
-                    if isinstance(v_cell,dict):
-                        self.modify(v_cell,key,value)
-    
-    def save(self,path):
-        xml_data = xmltodict.unparse(self.final_json, pretty=True)
-        with open(path,"w",encoding="utf-8") as f:
-            f.write(xml_data)
-
-class OFDTemplate(TemplateBase):
-    """根节点全局唯一"""
-    ofdjson = {
-        "ofd:OFD": {
-            "@xmlns:ofd": "http://blog.yuanhaiying.cn/",
-            "@Version": "1.1",
-            "@DocType": "OFD",
-            "ofd:DocBody": [{
-                "ofd:DocInfo": {
-                    "ofd:DocID": "0C1D4F7159954EEEDE517F7285E84DC4",
-                    "ofd:Creator": "easyofd",
-                    "ofd:author": "renoyuan",
-                    "ofd:authoremail": "renoyuan@foxmail.com",
-                    "ofd:CreatorVersion": "1.0",
-                    "ofd:CreationDate": "2023-10-27"
-                },
-                "ofd:DocRoot": "Doc_0/Document.xml"
-            }]
-        }
-    }
-
-class DocumentTemplate(TemplateBase):
-    """DOC 内唯一 表示DOC内部结构"""
-    key_map = {"Page":"ofd:Page"}
-    
-    ofdjson ={
-    "ofd:Document": {
-        "@xmlns:ofd": "http://blog.yuanhaiying.cn/",
-        "ofd:CommonData": {
-            "ofd:MaxUnitID": "106",
-            "ofd:PageArea": {
-                "ofd:PhysicalBox": "0 0 215.89999 279.39999"
-            },
-            "ofd:PublicRes": "PublicRes.xml",
-            "ofd:DocumentRes": "DocumentRes.xml"
-        },
-        "ofd:Pages": {
-            "ofd:Page": {
-                "@ID": "1",
-                "@BaseLoc": "Pages/Page_0/Content.xml"
+
+class OFDWrite(object):
+    """
+    写入ofd 工具类
+    """
+    def __init__(self,):
+        self.OP = 200/25.4
+        # self.OP = 1
+
+    def build_ofd_entrance(self, id_obj: CurId=None):
+        """
+        build_ofd_entrance
+        """
+        CreationDate = str(datetime.now())
+        ofd_entrance = OFDTemplate(CreationDate=CreationDate, id_obj=id_obj)
+        return ofd_entrance
+
+    def build_document(self, img_len, id_obj: CurId=None):
+        """
+        build_document
+        """
+        pages = []
+
+        for idx in range(img_len):
+            pages.append(
+                 {
+                "@ID": f"{idx+1}",
+                "@BaseLoc": f"Pages/Page_{idx}/Content.xml"
             }
-        }
-    }
-}
-    
-class DocumentResTemplate(TemplateBase):
-    """DOC 内唯一 表示MultyMedia 资源信息 如 图片 """
-    key_map = {"MultiMedia":"ofd:MultiMedia"}
-    ofdjson ={
-    "ofd:Res": {
-        "@xmlns:ofd": "http://blog.yuanhaiying.cn/",
-        "@BaseLoc": "Res",
-        "ofd:MultiMedias": {
-            "ofd:MultiMedia": [
-                {
-                    "@ID": "104",
+            )
+        document = DocumentTemplate(Page=pages, id_obj=id_obj)
+        return document
+
+    def build_document_res(self, img_len: int = 0, id_obj: CurId = None, pfd_res_uuid_map: [dict|None]=None):
+        """
+        build_document_res
+        """
+        MultiMedia = []
+        DrawParams = []  # todo DrawParams 参数后面有空增加
+        if img_len and not pfd_res_uuid_map:
+            for num in range(img_len):
+                MultiMedia.append({
+                    "@ID": f"9100{num}",
                     "@Type": "Image",
-                    "ofd:MediaFile": "Image_2.jpg"
-                }
-            ]
-        }
-    }
-}   
-
-class PulicResTemplate(TemplateBase):
-    """DOC 内唯一 公共配置资源信息 如 Font  Color 等"""
-    key_map = {"Font":"ofd:Font"}
-    
-    ofdjson = {
-    "ofd:Res": {
-        "@xmlns:ofd": "http://blog.yuanhaiying.cn/",
-        "@BaseLoc": "Res",
-        "ofd:ColorSpaces": {
-            "ofd:ColorSpace": {
-                "@ID": "4",
-                "@Type": "RGB"
-            }
-        },
-        "ofd:Fonts": {
-            "ofd:Font": [
-
-                {
-                    "@ID": "69",
-                    "@FontName": "STSong",
-                    "@FamilyName": "SimSun",
-                    "@Serif": "true",
-                    "@FixedWidth": "true",
+                    "ofd:MediaFile": f"Image_{num}.jpg"
+                })
+        elif pfd_res_uuid_map and (pfd_img := pfd_res_uuid_map.get("img")):
+            for res_uuid in pfd_img.keys():
+                name = f"Image_{res_uuid}.jpg"
+                MultiMedia.append({
+                    "@ID": 0,
+                    "@Type": "Image",
+                    "ofd:MediaFile": name,
+                    "res_uuid": res_uuid,
+
+                })
+
+
+
+        document_res = DocumentResTemplate(MultiMedia=MultiMedia, id_obj=id_obj)
+        return document_res
+
+    def build_public_res(self, id_obj: CurId=None, pfd_res_uuid_map: dict=None):
+        """
+        build_public_res
+        """
+        fonts = []
+        if pfd_font := pfd_res_uuid_map.get("font"):
+            for res_uuid, font in pfd_font.items():
+                fonts.append({
+                    "@ID": 0,
+                    "@FontName": font,
+                    "@FamilyName": font,  # 匹配替代字型
+                    "res_uuid": res_uuid,
+                    "@FixedWidth": "false",
+                    "@Serif": "false",
+                    "@Bold": "false",
                     "@Charset": "prc"
-                }
-            ]
-        }
-    }
-}
-  
-class ContentTemplate(TemplateBase):
-    """正文部分"""
-    key_map = {"ImageObject":"ofd:ImageObject",
-               "PathObject":"ofd:PathObject",
-               "TextObject":"ofd:TextObject",
-               "CGTransform":"ofd:CGTransform",
-               "PhysicalBox":"ofd:PhysicalBox",
-               }
-    ofdjson = {
-    "ofd:Page": {
-        "@xmlns:ofd": "http://blog.yuanhaiying.cn/",
-        "ofd:Area": {
-            "ofd:PhysicalBox": "0 0 211.62 141.08"
-        },
-        "ofd:Content": {
-            "ofd:Layer":  {
-                "@ID": "2",
-                "@Type": "Body",
-                "ofd:PathObject": [          {
-                        "@ID": "3",
-                        "@CTM": "0.3527 0 0 -0.3527 0.35 141.43001",
-                        "@Boundary": "-0.35 -0.35 212.33 141.78999",
-                        "@LineWidth": "1",
-                        "@MiterLimit": "10",
-                        "@Stroke": "false",
-                        "@Fill": "true",
-                        "ofd:FillColor": {
-                            "@ColorSpace": "4",
-                            "@Value": "255 255 255"
-                        },
-                        "ofd:StrokeColor": {
-                            "@ColorSpace": "4",
-                            "@Value": "0 0 0"
-                        },
-                        "ofd:Clips": {
-                            "ofd:Clip": {
-                                "ofd:Area": {
-                                    "ofd:Path": {
-                                        "@ID": "5",
-                                        "@Boundary": "0.00766 -0.00763 600 400.00003",
-                                        "@Stroke": "false",
-                                        "@Fill": "true",
-                                        "ofd:AbbreviatedData": "M 0 0 L 600 0 L 600 400.00003 L 0 400.00003 C"
-                                    }
-                                }
-                            }
-                        },
-                        "ofd:AbbreviatedData": "M -1 401 L 601 401 L 601 -1 L -1 -1 C"
-                    },],
-                "ofd:TextObject": [         {
-                        "@ID": "1",
-                        "@CTM": "7.054 0 0 7.054 0 134.026",
-                        "@Boundary": "69 7 72 7.6749",
-                        "@Font": "69",
-                        "@Size": "6.7028",
-                        "ofd:FillColor": {
-                            "@ColorSpace": "4",
-                            "@Value": "156 82 35"
-                        },
-                        "ofd:CGTransform": {
-                            "@CodePosition": "0",
-                            "@CodeCount": "10",
-                            "@GlyphCount": "10",
-                            "ofd:Glyphs": "18 10 11 42 60 53 24 11 42 61"
-                        },
-                        "ofd:TextCode": {
-                            "@X": "13.925",
-                            "@Y": "10",
-                            "@DeltaX": "7 7 7 7 7 7 7 7 7",
-                            "#text": "电⼦发票（普通发票）"
-                        }
-                    }],
-                "ofd:ImageObject": [{
-                        "@ID": "3",
-                        "@CTM": "19.7512 0 0 19.7512 0 0",
-                        "@Boundary": "7.23035 7.40671 19.7512 19.7512",
-                        "@ResourceID": "104"
-                    }],
-                }            
-        }}}
-                                        
-class OFDStructure(object):
-    """OFD structure"""
-    def __init__(self,name,ofd=OFDTemplate(),document=DocumentTemplate(),document_res=DocumentResTemplate(),pulic_res=PulicResTemplate(),content_res:list=[ContentTemplate()],res_static:dict={}):
-       self.name = name
-       self.ofd = ofd
-       self.document = document
-       self.document_res = document_res
-       self.pulic_res = pulic_res
-       self.content_res = content_res
-       self.res_static = res_static
-       
-    def __call__(self,):
-        with tempfile.TemporaryDirectory() as temp_dir:
-            # 创建过程目录
-            temp_dir_doc_0 = os.path.join(temp_dir, 'Doc_0')
-            temp_dir_pages = os.path.join(temp_dir, 'Doc_0',"Pages")
-            temp_dir_res = os.path.join(temp_dir, 'Doc_0',"Res")
-            for i in [temp_dir_doc_0,temp_dir_pages,temp_dir_res]:
-                # print(i)
-                os.mkdir(i)
-
-            # 写入 OFD
-            self.ofd.save(os.path.join(temp_dir, 'OFD.xml'))
-            
-            # 写入 Document
-            self.document.save(os.path.join(temp_dir_doc_0, 'Document.xml'))
-            
-            # 写入 DocumentRes
-            self.document_res.save(os.path.join(temp_dir_doc_0, 'DocumentRes.xml'))
-            
-            # 写入 PublicRes
-            self.pulic_res.save(os.path.join(temp_dir_doc_0, 'PublicRes.xml'))
-            
-            # 写入 content_res
-            for idx,page in enumerate(self.content_res):
-                temp_dir_pages_idx = os.path.join(temp_dir_pages, f"Page_{idx}")
-                os.mkdir(temp_dir_pages_idx)
-                # os.mkdir(i)
-                page.save( os.path.join(temp_dir_pages_idx, 'Content.xml'))
-                
-            # 写入静态资源
-            for k,v in self.res_static.items():
-                  with open(os.path.join(temp_dir_res,k),"wb") as f:
-                      f.write(v)
-                      
-            # 打包成ofd
-            zip = zipfile.ZipFile("test.ofd", "w", zipfile.ZIP_DEFLATED)
-            for path, dirnames, filenames in os.walk(temp_dir):
-                # 去掉目标跟路径，只对目标文件夹下边的文件及文件夹进行压缩
-                fpath = path.replace(temp_dir, '')
-        
-                for filename in filenames:
-                    zip.write(os.path.join(path, filename), os.path.join(fpath, filename))
-            zip.close()
-            with open("test.ofd","rb") as f:
-                content = f.read()
-            if os.path.exists("test.ofd"):
-               os.remove("test.ofd") 
-            return content
+                })
+        else:
+           pass
+
+        public_res = PublicResTemplate(Font=fonts, id_obj=id_obj)
+        return public_res
+
+    def build_content_res(self, pil_img_list=None, pdf_info_list=None, id_obj: CurId=None, pfd_res_uuid_map: dict=None):
+        """
+        pil_img_list - >一张图片是一页
+        content_res -> 写入 pdf 信息
+        """
+        PhysicalBox = None
+        content_res_list = []
+        if pil_img_list:
+            for idx, pil_img in enumerate(pil_img_list):
+                print(pil_img)
+                print(idx, pil_img[1], pil_img[2])
+                PhysicalBox = f"0 0 {pil_img[1]} {pil_img[2]}"
+                ImageObject = [{
+                                    "@ID": f"110{idx}",
+                                    "@CTM": f"{pil_img[1]} 0 0 {pil_img[2]} 0 0",
+                                    "@Boundary": f"0 0 {pil_img[1]} {pil_img[2]}",
+                                    "@ResourceID": f"9100{idx}"
+                                }]
+
+                conten = ContentTemplate(PhysicalBox=PhysicalBox, ImageObject=ImageObject,
+
+                                         CGTransform=[],PathObject=[],TextObject=[], id_obj=id_obj)
+                print(conten)
+                content_res_list.append(conten)
+        elif pdf_info_list:  # 写入读取后的pdf 结果 # todo 图片id 需要关联得提前定义或者有其他方式反向对齐
+
+            for idx, content in enumerate(pdf_info_list):
+                ImageObject = []
+                TextObject = []
+                PhysicalBox = pfd_res_uuid_map["other"]["page_size"][idx]
+                PhysicalBox = f"0 0 {PhysicalBox[0]} {PhysicalBox[1]}" # page_size 没有的话使用document 里面的
+                for block in content:
+                    # print(block)
+
+                    bbox = block['bbox']
+                    x0, y0, length, height = bbox[0] / self.OP, bbox[1] / self.OP, (bbox[2] - bbox[0]) / self.OP, (
+                                bbox[3] - bbox[1]) / self.OP
+                    if block["type"] == "text":
+
+                        count=len(block.get("text"))
+
+                        TextObject.append({
+                            "@ID": 0,
+                            "res_uuid": block.get("res_uuid"),  # 资源标识
+                            "@Font": "",
+                            "ofd:FillColor":{"Value": "156 82 35"},
 
+                            "ofd:TextCode":{
+                                "#text": block.get("text"),
+                                "@X":"0",
+                                "@Y":f"{block.get('size') / self.OP}",
+                                "@DeltaX": f"g {count-1} {length/count}"
+                            },
+
+                            "@size": block.get("size") / self.OP,
+                            "@Boundary": f"{x0} {y0} {length} {height}",
+
+                        })
+                    elif block["type"] == "img":
+                        ImageObject.append({
+                        "@ID": 0,
+                        "res_uuid": block.get("res_uuid"),  #资源标识
+
+                        "@Boundary": f"{x0} {y0} {length} {height}",
+                        "@ResourceID": f""  # 需要关联public res 里面的结果
+
+                })
+
+
+
+                # for i in content:
+                #     if i["type"] == "img":
+                #         ImageObject.append(i)
+                #     elif i["type"] == "text":
+                #         TextObject.append(i)
+
+                conten = ContentTemplate(PhysicalBox=PhysicalBox, ImageObject=ImageObject,
+
+                                         CGTransform=[], PathObject=[], TextObject=TextObject, id_obj=id_obj)
+                print(conten)
+                content_res_list.append(conten)
+        else:
+            pass
+        return content_res_list
+
+    def pil_2_bytes(self, image):
+        # 创建一个 BytesIO 对象
+        img_bytesio = BytesIO()
+
+        # 将图像保存到 BytesIO 对象
+        image.save(img_bytesio, format='PNG')  # 你可以根据需要选择其他图像格式
+
+        # 获取 BytesIO 对象中的字节
+        img_bytes = img_bytesio.getvalue()
+
+        # 关闭 BytesIO 对象
+        img_bytesio.close()
+        return img_bytes
+    
+    def __call__(self, pdf_bytes, cv2_img_list=None, optional_text=False):
+        """
+        0 解析pdf文件
+        1 构建必要的ofd template
+        2 转化为 ofd
+        """
+        pdf_obj = DPFParser()
+        if optional_text:  # 生成可编译ofd:
+            pdf_info_list, pfd_res_uuid_map = pdf_obj.extract_text_with_details(pdf_bytes) # 解析pdf
+            logger.debug(f"pdf_info_list: {pdf_info_list} \n pfd_res_uuid_map {pfd_res_uuid_map}")
+
+            page_pil_img_list = None
+
+        else:
+            if cv2_img_list:  # 读取 图片
+                page_pil_img_list = [(self.pil_2_bytes(Image.fromarray(cv2.cvtColor(_img,cv2.COLOR_BGR2RGB))),
+                                 _img.shape[1], _img.shape[0]) for _img in cv2_img_list]
+            else:  # 读取 pdf 转图片
+                img_list = pdf_obj.to_img(pdf_bytes)
+                page_pil_img_list = [(self.pil_2_bytes(Image.frombytes("RGB", [_img.width, _img.height],
+                                                          _img.samples)), _img.width, _img.height) for _img in img_list]
+
+        id_obj = CurId()
+
+        if page_pil_img_list:  # img 内容转ofd
+            ofd_entrance = self.build_ofd_entrance(id_obj=id_obj)
+            document = self.build_document(len(page_pil_img_list), id_obj=id_obj)
+            public_res = self.build_public_res(id_obj=id_obj)
+            document_res = self.build_document_res(len(page_pil_img_list), id_obj=id_obj)
+
+            content_res_list = self.build_content_res(page_pil_img_list, id_obj=id_obj)
+
+            res_static = {}  # 图片资源
+            for idx, pil_img_tuple in enumerate(page_pil_img_list):
+                res_static[f"Image_{idx}.jpg"] = pil_img_tuple[0]
+        else:
+            #  生成的文档结构对象需要传入id实例
+            ofd_entrance = self.build_ofd_entrance(id_obj=id_obj)
+            document = self.build_document(len(pdf_info_list), id_obj=id_obj)
+            public_res = self.build_public_res(id_obj=id_obj, pfd_res_uuid_map=pfd_res_uuid_map)
+            document_res = self.build_document_res(len(pdf_info_list), id_obj=id_obj, pfd_res_uuid_map=pfd_res_uuid_map)
+            content_res_list = self.build_content_res(pdf_info_list=pdf_info_list, id_obj=id_obj, pfd_res_uuid_map=pfd_res_uuid_map)
+
+            res_static = {}  # 图片资源
+
+            print("pfd_res_uuid_map", pfd_res_uuid_map)
+            img_dict = pfd_res_uuid_map.get("img")
+            if img_dict:
+                for key, v_io in img_dict.items():
+                    res_static[f"Image_{key}.jpg"] = v_io.getvalue()
+
+        # 生成 ofd 文件
+        ofd_byte = OFDStructure("123", ofd=ofd_entrance,document = document,public_res=public_res,
+                                document_res=document_res, content_res=content_res_list,res_static=res_static)(test=True)
+        return ofd_byte
+        
 if  __name__ == "__main__":
     
+    pdf_p = r"D:\renodoc\技术栈\GBT_33190-2016_电子文件存储与交换格式版式文档.pdf"
+    with open(pdf_p,"rb") as f:
+        content = f.read()
     
-    font = [
-                {
-                    "@ID": "69",
-                    "@FontName": "STSong",
-                    "@FamilyName": "SimSun",
-                    "@Serif": "true",
-                    "@FixedWidth": "true",
-                    "@Charset": "prc"
-                }
-            ]
+    ofd_content = OFDWrite()(content)
     
-    MultiMedia = [
-                {
-                    "@ID": "55",
-                    "@Type": "Image",
-                    "ofd:MediaFile": "Image_0.jpg"
-                }
-            ]
-            
-    pulic_res=PulicResTemplate(Font=font)
-    document_res=DocumentResTemplate(MultiMedia=MultiMedia)
-    ImageObject = [{
-                        "@ID": "55",
-                        "@CTM": "200 0 0 140 0 0",
-                        "@Boundary": "0 0 200 140",
-                        "@ResourceID": "55"
-                    }]
-    content_res = ContentTemplate(ImageObject=ImageObject,CGTransform=[],PathObject=[],TextObject=[])
-    path  = r"F:\code\easyofd\easyofd\draw\Image_0.jpg"
-    f = open(path, "rb")
-    content = f.read()
-    f.close()
-    res_static = {"Image_0.jpg":content}
-    ofd_byte = OFDStructure("123",pulic_res=pulic_res,document_res=document_res,content_res=[content_res],res_static=res_static)()
-    with open("test.ofd","wb") as f:
-        content = f.write(ofd_byte)
-                
+    with open("ofd.ofd", "wb") as f:
+        f.write(ofd_content)
+    
+
```

### Comparing `easyofd-0.1.1.5/easyofd/draw/pdf_parse.py` & `easyofd-0.3.0/easyofd/draw/pdf_parse.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,20 @@
-# -*- coding: utf-8 -*-
-
-"""
-# @Time    : 2022/11/14 0014 16:11
-# @Author  : Silva
-# @File    : pdf_parse_nice.py
-"""
-
 import os
 import re
+import io
+
 import json
 import time
 import copy
 import string
 import random
 from uuid import uuid1
 from decimal import Decimal
 from collections import OrderedDict
+
 # 第三方包
 import fitz
 from PIL import Image
 # import pdfplumber
 
 __ALL__ = ['pdf_ocr',"DPFParser"]
 
@@ -30,15 +25,139 @@
         elif isinstance(obj, Decimal):
             return float(obj)
         return json.JSONEncoder.default(self, obj)
 
 class DPFParser(object):
     def __init__(self, ):
         pass
-    def to_img(self,buffer_pdf):
+
+    def extract_text_with_details(self, pdf_bytes):
+        """
+        提取PDF每页的文本及其位置、字体信息。
+
+        :param pdf_path: PDF文件路径
+        :return: 包含每页文本及其详细信息的列表
+        [[
+
+        ]]
+        """
+        details_list = []
+        pdf_stream = io.BytesIO(pdf_bytes)
+
+        # 使用fitz.open直接打开BytesIO对象
+
+        with fitz.open(stream=pdf_stream, filetype="pdf") as doc:
+            res_uuid_map = {
+                "img":{},
+                "font":{},
+                "other":{}
+            } # 全局资源标识
+            for page_num in range(len(doc)):
+
+
+                page_details_list = []  # 页面内信息
+                page = doc.load_page(page_num)
+                rect = page.rect
+                width = rect.width
+                height = rect.height
+                if res_uuid_map["other"].get("page_size"):
+                    res_uuid_map["other"]["page_size"][page_num] = [width,height]
+                else :
+                    res_uuid_map["other"]["page_size"] = {page_num: [width, height]}
+                blocks = page.get_text("dict").get("blocks")  # 获取文本块信息
+                image_list = page.get_images(full=True)  # 获取页面上所有图片的详细信息
+                # print(blocks)
+                # 获取页面内文本信息
+                for block in blocks:
+                    block_text = block.get("text", "")
+                    block_rect = block["bbox"]  # 文本块的边界框，格式为[x0, y0, x1, y1]
+
+                    # 遍历块中的每一行
+                    for line in block.get("lines", []):
+                        line_text = line.get("spans", [{}])[0].get("text", "")  # 单行文本
+                        line_rect = line["bbox"]  # 行的边界框
+
+                        # 遍历行中的每一个跨度（span），获取字体信息
+                        for span in line.get("spans", []):
+                            span_text = span.get("text", "")
+                            font_size = span.get("size")  # 字体大小
+                            font_name = span.get("font")  # 字体名称
+                            res_uuid = None
+                            if font_name not in res_uuid_map["font"].values():
+                                res_uuid = str(uuid1())
+                                res_uuid_map["font"][res_uuid] = font_name
+                            else:
+                                keys = list(res_uuid_map["font"].keys())
+                                vs = list(res_uuid_map["font"].values())
+                                idx = vs.index(font_name)
+                                res_uuid =keys[idx]
+                            font_color = span.get("color")  # 字体颜色，默认可能没有
+                            span_rect = (
+                            line_rect[0], line_rect[1], line_rect[2], line_rect[3])  # 使用行的边界框作为参考，具体到单个字符或词可能需要更复杂的处理
+
+                            # 打印或存储信息
+                            print(
+                                f"Page: {page_num }, Text: '{span_text}', Font: {font_name}, Size: {font_size}, "
+                                f"Color: {font_color}, Rect: {span_rect} ,res_uuid {res_uuid}")
+
+                            # 存储信息到details_list中（根据需要调整存储格式）
+                            page_details_list.append({
+                                "page": page_num,
+                                "text": span_text,
+                                "font": font_name,
+                                "res_uuid": res_uuid,
+                                "size": font_size,
+                                "color": font_color,
+                                "bbox": list(span_rect),
+                                "type": "text"
+                            })
+
+                for image_index, img_info in enumerate(image_list):
+                    # 解析图片信息
+                    xref = img_info[0]
+                    base_image = doc.extract_image(xref)
+
+                    image_data = base_image["image"]  # 图片数据
+                    res_uuid = str(uuid1())
+
+                    img_io = io.BytesIO(image_data)
+                    res_uuid_map["img"][res_uuid] = img_io
+                    image_type = base_image["ext"]  # 图片类型
+                    smask = base_image["smask"]  # 图片类型
+                    xres = base_image["xres"]  # 图片类型
+                    yres = base_image["yres"]  # 图片类型
+                    width = base_image["width"]  # 图片宽度
+                    height = base_image["height"]  # 图片高度
+
+
+
+                    # 计算坐标（左下角和右上角）
+                    x0, y0, x1, y1 = xres, yres,xres+width,yres+height
+                    print(
+                        f"Page: {page_num}, image_type: '{image_type}',x0{x0}, y0{y0}, x1{x1}, y1{y1}  ")
+                    page_details_list.append({
+                        "page": page_num,
+                        "index": image_index,
+                        "x0": x0,
+                        "y0": y0,
+                        "x1": x1,
+                        "y1": y1,
+                        "bbox": [x0,y0,width,height],
+                        "width": width,
+                        "height": height,
+                        "res_uuid": res_uuid,
+                        "image_type": image_type,
+                        "type": "img"
+                    })
+
+                details_list.append(page_details_list)
+        # print("details_list",details_list)
+        return details_list, res_uuid_map
+    def to_img(self, buffer_pdf):
+        """转图片"""
         pix_list = []
         pdfDoc = fitz.open(stream=buffer_pdf)
         for pg in range(pdfDoc.page_count):
             page = pdfDoc[pg]
             rotate = int(0)
             # 每个尺寸的缩放系数为1.3，这将为我们生成分辨率提高2.6的图像。
             # 此处若是不做设置，默认图片大小为：792X612, dpi=96
```

### Comparing `easyofd-0.1.1.5/easyofd/ofd.py` & `easyofd-0.3.0/easyofd/ofd.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,24 +22,23 @@
 from easyofd.draw import DrawPDF,OFDWrite
 
 class OFD(object):
     """ofd对象"""
     def __init__(self,):
         self.data = None 
         
-    def read(self,ofd_f,fomat="b64",save_xml=False, xml_name="testxml"):
+    def read(self, ofd_f, fomat="b64", save_xml=False, xml_name="testxml"):
         """_summary_
-
         Args:
             file (_type_): _description_
             fomat (str, optional): _description_. Defaults to "path".
             fomat in ("path","b64","binary")
         """
         if fomat == "path":
-            with open(ofd_f,"rb") as f:
+            with open(ofd_f, "rb") as f:
                 ofd_f = str(base64.b64encode(f.read()),encoding="utf-8") 
         elif fomat == "b64":
             pass
         elif fomat == "binary":
             ofd_f = str(base64.b64encode(ofd_f),encoding="utf-8")
         else:
             raise "fomat Error: %s" % fomat
@@ -50,27 +49,29 @@
         """
         draw ofd xml
         初始化一个xml 文件
         self.data > file
         """
         assert self.data,f"data is None"
 
-    def pdf2ofd(self,pdfbyte):
+    def pdf2ofd(self, pdfbyte, optional_text=False):
         """pdf转ofd"""
-        ofd_byte = OFDWrite()(pdfbyte)
+        assert pdfbyte, f"pdfbyte is None"
+        logger.info(f"pdf2ofd")
+        ofd_byte = OFDWrite()(pdfbyte, optional_text=optional_text)
         return ofd_byte
     
     def to_pdf(self,):
         """return ofdbytes"""
 
-        assert self.data,f"data is None"
+        assert self.data, f"data is None"
         logger.info(f"to_pdf")
         return DrawPDF(self.data)()
     
-    def pdf2img(self,pdfbytes):
+    def pdf2img(self, pdfbytes):
         
         image_list = []
       
         
         doc = fitz.open(stream=pdfbytes, filetype="pdf")
       
         for page in doc:
@@ -85,19 +86,18 @@
         logger.info(f"to_jpg")
         return image_list
     
     def jpg2ofd(self,imglist:list):
         """
         imglist: cv2 image list
         """
-        
-        ofd_byte = OFDWrite()(None,CV2_img_list=imglist)
+        ofd_byte = OFDWrite()(cv2_img_list=imglist)
         return ofd_byte
     
-    def jpg2pfd(self,imglist:list ):
+    def jpg2pfd(self,imglist:list):
         """
         imglist: cv2 image list
         1 构建data 
         2 DrawPDF(self.data)()
         """
         
         data = OFDParser(None).img2data(imglist)
```

### Comparing `easyofd-0.1.1.5/easyofd/parser_ofd/__init__.py` & `easyofd-0.3.0/easyofd/parser_ofd/__init__.py`

 * *Files identical despite different names*

### Comparing `easyofd-0.1.1.5/easyofd/parser_ofd/file_deal.py` & `easyofd-0.3.0/easyofd/parser_ofd/file_deal.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     def unzip_file(self):
         """
         :param zip_path: ofd格式文件路径
         :param unzip_path: 解压后的文件存放目录
         :return: unzip_path
         """
         with open(self.zip_path,"wb") as f:
-                f.write(self.ofdbyte)
+            f.write(self.ofdbyte)
         self.unzip_path = self.zip_path.split('.')[0]
         with zipfile.ZipFile(self.zip_path, 'r') as f:
             for file in f.namelist():
                 f.extract(file, path=self.unzip_path)
         if self.save_xml:
             print("saving xml {}".format(self.xml_name))
             with zipfile.ZipFile(self.zip_path, 'r') as f:
@@ -54,15 +54,15 @@
         "xml读取对象其他b64"
         self.file_tree["root"] = self.unzip_path
         self.file_tree["pdf_name"] = self.pdf_name
         for root, dirs, files in os.walk(self.unzip_path):
             for file in files:
                 
                 abs_path = os.path.join(root,file)
-                
+                # 资源文件 则 b64 xml 则  xml——obj
                 self.file_tree[abs_path] = str(base64.b64encode(open(f"{abs_path}","rb").read()),"utf-8")  \
                     if "xml" not in file else xmltodict.parse(open(f"{abs_path}" , "r", encoding="utf-8").read())
         self.file_tree["root_doc"] = os.path.join(self.unzip_path,"OFD.xml") if os.path.join(self.unzip_path,"OFD.xml") in self.file_tree else ""
   
         if os.path.exists(self.unzip_path):
             shutil.rmtree(self.unzip_path)
```

### Comparing `easyofd-0.1.1.5/easyofd/parser_ofd/file_parser.py` & `easyofd-0.3.0/easyofd/parser_ofd/file_parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -58,37 +58,48 @@
 class OFDFileParser(FileParserBase):
     def __call__(self):
         info = {}
         # DocRoot 
         doc_root:list = []
         doc_root_key = "ofd:DocRoot" 
         # print(self.xml_obj,doc_root)
-        self.recursion_ext(self.xml_obj,doc_root,doc_root_key)
-        
+        self.recursion_ext(self.xml_obj, doc_root, doc_root_key)
         info["doc_root"] = doc_root
-        
+
+        signatures: list = []
+        signatures_key = "ofd:Signatures"
+        self.recursion_ext(self.xml_obj, signatures, signatures_key)
+        info["signatures"] = signatures
+
         # ofd:Creator 
-        creator:list = []
+        creator: list = []
         creator_key = "ofd:Creator" 
         self.recursion_ext(self.xml_obj,creator,creator_key)
         info["creator"] = creator
         
         # ofd:CreationDate 
         reation_date:list = []
         creation_date_key = "ofd:CreationDate" 
         self.recursion_ext(self.xml_obj,reation_date,creation_date_key)
-        info["creator"] = reation_date
+        info["creationDate"] = reation_date
         
         return info
 
 class DocumentFileParser(FileParserBase):
     """
     Document 为doc内的根节点 包含：
     1 文件的路径 2 doc的size 
     """
+    def loc2page_no(self,loc,idx):
+        pg_no = re.search(r"\d+", loc)
+        if pg_no:
+            pg_no = int(pg_no.group())
+        else:
+            pg_no = idx
+        return pg_no
     def __call__(self):
         document_info = {}
         
         # size 
         physical_box:list = []
         physical_box_key = "ofd:PhysicalBox" 
         self.recursion_ext(self.xml_obj,physical_box,physical_box_key)
@@ -104,20 +115,27 @@
         document_res:list = []
         document_res_key = "ofd:DocumentRes" 
         self.recursion_ext(self.xml_obj,document_res,document_res_key)
         document_info["document_res"] = document_res
         
         # ofd:Page 正文
         page:list = []
+        page_id_map = {}
         apage_key = "ofd:Page" 
         self.recursion_ext(self.xml_obj,page,apage_key)
         if page :
-            page = [i.get("@BaseLoc") if isinstance(i,dict) else i for i in page  ] 
+            page_id_map = {
+                i.get("@ID"): self.loc2page_no(i.get("@BaseLoc"), idx)
+                for idx, i in enumerate(page)
+                           }
+            page = [i.get("@BaseLoc") if isinstance(i, dict) else i for i in page  ]
+
         document_info["page"] = page
-        
+        document_info["page_id_map"] = page_id_map
+
         tpls:list = []
         template_page_key = "ofd:TemplatePage"
         self.recursion_ext(self.xml_obj,tpls,template_page_key)
         if tpls :
             tpls = [i.get("@BaseLoc") if isinstance(i,dict) else i for i in tpls  ] 
         document_info["tpls"] = tpls
         
@@ -268,11 +286,62 @@
         return info 
                             
 class AnnotationFileParser(FileParserBase):
     """
     Parser Annotation
     签名信息 暂不用
     """
-    pass 
-    
+    pass
+
+class SignaturesFileParser(FileParserBase):
+    """
+    Parser Signatures
+    签章信息-总
+    """
+
+    def __call__(self):
+        info = {}
+        signature_res: list = []
+        signature_res_key = "ofd:Signature"
+        self.recursion_ext(self.xml_obj, signature_res, signature_res_key)
+
+        if signature_res:
+            for i in signature_res:
+                info[i.get("@ID")] = {
+                    "BaseLoc": i.get("@BaseLoc"),
+                    "Type": i.get("@Type"),
+                    "ID": i.get("@ID"),
+
+                }
+        return info
+
+class SignatureFileParser(FileParserBase):
+    """
+    Parser Signature
+    签章信息
+    """
+
+    def __call__(self, prefix=""):
+        info = {}
+        StampAnnot_res: list = []
+        StampAnnot_res_key = "ofd:StampAnnot"
+
+        self.recursion_ext(self.xml_obj, StampAnnot_res, StampAnnot_res_key)
+
+        SignedValue_res: list = []
+        SignedValue_res_key = "ofd:SignedValue"
+        self.recursion_ext(self.xml_obj, SignedValue_res, SignedValue_res_key)
+
+        # print("SignedValue_res", SignedValue_res)
+        # print("prefix", prefix)
+        if StampAnnot_res:
+            for i in StampAnnot_res:
+                info = {
+                    "PageRef": i.get("@PageRef"),  # page id
+                    "Boundary": i.get("@Boundary"),
+                    "ID": i.get("@ID"),
+                    "SignedValue": f"{prefix}/{SignedValue_res[0]}" if SignedValue_res else f"{prefix}/SignedValue.dat",
+                }
+
+        return info
 if __name__ == "__main__":
     FileParserBase("")()
```

### Comparing `easyofd-0.1.1.5/easyofd.egg-info/PKG-INFO` & `easyofd-0.3.0/easyofd.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyofd
-Version: 0.1.1.5
+Version: 0.3.0
 Summary: easy operate OFD
 Home-page: https://github.com/renoyuan/easyofd
 Author: renoyuan
 Author-email: renoyuan@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -29,21 +29,22 @@
 
 5 添加gui 工具实现上述功能
 
 
 
 
 
-
-
 关于 jb2格式图片解析 
 使用了第三方库 jbig2dec 去读取jb2格式图片 参考下面链接安装使用jbig2dec 
 https://github.com/rillian/jbig2dec 
 
 
+:hand: 有疑问或者建议需求等等，优先看看文档和demo代码，没有的请提交issues，不要直接发邮件，不要直接发邮件。
+
+:hand: 有啥问题在 github 上提 issues，有空的时候会尽力解答以及优化。邮箱只接受问题文件不做回复。
 
 ​	
 
 :hand:[参考文档实现](https://openstd.samr.gov.cn/bzgk/gb/newGbInfo?hcno=3AF6682D939116B6F5EED53D01A9DB5D )
 
 项目链接： https://github.com/renoyuan/easyofd
 
@@ -75,13 +76,13 @@
 
 3 本库对你有所帮助可以star 支持一下作者，或者fork。
 
 
 
 ### 版本规划:
 
-3月有时间会可能重构下代码并添加相应的注释。
+
 因为ofd本质上就是国产的pdf所以对于pdf的解析也会考虑单独封装一个模块，这块还要考虑一下。
```

### Comparing `easyofd-0.1.1.5/easyofd.egg-info/SOURCES.txt` & `easyofd-0.3.0/easyofd.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 easyofd.egg-info/SOURCES.txt
 easyofd.egg-info/dependency_links.txt
 easyofd.egg-info/requires.txt
 easyofd.egg-info/top_level.txt
 easyofd/draw/__init__.py
 easyofd/draw/draw_ofd.py
 easyofd/draw/draw_pdf.py
+easyofd/draw/find_seal_img.py
 easyofd/draw/font_tools.py
 easyofd/draw/ofdtemplate.py
 easyofd/draw/pdf_parse.py
 easyofd/parser_ofd/__init__.py
 easyofd/parser_ofd/file_deal.py
 easyofd/parser_ofd/file_parser.py
+easyofd/parser_ofd/find_seal_img.py
 easyofd/parser_ofd/ofd_parser.py
 test/test.py
 test/test_muty.py
```

### Comparing `easyofd-0.1.1.5/setup.py` & `easyofd-0.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
 import setuptools 
- 
+from easyofd import __version__
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="easyofd", 
-    version="0.1.1.5",
+    version=__version__,
     author="renoyuan",    
     author_email="renoyuan@foxmail.com",    
     description="easy operate OFD",
     long_description=long_description,   
     long_description_content_type="text/markdown",
     url="https://github.com/renoyuan/easyofd",    
     packages=setuptools.find_packages(exclude=["README.md",".vscode", ".vscode.*", ".git", ".git.*"]),
@@ -21,11 +21,12 @@
     ],
     install_requires=[   ### 依赖包
         "reportlab>=3.6.11",
         "xmltodict>=0.13.0",
         "loguru>=0.7.2",
         "fontTools>=4.43.1",
         "PyMuPDF>=1.23.4",
-        "opencv-python>=4.6.0.66"
+        "opencv-python>=4.6.0.66",
+        "pyasn1>=0.6.0"
                      ],
     python_requires='>=3.8',   
 )
```

### Comparing `easyofd-0.1.1.5/test/test.py` & `easyofd-0.3.0/test/test.py`

 * *Files identical despite different names*

### Comparing `easyofd-0.1.1.5/test/test_muty.py` & `easyofd-0.3.0/test/test_muty.py`

 * *Files identical despite different names*

