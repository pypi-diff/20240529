# Comparing `tmp/ci_cloudconnector-0.93.tar.gz` & `tmp/ci_cloudconnector-0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ci_cloudconnector-0.93.tar", last modified: Tue May 28 10:05:27 2024, max compression
+gzip compressed data, was "ci_cloudconnector-0.94.tar", last modified: Wed May 29 18:21:08 2024, max compression
```

## Comparing `ci_cloudconnector-0.93.tar` & `ci_cloudconnector-0.94.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 10:05:27.824685 ci_cloudconnector-0.93/
-drwxrwxrwx   0        0        0        0 2024-05-28 10:05:27.817885 ci_cloudconnector-0.93/CI_CloudConnector.egg-info/
--rw-rw-rw-   0        0        0      358 2024-05-28 10:05:27.000000 ci_cloudconnector-0.93/CI_CloudConnector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2024-05-28 10:05:27.000000 ci_cloudconnector-0.93/CI_CloudConnector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 10:05:27.000000 ci_cloudconnector-0.93/CI_CloudConnector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-28 10:05:27.000000 ci_cloudconnector-0.93/CI_CloudConnector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      358 2024-05-28 10:05:27.821530 ci_cloudconnector-0.93/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-0.93/README.txt
--rw-rw-rw-   0        0        0    40227 2024-05-28 10:04:58.000000 ci_cloudconnector-0.93/logic.py
--rw-rw-rw-   0        0        0     6030 2024-05-28 09:59:09.000000 ci_cloudconnector-0.93/main.py
--rw-rw-rw-   0        0        0     1856 2024-05-28 09:52:46.000000 ci_cloudconnector-0.93/myservice.py
--rw-rw-rw-   0        0        0       42 2024-05-28 10:05:27.824685 ci_cloudconnector-0.93/setup.cfg
--rw-rw-rw-   0        0        0      791 2024-05-28 10:05:02.000000 ci_cloudconnector-0.93/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:21:08.394905 ci_cloudconnector-0.94/
+drwxrwxrwx   0        0        0        0 2024-05-29 18:21:08.387708 ci_cloudconnector-0.94/CI_CloudConnector.egg-info/
+-rw-rw-rw-   0        0        0      358 2024-05-29 18:21:08.000000 ci_cloudconnector-0.94/CI_CloudConnector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2024-05-29 18:21:08.000000 ci_cloudconnector-0.94/CI_CloudConnector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 18:21:08.000000 ci_cloudconnector-0.94/CI_CloudConnector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-05-29 18:21:08.000000 ci_cloudconnector-0.94/CI_CloudConnector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      358 2024-05-29 18:21:08.391921 ci_cloudconnector-0.94/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-0.94/README.txt
+-rw-rw-rw-   0        0        0    38752 2024-05-29 18:20:51.000000 ci_cloudconnector-0.94/logic.py
+-rw-rw-rw-   0        0        0     8241 2024-05-29 17:52:57.000000 ci_cloudconnector-0.94/main.py
+-rw-rw-rw-   0        0        0     2666 2024-05-29 17:20:02.000000 ci_cloudconnector-0.94/myservice.py
+-rw-rw-rw-   0        0        0       42 2024-05-29 18:21:08.395313 ci_cloudconnector-0.94/setup.cfg
+-rw-rw-rw-   0        0        0      791 2024-05-29 18:20:42.000000 ci_cloudconnector-0.94/setup.py
```

### Comparing `ci_cloudconnector-0.93/logic.py` & `ci_cloudconnector-0.94/logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import logging, time, datetime, sys, os, socket, configparser, random, tzlocal, glob, fnmatch
 import platform
 from datetime import datetime
 
 from cpppo.server.enip import address, client  # for EtherNet/IP communication
 
-VER = "0.93"
+VER = "0.94"
 
 TagsDefenitionFileName = "TagsDefenition.txt"
 TagsValuesFileName = "[NEW]TagsValues"
 TagsValueDir = "TagValues"
 HomeDir = "CI_LC"
 GetTagsFromServerMinRateSeconds = 10
 GetCloudVersionFromServerMinRateSeconds = 10
@@ -70,16 +70,15 @@
         log_handler.setFormatter(log_formatter)
 
         app_logger = logging.getLogger("root")
         app_logger.setLevel(default_log_level)
         app_logger.addHandler(log_handler)
         log_handler.doRollover()
 
-        app_logger.critical("===============================")
-        app_logger.critical("CI_CloudConnector Log Init ::" + VER)
+        app_logger.critical("initialize_log DONE")
         g_app_log = app_logger
 
     except Exception as ex:
         print("Error in initialize_log " +  str(ex))
 
 
 # ============================
@@ -97,18 +96,14 @@
 
 # ============================
 def setLogLevel(lvl):
     try:
         if str(lvl) in ["CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET"]:
             lvl = logging.getLevelName(str(lvl))
 
-        # print 'level=' + str(lvl)
-        if g_app_log:
-            g_app_log.critical("Set Log Level to " + logging.getLevelName(lvl))
-            g_app_log.setLevel(lvl)
     except Exception as inst:
         print("Error in setLogLevel", inst)
 
 
 # ============================
 def ci_print(msg, level=""):
     global g_app_log
@@ -206,15 +201,14 @@
 
             initialize_log(log_level)
 
             ci_print(f"Server Address: {cfg_server_address}", "INFO")
             ci_print(f"Username: {cfg_username}", "INFO")
             ci_print(f"Password: {cfg_password}", "INFO")
             ci_print(f"Max Files: {cfg_max_files}", "INFO")
-            ci_print(f"Logging Level: {log_level} {log_levels_info}", "INFO")
 
         else:
             ci_print(f"Config not found or overwrite is True, creating new one in {file_path}", "INFO")
             config = configparser.ConfigParser()
             config.add_section("Server")
             config.add_section("Logging")
 
@@ -942,15 +936,14 @@
 # ============================
 def getTagsDefenitionFromFile():
 
     try:
         f2 = open(TagsDefenitionFileName, "r")
         tags = json.load(f2)
         f2.close()
-        ci_print("Got " + str(len(tags)) + " Tags From File", "INFO")
         return tags
     except Exception as inst:
         handleError("Error in getTagsDefenitionFromFile", inst)
 
 
 # ============================
 def delTagsDefenitionFile():
@@ -978,25 +971,25 @@
 # ============================
 def saveValuesToFile(values, fileName):
 
     try:
         numOfFiles = len(
             fnmatch.filter(os.listdir("/" + HomeDir + "/" + TagsValueDir), "*.txt")
         )
-        ci_print("Number of files in folder : " + str(numOfFiles), "INFO")
+
         if numOfFiles < 10000:
             if fileName == "":
                 fileName = (
                     TagsValuesFileName
                     + datetime.now().strftime("%Y%m%d-%H%M%S%f")
                     + ".txt"
                 )
             # fileName = "./" + TagsValueDir + '/' + fileName
             fileName = "/" + HomeDir + "/" + TagsValueDir + "/" + fileName
-            ci_print("Start save Values To File " + fileName, "INFO")
+
             # write tags to file
             f = open(fileName, "w")
             json.dump(values, f)
             f.close()
             time.sleep(1)  # prevent two files in same ms
         else:
             ci_print("Too many files in folder!!!", "WARNING")
@@ -1026,26 +1019,21 @@
     try:
         i = 0
         dirpath = "/" + HomeDir + "/" + TagsValueDir + "/"
         filesSortedByTime = [
             s for s in os.listdir(dirpath) if os.path.isfile(os.path.join(dirpath, s))
         ]
         filesSortedByTime.sort(key=lambda s: os.path.getmtime(os.path.join(dirpath, s)))
-        ci_print(
-            "in Dir " + dirpath + " Found " + str(len(filesSortedByTime)) + " files",
-            "INFO",
-        )
+
         for file in filesSortedByTime:
             if file.endswith(".txt") and file.startswith("[NEW]"):
                 i = i + 1
-                ci_print("about to process file:" + file, "INFO")
                 handleValuesFile("/" + HomeDir + "/" + TagsValueDir + "/" + file, token)
 
-        if i > 0:
-            ci_print(str(i) + " Files handled", "INFO")
+
     except Exception as inst:
         ci_print("Error handleAllValuesFiles " + str(inst))
 
 
 # ============================
 def create_directories_if_missing():
     try:
@@ -1117,15 +1105,15 @@
 # Main Loop
 # ============================
 def Main():
 
     global ScanRateLastRead
     global currentToken
     try:
-        ci_print("Loop started at " + str(datetime.now()), "INFO")
+
         if currentToken == "":
             currentToken = get_cloud_token()
         # currently must get tags from cloud to init server before setting values
         tagsDefScanRatesAns = get_cloud_tags(currentToken)
         tagsDefScanRates = tagsDefScanRatesAns["Tags"]
 
         for scanRate in tagsDefScanRates:
@@ -1137,25 +1125,18 @@
             scanRateStr = str(scanRate)
             diff = 0
             if scanRateStr in ScanRateLastRead:
                 now = datetime.now()
                 diff = (now - ScanRateLastRead[scanRateStr]).total_seconds()
                 # print ('diff = -------' + str(diff))
 
-            ci_print("*********************", "INFO")
-            ci_print("diff=" + str(diff) + " scanRateInt=" + str(scanRateInt), "INFO")
 
             if diff + 3 > scanRateInt or diff == 0:
-                ci_print(
-                    "Get Tag Values For Scan Rate "
-                    + str(scanRate)
-                    + " ' time Form Last Run:"
-                    + str(diff)
-                    + " Sec", "INFO"
-                )
+
+
                 tagsDef = tagsDefScanRates[scanRate]
                 arranged_tags = arrange_by_connector_type(tagsDef)
 
                 for connector_type in arranged_tags:
                     print(connector_type)
                     values = None
                     if connector_type == "Simulation":
@@ -1174,33 +1155,30 @@
                                 if values == []:
                                     time.sleep(1)
                                     ci_print("Ethernet Empty values ::2", "ERROR")
                                     values = readEtherNetIP_Tags(arranged_tags[connector_type])
 
                     if len(values) > 0:
                         ci_print(f'VALUE: {values[0]["value"]}, TAGS: {len(values)}', 'INFO')
-                        print(f'SCANRATE: {scanRate}, DIFF: {diff}')
+                        print(f'ScanRate: {scanRate}, DIFF: {diff}')
                     else:
                         ci_print(f'NO VALUES', 'ERROR')
-                        print(f'SCANRATE: {scanRate}, DIFF: {diff}')
+                        print(f'ScanRate: {scanRate}, DIFF: {diff}')
 
                     if values:
                         saveValuesToFile(values, "")
                         removeOldestFile()
 
                         now = datetime.now()
-                        ci_print("SCANRATE TIME UPDATED==>" + str(now), "INFO")
                         ScanRateLastRead[scanRateStr] = now
 
 
         if currentToken != "":
             handleAllValuesFiles(currentToken)
         else:
             ci_print("No Token, skipping upload step", "WARNING")
     except Exception as inst:
         handleError("Error in Main", inst)
         currentToken = ""
 
-    ci_print("===============================", "INFO")
-    ci_print("CI_CloudConnector Ended", "INFO")
```

### Comparing `ci_cloudconnector-0.93/setup.py` & `ci_cloudconnector-0.94/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     return ans
 
 
 
 setup(
     name="CI_CloudConnector",
-    version="0.93",
+    version="0.94",
     packages=find_packages(),
     py_modules=["logic", "main", "setup", "myservice"],
     description="IOT application that collects data from PLC (ModBus or AnB Ethernet/IP) and sends it to the cloud using HTTPS",
     author="Yochai",
     author_email="yochaim@contel.co.il",
     install_requires=[],
     url="https://trunovate.com/",
```

