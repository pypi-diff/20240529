# Comparing `tmp/nodens_gateway-24.5.4a0.tar.gz` & `tmp/nodens_gateway-24.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodens_gateway-24.5.4a0.tar", last modified: Tue May 21 18:17:23 2024, max compression
+gzip compressed data, was "nodens_gateway-24.5.5.tar", last modified: Wed May 29 17:06:05 2024, max compression
```

## Comparing `nodens_gateway-24.5.4a0.tar` & `nodens_gateway-24.5.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 18:17:23.081523 nodens_gateway-24.5.4a0/
--rw-rw-rw-   0        0        0     1122 2024-01-09 16:54:16.000000 nodens_gateway-24.5.4a0/LICENSE
--rw-rw-rw-   0        0        0        0 2023-11-08 16:47:38.000000 nodens_gateway-24.5.4a0/MANIFEST.in
--rw-rw-rw-   0        0        0     4328 2024-05-21 18:17:23.078520 nodens_gateway-24.5.4a0/PKG-INFO
--rw-rw-rw-   0        0        0     2429 2023-11-29 17:07:27.000000 nodens_gateway-24.5.4a0/README.md
--rw-rw-rw-   0        0        0      818 2024-05-21 18:16:39.000000 nodens_gateway-24.5.4a0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-21 18:17:23.081523 nodens_gateway-24.5.4a0/setup.cfg
--rw-rw-rw-   0        0        0       53 2023-11-10 12:49:30.000000 nodens_gateway-24.5.4a0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 18:17:22.817244 nodens_gateway-24.5.4a0/src/
-drwxrwxrwx   0        0        0        0 2024-05-21 18:17:22.816241 nodens_gateway-24.5.4a0/src/nodens/
-drwxrwxrwx   0        0        0        0 2024-05-21 18:17:22.951429 nodens_gateway-24.5.4a0/src/nodens/gateway/
--rw-rw-rw-   0        0        0    13491 2024-05-21 18:16:37.000000 nodens_gateway-24.5.4a0/src/nodens/gateway/__init__.py
--rw-rw-rw-   0        0        0     8583 2024-05-21 13:43:36.000000 nodens_gateway-24.5.4a0/src/nodens/gateway/__main__.py
--rw-rw-rw-   0        0        0    86278 2024-05-21 18:10:02.000000 nodens_gateway-24.5.4a0/src/nodens/gateway/nodens_fns.py
--rw-rw-rw-   0        0        0     9979 2024-01-15 12:37:53.000000 nodens_gateway-24.5.4a0/src/nodens/gateway/nodens_insight_hub.py
--rw-rw-rw-   0        0        0     4567 2024-02-03 15:44:49.000000 nodens_gateway-24.5.4a0/src/nodens/gateway/nodens_mesh.py
--rw-rw-rw-   0        0        0    25996 2024-05-21 18:00:48.000000 nodens_gateway-24.5.4a0/src/nodens/gateway/nodens_serv.py
--rw-rw-rw-   0        0        0    11052 2024-05-21 17:00:26.000000 nodens_gateway-24.5.4a0/src/nodens/gateway/nodens_thingsboard.py
-drwxrwxrwx   0        0        0        0 2024-05-21 18:17:23.076520 nodens_gateway-24.5.4a0/src/nodens_gateway.egg-info/
--rw-rw-rw-   0        0        0     4328 2024-05-21 18:17:22.000000 nodens_gateway-24.5.4a0/src/nodens_gateway.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1821 2023-11-11 13:34:07.000000 nodens_gateway-24.5.4a0/src/nodens_gateway.egg-info/PKG-INFO-Hawk
--rw-rw-rw-   0        0        0      640 2024-05-21 18:17:22.000000 nodens_gateway-24.5.4a0/src/nodens_gateway.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 18:17:22.000000 nodens_gateway-24.5.4a0/src/nodens_gateway.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-05-21 18:17:22.000000 nodens_gateway-24.5.4a0/src/nodens_gateway.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       44 2023-11-11 13:34:07.000000 nodens_gateway-24.5.4a0/src/nodens_gateway.egg-info/requires-Hawk.txt
--rw-rw-rw-   0        0        0       70 2024-05-21 18:17:22.000000 nodens_gateway-24.5.4a0/src/nodens_gateway.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-21 18:17:22.000000 nodens_gateway-24.5.4a0/src/nodens_gateway.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 17:06:05.910291 nodens_gateway-24.5.5/
+-rw-rw-rw-   0        0        0     1122 2024-01-09 16:54:16.000000 nodens_gateway-24.5.5/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-11-08 16:47:38.000000 nodens_gateway-24.5.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4326 2024-05-29 17:06:05.902737 nodens_gateway-24.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2429 2023-11-29 17:07:27.000000 nodens_gateway-24.5.5/README.md
+-rw-rw-rw-   0        0        0      817 2024-05-29 17:04:31.000000 nodens_gateway-24.5.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-29 17:06:05.910291 nodens_gateway-24.5.5/setup.cfg
+-rw-rw-rw-   0        0        0       53 2023-11-10 12:49:30.000000 nodens_gateway-24.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:06:05.020824 nodens_gateway-24.5.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 17:06:05.018009 nodens_gateway-24.5.5/src/nodens/
+drwxrwxrwx   0        0        0        0 2024-05-29 17:06:05.554773 nodens_gateway-24.5.5/src/nodens/gateway/
+-rw-rw-rw-   0        0        0    13490 2024-05-29 17:05:10.000000 nodens_gateway-24.5.5/src/nodens/gateway/__init__.py
+-rw-rw-rw-   0        0        0     8583 2024-05-21 13:43:36.000000 nodens_gateway-24.5.5/src/nodens/gateway/__main__.py
+-rw-rw-rw-   0        0        0    89293 2024-05-27 17:20:49.000000 nodens_gateway-24.5.5/src/nodens/gateway/nodens_fns.py
+-rw-rw-rw-   0        0        0     9979 2024-01-15 12:37:53.000000 nodens_gateway-24.5.5/src/nodens/gateway/nodens_insight_hub.py
+-rw-rw-rw-   0        0        0     4554 2024-05-24 12:27:56.000000 nodens_gateway-24.5.5/src/nodens/gateway/nodens_mesh.py
+-rw-rw-rw-   0        0        0    27390 2024-05-24 21:06:33.000000 nodens_gateway-24.5.5/src/nodens/gateway/nodens_serv.py
+-rw-rw-rw-   0        0        0    11148 2024-05-27 17:26:36.000000 nodens_gateway-24.5.5/src/nodens/gateway/nodens_thingsboard.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:06:05.895016 nodens_gateway-24.5.5/src/nodens_gateway.egg-info/
+-rw-rw-rw-   0        0        0     4326 2024-05-29 17:06:04.000000 nodens_gateway-24.5.5/src/nodens_gateway.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1821 2023-11-11 13:34:07.000000 nodens_gateway-24.5.5/src/nodens_gateway.egg-info/PKG-INFO-Hawk
+-rw-rw-rw-   0        0        0      640 2024-05-29 17:06:04.000000 nodens_gateway-24.5.5/src/nodens_gateway.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 17:06:04.000000 nodens_gateway-24.5.5/src/nodens_gateway.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-05-29 17:06:04.000000 nodens_gateway-24.5.5/src/nodens_gateway.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       44 2023-11-11 13:34:07.000000 nodens_gateway-24.5.5/src/nodens_gateway.egg-info/requires-Hawk.txt
+-rw-rw-rw-   0        0        0       70 2024-05-29 17:06:04.000000 nodens_gateway-24.5.5/src/nodens_gateway.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-29 17:06:04.000000 nodens_gateway-24.5.5/src/nodens_gateway.egg-info/top_level.txt
```

### Comparing `nodens_gateway-24.5.4a0/LICENSE` & `nodens_gateway-24.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.4a0/PKG-INFO` & `nodens_gateway-24.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodens-gateway
-Version: 24.5.4a0
+Version: 24.5.5
 Summary: Run the NodeNs gateway
 Author-email: Khalid Z Rajab <khalid@nodens.eu>
 License: The MIT License (MIT)
         
         Copyright (c) 2024 Khalid Rajab and NodeNs Medical Ltd.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nodens_gateway-24.5.4a0/README.md` & `nodens_gateway-24.5.5/README.md`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.4a0/pyproject.toml` & `nodens_gateway-24.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nodens-gateway"
-version = "24.5.4a"
+version = "24.5.5"
 description = "Run the NodeNs gateway"
 readme = "README.md"
 authors = [{ name = "Khalid Z Rajab", email = "khalid@nodens.eu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `nodens_gateway-24.5.4a0/src/nodens/gateway/__init__.py` & `nodens_gateway-24.5.5/src/nodens/gateway/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 global APPNAME
 global APPAUTHOR
 global CWD
 
 # Some information
 __title__ = "nodens-gateway"
-__version__ = "24.5.4a"
+__version__ = "24.5.5"
 __author__ = "Khalid Z Rajab"
 __author_email__ = "khalid@nodens.eu"
 __copyright__ = "Copyright (c) 2024 " + __author__
 __license__ = "MIT"
 
 APPNAME = "Gateway"
 APPAUTHOR = "NodeNs"
```

### Comparing `nodens_gateway-24.5.4a0/src/nodens/gateway/__main__.py` & `nodens_gateway-24.5.5/src/nodens/gateway/__main__.py`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.4a0/src/nodens/gateway/nodens_fns.py` & `nodens_gateway-24.5.5/src/nodens/gateway/nodens_fns.py`

 * *Files 2% similar despite different names*

```diff
@@ -785,21 +785,22 @@
             nodens.logger.warning(f"GaitParameters.reset_tracks. Sensor id: {sensor_id} does not match {self.sensor_id}")
 
 
     def calculate_gait_parameters(self, track_id=[]):
         """This function calculates gait parameters for all tracks recorded with this sensor, over num_hist_frames."""
         """To calculate parameters for a specific track, specify the track_id."""
 
+        self.gait_str = ""
         if (track_id == []):
             for track_gaits in self.track_gait_params:
                 track_gaits.gait = np.bincount(np.digitize(track_gaits.speed, track_gaits.gait_bins))
                 if len(self.gait_str) > 0:
                     self.gait_str += ";"
                 self.gait_str += ','.join(map(str, track_gaits.gait))
-
+                
         else:
             ind_t = self.track_id.index(track_id)
             self.track_gait_params[ind_t].gait = np.bincount(np.digitize(self.track_gait_params[ind_t].speed, self.track_gait_params[ind_t].gait_bins))
 
 
 
 # Occupant track history #
@@ -849,90 +850,125 @@
         self.track_del_flag = []
         
     # Use this to refresh the histories
     def refresh(self, sensor_id):
         # Check for this specific sensor
         ind_s = self.sensor_id.index(sensor_id)
 
-        self.id[ind_s] = [] 
-
         self.xh[ind_s] = np.empty([self.xh.shape[1],self.xh.shape[2]], dtype=object)
         self.yh[ind_s] = np.empty([self.yh.shape[1],self.yh.shape[2]], dtype=object)
 
         self.e_ud_h[ind_s] = np.empty([self.e_ud_h.shape[1]], dtype=object)
         self.e_pc_h[ind_s] = np.empty([self.e_pc_h.shape[1]], dtype=object)
 
-        self.tot_dist[ind_s] = []
-        self.max_dist[ind_s] = [] 
-        self.flag_active[ind_s] = []
-        self.time_inactive_start[ind_s] = [] 
+        # self.tot_dist[ind_s] = 0*self.tot_dist[ind_s]
+        # self.max_dist[ind_s] = 0*self.max_dist[ind_s] 
+        # self.flag_active[ind_s] = 1*self.flag_active[ind_s]
+        for time in self.time_inactive_start[ind_s]:
+            time = dt.datetime.now(dt.timezone.utc)
 
         # Reset room heatmap
         self.room_heatmap[ind_s].reset_heatmap()
 
         # Reset gait parameters
         self.gait_params[ind_s].reset_tracks(sensor_id)
     
     # Use this to update a track location everytime one is detected.
     def update(self, sensor_id, track_id=[], X=[], Y=[], sensor_data=[]):
         if (sensor_id in self.sensor_id):
             # Check for this specific sensor
             ind_s = self.sensor_id.index(sensor_id)
+            #nodens.logger.info(f"OH.update. sensor_id: {sensor_id}. ind_s: {ind_s}. track_id: {track_id}. self.id[ind_s]: {self.id[ind_s]}. LOGIC: track exists: {track_id in self.id[ind_s]}")
 
             if (track_id == []):
                 pass
             elif (track_id in self.id[ind_s]):
                 # Check for this specific track
                 ind_t = self.id[ind_s].index(track_id)
 
                 # Update coordinates
                 self.x0[ind_s][ind_t] = self.x1[ind_s][ind_t]
                 self.y0[ind_s][ind_t] = self.y1[ind_s][ind_t]
                 self.x1[ind_s][ind_t] = X
                 self.y1[ind_s][ind_t] = Y
 
                 # Update location histories
-                self.xh[ind_s][ind_t] = np.roll(self.xh[ind_s][ind_t],1)
-                self.xh[ind_s][ind_t][0] = X
-                self.yh[ind_s][ind_t] = np.roll(self.yh[ind_s][ind_t],1)
-                self.yh[ind_s][ind_t][0] = Y
+                try:
+                    self.xh[ind_s][ind_t] = np.roll(self.xh[ind_s][ind_t],1)
+                    self.xh[ind_s][ind_t][0] = X
+                    self.yh[ind_s][ind_t] = np.roll(self.yh[ind_s][ind_t],1)
+                    self.yh[ind_s][ind_t][0] = Y
+                except Exception as e:
+                    nodens.logger.error(f"OH.update. ind_s: {ind_s}. ind_t: {ind_t}. xh: {self.xh}. e: {e}")
 
                 # Update energy  - UD currently only has one sig. TODO: check tid and then find other sigs + don't forget to add to new_track
                 if sensor_data != []:       # Process only if receiving full data packet.
-                    self.e_ud_h[ind_s] = np.roll(self.e_ud_h[ind_s],1)
-                    self.e_ud_h[ind_s][0] = sensor_data.ud.signature_energy
-                    self.e_pc_h[ind_s] = np.roll(self.e_pc_h[ind_s],1)
-                    self.e_pc_h[ind_s][0] = sensor_data.pc.energy[0]
+                    try:
+                        self.e_ud_h[ind_s] = np.roll(self.e_ud_h[ind_s],1)
+                    except Exception as e:
+                        nodens.logger.error(f"OH.update 1. e: {e}")
+                    try:
+                        self.e_ud_h[ind_s][0] = sensor_data.ud.signature_energy
+                    except Exception as e:
+                        nodens.logger.error(f"OH.update 2. e: {e}")
+                    try:
+                        self.e_pc_h[ind_s] = np.roll(self.e_pc_h[ind_s],1)
+                    except Exception as e:
+                        nodens.logger.error(f"OH.update 3. e: {e}")
+                    try:                        
+                        self.e_pc_h[ind_s][0] = sensor_data.pc.energy[0]
+                    except Exception as e:
+                        self.e_pc_h[ind_s][0] = sensor_data.pc.energy
 
 
                 # Update activity statistics
-                self.activity_detection(sensor_id, track_id)
+                try:
+                    self.activity_detection(sensor_id, track_id)
+                except Exception as e:
+                    nodens.logger.error(f"OH.update activity_detection. e: {e}")
 
                 # Update heatmap
-                self.room_heatmap[ind_s].update_heatmap(X,Y)
+                try:
+                    self.room_heatmap[ind_s].update_heatmap(X,Y)
+                except Exception as e:
+                    nodens.logger.error(f"OH.update room_heatmap. e: {e}")
 
                 # Update gait parameters
-                self.gait_params[ind_s].update_track(sensor_id, track_id, self.xh[ind_s][ind_t], self.yh[ind_s][ind_t])
+                try:
+                    self.gait_params[ind_s].update_track(sensor_id, track_id, self.xh[ind_s][ind_t], self.yh[ind_s][ind_t])
+                except Exception as e:
+                    nodens.logger.error(f"OH.update gait_params. e: {e}")
 
             else:
                 # Record new values if track did not previously exist
                 #if track_id != []:
-                self.new_track(sensor_id,track_id,X,Y,new_sensor_flag=0)
+                try:
+                    nodens.logger.info("NEW TRACK 1")
+                    self.new_track(sensor_id,track_id,X,Y,new_sensor_flag=0)
+                except Exception as e:
+                    nodens.logger.error(f"OH.update new_track 1. e: {e}")
         else:
-            self.new_sensor(sensor_id)
+            try:
+                self.new_sensor(sensor_id)
+            except Exception as e:
+                    nodens.logger.error(f"OH.update new_sensor. e: {e}")
             if track_id != []:
-                self.new_track(sensor_id,track_id,X,Y,new_sensor_flag=1)
+                try:
+                    nodens.logger.info("NEW TRACK 2")
+                    self.new_track(sensor_id,track_id,X,Y,new_sensor_flag=1)
+                except Exception as e:
+                    nodens.logger.error(f"OH.update new_track 2. e: {e}")
 
 
     # Procedure when a new track is detected
     def new_track(self,sensor_id,track_id,X,Y,new_sensor_flag):
         ind_s = self.sensor_id.index(sensor_id)
         # if new_sensor_flag == 0:
         self.id[ind_s].append(track_id)
-
+        
         self.x0[ind_s].append(X)
         self.y0[ind_s].append(Y)
         self.x1[ind_s].append(X)
         self.y1[ind_s].append(Y)
 
         self.tot_dist[ind_s].append(0)
         self.max_dist[ind_s].append(0)
@@ -1009,18 +1045,18 @@
             self.y1[ind_s].pop(ind_t)
 
             self.tot_dist[ind_s].pop(ind_t)
             self.max_dist[ind_s].pop(ind_t)
             self.flag_active[ind_s].pop(ind_t)   # By default mark them as active
             self.time_inactive_start[ind_s].pop(ind_t)
             
-            self.xh = np.delete(self.xh, ind_t, axis=1)
-            self.yh = np.delete(self.yh, ind_t, axis=1)
+            self.xh[ind_s][ind_t] = np.empty((self.num_hist_frames),dtype=object)
+            self.yh[ind_s][ind_t] = np.empty((self.num_hist_frames),dtype=object)
 
-            self.id[ind_s].pop(track_id)
+            self.id[ind_s].pop(ind_t)
 
             # Delete gait params
             self.gait_params[ind_s].delete_track(sensor_id, track_id)
     
     # Use this to check entryways and see if anyone has entered/left the room
     def entryway(self, sensor_id, track_id, ew):
         if (sensor_id in ew.id):
@@ -1053,43 +1089,48 @@
             except:
                 nodens.logger.warning('Entryway update issue. (sx0,sx1)=({},{}). (sy0,sy1)=({},{})'.format(sx0,sx1,sy0,sy1))
     
     # Track activity/inactivity statistics
     def activity_detection(self, sensor_id, track_id, tot_dist_thresh=1, max_dist_thresh=1):
         ind_s = self.sensor_id.index(sensor_id)
         ind_t = self.id[ind_s].index(track_id)
-        
-        # Non-None values from history
-        xh =  [val for i,val in enumerate(self.xh[ind_s][ind_t]) if val is not None]
-        yh =  [val for i,val in enumerate(self.yh[ind_s][ind_t]) if val is not None]
 
-        # Calculate distances for each frame
-        try:
-            xd = np.subtract(xh[1:],xh[0:-1])
-            yd = np.subtract(yh[1:],yh[0:-1])
-            rd = (xd**2 + yd**2)**0.5
-
-            # Find statistics
-            self.tot_dist[ind_s][ind_t] =  np.sum(rd)
-            self.max_dist[ind_s][ind_t] = np.max(rd)
-
-            # Check if active
-            if self.tot_dist[ind_s][ind_t] > tot_dist_thresh:
-                self.flag_active[ind_s][ind_t] = 1
-                #print("Active!)")
-            elif self.max_dist[ind_s][ind_t] > max_dist_thresh:
-                self.flag_active[ind_s][ind_t] = 1
-                #print("Active!)")
-            else:
-                if (self.flag_active[ind_s][ind_t] == 1):
-                    self.time_inactive_start[ind_s][ind_t] = dt.datetime.now(dt.timezone.utc)
-                self.flag_active[ind_s][ind_t] = 0
+        xh_check = self.xh[ind_s][ind_t][1:]
 
-        except Exception as e:
-            nodens.logger.error(f"""Error {e.args}.""")
+        if all( x is None for x in xh_check) == False :
+            
+            
+            # Non-None values from history
+            xh =  [val for i,val in enumerate(self.xh[ind_s][ind_t]) if val is not None]
+            yh =  [val for i,val in enumerate(self.yh[ind_s][ind_t]) if val is not None]
+
+            # Calculate distances for each frame
+            try:
+                xd = np.subtract(xh[1:],xh[0:-1])
+                yd = np.subtract(yh[1:],yh[0:-1])
+                rd = (xd**2 + yd**2)**0.5
+
+                # Find statistics
+                self.tot_dist[ind_s][ind_t] =  np.sum(rd)
+                self.max_dist[ind_s][ind_t] = np.max(rd)
+
+                # Check if active
+                if self.tot_dist[ind_s][ind_t] > tot_dist_thresh:
+                    self.flag_active[ind_s][ind_t] = 1
+                    #print("Active!)")
+                elif self.max_dist[ind_s][ind_t] > max_dist_thresh:
+                    self.flag_active[ind_s][ind_t] = 1
+                    #print("Active!)")
+                else:
+                    if (self.flag_active[ind_s][ind_t] == 1):
+                        self.time_inactive_start[ind_s][ind_t] = dt.datetime.now(dt.timezone.utc)
+                    self.flag_active[ind_s][ind_t] = 0
+
+            except Exception as e:
+                nodens.logger.error(f"""OH.activity_detection. {e.args}. sensor_id: {sensor_id}. track_id: {track_id}.""")
             #print("Inactive since {} for track: {} with dist: {}".format(self.time_inactive_start[ind_s][ind_t], track_id, self.tot_dist[ind_s][ind_t], self.max_dist[ind_s][ind_t]))
 
         # Calculate total energies for each frame
         # try:
         #     ud_e = [val for val in self.e_ud_h[ind_s][ind_t] if val is not None]
         #     print(f"ud: {ud_e}")
 
@@ -1103,61 +1144,69 @@
             self.most_inactive_time[ind_s] = None
         else:
             inactive_idx = min(range(len(inactive_tracks)), key=inactive_tracks.__getitem__)
             self.most_inactive_track[ind_s] = self.id[ind_s][inactive_idx]
             self.most_inactive_time[ind_s] = dt.datetime.now(dt.timezone.utc) - self.time_inactive_start[ind_s][inactive_idx]
 
     # Calculate outputs
-    def calculate_outputs(self, thresh_distance = 0, energy_threshold = 0):
+    def calculate_outputs(self, sensor_id, thresh_distance = 0, energy_threshold = 0):
         # Re-initialise outputs
         self.outputs = []
         #self.outputs.__init__()
 
-        for idx, sensor in enumerate(self.sensor_id):    # For each sensor
-            self.outputs.append(self.Outputs())
-            self.outputs[idx].sensor_id = sensor
-            if len(self.id[idx]) > 0:
-                # Determine track to send
-                if max(self.tot_dist[idx]) >= thresh_distance: # Distance threshold at 0 for now, until UD sig tid is found.
-                    tid = self.tot_dist[idx].index(max(self.tot_dist[idx]))
-
-                    self.outputs[idx].track_id = self.id[idx][tid]
-
-                    # Record parameters
-                    self.outputs[idx].track_X = self.x1[idx][tid]
-                    self.outputs[idx].track_Y = self.y1[idx][tid]
-                    self.outputs[idx].distance_moved = self.tot_dist[idx][tid]
-                    
-                else:
-                    pass
-                    #tid = self.ud_energy[idx].index(max(self.ud_energy[idx]))
+        ind_s = self.sensor_id.index(sensor_id)
 
-                # Gait parameters
-                self.gait_params[idx].calculate_gait_parameters()
-                self.outputs[idx].gait_string = self.gait_params[idx].gait_str
-
-            # Energy statistics (for scene not track)
-            ud_e = [val for val in self.e_ud_h[idx] if val is not None]
-            self.outputs[idx].ud_energy = sum(ud_e)
-            if self.outputs[idx].ud_energy > energy_threshold:
-                self.outputs[idx].was_active = 1
-            else:
-                self.outputs[idx].was_active = 0
-            pc_e = [val for val in self.e_pc_h[idx] if val is not None]
-            self.outputs[idx].pc_energy = sum(pc_e)
             
-            # Room heatmaps
-            self.room_heatmap[idx].prepare_heatmap_string()
-            self.outputs[idx].heatmap_string = self.room_heatmap[idx].heatmap_string
-
-            # Delete tracks which have left
-            for ind_t, track in enumerate(self.id[idx]):
-                if track in self.track_del_flag[idx]:
-                    self.delete_track(sensor,track,mark_to_delete=0)
-            self.track_del_flag[idx] = []
+        if len(self.outputs) <= ind_s:
+            while True:
+                self.outputs.append(self.Outputs())
+                if len(self.outputs) > ind_s:
+                    break
+
+        self.outputs[ind_s] = self.Outputs()
+        self.outputs[ind_s].sensor_id = sensor_id
+        if len(self.id[ind_s]) > 0:
+            # Determine track to send
+            if max(self.tot_dist[ind_s]) >= thresh_distance: # Distance threshold at 0 for now, until UD sig tid is found.
+                tid = self.tot_dist[ind_s].index(max(self.tot_dist[ind_s]))
+
+                self.outputs[ind_s].track_id = self.id[ind_s][tid]
+
+                # Record parameters
+                self.outputs[ind_s].track_X = self.x1[ind_s][tid]
+                self.outputs[ind_s].track_Y = self.y1[ind_s][tid]
+                self.outputs[ind_s].distance_moved = self.tot_dist[ind_s][tid]
+                
+            else:
+                pass
+                #tid = self.ud_energy[ind_s].index(max(self.ud_energy[ind_s]))
+
+            # Gait parameters
+            self.gait_params[ind_s].calculate_gait_parameters()
+            self.outputs[ind_s].gait_string = self.gait_params[ind_s].gait_str
+
+        # Energy statistics (for scene not track)
+        ud_e = [val for val in self.e_ud_h[ind_s] if val is not None]
+        self.outputs[ind_s].ud_energy = sum(ud_e)
+        if self.outputs[ind_s].ud_energy > energy_threshold:
+            self.outputs[ind_s].was_active = 1
+        else:
+            self.outputs[ind_s].was_active = 0
+        pc_e = [val for val in self.e_pc_h[ind_s] if val is not None]
+        self.outputs[ind_s].pc_energy = sum(pc_e)
+        
+        # Room heatmaps
+        self.room_heatmap[ind_s].prepare_heatmap_string()
+        self.outputs[ind_s].heatmap_string = self.room_heatmap[ind_s].heatmap_string
+
+        # Delete tracks which have left
+        for ind_t, track in enumerate(self.id[ind_s]):
+            if track in self.track_del_flag[ind_s]:
+                self.delete_track(sensor_id,track,mark_to_delete=0)
+        self.track_del_flag[ind_s] = []
 
 
     
     # Class to define outputs
     class Outputs:
         def __init__(self) -> None:
             self.sensor_id = []
@@ -1630,20 +1679,20 @@
 
 ## ~~~ CLASSIFICATION ~~~ ##
 
 class classifierEngine:
     """Classifier engine. Currently a placeholder with a simple test."""
     def __init__(self, num_segments, class_frames_check, activity_wait_frames, energy_threshold):
         # Class buffer : class must have all positive hits to cause alert
-        self.class_buffer = np.zeros(shape=[class_frames_check,1])
+        self.class_buffer = np.zeros(shape=[class_frames_check,])
 
         # Data buffers: used for calculating
-        self.ud_sig_buffer = np.zeros(shape=[num_segments,1])
-        self.z_lf_buffer = np.zeros(shape=[num_segments,1])
-        self.z_track_buffer = np.zeros(shape=[num_segments,1])
+        self.ud_sig_buffer = np.zeros(shape=[num_segments,])
+        self.z_lf_buffer = np.zeros(shape=[num_segments,])
+        self.z_track_buffer = np.zeros(shape=[num_segments,])
 
         self.ud_sig_energy = 0
         self.zt_bw = 0
         self.zt_grad_mean = 0
         self.z_lf = 0
         
         self.fall_score = 0
@@ -1674,22 +1723,28 @@
         try:
            self.z_track_buffer[0] = sensor_data.track.Z[t_idx]
         except:
             self.z_track_buffer[0] = None
 
         # Calculations
         self.ud_sig_energy = np.sum(self.ud_sig_buffer)
-        try:
-            self.zt_bw = np.nanmax(self.z_track_buffer) - np.nanmin(self.z_track_buffer)
-        except:
+        if (np.isnan(self.z_track_buffer).all() == False):
+            try:
+                self.zt_bw = np.nanmax(self.z_track_buffer) - np.nanmin(self.z_track_buffer)
+            except:
+                self.zt_bw = 0
+        else:
             self.zt_bw = 0
         self.zt_grad_mean = (self.z_track_buffer[-1] - self.z_track_buffer[0])/len(self.z_track_buffer)
-        try:
-            self.z_lf = np.nanmin(self.z_lf_buffer)
-        except: 
+        if (np.isnan(self.z_lf_buffer).all() == False):
+            try:
+                self.z_lf = np.nanmin(self.z_lf_buffer)
+            except: 
+                self.z_lf = 0
+        else:
             self.z_lf = 0
         self.frames_since_activity += 1
 
     def activity_check(self):
         if self.ud_sig_energy > self.energy_threshold:
             self.activity_flag = 1
         else:
@@ -1723,28 +1778,28 @@
         self.sit_score_energy = self.find_score(self.ud_sig_energy,2800,6000)
         self.sit_score = 0.25*100*(self.sit_score_bw + self.sit_score_grad + 
                                    self.sit_score_lf + self.sit_score_energy)
 
         self.activity_check()
         
         classes = ['None', 'Fall', 'Jump', 'Sit']
-        if self.activity_flag == 1:
-            scores = [0, self.fall_score, self.jump_score, self.sit_score]
-            self.class_buffer = np.roll(self.class_buffer, 1)
-            self.class_buffer[0] = scores.index(max(scores))
-            if np.min(self.class_buffer) == np.max(self.class_buffer) and self.frames_since_activity >= self.activity_wait_frames:
-                self.classification = self.class_buffer[0][0]
-                self.frames_since_activity = 0
-                self.activity_alert = 1
-                print("ACTIVITY DETECTED: {}".format(self.classification))
-                print("Scores: {}, {}, {}".format(self.fall_score, self.jump_score, self.sit_score))
-
-        else:
-            self.class_buffer = np.roll(self.class_buffer, 1)
-            self.class_buffer[0] = 0
+        # if self.activity_flag == 1:
+        #     scores = [0, self.fall_score, self.jump_score, self.sit_score]
+        #     self.class_buffer = np.roll(self.class_buffer, 1)
+        #     self.class_buffer[0] = scores.index(max(scores))
+        #     if np.min(self.class_buffer) == np.max(self.class_buffer) and self.frames_since_activity >= self.activity_wait_frames:
+        #         self.classification = self.class_buffer[0][0]
+        #         self.frames_since_activity = 0
+        #         self.activity_alert = 1
+        #         print("ACTIVITY DETECTED: {}".format(self.classification))
+        #         print("Scores: {}, {}, {}".format(self.fall_score, self.jump_score, self.sit_score))
+
+        # else:
+        #     self.class_buffer = np.roll(self.class_buffer, 1)
+        #     self.class_buffer[0] = 0
 
 ## ~~~~~~~~~~~~~~~~~~~~~~ ##
 
 def convert_4_to_1(arg1, *argv):
     if  isinstance(arg1, (np.ndarray,)):
         arg1 = np.ndarray.tolist(arg1)
     if  isinstance(arg1, (list,)):   
@@ -1852,19 +1907,25 @@
         if flag_track is False:
             self.track = track([])
         if flag_pc is False:
             self.pc = point_cloud_3D_new([], sv.radar_version)
             self.pc_history.update_history(self.pc)
 
     def tlvN(self, data, j):
-        lenN = convert_4_to_1(data[j+4:j+8])
-        if (lenN == 65536):
-            nodens.logger.warning("Data packet TLV length error. j: {}. len: {}.".format(j,len(data)))
-        dataN = data[j:j+lenN]
-        j += lenN
+        if len(data) > j+8:
+            lenN = convert_4_to_1(data[j+4:j+8])
+            if (lenN == 65536):
+                nodens.logger.warning("Data packet TLV length error. j: {}. len: {}.".format(j,len(data)))
+            dataN = data[j:j+lenN]
+            j += lenN
+        else:
+            nodens.logger.warning(f"End of data packet with remaining data: {data[j:]}")
+            j = 65535
+            lenN = 0
+            dataN = []
         
         return j,lenN,dataN
 
 class sendCMDtoSensor(object):
     """Send a command (e.g. a new configuration) to the sensor via MQTT."""
     def full_data_off(rcp,cp):
         config_full_data = "CMD: FULL DATA OFF."
```

### Comparing `nodens_gateway-24.5.4a0/src/nodens/gateway/nodens_insight_hub.py` & `nodens_gateway-24.5.5/src/nodens/gateway/nodens_insight_hub.py`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.4a0/src/nodens/gateway/nodens_mesh.py` & `nodens_gateway-24.5.5/src/nodens/gateway/nodens_mesh.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,19 +111,18 @@
             self.info_timestamp_history = []
 
         def receive_msg(self, payload, timestamp):
             self.last_msg = payload[5:]
             self.last_msg_timestamp = timestamp
             self.msg_history.insert(0,payload[5:])
             self.msg_timestamp_history.insert(0,timestamp)
-            nodens.logger.info("Message received: {}".format(self.last_msg))
 
-        def receive_info(self, payload, timestamp):
+        def receive_info(self, payload, timestamp, sensor_id):
             self.last_info = payload
             self.last_info_timestamp = timestamp
             self.info_history.insert(0,payload)
             self.info_timestamp_history.insert(0,timestamp)
-            nodens.logger.info("Info received: {}".format(self.last_info))
+            nodens.logger.info("Info received: {} for sensor: {} at timestamp: {}".format(self.last_info, sensor_id, timestamp))
 
 
 MESH = mesh()
```

### Comparing `nodens_gateway-24.5.4a0/src/nodens/gateway/nodens_serv.py` & `nodens_gateway-24.5.5/src/nodens/gateway/nodens_serv.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,22 +164,29 @@
                 #print(heartbeat, end='')
                 mqttDataTemp = [T.strftime("%H:%M:%S")]
                 mqttDataTemp.append(mqttData['addr'])
                 mqttDataTemp.append(mqttData['data'])
                 mqttData_SAVEFull.append(mqttDataTemp)
 
                 temp_current_occupants = []
-                try:
-                    if ndns_fns.sd.track.num_tracks > 0:
-                        for idx, track in enumerate(ndns_fns.sd.track.tid):
-                            temp_current_occupants.append(track)
-                            ndns_fns.oh.update(mqttData['addr'],track,ndns_fns.sd.track.X[idx],ndns_fns.sd.track.Y[idx],ndns_fns.sd)
-                    ndns_fns.oh.sensor_activity(mqttData['addr'])
-                except Exception as e:
-                    nodens.logger.warning(f"{e}")
+                
+                if ndns_fns.sd.track.num_tracks > 0:
+                    for idx, track in enumerate(ndns_fns.sd.track.tid):
+                        temp_current_occupants.append(track)
+                        ndns_fns.oh.update(mqttData['addr'],track,ndns_fns.sd.track.X[idx],ndns_fns.sd.track.Y[idx],ndns_fns.sd)
+                        # except Exception as e:
+                        #     nodens.logger.warning(f"SERV update. {e}. sensor_id: {mqttData['addr']}. num_tracks: {ndns_fns.sd.track.num_tracks}. tid: {ndns_fns.sd.track.tid}.",
+                        #                           f"idx: {idx}. track: {track}. X: {ndns_fns.sd.track.X}. Y: {ndns_fns.sd.track.Y}. ids: {ndns_fns.oh.id}",
+                        #                           f"ind_s: {ndns_fns.oh.sensor_id.index(mqttData['addr'])}. ind_t: {ndns_fns.oh.id[ndns_fns.oh.sensor_id.index(mqttData['addr'])].index(track)}")
+                            
+                    try:
+                        ndns_fns.oh.sensor_activity(mqttData['addr'])
+                    except Exception as e:
+                            nodens.logger.warning(f"SERV sensor_activity. {e}. sensor_id: {mqttData['addr']}.")   
+                
 
                 # Update time period occupancy data
                 if mqttData['addr'] not in ndns_fns.ew.id:
                     ndns_fns.ew.update(mqttData['addr'])
                 send_idx_e = ndns_fns.ew.id.index(mqttData['addr'])
 
                 ndns_fns.si.update_refresh(sen_idx, send_idx_e, T, ndns_fns.ew)
@@ -187,38 +194,43 @@
 
                 #TODO: check cloud update
                 if ((T - ndns_fns.si.period_t[sen_idx]).total_seconds() > nodens.cp.CLOUD_WRITE_TIME):
                     # Mark for deletion tracks which have left
                     ndns_fns.oh.delete_track(mqttData['addr'], temp_current_occupants, mark_to_delete=1)
 
                     # Calculate occupant history outputs
-                    ndns_fns.oh.calculate_outputs()
+                    ndns_fns.oh.calculate_outputs(mqttData['addr'])
 
                     mqttTime = json.loads("{\"Time\": \"" + str(T) + "\"}")
-                    mqttClass = json.loads("{\"Activity detected\": \"" + str(int(ndns_fns.class_eng.activity_alert))
-                                        + "\", \"Activity type\": \"" + str(int(ndns_fns.class_eng.classification))
-                                        + "\"}")
+                    # mqttClass = json.loads("{\"Activity detected\": \"" + str(int(ndns_fns.class_eng.activity_alert))
+                    #                     + "\", \"Activity type\": \"" + str(int(ndns_fns.class_eng.classification))
+                    #                     + "\"}")
                     mqttDataFinal = {**mqttData, #'addr' : mqttData['addr'],
                                     'Sensor timestamp' : T,
                                     'Average period occupancy' : ndns_fns.si.period_sum_occ[sen_idx]/ndns_fns.si.period_N[sen_idx], 
                                     'Maximum period occupancy' : ndns_fns.si.period_max_occ[sen_idx],
                                     'Average entryway occupancy' : ndns_fns.si.ew_period_sum_occ[sen_idx]/ndns_fns.si.period_N[sen_idx], 
                                     'Maximum entryway occupancy' : ndns_fns.si.ew_period_max_occ[sen_idx],
-                                    'Full data flag' : 1,
-                                    'Track id' : ndns_fns.oh.outputs[sen_idx].track_id,
-                                    'X' : ndns_fns.oh.outputs[sen_idx].track_X,
-                                    'Y' : ndns_fns.oh.outputs[sen_idx].track_Y,
-                                    'Distance moved' : ndns_fns.oh.outputs[sen_idx].distance_moved,
-                                    'Was active' : ndns_fns.oh.outputs[sen_idx].was_active,
-                                    'UD energy' : ndns_fns.oh.outputs[sen_idx].ud_energy,
-                                    'PC energy' : ndns_fns.oh.outputs[sen_idx].pc_energy,
-                                    'Presence detected' : ndns_fns.sd.presence.present,
-                                    'Occupancy heatmap' : ndns_fns.oh.outputs[sen_idx].heatmap_string,
-                                    'Gait distribution' : ndns_fns.oh.outputs[sen_idx].gait_string
-                                    }
+                                    'Full data flag' : 0}
+                    try:
+                        mqttDataFinal = {**mqttDataFinal,
+                                        'Track id' : ndns_fns.oh.outputs[sen_idx].track_id,
+                                        'X' : ndns_fns.oh.outputs[sen_idx].track_X,
+                                        'Y' : ndns_fns.oh.outputs[sen_idx].track_Y,
+                                        'Distance moved' : ndns_fns.oh.outputs[sen_idx].distance_moved,
+                                        'Was active' : ndns_fns.oh.outputs[sen_idx].was_active,
+                                        'UD energy' : ndns_fns.oh.outputs[sen_idx].ud_energy,
+                                        'PC energy' : ndns_fns.oh.outputs[sen_idx].pc_energy,
+                                        'Presence detected' : ndns_fns.sd.presence.present,
+                                        'Occupancy heatmap' : ndns_fns.oh.outputs[sen_idx].heatmap_string,
+                                        'Gait distribution' : ndns_fns.oh.outputs[sen_idx].gait_string
+                                        }
+                    except Exception as e:
+                        nodens.logger.error(f"{e}. sen_idx: {sen_idx}. len oh: {len(ndns_fns.oh.outputs)}")
+
 
                     ndns_fns.class_eng.activity_alert = 0
                     try:
                         send_idx_o = ndns_fns.oh.sens_idx.index(mqttData['addr'])
                         mqttDataFinal = {**mqttDataFinal, 
                                     'Most inactive track' : ndns_fns.oh.most_inactive_track[send_idx_o],
                                     'Most inactive time' : str(ndns_fns.oh.most_inactive_time[send_idx_o]),
@@ -315,18 +327,18 @@
                         except:
                             occ_info = mqttDataFinal['Occupancy Info'][0]
                         # nodens.logger.debug('OCCUPANCY INFO')
 
                         # Update occupancy history and entryways for each occupant
                         for i in range(len(occ_info)):      # NodeNs KZR FIX: update ESP to create new payload
                             temp = occ_info[i]
-                            temp_current_occupants.append(temp['Occupant ID'])
-                            ndns_fns.oh.update(mqttData['addr'],temp['Occupant ID'],temp['X'],temp['Y'])
+                            temp_current_occupants.append(int(temp['Occupant ID']))
+                            ndns_fns.oh.update(mqttData['addr'],int(temp['Occupant ID']),temp['X'],temp['Y'])
                             # Check if occupant has crossed entryway
-                            ndns_fns.oh.entryway(mqttData['addr'],temp['Occupant ID'], ndns_fns.ew)
+                            ndns_fns.oh.entryway(mqttData['addr'],int(temp['Occupant ID']), ndns_fns.ew)
                             # nodens.logger.debug('Occupant no.: {}. X: {}. Y = {}.'.format(temp['Occupant ID'],temp['X'],temp['Y']))
 
                         # Look at general activity stats
                         ndns_fns.oh.sensor_activity(mqttData['addr'])
                     else:
                         ndns_fns.oh.update(mqttData['addr'])
                         ndns_fns.oh.sensor_activity(mqttData['addr'])
@@ -363,38 +375,43 @@
 
                     ## ~~~~~~~~~~~ SEND TO CLOUD ~~~~~~~~~ ##
                     if ((T - ndns_fns.si.period_t[sen_idx]).total_seconds() > nodens.cp.CLOUD_WRITE_TIME):
                         # Mark for deletion tracks which have left
                         ndns_fns.oh.delete_track(mqttData['addr'], temp_current_occupants, mark_to_delete=1)
 
                         # Calculate occupant history outputs
-                        ndns_fns.oh.calculate_outputs()
+                        ndns_fns.oh.calculate_outputs(mqttData['addr'])
 
+                        
                         mqttTime = json.loads("{\"Time\": \"" + str(T) + "\"}")
-                        mqttClass = json.loads("{\"Activity detected\": \"" + str(int(ndns_fns.class_eng.activity_alert))
-                                            + "\", \"Activity type\": \"" + str(int(ndns_fns.class_eng.classification))
-                                            + "\"}")
-                        mqttDataFinal = {**mqttTime, **mqttData, **mqttClass, **mqttDataFinal, 
-                                         'Sensor timestamp' : T,
+                        # mqttClass = json.loads("{\"Activity detected\": \"" + str(int(ndns_fns.class_eng.activity_alert))
+                        #                     + "\", \"Activity type\": \"" + str(int(ndns_fns.class_eng.classification))
+                        #                     + "\"}")
+                        mqttDataFinal = {**mqttTime, **mqttData, **mqttDataFinal, 
+                                        'Sensor timestamp' : T,
                                         'Average period occupancy' : ndns_fns.si.period_sum_occ[sen_idx]/ndns_fns.si.period_N[sen_idx], 
                                         'Maximum period occupancy' : ndns_fns.si.period_max_occ[sen_idx],
                                         'Average entryway occupancy' : ndns_fns.si.ew_period_sum_occ[sen_idx]/ndns_fns.si.period_N[sen_idx], 
                                         'Maximum entryway occupancy' : ndns_fns.si.ew_period_max_occ[sen_idx],
-                                        'Full data flag' : 0,
-                                        'Track id' : ndns_fns.oh.outputs[sen_idx].track_id,
-                                        'X' : ndns_fns.oh.outputs[sen_idx].track_X,
-                                        'Y' : ndns_fns.oh.outputs[sen_idx].track_Y,
-                                        'Distance moved' : ndns_fns.oh.outputs[sen_idx].distance_moved,
-                                        'Was active' : ndns_fns.oh.outputs[sen_idx].was_active,
-                                        'UD energy' : ndns_fns.oh.outputs[sen_idx].ud_energy,
-                                        'PC energy' : ndns_fns.oh.outputs[sen_idx].pc_energy,
-                                        'Presence detected' : ndns_fns.sd.presence.present,
-                                        'Occupancy heatmap' : ndns_fns.oh.outputs[sen_idx].heatmap_string,
-                                        'Gait distribution' : ndns_fns.oh.outputs[sen_idx].gait_string
-                                        }
+                                        'Full data flag' : 0}
+                        try:
+                            mqttDataFinal = {**mqttDataFinal,
+                                            'Track id' : ndns_fns.oh.outputs[sen_idx].track_id,
+                                            'X' : ndns_fns.oh.outputs[sen_idx].track_X,
+                                            'Y' : ndns_fns.oh.outputs[sen_idx].track_Y,
+                                            'Distance moved' : ndns_fns.oh.outputs[sen_idx].distance_moved,
+                                            'Was active' : ndns_fns.oh.outputs[sen_idx].was_active,
+                                            'UD energy' : ndns_fns.oh.outputs[sen_idx].ud_energy,
+                                            'PC energy' : ndns_fns.oh.outputs[sen_idx].pc_energy,
+                                            'Presence detected' : ndns_fns.sd.presence.present,
+                                            'Occupancy heatmap' : ndns_fns.oh.outputs[sen_idx].heatmap_string,
+                                            'Gait distribution' : ndns_fns.oh.outputs[sen_idx].gait_string
+                                            }
+                        except Exception as e:
+                            nodens.logger.error(f"{e}. sen_idx: {sen_idx}. len oh: {len(ndns_fns.oh.outputs)}")
                         
                         ndns_fns.class_eng.activity_alert = 0
                         try:
                             send_idx_o = ndns_fns.oh.sens_idx.index(mqttData['addr'])
                             mqttDataFinal = {**mqttDataFinal, 
                                         'Most inactive track' : ndns_fns.oh.most_inactive_track[send_idx_o],
                                         'Most inactive time' : str(ndns_fns.oh.most_inactive_time[send_idx_o]),
@@ -432,28 +449,28 @@
         
                 if mqttDataFinal['type'] == 'bytes':
                     ndns_fns.si.last_t[sen_idx] = T
                     heartbeat += "+"
                     heartbeat = "\r" + heartbeat
                     # print(heartbeat, end='')
                     if 'Sensor Information' in mqttDataFinal:
-                        nodens.logger.debug("\nSensor information: {} for Device: {}\n". format(mqttDataFinal['Sensor Information'], mqttDataFinal['addr']))
+                        nodens.logger.info("\nSensor information: {} for Device: {}\n". format(mqttDataFinal['Sensor Information'], mqttDataFinal['addr']))
 
                         # Check for sensor version
                         temp = mqttDataFinal['Sensor Information']
                         
                         if temp[0:7] == 'VERSION':
                             ndns_fns.sv.parse(temp[9:])
 
                         elif temp[0:6] == 'CONFIG':
                             ndns_fns.rcp.receive_config(temp[8:])
 
                         elif temp[0:3] == 'MSG':
                             ndns_mesh.MESH.status.receive_msg(temp, mqttDataFinal['timestamp'])
-                            ndns_mesh.MESH.status.receive_info(temp, mqttDataFinal['timestamp'])
+                            ndns_mesh.MESH.status.receive_info(temp, mqttDataFinal['timestamp'], mqttDataFinal['addr'])
                             if ndns_mesh.MESH.status.last_msg.find("NEW CONFIG!") >= 0:
                                 msg = ndns_mesh.MESH.status.last_msg
                                 i0 = msg.find("X=")
                                 i1 = msg[i0:].find(",")
                                 i2 = msg[i0:].find(")")
 
                                 ndns_fns.rcp.ROOM_X_MIN = (msg[i0+3:i0+i1])
@@ -463,15 +480,15 @@
                                 i1 = (msg[i0:].find(","))
                                 i2 = msg[i0:].find(")")
 
                                 ndns_fns.rcp.ROOM_Y_MIN = (msg[i0+3:i0+i1])
                                 ndns_fns.rcp.ROOM_Y_MAX = (msg[i0+i1+1:i0+i2])
 
                         else:
-                            ndns_mesh.MESH.status.receive_info(temp, mqttDataFinal['timestamp'])
+                            ndns_mesh.MESH.status.receive_info(temp, mqttDataFinal['timestamp'], mqttDataFinal['addr'])
                 
                 elif mqttDataFinal['type'] == 'heartbeat':
                     heartbeat += "."
                     heartbeat = "\r" + heartbeat
                     #print(heartbeat, end='')
                 else:
                     nodens.logger.warning("Another type: {}".format(mqttDataFinal))
```

### Comparing `nodens_gateway-24.5.4a0/src/nodens/gateway/nodens_thingsboard.py` & `nodens_gateway-24.5.5/src/nodens/gateway/nodens_thingsboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,15 +246,15 @@
             #         print("TB_CONNECT: {}".format(TB_CONNECT))
             #     else:
             #         time.sleep(1)
 
         try:
             json_message = json.dumps(self.payload)
         except Exception as e:
-            logging.error(f"ERROR {e.args}. Payload:{self.payload}")
+            nodens.logger.error(f"THINGSBOARD: {e.args}. Payload:{self.payload}")
 
         flag = 0
         while flag == 0:
             try:
                 self.client.publish(nodens.cp.TB_PUB_TOPIC, json_message, qos=1)
                 flag = 1
             except Exception as e:
@@ -269,12 +269,12 @@
                 for i in range(len(self.subscribed_sensors)):
                     self.client_sub[i].connect(nodens.cp.TB_HOST,nodens.cp.TB_PORT,nodens.cp.TB_KEEPALIVE)
                     self.client_sub[i].loop_start()
                     self.client_sub[i].subscribe(nodens.cp.TB_ATTRIBUTES_TOPIC, qos=1)
                 flag = 1
                 FLAG_TX_IN_PROGRESS = 0
             except Exception as e:
-                nodens.logger.error(f"THINGSBOARD: multiline payload finalise error: {e.args}")
+                nodens.logger.error(f"THINGSBOARD: multiline payload finalise error: {e.args}. Topic: {nodens.cp.TB_ATTRIBUTES_TOPIC}. Sensor: {self.subscribed_sensors[i]}, {i}")
                 sleep(1)
 
 TB = tb()
```

### Comparing `nodens_gateway-24.5.4a0/src/nodens_gateway.egg-info/PKG-INFO` & `nodens_gateway-24.5.5/src/nodens_gateway.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodens-gateway
-Version: 24.5.4a0
+Version: 24.5.5
 Summary: Run the NodeNs gateway
 Author-email: Khalid Z Rajab <khalid@nodens.eu>
 License: The MIT License (MIT)
         
         Copyright (c) 2024 Khalid Rajab and NodeNs Medical Ltd.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nodens_gateway-24.5.4a0/src/nodens_gateway.egg-info/PKG-INFO-Hawk` & `nodens_gateway-24.5.5/src/nodens_gateway.egg-info/PKG-INFO-Hawk`

 * *Files identical despite different names*

### Comparing `nodens_gateway-24.5.4a0/src/nodens_gateway.egg-info/SOURCES.txt` & `nodens_gateway-24.5.5/src/nodens_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

