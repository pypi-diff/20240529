# Comparing `tmp/DatastreamPy-2.0.28-py3-none-any.whl.zip` & `tmp/DatastreamPy-2.0.30-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 51262 bytes, number of entries: 11
+Zip file size: 51333 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat    16190 b- defN 24-May-02 11:26 DatastreamPy/DSConnect.py
--rw-rw-rw-  2.0 fat    22949 b- defN 24-May-21 09:47 DatastreamPy/DSUserDataObjectBase.py
+-rw-rw-rw-  2.0 fat    22949 b- defN 24-May-23 17:36 DatastreamPy/DSUserDataObjectBase.py
 -rw-rw-rw-  2.0 fat     5633 b- defN 24-May-02 11:26 DatastreamPy/DS_Requests.py
--rw-rw-rw-  2.0 fat    27581 b- defN 24-May-21 09:43 DatastreamPy/DS_Response.py
+-rw-rw-rw-  2.0 fat    27746 b- defN 24-May-23 17:25 DatastreamPy/DS_Response.py
 -rw-rw-rw-  2.0 fat    60200 b- defN 24-May-02 11:26 DatastreamPy/DatastreamEconomicFilters.py
 -rw-rw-rw-  2.0 fat    52895 b- defN 24-May-02 11:26 DatastreamPy/DatastreamUserCreated_TimeSeries.py
 -rw-rw-rw-  2.0 fat     1041 b- defN 24-May-02 11:26 DatastreamPy/__init__.py
--rw-rw-rw-  2.0 fat    27395 b- defN 24-May-21 09:47 DatastreamPy-2.0.28.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-21 09:47 DatastreamPy-2.0.28.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-May-21 09:47 DatastreamPy-2.0.28.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      955 b- defN 24-May-21 09:47 DatastreamPy-2.0.28.dist-info/RECORD
-11 files, 214944 bytes uncompressed, 49644 bytes compressed:  76.9%
+-rw-rw-rw-  2.0 fat    27395 b- defN 24-May-23 17:39 DatastreamPy-2.0.30.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-23 17:39 DatastreamPy-2.0.30.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-May-23 17:39 DatastreamPy-2.0.30.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      955 b- defN 24-May-23 17:39 DatastreamPy-2.0.30.dist-info/RECORD
+11 files, 215109 bytes uncompressed, 49715 bytes compressed:  76.9%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: DatastreamPy/DatastreamUserCreated_TimeSeries.py
 Comment: 
 
 Filename: DatastreamPy/__init__.py
 Comment: 
 
-Filename: DatastreamPy-2.0.28.dist-info/METADATA
+Filename: DatastreamPy-2.0.30.dist-info/METADATA
 Comment: 
 
-Filename: DatastreamPy-2.0.28.dist-info/WHEEL
+Filename: DatastreamPy-2.0.30.dist-info/WHEEL
 Comment: 
 
-Filename: DatastreamPy-2.0.28.dist-info/top_level.txt
+Filename: DatastreamPy-2.0.30.dist-info/top_level.txt
 Comment: 
 
-Filename: DatastreamPy-2.0.28.dist-info/RECORD
+Filename: DatastreamPy-2.0.30.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## DatastreamPy/DSUserDataObjectBase.py

```diff
@@ -20,15 +20,15 @@
 from enum import IntEnum
 import pytz
 import json
 import re
 from datetime import datetime, timedelta, date
 
 class DSPackageInfo:
-    buildVer = '2.0.28'
+    buildVer = '2.0.30'
     appId = 'DatastreamPy-' + buildVer
     UserAgent = ' DatastreamPy/' + buildVer
 
 class DSUserObjectFault(Exception):
     """
     DSUserObjectFault exception is a representation of the DSFault error returned from the API server.
     DSFaults are returned for the following reasons:
```

## DatastreamPy/DS_Response.py

```diff
@@ -1612,113 +1612,124 @@
 000064b0: 662e 5f67 6574 5f44 6174 6174 7970 6556  f._get_DatatypeV
 000064c0: 616c 7565 7328 7265 7370 6f6e 7365 5f6a  alues(response_j
 000064d0: 736f 6e29 0d0a 2020 2020 2020 2020 6966  son)..        if
 000064e0: 2028 6c65 6e28 6461 7465 735f 636f 6e76   (len(dates_conv
 000064f0: 6572 7465 6429 203d 3d20 6c65 6e28 6461  erted) == len(da
 00006500: 7461 6672 616d 652e 696e 6465 7829 293a  taframe.index)):
 00006510: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
-00006520: 7461 6672 616d 652e 696e 6465 782e 6e61  taframe.index.na
-00006530: 6d65 203d 2027 4461 7465 7327 0d0a 2020  me = 'Dates'..  
-00006540: 2020 2020 2020 2020 2020 6461 7461 6672            datafr
-00006550: 616d 652e 696e 6465 7820 3d20 6461 7465  ame.index = date
-00006560: 735f 636f 6e76 6572 7465 640d 0a20 2020  s_converted..   
+00006520: 7461 6672 616d 652e 696e 6465 7820 3d20  taframe.index = 
+00006530: 6461 7465 735f 636f 6e76 6572 7465 640d  dates_converted.
+00006540: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+00006550: 6166 7261 6d65 2e69 6e64 6578 2e6e 616d  aframe.index.nam
+00006560: 6520 3d20 2744 6174 6573 270d 0a20 2020  e = 'Dates'..   
 00006570: 2020 2020 2065 6c69 6620 286c 656e 2864       elif (len(d
 00006580: 6174 6573 5f63 6f6e 7665 7274 6564 2920  ates_converted) 
 00006590: 3d3d 2031 293a 0d0a 2020 2020 2020 2020  == 1):..        
 000065a0: 2020 2020 6461 7461 6672 616d 655b 2744      dataframe['D
 000065b0: 6174 6573 275d 203d 2064 6174 6573 5f63  ates'] = dates_c
-000065c0: 6f6e 7665 7274 6564 5b30 5d0d 0a20 2020  onverted[0]..   
-000065d0: 2020 2020 2020 2020 2069 6620 286c 656e           if (len
-000065e0: 2864 6174 6166 7261 6d65 2e69 6e64 6578  (dataframe.index
-000065f0: 2920 3e20 6c65 6e28 6461 7465 735f 636f  ) > len(dates_co
-00006600: 6e76 6572 7465 6429 293a 0d0a 2020 2020  nverted)):..    
-00006610: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00006620: 6672 616d 652e 696e 6465 7820 3d20 6461  frame.index = da
-00006630: 7461 6672 616d 655b 2744 6174 6573 275d  taframe['Dates']
-00006640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006650: 2020 6461 7461 6672 616d 6520 3d20 6461    dataframe = da
-00006660: 7461 6672 616d 652e 6472 6f70 2863 6f6c  taframe.drop(col
-00006670: 756d 6e73 3d27 4461 7465 7327 2c20 6178  umns='Dates', ax
-00006680: 6973 203d 2031 290d 0a20 2020 2020 2020  is = 1)..       
-00006690: 200d 0a20 2020 2020 2020 200d 0a20 2020   ..        ..   
-000066a0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-000066b0: 2020 2023 2020 2020 6966 2028 6c65 6e28     #    if (len(
-000066c0: 6461 7465 735f 636f 6e76 6572 7465 6429  dates_converted)
-000066d0: 203e 2031 293a 0d0a 2020 2020 2020 2020   > 1):..        
-000066e0: 2320 2020 2020 2020 2023 6461 7461 6672  #        #datafr
-000066f0: 616d 652e 696e 7365 7274 286c 6f63 203d  ame.insert(loc =
-00006700: 2030 2c20 636f 6c75 6d6e 203d 2027 4461   0, column = 'Da
-00006710: 7465 7327 2c20 7661 6c75 6520 3d20 6461  tes', value = da
-00006720: 7465 735f 636f 6e76 6572 7465 6429 0d0a  tes_converted)..
-00006730: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-00006740: 2064 6174 6166 7261 6d65 2e69 6e64 6578   dataframe.index
-00006750: 203d 2064 6174 6573 5f63 6f6e 7665 7274   = dates_convert
-00006760: 6564 0d0a 2020 2020 2020 2020 2320 2020  ed..        #   
-00006770: 2020 2020 2064 6174 6166 7261 6d65 2e69       dataframe.i
-00006780: 6e64 6578 2e6e 616d 6520 3d20 2744 6174  ndex.name = 'Dat
-00006790: 6573 270d 0a20 2020 2020 2020 2023 656c  es'..        #el
-000067a0: 6966 2028 6c65 6e28 6461 7465 735f 636f  if (len(dates_co
-000067b0: 6e76 6572 7465 6429 203d 3d20 3129 3a0d  nverted) == 1):.
-000067c0: 0a20 2020 2020 2020 2023 2020 2020 6461  .        #    da
-000067d0: 7461 6672 616d 655b 2744 6174 6573 275d  taframe['Dates']
-000067e0: 203d 2064 6174 6573 5f63 6f6e 7665 7274   = dates_convert
-000067f0: 6564 5b30 5d0d 0a20 2020 2020 2020 200d  ed[0]..        .
-00006800: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00006810: 6461 7461 6672 616d 650d 0a0d 0a20 2020  dataframe....   
-00006820: 2064 6566 205f 666f 726d 6174 5f62 756e   def _format_bun
-00006830: 646c 655f 7265 7370 6f6e 7365 2873 656c  dle_response(sel
-00006840: 662c 7265 7370 6f6e 7365 5f6a 736f 6e29  f,response_json)
-00006850: 3a0d 0a20 2020 2020 2020 2066 6f72 6d61  :..        forma
-00006860: 7474 6564 5265 7370 203d 205b 5d0d 0a20  ttedResp = [].. 
-00006870: 2020 2020 2020 2066 6f72 2065 6163 6844         for eachD
-00006880: 6174 6152 6573 706f 6e73 6520 696e 2072  ataResponse in r
-00006890: 6573 706f 6e73 655f 6a73 6f6e 5b27 4461  esponse_json['Da
-000068a0: 7461 5265 7370 6f6e 7365 7327 5d3a 0d0a  taResponses']:..
-000068b0: 2020 2020 2020 2020 2020 2020 6466 203d              df =
-000068c0: 2073 656c 662e 5f66 6f72 6d61 745f 5265   self._format_Re
-000068d0: 7370 6f6e 7365 2865 6163 6844 6174 6152  sponse(eachDataR
-000068e0: 6573 706f 6e73 6529 0d0a 2020 2020 2020  esponse)..      
-000068f0: 2020 2020 2020 666f 726d 6174 7465 6452        formattedR
-00006900: 6573 702e 6170 7065 6e64 2864 6629 2020  esp.append(df)  
-00006910: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00006920: 200d 0a20 2020 2020 2020 2072 6574 7572   ..        retur
-00006930: 6e20 666f 726d 6174 7465 6452 6573 700d  n formattedResp.
-00006940: 0a20 2020 0d0a 2020 2020 2020 200d 0a20  .   ..       .. 
-00006950: 2020 2064 6566 205f 6765 745f 6d65 7461     def _get_meta
-00006960: 6461 7461 2873 656c 662c 206a 736f 6e52  data(self, jsonR
-00006970: 6573 7029 3a0d 0a20 2020 2020 2020 206e  esp):..        n
-00006980: 616d 6573 203d 207b 7d0d 0a20 2020 2020  ames = {}..     
-00006990: 2020 2069 6620 6a73 6f6e 5265 7370 5b27     if jsonResp['
-000069a0: 5379 6d62 6f6c 4e61 6d65 7327 5d3a 0d0a  SymbolNames']:..
-000069b0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000069c0: 6920 696e 206a 736f 6e52 6573 705b 2753  i in jsonResp['S
-000069d0: 796d 626f 6c4e 616d 6573 275d 3a0d 0a20  ymbolNames']:.. 
-000069e0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000069f0: 616d 6573 2e75 7064 6174 6528 7b69 5b27  ames.update({i['
-00006a00: 4b65 7927 5d3a 2069 5b27 5661 6c75 6527  Key']: i['Value'
-00006a10: 5d7d 290d 0a20 2020 2020 2020 2020 2020  ]})..           
-00006a20: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
-00006a30: 6620 6a73 6f6e 5265 7370 5b27 4461 7461  f jsonResp['Data
-00006a40: 5479 7065 4e61 6d65 7327 5d3a 0d0a 2020  TypeNames']:..  
-00006a50: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
-00006a60: 696e 206a 736f 6e52 6573 705b 2744 6174  in jsonResp['Dat
-00006a70: 6154 7970 654e 616d 6573 275d 3a0d 0a20  aTypeNames']:.. 
-00006a80: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00006a90: 616d 6573 2e75 7064 6174 6528 7b69 5b27  ames.update({i['
-00006aa0: 4b65 7927 5d3a 2069 5b27 5661 6c75 6527  Key']: i['Value'
-00006ab0: 5d7d 290d 0a20 2020 2020 2020 2070 7269  ]})..        pri
-00006ac0: 6e74 286e 616d 6573 290d 0a20 2020 2020  nt(names)..     
-00006ad0: 2020 200d 0a0d 0a20 2020 2064 6566 205f     ....    def _
-00006ae0: 6765 745f 6d65 7461 6461 7461 5f62 756e  get_metadata_bun
-00006af0: 646c 6528 7365 6c66 2c20 6a73 6f6e 5265  dle(self, jsonRe
-00006b00: 7370 293a 0d0a 2020 2020 2020 2020 666f  sp):..        fo
-00006b10: 7220 6561 6368 4461 7461 5265 7370 6f6e  r eachDataRespon
-00006b20: 7365 2069 6e20 6a73 6f6e 5265 7370 3a0d  se in jsonResp:.
-00006b30: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00006b40: 662e 5f67 6574 5f6d 6574 6164 6174 6128  f._get_metadata(
-00006b50: 6561 6368 4461 7461 5265 7370 6f6e 7365  eachDataResponse
-00006b60: 290d 0a23 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  )..#------------
-00006b70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006b80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006b90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006bb0: 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d 0a         ---------....
+000065c0: 6f6e 7665 7274 6564 5b30 5d20 2320 5468  onverted[0] # Th
+000065d0: 6973 2070 6f70 756c 6174 6573 2061 2063  is populates a c
+000065e0: 6f6c 756d 6e20 6e61 6d65 6420 2744 6174  olumn named 'Dat
+000065f0: 6573 2720 7769 7468 2073 696e 676c 6520  es' with single 
+00006600: 4461 7465 2067 6976 656e 200d 0a20 2020  Date given ..   
+00006610: 2020 2020 2020 2020 2064 6174 6166 7261           datafra
+00006620: 6d65 2e69 6e64 6578 203d 2064 6174 6166  me.index = dataf
+00006630: 7261 6d65 5b27 4461 7465 7327 5d20 2320  rame['Dates'] # 
+00006640: 636f 7079 2074 6865 2063 6f6c 756d 6e20  copy the column 
+00006650: 746f 2074 6865 2069 6e64 6578 2063 6f6c  to the index col
+00006660: 756d 6e0d 0a20 2020 2020 2020 2020 2020  umn..           
+00006670: 2064 6174 6166 7261 6d65 2e69 6e64 6578   dataframe.index
+00006680: 2e6e 616d 6520 3d20 2744 6174 6573 2720  .name = 'Dates' 
+00006690: 2320 5468 6973 2077 696c 6c20 7365 7420  # This will set 
+000066a0: 7468 6520 696e 6465 7820 636f 6c75 6d6e  the index column
+000066b0: 206e 616d 6520 746f 2027 4461 7465 7327   name to 'Dates'
+000066c0: 2077 6865 6e20 6466 2069 7320 666f 726d   when df is form
+000066d0: 6564 0d0a 2020 2020 2020 2020 2020 2020  ed..            
+000066e0: 6461 7461 6672 616d 6520 3d20 6461 7461  dataframe = data
+000066f0: 6672 616d 652e 6472 6f70 2863 6f6c 756d  frame.drop(colum
+00006700: 6e73 3d27 4461 7465 7327 2c20 6178 6973  ns='Dates', axis
+00006710: 203d 2031 2920 2320 6472 6f70 2074 6865   = 1) # drop the
+00006720: 206f 6c64 2063 6f6c 756d 6e20 0d0a 2020   old column ..  
+00006730: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00006740: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+00006750: 2020 2020 2020 2020 2320 2020 2069 6620          #    if 
+00006760: 286c 656e 2864 6174 6573 5f63 6f6e 7665  (len(dates_conve
+00006770: 7274 6564 2920 3e20 3129 3a0d 0a20 2020  rted) > 1):..   
+00006780: 2020 2020 2023 2020 2020 2020 2020 2364       #        #d
+00006790: 6174 6166 7261 6d65 2e69 6e73 6572 7428  ataframe.insert(
+000067a0: 6c6f 6320 3d20 302c 2063 6f6c 756d 6e20  loc = 0, column 
+000067b0: 3d20 2744 6174 6573 272c 2076 616c 7565  = 'Dates', value
+000067c0: 203d 2064 6174 6573 5f63 6f6e 7665 7274   = dates_convert
+000067d0: 6564 290d 0a20 2020 2020 2020 2023 2020  ed)..        #  
+000067e0: 2020 2020 2020 6461 7461 6672 616d 652e        dataframe.
+000067f0: 696e 6465 7820 3d20 6461 7465 735f 636f  index = dates_co
+00006800: 6e76 6572 7465 640d 0a20 2020 2020 2020  nverted..       
+00006810: 2023 2020 2020 2020 2020 6461 7461 6672   #        datafr
+00006820: 616d 652e 696e 6465 782e 6e61 6d65 203d  ame.index.name =
+00006830: 2027 4461 7465 7327 0d0a 2020 2020 2020   'Dates'..      
+00006840: 2020 2365 6c69 6620 286c 656e 2864 6174    #elif (len(dat
+00006850: 6573 5f63 6f6e 7665 7274 6564 2920 3d3d  es_converted) ==
+00006860: 2031 293a 0d0a 2020 2020 2020 2020 2320   1):..        # 
+00006870: 2020 2064 6174 6166 7261 6d65 5b27 4461     dataframe['Da
+00006880: 7465 7327 5d20 3d20 6461 7465 735f 636f  tes'] = dates_co
+00006890: 6e76 6572 7465 645b 305d 0d0a 2020 2020  nverted[0]..    
+000068a0: 2020 2020 0d0a 2020 2020 2020 2020 7265      ..        re
+000068b0: 7475 726e 2064 6174 6166 7261 6d65 0d0a  turn dataframe..
+000068c0: 0d0a 2020 2020 6465 6620 5f66 6f72 6d61  ..    def _forma
+000068d0: 745f 6275 6e64 6c65 5f72 6573 706f 6e73  t_bundle_respons
+000068e0: 6528 7365 6c66 2c72 6573 706f 6e73 655f  e(self,response_
+000068f0: 6a73 6f6e 293a 0d0a 2020 2020 2020 2020  json):..        
+00006900: 666f 726d 6174 7465 6452 6573 7020 3d20  formattedResp = 
+00006910: 5b5d 0d0a 2020 2020 2020 2020 666f 7220  []..        for 
+00006920: 6561 6368 4461 7461 5265 7370 6f6e 7365  eachDataResponse
+00006930: 2069 6e20 7265 7370 6f6e 7365 5f6a 736f   in response_jso
+00006940: 6e5b 2744 6174 6152 6573 706f 6e73 6573  n['DataResponses
+00006950: 275d 3a0d 0a20 2020 2020 2020 2020 2020  ']:..           
+00006960: 2064 6620 3d20 7365 6c66 2e5f 666f 726d   df = self._form
+00006970: 6174 5f52 6573 706f 6e73 6528 6561 6368  at_Response(each
+00006980: 4461 7461 5265 7370 6f6e 7365 290d 0a20  DataResponse).. 
+00006990: 2020 2020 2020 2020 2020 2066 6f72 6d61             forma
+000069a0: 7474 6564 5265 7370 2e61 7070 656e 6428  ttedResp.append(
+000069b0: 6466 2920 2020 2020 200d 0a20 2020 2020  df)      ..     
+000069c0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000069d0: 7265 7475 726e 2066 6f72 6d61 7474 6564  return formatted
+000069e0: 5265 7370 0d0a 2020 200d 0a20 2020 2020  Resp..   ..     
+000069f0: 2020 0d0a 2020 2020 6465 6620 5f67 6574    ..    def _get
+00006a00: 5f6d 6574 6164 6174 6128 7365 6c66 2c20  _metadata(self, 
+00006a10: 6a73 6f6e 5265 7370 293a 0d0a 2020 2020  jsonResp):..    
+00006a20: 2020 2020 6e61 6d65 7320 3d20 7b7d 0d0a      names = {}..
+00006a30: 2020 2020 2020 2020 6966 206a 736f 6e52          if jsonR
+00006a40: 6573 705b 2753 796d 626f 6c4e 616d 6573  esp['SymbolNames
+00006a50: 275d 3a0d 0a20 2020 2020 2020 2020 2020  ']:..           
+00006a60: 2066 6f72 2069 2069 6e20 6a73 6f6e 5265   for i in jsonRe
+00006a70: 7370 5b27 5379 6d62 6f6c 4e61 6d65 7327  sp['SymbolNames'
+00006a80: 5d3a 0d0a 2020 2020 2020 2020 2020 2020  ]:..            
+00006a90: 2020 2020 6e61 6d65 732e 7570 6461 7465      names.update
+00006aa0: 287b 695b 274b 6579 275d 3a20 695b 2756  ({i['Key']: i['V
+00006ab0: 616c 7565 275d 7d29 0d0a 2020 2020 2020  alue']})..      
+00006ac0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00006ad0: 2020 2020 6966 206a 736f 6e52 6573 705b      if jsonResp[
+00006ae0: 2744 6174 6154 7970 654e 616d 6573 275d  'DataTypeNames']
+00006af0: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
+00006b00: 6f72 2069 2069 6e20 6a73 6f6e 5265 7370  or i in jsonResp
+00006b10: 5b27 4461 7461 5479 7065 4e61 6d65 7327  ['DataTypeNames'
+00006b20: 5d3a 0d0a 2020 2020 2020 2020 2020 2020  ]:..            
+00006b30: 2020 2020 6e61 6d65 732e 7570 6461 7465      names.update
+00006b40: 287b 695b 274b 6579 275d 3a20 695b 2756  ({i['Key']: i['V
+00006b50: 616c 7565 275d 7d29 0d0a 2020 2020 2020  alue']})..      
+00006b60: 2020 7072 696e 7428 6e61 6d65 7329 0d0a    print(names)..
+00006b70: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+00006b80: 6465 6620 5f67 6574 5f6d 6574 6164 6174  def _get_metadat
+00006b90: 615f 6275 6e64 6c65 2873 656c 662c 206a  a_bundle(self, j
+00006ba0: 736f 6e52 6573 7029 3a0d 0a20 2020 2020  sonResp):..     
+00006bb0: 2020 2066 6f72 2065 6163 6844 6174 6152     for eachDataR
+00006bc0: 6573 706f 6e73 6520 696e 206a 736f 6e52  esponse in jsonR
+00006bd0: 6573 703a 0d0a 2020 2020 2020 2020 2020  esp:..          
+00006be0: 2020 7365 6c66 2e5f 6765 745f 6d65 7461    self._get_meta
+00006bf0: 6461 7461 2865 6163 6844 6174 6152 6573  data(eachDataRes
+00006c00: 706f 6e73 6529 0d0a 232d 2d2d 2d2d 2d2d  ponse)..#-------
+00006c10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006c20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006c30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a  --------------..
+00006c60: 0d0a                                     ..
```

## Comparing `DatastreamPy-2.0.28.dist-info/METADATA` & `DatastreamPy-2.0.30.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DatastreamPy
-Version: 2.0.28
+Version: 2.0.30
 Summary: Python package for Datastream Web Services API
 Author: LSEG
 Author-email: datastreamapi@lseg.com
 License: Apache Software License (http://www.apache.org/licenses/LICENSE-2.0)
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
```

## Comparing `DatastreamPy-2.0.28.dist-info/RECORD` & `DatastreamPy-2.0.30.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 DatastreamPy/DSConnect.py,sha256=fyKii7eJU95M3Xsm-SB-2GgvJg_2_NHOVZ3sFmQ_0ik,16190
-DatastreamPy/DSUserDataObjectBase.py,sha256=LnfYeqvQAqMBj_TCiYhGosxO9JZ4kt-ZafDJ76p4TGM,22949
+DatastreamPy/DSUserDataObjectBase.py,sha256=5aTbKz1N-e90l7aPE0Dwb6Ixc2dwDDJUpCfayEgOThQ,22949
 DatastreamPy/DS_Requests.py,sha256=uPFJe8C54guWFSZS8tvQNsn00hnUF7ipVNX8JtAAzxo,5633
-DatastreamPy/DS_Response.py,sha256=aYRV_3qwvdLcOF12OBeJvdPDaTZljvH73Nnvd-62_HY,27581
+DatastreamPy/DS_Response.py,sha256=yt26JIosKyy01ruLgeYZs10w8a60ORBuE8BQdabPrCE,27746
 DatastreamPy/DatastreamEconomicFilters.py,sha256=73gTd_naqDrTW6DH2QXQ2tc5C_uTEvwSZi8w-CpHPdY,60200
 DatastreamPy/DatastreamUserCreated_TimeSeries.py,sha256=nVgv0IhgMu5_FiSrA3lpcE3248gNasdWIl0-iMJ71zo,52895
 DatastreamPy/__init__.py,sha256=EoZTqqEHz9OQbUFrGYtT-80Nw8WV5BYGUgxsvKvIV2U,1041
-DatastreamPy-2.0.28.dist-info/METADATA,sha256=xC3DqOaiOANptalGHrGJ7rhfyjFNywF58nC045tXGhM,27395
-DatastreamPy-2.0.28.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-DatastreamPy-2.0.28.dist-info/top_level.txt,sha256=B3hGJALzw6vwaMsJGwuxz537PgGsGd3KUkSh0OvQcAc,13
-DatastreamPy-2.0.28.dist-info/RECORD,,
+DatastreamPy-2.0.30.dist-info/METADATA,sha256=UCQEkQA-uiBk3n3py4CrSgacakX3-mj1-Ygj-bKWWIE,27395
+DatastreamPy-2.0.30.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+DatastreamPy-2.0.30.dist-info/top_level.txt,sha256=B3hGJALzw6vwaMsJGwuxz537PgGsGd3KUkSh0OvQcAc,13
+DatastreamPy-2.0.30.dist-info/RECORD,,
```

