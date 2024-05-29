# Comparing `tmp/bribrain-1.0.4.tar.gz` & `tmp/bribrain-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bribrain-1.0.4.tar", last modified: Tue Apr 23 08:53:07 2024, max compression
+gzip compressed data, was "dist/bribrain-1.0.5.tar", last modified: Tue May 28 07:16:02 2024, max compression
```

## Comparing `bribrain-1.0.4.tar` & `bribrain-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 cdsw      (8536) cdsw      (8536)        0 2024-04-23 08:53:07.000000 bribrain-1.0.4/
-drwxr-xr-x   0 cdsw      (8536) cdsw      (8536)        0 2024-04-23 08:53:07.000000 bribrain-1.0.4/bribrain/
--rwx------   0 cdsw      (8536) cdsw      (8536)       90 2024-04-23 08:42:53.000000 bribrain-1.0.4/bribrain/__init__.py
--rwx------   0 cdsw      (8536) cdsw      (8536)     2456 2024-04-23 08:42:53.000000 bribrain-1.0.4/bribrain/config.py
--rwx------   0 cdsw      (8536) cdsw      (8536)     4330 2024-04-23 08:42:53.000000 bribrain-1.0.4/bribrain/function.py
--rwx------   0 cdsw      (8536) cdsw      (8536)    81374 2024-04-23 08:52:31.000000 bribrain-1.0.4/bribrain/ingestion.py
--rwx------   0 cdsw      (8536) cdsw      (8536)    16561 2024-04-23 08:42:53.000000 bribrain-1.0.4/bribrain/load.py
-drwxr-xr-x   0 cdsw      (8536) cdsw      (8536)        0 2024-04-23 08:53:07.000000 bribrain-1.0.4/bribrain.egg-info/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      460 2024-04-23 08:53:07.000000 bribrain-1.0.4/bribrain.egg-info/PKG-INFO
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      267 2024-04-23 08:53:07.000000 bribrain-1.0.4/bribrain.egg-info/SOURCES.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2024-04-23 08:53:07.000000 bribrain-1.0.4/bribrain.egg-info/dependency_links.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       40 2024-04-23 08:53:07.000000 bribrain-1.0.4/bribrain.egg-info/requires.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        9 2024-04-23 08:53:07.000000 bribrain-1.0.4/bribrain.egg-info/top_level.txt
--rwx------   0 cdsw      (8536) cdsw      (8536)      647 2024-04-23 08:52:51.000000 bribrain-1.0.4/setup.py
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      460 2024-04-23 08:53:07.000000 bribrain-1.0.4/PKG-INFO
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       38 2024-04-23 08:53:07.000000 bribrain-1.0.4/setup.cfg
+drwxr-xr-x   0 cdsw      (8536) cdsw      (8536)        0 2024-05-28 07:16:02.000000 bribrain-1.0.5/
+drwxr-xr-x   0 cdsw      (8536) cdsw      (8536)        0 2024-05-28 07:16:02.000000 bribrain-1.0.5/bribrain/
+-rwx------   0 cdsw      (8536) cdsw      (8536)       90 2024-04-23 08:42:53.000000 bribrain-1.0.5/bribrain/__init__.py
+-rwx------   0 cdsw      (8536) cdsw      (8536)     2632 2024-05-28 06:58:16.000000 bribrain-1.0.5/bribrain/config.py
+-rwx------   0 cdsw      (8536) cdsw      (8536)     4330 2024-04-23 08:42:53.000000 bribrain-1.0.5/bribrain/function.py
+-rwx------   0 cdsw      (8536) cdsw      (8536)    81374 2024-04-23 08:52:31.000000 bribrain-1.0.5/bribrain/ingestion.py
+-rwx------   0 cdsw      (8536) cdsw      (8536)    16599 2024-05-28 07:08:44.000000 bribrain-1.0.5/bribrain/load.py
+drwxr-xr-x   0 cdsw      (8536) cdsw      (8536)        0 2024-05-28 07:16:02.000000 bribrain-1.0.5/bribrain.egg-info/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      458 2024-05-28 07:16:01.000000 bribrain-1.0.5/bribrain.egg-info/PKG-INFO
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      267 2024-05-28 07:16:01.000000 bribrain-1.0.5/bribrain.egg-info/SOURCES.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2024-05-28 07:16:01.000000 bribrain-1.0.5/bribrain.egg-info/dependency_links.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       40 2024-05-28 07:16:01.000000 bribrain-1.0.5/bribrain.egg-info/requires.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        9 2024-05-28 07:16:01.000000 bribrain-1.0.5/bribrain.egg-info/top_level.txt
+-rwx------   0 cdsw      (8536) cdsw      (8536)      620 2024-05-28 07:15:27.000000 bribrain-1.0.5/setup.py
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      458 2024-05-28 07:16:02.000000 bribrain-1.0.5/PKG-INFO
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       38 2024-05-28 07:16:02.000000 bribrain-1.0.5/setup.cfg
```

### Comparing `bribrain-1.0.4/bribrain/config.py` & `bribrain-1.0.5/bribrain/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ###  UPDATED AT     : 07 MARET 2024                         ###
 ###  COPYRIGHT      : ANDRI ARIYANTO                        ###
 ###  DESCRIPTION    : Module untuk pembuatan spark session  ###
 #=============================================================#
 
 from pyspark.sql import SparkSession
 
-def sparkSession(appname="Bribrain Spark Session", executor="small", instances=2, cores=4, memory=4, overhead=2):
+def sparkSession(appname="Bribrain Spark Session", executor="small", instances=2, cores=4, memory=4, overhead=2, verbose=True):
   """Membuat spark session yang dapat digunakan untuk proses data engineering
 
   Args:
       appname (str): Nama dari spark session
           (default is Bribrain Spark Session)
       executor (str): Standard resource yang dapat dipilih untuk spark session 
           (optional is small, medium, high, custom)
@@ -21,14 +21,16 @@
           (default is 2)
       cores (int): Config untuk menentukan cores spark session
           (default is 4)
       memory (int): Config untuk menentukan memory spark session
           (default is 4)
       overhead (int): Config untuk menentukan overhead spark session
           (default is 2)
+      verbose (bool): Config untuk menampilkan console progress
+          (default is True)
     
   Returns:
       pyspark.sql.session.SparkSession: Spark session untuk proses data engineering
   """
   
   # pendefinisian resouce pyspark
   if   executor=="small":
@@ -36,25 +38,30 @@
   elif executor=="medium":
     config = [4, 4, 6, 2]
   elif executor=="high":
     config = [6, 5, 8, 4]
   elif executor=="custom":
     config = [instances, cores, memory, overhead]
   
+  if verbose:
+    verbose = "true"
+  elif:
+    verbose = "false"
+    
   # pembuatan spark session
   spark = SparkSession\
     .builder\
     .appName(appname)\
     .config("spark.sql.crossJoin.enabled", "true")\
     .config("spark.dynamicAllocation.enabled", "false")\
     .config("spark.executor.instances", "{}".format(config[0]))\
     .config("spark.executor.cores", "{}".format(config[1]))\
     .config("spark.executor.memory", "{}g".format(config[2]))\
     .config("spark.yarn.executor.memoryOverhead", "{}g".format(config[3]))\
     .config("spark.sql.broadcastTimeout", "36000")\
     .config("spark.sql.legacy.allowCreatingManagedTableUsingNonemptyLocation", "true")\
-    .config("spark.ui.showConsoleProgress", "false")\
+    .config("spark.ui.showConsoleProgress", verbose)\
     .config("spark.network.timeout", 60)\
     .enableHiveSupport()\
     .getOrCreate()
     
   return spark
```

### Comparing `bribrain-1.0.4/bribrain/function.py` & `bribrain-1.0.5/bribrain/function.py`

 * *Files identical despite different names*

### Comparing `bribrain-1.0.4/bribrain/ingestion.py` & `bribrain-1.0.5/bribrain/ingestion.py`

 * *Files identical despite different names*

### Comparing `bribrain-1.0.4/bribrain/load.py` & `bribrain-1.0.5/bribrain/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   """
   
   if schema.startswith("dev"):
     hdfs_path = "/dev/"
   else:
     hdfs_path = "/user/hive/warehouse/"
   
-  print("Write table to Hive: {}.{}".format(schema, table))
+  print("Write table to Hive: {0}.{1}".format(schema, table))
     
   # pengecekan partitioned table
   if partition:
     
     # kondisi ketika tabel berpartisi
     partition = partition.split(",")
     list_partition = df.select(partition).distinct().collect()
@@ -47,107 +47,107 @@
     
     first = True
     row_total = 0
     
     # loop untuk penulisan data per partisi sesuai standard blocksize
     for i, row in enumerate(list_partition):
       
-      condition = ' AND '.join(["{}='{}'".format(col, row[col]) for col in partition])
+      condition = ' AND '.join(["{0}='{1}'".format(col, row[col]) for col in partition])
       df_write = df.filter(condition)
-      
+
 
       if not repartition_number:
         tag = '_'.join([row[col].strip() for col in partition]).lower()
 
-        spark.sql("DROP TABLE IF EXISTS {}.sample_{}_{}".format(schema, table, tag))
+        spark.sql("DROP TABLE IF EXISTS {0}.sample_{1}_{2}".format(schema, table, tag))
 
         # penulisan sample data untuk estimasi ukuran data
         df_write\
           .sample(False,0.1,None)\
           .write\
           .format("parquet")\
           .mode("overwrite")\
-          .saveAsTable("{}.sample_{}_{}".format(schema, table, tag))
+          .saveAsTable("{0}.sample_{1}_{2}".format(schema, table, tag))
 
         # mendapatkan metadata content summary dari sample table
         path = lambda p: spark._jvm.org.apache.hadoop.fs.Path(p)
         fs = spark._jvm.org.apache.hadoop.fs.FileSystem.get(spark._jsc.hadoopConfiguration())
-        hdfs_folder = fs.getContentSummary(path(hdfs_path+"{}.db/sample_{}_{}/".format(schema, table, tag)))
+        hdfs_folder = fs.getContentSummary(path(hdfs_path+"{0}.db/sample_{1}_{2}/".format(schema, table, tag)))
 
         # kalkulasi jumlah file yang optimal sesuai standard blocksize
         blocksize_number = float(hdfs_folder.getLength()*10)/float(blocksize*1024*1024)
         repartition_number = int(1 if blocksize_number < 1 else blocksize_number)
 
-        spark.sql("DROP TABLE {}.sample_{}_{}".format(schema, table, tag))
+        spark.sql("DROP TABLE {0}.sample_{1}_{2}".format(schema, table, tag))
 
       # set jumlah file sesuai hasil kalkulasi
       df_write = df_write.repartition(repartition_number)
     
       # penghapusan data partisi jika sudah ada di target tabel
-      if spark.sql("SHOW TABLES IN {} LIKE '{}'".format(schema, table)).count() != 0:
-        query_drop_partition = "ALTER TABLE {}.{} DROP IF EXISTS PARTITION({})".format(schema, table, condition.replace(" AND ",","))
+      if spark.sql("SHOW TABLES IN {0} LIKE '{1}'".format(schema, table)).count() != 0:
+        query_drop_partition = "ALTER TABLE {0}.{1} DROP IF EXISTS PARTITION({2})".format(schema, table, condition.replace(" AND ",","))
         spark.sql(query_drop_partition) # menghapus partisi di spark
 
       # penulisan pyspark dataframe ke hdfs
       df_write\
         .write\
         .format("parquet")\
         .partitionBy(partition)\
         .mode(mode)\
-        .saveAsTable("{}.{}".format(schema,table))
+        .saveAsTable("{0}.{1}".format(schema,table))
 
-      spark.sql("MSCK REPAIR TABLE {}.{}".format(schema, table)) # memperbaiki tabel
-      spark.sql("ANALYZE TABLE {}.{} PARTITION ({}) COMPUTE STATISTICS".format(schema, table, condition.replace(" AND ",","))) # kalkulasi data
-      spark.sql("REFRESH TABLE {}.{}".format(schema, table)) # refresh tabel di spark
+      spark.sql("MSCK REPAIR TABLE {0}.{1}".format(schema, table)) # memperbaiki tabel
+      spark.sql("ANALYZE TABLE {0}.{1} PARTITION ({2}) COMPUTE STATISTICS".format(schema, table, condition.replace(" AND ",","))) # kalkulasi data
+      spark.sql("REFRESH TABLE {0}.{1}".format(schema, table)) # refresh tabel di spark
       
 
       first = False
       if not first: mode="append"
         
       row_count = df_write.count()
       row_total += row_count
-      print("{}) Count Record ({}) = {}".format(str(i+1).ljust(unit, " "), condition.replace(" AND ",","), row_count))
+      print("{0}) Count Record ({1}) = {2}".format(str(i+1).ljust(unit, " "), condition.replace(" AND ",","), row_count))
 
   else:
     
     if not repartition_number:
       # kondisi ketika tabel berpartisi    
-      spark.sql("DROP TABLE IF EXISTS {}.sample_{}".format(schema, table))
+      spark.sql("DROP TABLE IF EXISTS {0}.sample_{1}".format(schema, table))
 
       # penulisan sample data untuk estimasi ukuran data
       df\
         .sample(False,0.1,None)\
         .write\
         .format("parquet")\
         .mode("overwrite")\
-        .saveAsTable("{}.sample_{}".format(schema, table))
+        .saveAsTable("{0}.sample_{1}".format(schema, table))
 
       # mendapatkan metadata content summary dari sample table
       path = lambda p: spark._jvm.org.apache.hadoop.fs.Path(p)
       fs = spark._jvm.org.apache.hadoop.fs.FileSystem.get(spark._jsc.hadoopConfiguration())
-      hdfs_folder = fs.getContentSummary(path(hdfs_path+"{}.db/sample_{}_{}/".format(schema, table)))
+      hdfs_folder = fs.getContentSummary(path(hdfs_path+"{0}.db/sample_{1}/".format(schema, table)))
 
       # kalkulasi jumlah file yang optimal sesuai standard blocksize
       blocksize_number = float(hdfs_folder.getLength()*10)/float(blocksize*1024*1024)
       repartition_number = int(1 if blocksize_number < 1 else blocksize_number)
 
-      spark.sql("DROP TABLE {}.sample_{}".format(schema, table))
+      spark.sql("DROP TABLE {0}.sample_{1}".format(schema, table))
 
     # set jumlah file sesuai hasil kalkulasi
     df = df.repartition(repartition_number)
 
     # penulisan pyspark dataframe ke hdfs
     df\
       .write\
       .format("parquet")\
       .mode(mode)\
-      .saveAsTable("{}.{}".format(schema,table))
+      .saveAsTable("{0}.{1}".format(schema,table))
 
-    spark.sql("ANALYZE TABLE {}.{} COMPUTE STATISTICS".format(schema, table)) # kalkulasi data
-    spark.sql("REFRESH TABLE {}.{}".format(schema, table)) # refresh tabel di spark
+    spark.sql("ANALYZE TABLE {0}.{1} COMPUTE STATISTICS".format(schema, table)) # kalkulasi data
+    spark.sql("REFRESH TABLE {0}.{1}".format(schema, table)) # refresh tabel di spark
     
 
   print("\n====>> Grand Total Record =", df.count())
```

### Comparing `bribrain-1.0.4/setup.py` & `bribrain-1.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.4'
-DESCRIPTION = 'Standard code for Dept BRIBrain'
+VERSION = '1.0.5'
 
 # Setting up
+
 setup(
     name="bribrain",
     version=VERSION,
     author="Andri Ariyanto",
     author_email="ariyant.andri@gmail.com",
-    description=DESCRIPTION,
+    description="Standard code for Dept BRIBrain",
     packages=find_packages(),
     install_requires=['mysql-connector-python==8.0.28', 'psycopg2'],
-    keywords=['python', 'ddb', 'bribrain', 'andri', 'gondrol'],
+    keywords=['python', 'ddb', 'dbb', 'bribrain', 'gondrol'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

