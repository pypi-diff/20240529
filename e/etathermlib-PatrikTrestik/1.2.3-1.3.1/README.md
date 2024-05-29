# Comparing `tmp/etathermlib-PatrikTrestik-1.2.3.tar.gz` & `tmp/etathermlib_patriktrestik-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etathermlib-PatrikTrestik-1.2.3.tar", last modified: Fri Dec  1 10:09:10 2023, max compression
+gzip compressed data, was "etathermlib_patriktrestik-1.3.1.tar", last modified: Wed May 29 18:01:37 2024, max compression
```

## Comparing `etathermlib-PatrikTrestik-1.2.3.tar` & `etathermlib_patriktrestik-1.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-12-01 10:09:10.632939 etathermlib-PatrikTrestik-1.2.3/
--rw-rw-rw-   0        0        0      651 2023-12-01 10:09:10.628942 etathermlib-PatrikTrestik-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-12-01 08:47:17.000000 etathermlib-PatrikTrestik-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-12-01 10:09:10.606763 etathermlib-PatrikTrestik-1.2.3/etathermlib/
--rw-rw-rw-   0        0        0        0 2023-10-19 09:03:40.000000 etathermlib-PatrikTrestik-1.2.3/etathermlib/__init__.py
--rw-rw-rw-   0        0        0     9475 2023-12-01 10:08:36.000000 etathermlib-PatrikTrestik-1.2.3/etathermlib/etatherm.py
-drwxrwxrwx   0        0        0        0 2023-12-01 10:09:10.625940 etathermlib-PatrikTrestik-1.2.3/etathermlib_PatrikTrestik.egg-info/
--rw-rw-rw-   0        0        0      651 2023-12-01 10:09:10.000000 etathermlib-PatrikTrestik-1.2.3/etathermlib_PatrikTrestik.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-12-01 10:09:10.000000 etathermlib-PatrikTrestik-1.2.3/etathermlib_PatrikTrestik.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-01 10:09:10.000000 etathermlib-PatrikTrestik-1.2.3/etathermlib_PatrikTrestik.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-12-01 10:09:10.000000 etathermlib-PatrikTrestik-1.2.3/etathermlib_PatrikTrestik.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-01 10:09:10.632939 etathermlib-PatrikTrestik-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0      709 2023-12-01 10:08:44.000000 etathermlib-PatrikTrestik-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:01:37.932544 etathermlib_patriktrestik-1.3.1/
+-rw-rw-rw-   0        0        0      651 2024-05-29 18:01:37.926460 etathermlib_patriktrestik-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-12-01 08:47:17.000000 etathermlib_patriktrestik-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 18:01:37.904518 etathermlib_patriktrestik-1.3.1/etathermlib/
+-rw-rw-rw-   0        0        0        0 2023-10-19 09:03:40.000000 etathermlib_patriktrestik-1.3.1/etathermlib/__init__.py
+-rw-rw-rw-   0        0        0     9605 2024-05-29 18:01:03.000000 etathermlib_patriktrestik-1.3.1/etathermlib/etatherm.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:01:37.924473 etathermlib_patriktrestik-1.3.1/etathermlib_PatrikTrestik.egg-info/
+-rw-rw-rw-   0        0        0      651 2024-05-29 18:01:37.000000 etathermlib_patriktrestik-1.3.1/etathermlib_PatrikTrestik.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-05-29 18:01:37.000000 etathermlib_patriktrestik-1.3.1/etathermlib_PatrikTrestik.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 18:01:37.000000 etathermlib_patriktrestik-1.3.1/etathermlib_PatrikTrestik.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-29 18:01:37.000000 etathermlib_patriktrestik-1.3.1/etathermlib_PatrikTrestik.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 18:01:37.932544 etathermlib_patriktrestik-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      709 2024-05-29 18:01:03.000000 etathermlib_patriktrestik-1.3.1/setup.py
```

### Comparing `etathermlib-PatrikTrestik-1.2.3/PKG-INFO` & `etathermlib_patriktrestik-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etathermlib-PatrikTrestik
-Version: 1.2.3
+Version: 1.3.1
 Summary: Etatherm heating regulation TCP interface library
 Home-page: https://github.com/PatrikTrestik/etathermlib
 Author: Patrik Trestik
 Author-email: patrikt@volny.cz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `etathermlib-PatrikTrestik-1.2.3/etathermlib/etatherm.py` & `etathermlib_patriktrestik-1.3.1/etathermlib/etatherm.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 import asyncio
 
 
 class Etatherm:
     '''Etather protocol implementation'''
     _responseDelay=4
 
-    def __init__(self, host: str, port:int):
+    def __init__(self, host: str, port:int, a:int, j:int):
         self._host=host
         self._port=port
         self._params=None
+        self.a=a
+        self.j=j
 
     def __get_header(self, a:int,j:int):
         return b'\x10\x01'+a.to_bytes(1,'big')+j.to_bytes(1,'big')
 
     def __get_addr_read(self, addr:bytes, cnt:int):
         if (cnt%2!=0):
             cnt+=1
@@ -140,27 +142,27 @@
 
     async def __read_params(self) -> None:
         start=0x1100
         name_start=0x1030
         res={}
         for pos in range(1,17): 
             addr=start+(pos-1)*0x10
-            (params, error)=await self.__send_read_request(0,1, addr.to_bytes(2,'big'), 4)
+            (params, error)=await self.__send_read_request(self.a,self.j, addr.to_bytes(2,'big'), 4)
             if params is None:
                 res[pos]=(False, "<timeout>", 5, 1)
                 continue
             used=params[0] & 0x07
             used=not (used==0)
             shift = params[2] & 0x3F
             shift = shift-(64*(shift//32))
             step=(params[2] & 0xc0) >> 6
             step=step+1
             if used:
                 addr=name_start+(pos-1)*8
-                (name, error)=await self.__send_read_request(0,1, addr.to_bytes(2,'big'), 8)
+                (name, error)=await self.__send_read_request(self.a,self.j, addr.to_bytes(2,'big'), 8)
                 if name is None:
                     name=b''
                 end=name.find(b'\x00')
                 if end!=-1:
                     name=name[:end]
                 name=name.decode("1250")
             else:
@@ -175,15 +177,15 @@
         if self._params is None:
             return None
         res={pos:{'name': p['name'],'min':(1+p['shift'])*p['step'], 'max':(30+p['shift'])*p['step']} for pos,p in self._params.items() if p['used']}
         return res
 
     async def get_current_temperatures(self)-> (dict[int,int] | None):
         '''Read actual temperatures as measured on all positions.'''
-        (data, _)=await self.__send_read_request(0,1, b'\x00\x60', 16)
+        (data, _)=await self.__send_read_request(self.a,self.j, b'\x00\x60', 16)
         if self._params is None:
             await self.__read_params()
         if data is None or len(data)!=16 or self._params is None:
             return None
         res={}
         for pos in range(1,17):
             b=data[pos-1]
@@ -196,52 +198,52 @@
         return (time_in.minute // 15)+(time_in.hour*4)+(time_in.day*32*4)+(time_in.month*32*32*4)
 
     async def set_mode(self, pos:int, auto:bool) ->bool:
         '''Set heating mode.'''
         start=0x1100
         addr=start+(pos-1)*0x10+0x03
         
-        (data, _)=await self.__send_read_request(0,1,addr.to_bytes(2,'big'),6)
+        (data, _)=await self.__send_read_request(self.a,self.j,addr.to_bytes(2,'big'),6)
         if data is None:
             return False
         if auto:
             data=bytes([data[0] & 0xDF]) + b'\x10\x80\x10\x80'
         else:
             data=bytes([data[0] | 0x20]) + data[1:5]        
-        (success, _)=await self.__send_write_request(0,1, addr.to_bytes(2,'big'), data)
+        (success, _)=await self.__send_write_request(self.a,self.j, addr.to_bytes(2,'big'), data)
 
         if not success:
             return False
         return True
 
     async def set_temporary_temperature(self, pos:int, temperature: int, duration: int=120)-> bool:
         '''Set temporary temperature on position. :Operativní změna: '''
         start=0x1100
         addr=start+(pos-1)*0x10+0x03
         
         if self._params is None:
             await self.__read_params()
         position=self._params[pos]
         temp=(floor(temperature)//position['step']-position['shift']) & 0x1f
-        (data, _)=await self.__send_read_request(0,1,addr.to_bytes(2,'big'),1)
+        (data, _)=await self.__send_read_request(self.a,self.j,addr.to_bytes(2,'big'),1)
         if data is None:
             return False
         now = datetime.now()
         start=self.__get_toy(now-timedelta(minutes=0))
         end=self.__get_toy(now+timedelta(minutes=duration+1))
         data=bytes([(data[0] & 0xC0)+temp])+start.to_bytes(2,'big')+end.to_bytes(2,'big')
-        (success, _)=await self.__send_write_request(0,1, addr.to_bytes(2,'big'), data)
+        (success, _)=await self.__send_write_request(self.a,self.j, addr.to_bytes(2,'big'), data)
 
         if not success:
             return False
         return True
 
     async def get_required_temperatures(self) -> (dict[int,dict[str,any]] | None):
         '''Returns "temp" - required temperature, "flag" - 0:summer, 1:HDO, 2:temporary temperature, 3:permanent temperature, 4:scheduled '''
-        (data, _)=await self.__send_read_request(0,1, b'\x00\x70', 16)
+        (data, _)=await self.__send_read_request(self.a,self.j, b'\x00\x70', 16)
         if self._params is None:
             await self.__read_params()
         if data is None or len(data)!=16 or self._params is None:
             return None
         res={}
         for pos in range(1,17):
             b=data[pos-1] & 0x1f
```

### Comparing `etathermlib-PatrikTrestik-1.2.3/etathermlib_PatrikTrestik.egg-info/PKG-INFO` & `etathermlib_patriktrestik-1.3.1/etathermlib_PatrikTrestik.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etathermlib-PatrikTrestik
-Version: 1.2.3
+Version: 1.3.1
 Summary: Etatherm heating regulation TCP interface library
 Home-page: https://github.com/PatrikTrestik/etathermlib
 Author: Patrik Trestik
 Author-email: patrikt@volny.cz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `etathermlib-PatrikTrestik-1.2.3/setup.py` & `etathermlib_patriktrestik-1.3.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import distutils.command.clean
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="etathermlib-PatrikTrestik",
-    version="1.2.3",
+    version="1.3.1",
     author="Patrik Trestik",
     author_email="patrikt@volny.cz",
     description="Etatherm heating regulation TCP interface library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/PatrikTrestik/etathermlib",
     packages=find_packages(),
```

