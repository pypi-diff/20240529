# Comparing `tmp/dianDataAna-0.3.tar.gz` & `tmp/dianDataAna-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dianDataAna-0.3.tar", last modified: Tue May 28 09:21:29 2024, max compression
+gzip compressed data, was "dianDataAna-0.4.tar", last modified: Wed May 29 04:53:08 2024, max compression
```

## Comparing `dianDataAna-0.3.tar` & `dianDataAna-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 09:21:29.030062 dianDataAna-0.3/
--rw-rw-rw-   0        0        0      102 2024-05-28 09:21:29.028061 dianDataAna-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-28 09:21:29.010176 dianDataAna-0.3/dianDataAna/
--rw-rw-rw-   0        0        0     5104 2024-05-28 09:20:23.000000 dianDataAna-0.3/dianDataAna/DataRead.py
--rw-rw-rw-   0        0        0       48 2024-05-28 08:23:22.000000 dianDataAna-0.3/dianDataAna/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 09:21:29.026061 dianDataAna-0.3/dianDataAna.egg-info/
--rw-rw-rw-   0        0        0      102 2024-05-28 09:21:28.000000 dianDataAna-0.3/dianDataAna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2024-05-28 09:21:28.000000 dianDataAna-0.3/dianDataAna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 09:21:28.000000 dianDataAna-0.3/dianDataAna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-28 09:21:28.000000 dianDataAna-0.3/dianDataAna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-05-28 07:23:06.000000 dianDataAna-0.3/license.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 09:21:29.030062 dianDataAna-0.3/setup.cfg
--rw-rw-rw-   0        0        0      234 2024-05-28 09:20:58.000000 dianDataAna-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 04:53:08.606596 dianDataAna-0.4/
+-rw-rw-rw-   0        0        0      102 2024-05-29 04:53:08.604624 dianDataAna-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-29 04:53:08.589283 dianDataAna-0.4/dianDataAna/
+-rw-rw-rw-   0        0        0     6064 2024-05-29 04:51:57.000000 dianDataAna-0.4/dianDataAna/DataRead.py
+-rw-rw-rw-   0        0        0       48 2024-05-28 08:23:22.000000 dianDataAna-0.4/dianDataAna/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 04:53:08.600364 dianDataAna-0.4/dianDataAna.egg-info/
+-rw-rw-rw-   0        0        0      102 2024-05-29 04:53:08.000000 dianDataAna-0.4/dianDataAna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2024-05-29 04:53:08.000000 dianDataAna-0.4/dianDataAna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 04:53:08.000000 dianDataAna-0.4/dianDataAna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-29 04:53:08.000000 dianDataAna-0.4/dianDataAna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-05-28 07:23:06.000000 dianDataAna-0.4/license.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 04:53:08.606596 dianDataAna-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      234 2024-05-29 04:52:11.000000 dianDataAna-0.4/setup.py
```

### Comparing `dianDataAna-0.3/dianDataAna/DataRead.py` & `dianDataAna-0.4/dianDataAna/DataRead.py`

 * *Files 13% similar despite different names*

```diff
@@ -116,17 +116,35 @@
                 output_column.append([])
                 # print([column3]+[column2])
                 output_column[j]=column3
                 output_column[j+1]=column2
                 i += 1
                 j += 2
     return(output_column)  # 输出[[x1],[y1],[x2],[y2]]
-
 # to here: Tensile data reader
+
+
 # print(IR_data_reader("./IR.txt",0,1000)[0])
 # print(Tensile_data_reader("Tensile.csv"))
 # test = Tensile_data_reader("Tensile.csv")
 # j=0
 # for count_i in range(0, 3):
 #     plt.plot(test[j],test[j+1])
 #     j+=2
-# plt.show()
+# plt.show()
+def write_to_txt(output_filename, list_input, reverse=True):  # 写入list(一般是其他fuc转换为的list),当reverse为True，将按列储存转换为按行储存，然后输出到output_filename中
+    # 找到最长的列长度
+    max_length = max(len(column) for column in list_input)
+    # 将每列填充到相同的长度
+    padded_columns = [column + [''] * (max_length - len(column)) for column in list_input]
+    # 转置列表
+    list_of_reverse = list(zip(*padded_columns))
+    if reverse == True:
+        with open('./'+output_filename,'w',encoding='utf-8') as writeObject1:
+            for row in list_of_reverse:
+                # line = ','.join(str(row))
+                writeObject1.write(str(row).replace('(','').replace(')','')+'\n')
+        writeObject1.close()
+    # print(list_of_reverse)
+    return list_of_reverse  # 返回置换后的list
+# listt=IR_data_reader('./IR.txt')
+# write_to_txt('IR.txt', listt)
```

