# Comparing `tmp/google-csv-helper-1.2.3.tar.gz` & `tmp/google_csv_helper-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-csv-helper-1.2.3.tar", last modified: Fri Feb  2 15:02:39 2024, max compression
+gzip compressed data, was "google_csv_helper-1.2.4.tar", last modified: Wed May 29 15:19:14 2024, max compression
```

## Comparing `google-csv-helper-1.2.3.tar` & `google_csv_helper-1.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:02:39.753010 google-csv-helper-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-02 15:02:31.000000 google-csv-helper-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-02-02 15:02:39.753010 google-csv-helper-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-02-02 15:02:31.000000 google-csv-helper-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:02:39.749010 google-csv-helper-1.2.3/google_csv_helper/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-02 15:02:31.000000 google-csv-helper-1.2.3/google_csv_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-02-02 15:02:31.000000 google-csv-helper-1.2.3/google_csv_helper/adsense_csv_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-02-02 15:02:31.000000 google-csv-helper-1.2.3/google_csv_helper/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-02-02 15:02:31.000000 google-csv-helper-1.2.3/google_csv_helper/csv_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    16332 2024-02-02 15:02:31.000000 google-csv-helper-1.2.3/google_csv_helper/csv_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-02-02 15:02:31.000000 google-csv-helper-1.2.3/google_csv_helper/ga3_csv_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-02-02 15:02:31.000000 google-csv-helper-1.2.3/google_csv_helper/ga4_csv_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-02-02 15:02:31.000000 google-csv-helper-1.2.3/google_csv_helper/google_common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:02:39.753010 google-csv-helper-1.2.3/google_csv_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-02-02 15:02:39.000000 google-csv-helper-1.2.3/google_csv_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-02-02 15:02:39.000000 google-csv-helper-1.2.3/google_csv_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 15:02:39.000000 google-csv-helper-1.2.3/google_csv_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-02 15:02:39.000000 google-csv-helper-1.2.3/google_csv_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-02 15:02:39.000000 google-csv-helper-1.2.3/google_csv_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-02 15:02:39.000000 google-csv-helper-1.2.3/google_csv_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-02 15:02:39.753010 google-csv-helper-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-02-02 15:02:31.000000 google-csv-helper-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:19:14.601137 google_csv_helper-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-29 15:19:03.000000 google_csv_helper-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-05-29 15:19:14.601137 google_csv_helper-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-29 15:19:03.000000 google_csv_helper-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:19:14.597137 google_csv_helper-1.2.4/google_csv_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-29 15:19:03.000000 google_csv_helper-1.2.4/google_csv_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-05-29 15:19:03.000000 google_csv_helper-1.2.4/google_csv_helper/adsense_csv_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11673 2024-05-29 15:19:03.000000 google_csv_helper-1.2.4/google_csv_helper/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-29 15:19:03.000000 google_csv_helper-1.2.4/google_csv_helper/csv_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16332 2024-05-29 15:19:03.000000 google_csv_helper-1.2.4/google_csv_helper/csv_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-29 15:19:03.000000 google_csv_helper-1.2.4/google_csv_helper/ga3_csv_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-05-29 15:19:03.000000 google_csv_helper-1.2.4/google_csv_helper/ga4_csv_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-05-29 15:19:03.000000 google_csv_helper-1.2.4/google_csv_helper/google_common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:19:14.601137 google_csv_helper-1.2.4/google_csv_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-05-29 15:19:14.000000 google_csv_helper-1.2.4/google_csv_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 15:19:14.000000 google_csv_helper-1.2.4/google_csv_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:19:14.000000 google_csv_helper-1.2.4/google_csv_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-29 15:19:14.000000 google_csv_helper-1.2.4/google_csv_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-29 15:19:14.000000 google_csv_helper-1.2.4/google_csv_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 15:19:14.000000 google_csv_helper-1.2.4/google_csv_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 15:19:14.601137 google_csv_helper-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-29 15:19:03.000000 google_csv_helper-1.2.4/setup.py
```

### Comparing `google-csv-helper-1.2.3/LICENSE` & `google_csv_helper-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `google-csv-helper-1.2.3/google_csv_helper/adsense_csv_helper.py` & `google_csv_helper-1.2.4/google_csv_helper/ga4_csv_helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,28 +2,26 @@
 
 from google_csv_helper import csv_common
 from google_csv_helper import csv_helper
 
 import pandas
 import datetime
 
-class AdsenseCSVHelper(csv_helper.CSVHelper):
+class GA4CSVHelper(csv_helper.CSVHelper):
     def getDateRangeReport(self, dataframe: pandas.DataFrame, keyFieldName:str, valueFilterBegin:str, valueFilterEnd:str, minmaxDateInputFormat:str, minmaxDateOutputFormat:str ):
         output = {}
         if len(dataframe.index) == 0:
             if self.debugMode:
                 print(f"[WARNING] dataframe is empty.")
             return output
 
         pickedData = dataframe[ (dataframe[keyFieldName] >= valueFilterBegin) & (dataframe[keyFieldName] <= valueFilterEnd) ]
         if len(pickedData.index) == 0:
             if self.debugMode:
-                print(f"[WARNING] dataframe is empty, too. valueFilterBegin: {valueFilterBegin}, valueFilterEnd: {valueFilterEnd}")
-                print(f"dataframe with (dataframe[keyFieldName] >= valueFilterBegin): { dataframe[ (dataframe[keyFieldName] >= valueFilterBegin) ] }")
-                print(f"dataframe with (dataframe[keyFieldName] <= valueFilterEnd): { dataframe[ (dataframe[keyFieldName] <= valueFilterEnd) ] }")
+                print(f"[WARNING] dataframe is empty, too")
             return output
 
         maxRow = pickedData[ pickedData['Estimated earnings (USD)'] == pickedData['Estimated earnings (USD)'].max() ]
         minRow = pickedData[ pickedData['Estimated earnings (USD)'] == pickedData['Estimated earnings (USD)'].min() ]
 
         maxRowDateInfo = datetime.datetime.strftime(datetime.datetime.strptime(maxRow.iloc[0][keyFieldName], minmaxDateInputFormat), minmaxDateOutputFormat)
         minRowDateInfo = datetime.datetime.strftime(datetime.datetime.strptime(minRow.iloc[0][keyFieldName], minmaxDateInputFormat), minmaxDateOutputFormat)
@@ -106,15 +104,15 @@
                 if self.debugMode:
                     print(f"Skip by checking columns['Date']['Date']: {target}")
                 continue
             if 'Estimated earnings (USD)' not in v["Date"].columns:
                 if self.debugMode:
                     print(f"Skip by checking columns['Date']['Estimated earnings (USD)']: {target}")
                 continue
-
+    
             prevItemInfo = self.getDateRangeReport(v["Date"], 'Date', prevDateFilterBegin, prevDateFilterEnd, '%Y-%m-%d', '%m/%d %a')
             item = self.getDateRangeReport(v["Date"], 'Date', DateFilterBegin, DateFilterEnd, '%Y-%m-%d', '%m/%d %a')
     
             compareInfo = {}
             for lookup in csv_common.CSV_OUTPUT_REPORT_COMPARISON_INFO:
                 if lookup not in item or lookup not in prevItemInfo:
                     compareInfo[lookup] = 0
```

### Comparing `google-csv-helper-1.2.3/google_csv_helper/cmd.py` & `google_csv_helper-1.2.4/google_csv_helper/cmd.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,14 +21,17 @@
             except ValueError:
                 raise argparse.ArgumentTypeError(f"not a valid date: {data}")
         return output
     parser = argparse.ArgumentParser()
     parser.add_argument("csv_dir", nargs="*", type=str, help="the directory where the csv file is located")
     parser.add_argument("--output", choices=['json', 'markdown'], default='markdown', help="results format")
     parser.add_argument("--output-type", choices=['adsense', 'ga3', 'ga4'], default="adsense", help="the report")
+    parser.add_argument("--output-chart", type=str, default="", help="draw cumulative average charts for specific columns identified by field names (multiple fields separated by commas)")
+    parser.add_argument("--output-chart-field-candidate", action="store_true", default=False, help="show field name for drawing cumulative average charts")
+    parser.add_argument("--output-chart-config", type=str, default="{}", help="cumulative average chart configuration")
     parser.add_argument("--report", choices=['date', 'week', 'month'], default='date', help="the report type")
     parser.add_argument("--debug", action="store_true", default=False, help="output the debug messages")
     parser.add_argument("--version", action="store_true", default=False, help="show the version")
     parser.add_argument("--enddate", default="today", type=valid_date, help="date for csv key field filter, date format = 'YYYY-mm-dd'")
     parser.add_argument("--adsense-filename-keyword", type=str, default="adsense", help="the keyword on csv filename of adsense")
     parser.add_argument("--admob-filename-keyword", type=str, default="admob", help="the keyword on csv filename of admob")
     parser.add_argument("--ga-filename-keyword", type=str, default="ga", help="the keyword on csv filename of gogle anayltics")
@@ -181,21 +184,43 @@
 
     if args.debug:
         obj.enableDebug()
 
     #obj.setImportCSVDuplicateRules('default', 'last')
     obj.readAllCSVRawFile()
 
+    output_chart = {
+        'config' : { 
+            'height': 10,
+        }, 'columns': {
+        }, 'debug': {
+            'showChartColumnName': args.output_chart_field_candidate,
+        }
+    }
+    if args.output_chart != '':
+        for fieldName in args.output_chart.split(','):
+            fieldName = fieldName.strip()
+            if len(fieldName) == 0:
+                continue
+            output_chart['columns'][fieldName] = fieldName
+    if args.output_chart_config != '' and args.output_chart_config != '{}':
+       try:
+           test_json_value = json.loads(args.output_chart_config)
+           output_chart['config'] = test_json_value
+       except Exception as e:
+           if args.debug:
+               print(e)
+
     if args.output == 'markdown':
         if args.report == 'date':
             if args.output_type == 'adsense':
                 print("## Current:")
-                print(obj.getDailyMarkDownReport(args.enddate, csv_filename_pattern))
+                print(obj.getDailyMarkDownReport(args.enddate, csv_filename_pattern, output_chart))
                 print("## Previuos:")
-                print(obj.getDailyMarkDownReport(args.enddate.replace(day=1), csv_filename_pattern))
+                print(obj.getDailyMarkDownReport(args.enddate.replace(day=1), csv_filename_pattern, output_chart))
             else:
                 print("## Current:")
                 print(obj.getDailyMarkDownReport(args.enddate, csv_filename_pattern))
                 print("## Previuos:")
                 print(obj.getDailyMarkDownReport(args.enddate - datetime.timedelta(days=7), csv_filename_pattern))
     else:
         if args.report == 'date':
```

### Comparing `google-csv-helper-1.2.3/google_csv_helper/csv_common.py` & `google_csv_helper-1.2.4/google_csv_helper/csv_common.py`

 * *Files identical despite different names*

### Comparing `google-csv-helper-1.2.3/google_csv_helper/csv_helper.py` & `google_csv_helper-1.2.4/google_csv_helper/csv_helper.py`

 * *Files identical despite different names*

### Comparing `google-csv-helper-1.2.3/google_csv_helper/ga3_csv_helper.py` & `google_csv_helper-1.2.4/google_csv_helper/ga3_csv_helper.py`

 * *Files identical despite different names*

### Comparing `google-csv-helper-1.2.3/google_csv_helper/ga4_csv_helper.py` & `google_csv_helper-1.2.4/google_csv_helper/adsense_csv_helper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # -*- encoding: utf-8 -*-
 
 from google_csv_helper import csv_common
 from google_csv_helper import csv_helper
 
 import pandas
 import datetime
+import asciichartpy
 
-class GA4CSVHelper(csv_helper.CSVHelper):
+class AdsenseCSVHelper(csv_helper.CSVHelper):
     def getDateRangeReport(self, dataframe: pandas.DataFrame, keyFieldName:str, valueFilterBegin:str, valueFilterEnd:str, minmaxDateInputFormat:str, minmaxDateOutputFormat:str ):
-        output = {}
+        output = { 'raw': None }
         if len(dataframe.index) == 0:
             if self.debugMode:
                 print(f"[WARNING] dataframe is empty.")
             return output
 
         pickedData = dataframe[ (dataframe[keyFieldName] >= valueFilterBegin) & (dataframe[keyFieldName] <= valueFilterEnd) ]
         if len(pickedData.index) == 0:
             if self.debugMode:
-                print(f"[WARNING] dataframe is empty, too")
+                print(f"[WARNING] dataframe is empty, too. valueFilterBegin: {valueFilterBegin}, valueFilterEnd: {valueFilterEnd}")
+                print(f"dataframe with (dataframe[keyFieldName] >= valueFilterBegin): { dataframe[ (dataframe[keyFieldName] >= valueFilterBegin) ] }")
+                print(f"dataframe with (dataframe[keyFieldName] <= valueFilterEnd): { dataframe[ (dataframe[keyFieldName] <= valueFilterEnd) ] }")
             return output
 
         maxRow = pickedData[ pickedData['Estimated earnings (USD)'] == pickedData['Estimated earnings (USD)'].max() ]
         minRow = pickedData[ pickedData['Estimated earnings (USD)'] == pickedData['Estimated earnings (USD)'].min() ]
 
         maxRowDateInfo = datetime.datetime.strftime(datetime.datetime.strptime(maxRow.iloc[0][keyFieldName], minmaxDateInputFormat), minmaxDateOutputFormat)
         minRowDateInfo = datetime.datetime.strftime(datetime.datetime.strptime(minRow.iloc[0][keyFieldName], minmaxDateInputFormat), minmaxDateOutputFormat)
@@ -30,14 +33,16 @@
         output['Average earnings (USD)'] = pickedData['Estimated earnings (USD)'].mean()
         output['Average CPC'] = pickedData['Estimated earnings (USD)'].sum() / pickedData['Clicks'].sum()
         output['Average Impressions'] = pickedData['Impressions'].mean()
         output['Lowest earnings'] = minRow['Estimated earnings (USD)'].sum()
         output['Lowest earnings info'] = minRowDateInfo
         output['Highest earnings'] = maxRow['Estimated earnings (USD)'].sum()
         output['Highest earnings info'] = maxRowDateInfo
+
+        output['raw'] = pickedData
         
         return output
 
     def getDailySummaryReport(self, pickedDate: datetime.date, pickedReportKeyword: list[str]):
         output = {
             "input": {
                 "pickedDate": pickedDate,
@@ -60,14 +65,16 @@
                     ],
                     "data": [],
                     "total": {
                         "Cumulative Revenue": 0.0,
                         "Average Daily Revenue": 0.0,
                     },
                 },
+                "raw": {
+                }
             },
         }
 
         today = pickedDate
         if today.day == 1:
             today = today - datetime.timedelta(days=1)
             DateFilterBegin = f"{today.replace(day=1)}"
@@ -104,17 +111,18 @@
                 if self.debugMode:
                     print(f"Skip by checking columns['Date']['Date']: {target}")
                 continue
             if 'Estimated earnings (USD)' not in v["Date"].columns:
                 if self.debugMode:
                     print(f"Skip by checking columns['Date']['Estimated earnings (USD)']: {target}")
                 continue
-    
+
             prevItemInfo = self.getDateRangeReport(v["Date"], 'Date', prevDateFilterBegin, prevDateFilterEnd, '%Y-%m-%d', '%m/%d %a')
             item = self.getDateRangeReport(v["Date"], 'Date', DateFilterBegin, DateFilterEnd, '%Y-%m-%d', '%m/%d %a')
+            output["output"]["raw"][target] = [ item["raw"], prevItemInfo["raw"] ]
     
             compareInfo = {}
             for lookup in csv_common.CSV_OUTPUT_REPORT_COMPARISON_INFO:
                 if lookup not in item or lookup not in prevItemInfo:
                     compareInfo[lookup] = 0
                     continue
                 compareInfo[lookup] = (item[lookup] - prevItemInfo[lookup]) * 100 / prevItemInfo[lookup]
@@ -136,24 +144,57 @@
             if 'Estimated earnings (USD)' in item:
                 output["output"]["csv"]["total"]["Cumulative Revenue"] += item['Estimated earnings (USD)']
             if 'Average earnings (USD)' in item:
                 output["output"]["csv"]["total"]["Average Daily Revenue"] += item['Average earnings (USD)']
 
         return output
 
-    def getDailyMarkDownReport(self, pickedDate: datetime.date, pickedReportKeyword: list[str]) -> str:
+    def getDailyMarkDownReport(self, pickedDate: datetime.date, pickedReportKeyword: list[str], charts: dict = {}) -> str:
         data = self.getDailySummaryReport(pickedDate, pickedReportKeyword)
 
         output = [ 
             f"### Date Range: {data['output']['date']['duration']['begin']} ~ {data['output']['date']['duration']['end']}",
             f"#### Compare to previous period: {data['output']['date']['previous']['begin']} ~ {data['output']['date']['previous']['end']}",
             f"| Item | Cumulative Revenue | Average Daily Revenue | Average CPC | Min Daily Revenue | Max Daily Revenue ",
             f"| -- | --: | --: | --: | --: | --: ",
         ]
 
         for item in data["output"]["csv"]["data"]:
             output.append( f"| {item[0]} | {item[1]:,.2f} | {item[3]:,.2f} ({item[4]:.2f}%) | {item[5]:.4f} ({item[6]:.2f}%) | {item[7]:,.2f} [{item[8]}] | {item[9]:,.2f} [{item[10]}] " )
 
         output.append( f"| Total | {data['output']['csv']['total']['Cumulative Revenue']:,.2f} | {data['output']['csv']['total']['Average Daily Revenue']:,.2f} | | | ")
 
-        return "\n".join(output)
+        #charts = {
+        #    'config': {'height': 10},
+        #    'columns': {
+        #        'Estimated earnings (USD)': 'Estimated earnings (USD)',
+        #        'CPC (USD)': 'CPC (USD)',
+        #    }, 'debug': {
+        #        'showColumns': False
+        #    }
+        #}
+        if 'config' in charts and 'columns' in charts and len(charts['columns']) > 0:
+            output.append("#### ref")
+            chartsConfig = charts['config']
+            chartsOutput = charts['columns']
+            for selectedColumn, outputColumn in chartsOutput.items():
+                for k, v in data['output']['raw'].items():
+                    if len(v) == 0 or not isinstance(v[0], pandas.DataFrame):
+                        continue
+                    selectedDataFrame = v[0]
+                    if 'debug' in charts and 'showChartColumnName' in charts['debug'] and charts['debug']['showChartColumnName']:
+                        print(f"[INFO] {k} field name for drawing chart: {selectedDataFrame.columns.to_list()}")
+                    for selectedColumn in chartsOutput.keys():
+                        if selectedColumn not in selectedDataFrame.columns:
+                            continue
+                        #targetValues = list(selectedDataFrame[selectedColumn])
+                        #avgValues = []
+                        #for i in range(len(targetValues)):
+                        #    avgValues.append(sum(targetValues[0:i+1])/(i+1) if i > 0 else targetValues[i])
+                        avgValues = selectedDataFrame[selectedColumn].expanding().mean().tolist()
+
+                        output.append(f"##### {k} - Cumulative Average of '{selectedColumn}' Chart:")
+                        output.append("```")
+                        output.append(asciichartpy.plot(avgValues, cfg=chartsConfig))
+                        output.append("```")
 
+        return "\n".join(output)
```

### Comparing `google-csv-helper-1.2.3/google_csv_helper/google_common.py` & `google_csv_helper-1.2.4/google_csv_helper/google_common.py`

 * *Files identical despite different names*

### Comparing `google-csv-helper-1.2.3/google_csv_helper.egg-info/SOURCES.txt` & `google_csv_helper-1.2.4/google_csv_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-csv-helper-1.2.3/setup.py` & `google_csv_helper-1.2.4/setup.py`

 * *Files identical despite different names*

