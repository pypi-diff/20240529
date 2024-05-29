# Comparing `tmp/turbocase-1.4.2.tar.gz` & `tmp/turbocase-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbocase-1.4.2.tar", last modified: Mon May 27 15:13:44 2024, max compression
+gzip compressed data, was "turbocase-1.5.0.tar", last modified: Wed May 29 20:42:45 2024, max compression
```

## Comparing `turbocase-1.4.2.tar` & `turbocase-1.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 15:13:44.753028 turbocase-1.4.2/
--rw-r--r--   0 root         (0) root         (0)     1069 2024-05-15 14:32:06.000000 turbocase-1.4.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      271 2024-05-27 15:13:44.749695 turbocase-1.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2844 2024-05-17 13:48:51.000000 turbocase-1.4.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 15:13:44.753028 turbocase-1.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      459 2024-05-27 15:13:26.000000 turbocase-1.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 15:13:44.749695 turbocase-1.4.2/turbocase/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 00:06:28.000000 turbocase-1.4.2/turbocase/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1048 2024-05-17 16:22:48.000000 turbocase-1.4.2/turbocase/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1687 2024-05-26 14:19:02.000000 turbocase-1.4.2/turbocase/cases.py
--rw-r--r--   0 root         (0) root         (0)    12488 2024-05-27 15:10:48.000000 turbocase-1.4.2/turbocase/kicad.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 15:13:44.749695 turbocase-1.4.2/turbocase/parts/
--rw-r--r--   0 root         (0) root         (0)     1664 2024-05-26 14:17:50.000000 turbocase-1.4.2/turbocase/parts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1598 2024-05-23 00:53:13.000000 turbocase-1.4.2/turbocase/parts/batteryholder.py
--rw-r--r--   0 root         (0) root         (0)     1112 2024-05-26 14:25:33.000000 turbocase-1.4.2/turbocase/parts/cutout.py
--rw-r--r--   0 root         (0) root         (0)     3008 2024-05-26 13:34:36.000000 turbocase-1.4.2/turbocase/parts/keyhole.py
--rw-r--r--   0 root         (0) root         (0)     3472 2024-05-26 13:51:45.000000 turbocase-1.4.2/turbocase/parts/screws.py
--rw-r--r--   0 root         (0) root         (0)     2373 2024-05-23 01:24:44.000000 turbocase-1.4.2/turbocase/parts/shape.py
--rw-r--r--   0 root         (0) root         (0)     4585 2024-05-27 09:39:56.000000 turbocase-1.4.2/turbocase/scad.py
--rw-r--r--   0 root         (0) root         (0)     1279 2024-05-15 18:26:04.000000 turbocase-1.4.2/turbocase/vector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 15:13:44.749695 turbocase-1.4.2/turbocase.egg-info/
--rw-r--r--   0 root         (0) root         (0)      271 2024-05-27 15:13:44.000000 turbocase-1.4.2/turbocase.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      515 2024-05-27 15:13:44.000000 turbocase-1.4.2/turbocase.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 15:13:44.000000 turbocase-1.4.2/turbocase.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2024-05-27 15:13:44.000000 turbocase-1.4.2/turbocase.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-27 15:13:44.000000 turbocase-1.4.2/turbocase.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-27 15:13:44.000000 turbocase-1.4.2/turbocase.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:42:45.137396 turbocase-1.5.0/
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-05-15 14:32:06.000000 turbocase-1.5.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      271 2024-05-29 20:42:45.137396 turbocase-1.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2844 2024-05-17 13:48:51.000000 turbocase-1.5.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 20:42:45.137396 turbocase-1.5.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      459 2024-05-29 20:34:08.000000 turbocase-1.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:42:45.134063 turbocase-1.5.0/turbocase/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 00:06:28.000000 turbocase-1.5.0/turbocase/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1196 2024-05-29 20:39:08.000000 turbocase-1.5.0/turbocase/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2024-05-29 15:30:56.000000 turbocase-1.5.0/turbocase/cases.py
+-rw-r--r--   0 root         (0) root         (0)    13453 2024-05-29 20:24:14.000000 turbocase-1.5.0/turbocase/kicad.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:42:45.137396 turbocase-1.5.0/turbocase/parts/
+-rw-r--r--   0 root         (0) root         (0)     1664 2024-05-26 14:17:50.000000 turbocase-1.5.0/turbocase/parts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2024-05-23 00:53:13.000000 turbocase-1.5.0/turbocase/parts/batteryholder.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-05-26 14:25:33.000000 turbocase-1.5.0/turbocase/parts/cutout.py
+-rw-r--r--   0 root         (0) root         (0)     3008 2024-05-26 13:34:36.000000 turbocase-1.5.0/turbocase/parts/keyhole.py
+-rw-r--r--   0 root         (0) root         (0)     3472 2024-05-26 13:51:45.000000 turbocase-1.5.0/turbocase/parts/screws.py
+-rw-r--r--   0 root         (0) root         (0)     2373 2024-05-23 01:24:44.000000 turbocase-1.5.0/turbocase/parts/shape.py
+-rw-r--r--   0 root         (0) root         (0)     5938 2024-05-29 20:40:27.000000 turbocase-1.5.0/turbocase/scad.py
+-rw-r--r--   0 root         (0) root         (0)     1279 2024-05-15 18:26:04.000000 turbocase-1.5.0/turbocase/vector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:42:45.137396 turbocase-1.5.0/turbocase.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      271 2024-05-29 20:42:45.000000 turbocase-1.5.0/turbocase.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      515 2024-05-29 20:42:45.000000 turbocase-1.5.0/turbocase.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 20:42:45.000000 turbocase-1.5.0/turbocase.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2024-05-29 20:42:45.000000 turbocase-1.5.0/turbocase.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-29 20:42:45.000000 turbocase-1.5.0/turbocase.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-29 20:42:45.000000 turbocase-1.5.0/turbocase.egg-info/top_level.txt
```

### Comparing `turbocase-1.4.2/LICENSE.txt` & `turbocase-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `turbocase-1.4.2/README.md` & `turbocase-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `turbocase-1.4.2/turbocase/__main__.py` & `turbocase-1.5.0/turbocase/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,22 +8,23 @@
     parser = argparse.ArgumentParser()
     parser.add_argument('pcb', help='Input kicad PCB file')
     parser.add_argument('output', help='Generated openSCAD case template')
     parser.add_argument('--layer', help='Layer with the case inner-outline [defaults to User.6]', default='User.6')
     parser.add_argument('--bottom', help='Bottom thickness in mm [default 1.2]', default=1.2, type=float)
     parser.add_argument('--wall', help='Wall thickness in mm [default 1.2]', default=1.2, type=float)
     parser.add_argument('--standoff', help='Height generated for the PCB mounts in mm[default 5]', default=5, type=float)
+    parser.add_argument('--show-pcb', help='Show the PCB placeholder by default [default false]', default=False, type=bool)
     args = parser.parse_args()
 
     case = load_pcb(args.pcb, args.layer)
 
     case.floor_thickness = args.bottom
     case.wall_thickness = args.wall
     case.standoff_height = args.standoff
 
-    code = scad.generate(case)
+    code = scad.generate(case, show_pcb=args.show_pcb)
     with open(args.output, 'w') as handle:
         handle.write(code)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `turbocase-1.4.2/turbocase/cases.py` & `turbocase-1.5.0/turbocase/cases.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 class Case:
     connectors: list[Connector]
 
     def __init__(self):
         self.inner_path = []
         self.pcb_mount = []
         self.pcb_thickness = 1.6
+        self.pcb_path = []
+        self.pcb_holes = []
         self.floor_thickness = 1.2
         self.wall_thickness = 1.2
         self.standoff_height = 5
 
         self.cutouts = []
 
         self.max_connector_height = 0
```

### Comparing `turbocase-1.4.2/turbocase/kicad.py` & `turbocase-1.5.0/turbocase/kicad.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,14 +80,25 @@
 class Shape:
     @classmethod
     def from_single(cls, graphic):
         res = cls()
         res.append(graphic)
         return res
 
+    @classmethod
+    def make_circle(cls, center, radius, layer=None):
+        if layer is None:
+            layer = 'User.6'
+
+        return Shape.from_single(Sym([sexpdata.Symbol('gr_circle'),
+                                      [sexpdata.Symbol('center'), center[0], center[1]],
+                                      [sexpdata.Symbol('end'), center[0], center[1] + radius],
+                                      [sexpdata.Symbol('layer'), layer],
+                                      ]))
+
     def __init__(self):
         self.parts = []
         self.start = ()
         self.end = ()
         self.point = ()
         self.radius = 0
         self._bounds = None
@@ -293,14 +304,15 @@
 
     with open(pcb_file) as handle:
         pcb = sexpdata.load(handle)
 
     result = Case()
 
     outline_shapes = []
+    edgecuts_shapes = []
     mountingholes = []
     connectors = []
     parts = []
 
     for symbol in pcb:
         if not isinstance(symbol, list):
             continue
@@ -312,30 +324,36 @@
                 result.pcb_thickness = general['thickness'][0]
 
             if name in ['segment', 'gr_line', 'gr_arc', 'gr_poly', 'gr_rect', 'gr_circle']:
                 for sub in symbol:
                     if isinstance(sub, list):
                         if sub[0].value() == 'layer' and sub[1] == outline_layer:
                             outline_shapes.append(Sym(symbol))
+                        if sub[0].value() == 'layer' and sub[1] == 'Edge.Cuts':
+                            edgecuts_shapes.append(Sym(symbol))
 
             if name == 'footprint':
                 footprint = Sym(symbol)
 
                 if ':MountingHole_' in footprint[0]:
                     mountingholes.append(footprint)
                 elif 'TurboCase' in footprint[0]:
                     parts.append(footprint)
                 else:
                     for prop in footprint['property']:
                         if len(prop) == 2 and prop[0] == 'Height':
                             connectors.append(footprint)
 
     outline = sort_outline(outline_shapes)
+    edge_cuts = sort_outline(edgecuts_shapes)
 
     path = outline[0].path()
+    result.pcb_path = edge_cuts[0].path()
+    if len(edge_cuts) > 1:
+        result.pcb_holes = edge_cuts[1:]
 
     result.inner_path = path
     if len(outline) > 1:
         result.cutouts = outline[1:]
 
     for hole in mountingholes:
         center = hole['at'][:]
@@ -355,14 +373,15 @@
                 diam = max(circle['end'][0], circle['end'][1]) * 2
                 if diam > space:
                     space = diam
         else:
             space = drill_space
 
         result.pcb_mount.append((center, drill, space, hole.property['Reference']))
+        result.pcb_holes.append(Shape.make_circle(center, drill / 2))
 
     max_height = 0
     for item in connectors:
         ref = item.property['Reference']
         footprint = item.property['Footprint']
         desc = item.property['Description']
         height = float(item.property['Height'])
@@ -382,14 +401,16 @@
         c = Connector()
         c.prop_height = height
         c.reference = ref
         c.footprint = footprint
         c.description = desc
         c.bounds = shape_bounds(shapes)
         c.position = item['at'][:]
+        if len(c.position) == 2:
+            c.position = c.position + [0]
         result.connectors.append(c)
     result.max_connector_height = max_height
 
     modules = set()
     partlib = get_all_parts()
 
     for part in parts:
```

### Comparing `turbocase-1.4.2/turbocase/parts/__init__.py` & `turbocase-1.5.0/turbocase/parts/__init__.py`

 * *Files identical despite different names*

### Comparing `turbocase-1.4.2/turbocase/parts/batteryholder.py` & `turbocase-1.5.0/turbocase/parts/batteryholder.py`

 * *Files identical despite different names*

### Comparing `turbocase-1.4.2/turbocase/parts/cutout.py` & `turbocase-1.5.0/turbocase/parts/cutout.py`

 * *Files identical despite different names*

### Comparing `turbocase-1.4.2/turbocase/parts/keyhole.py` & `turbocase-1.5.0/turbocase/parts/keyhole.py`

 * *Files identical despite different names*

### Comparing `turbocase-1.4.2/turbocase/parts/screws.py` & `turbocase-1.5.0/turbocase/parts/screws.py`

 * *Files identical despite different names*

### Comparing `turbocase-1.4.2/turbocase/parts/shape.py` & `turbocase-1.5.0/turbocase/parts/shape.py`

 * *Files identical despite different names*

### Comparing `turbocase-1.4.2/turbocase/scad.py` & `turbocase-1.5.0/turbocase/scad.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 _template = """
-
 module wall (thickness, height) {
     linear_extrude(height) {
         difference() {
             offset(r=thickness)
                 children();
             children();
         }
@@ -47,24 +46,50 @@
     for p in points:
         parts.append(f'[{p[0]},{p[1]}]')
     result += ', '.join(parts)
     result += ']);\n'
     return result
 
 
-def generate(case):
+def _make_pcb_module(case):
+    result = 'module pcb() {\n'
+    result += f'    thickness = {case.pcb_thickness};\n\n'
+    result += '    color("#009900")\n'
+    result += '    difference() {\n'
+    result += f'        linear_extrude(thickness) ' + '{\n'
+    result += '            ' + _make_scad_polygon(case.pcb_path)
+    result += '        }\n'
+    for shape in case.pcb_holes:
+        if shape.is_circle:
+            result += f'    translate([{shape.point[0]}, {shape.point[1]}, -1])\n'
+            result += f'        cylinder(thickness+2, {shape.radius}, {shape.radius}, $fn=32);\n'
+        elif shape.is_rect:
+            result += f'    translate([{shape.point[0]}, {shape.point[1]}, 0])\n'
+            result += f'        cube([{shape.width}, {shape.height}, thickness + 2], center=true);\n'
+        else:
+            result += f'    translate([0, 0, -1])\n'
+            result += f'    linear_extrude(thickness+2) \n'
+            result += f'        {_make_scad_polygon(shape.path())}\n'
+    result += '    }\n'
+    result += '}\n\n'
+    return result
+
+
+def generate(case, show_pcb=False):
     """
     :type case: Case
     """
-
-    result = _template + "\n"
+    result = 'show_pcb = ' + ('true' if show_pcb else 'false') + ';\n\n'
+    result += _template.lstrip() + "\n"
 
     for m in case.modules:
         result += m + "\n"
 
+    result += _make_pcb_module(case)
+
     center = case.get_center()
     result += f'scale([1, -1, 1])\n'
     result += f'translate([-{center[0]}, -{center[1]}, 0]) ' + '{\n'
 
     result += f'    standoff_height = {case.standoff_height};\n'
     result += f'    floor_height = {case.floor_thickness};\n'
     result += f'    pcb_thickness = {case.pcb_thickness};\n'
@@ -87,31 +112,36 @@
             result += f'    translate([0, 0, -1])\n'
             result += f'    #linear_extrude(floor_height+2) \n'
             result += f'        {_make_scad_polygon(shape.path())}\n'
 
     for conn in sorted(case.connectors, key=lambda x: x.reference):
         result += f'    // {conn.reference} {conn.footprint} {conn.description}\n'
         result += f'    translate([{conn.position[0]}, {conn.position[1]}, pcb_top])\n' \
-                  f'    rotate([0, 0, {conn.position[2] + 180}])\n' \
+                  f'    rotate([0, 0, {-conn.position[2]}])\n' \
                   f'        #connector({conn.bounds[0]},{conn.bounds[1]},{conn.bounds[2]},{conn.bounds[3]},{conn.prop_height + 0.2});\n\n'
 
     for part in case.parts:
         if part.substract is None:
             continue
         z = 'floor_height'
         if part.offset_pcb:
             z = 'pcb_top'
         result += f'    // {part.description}\n'
         result += f'    translate([{part.position[0]}, {part.position[1]}, {z}])\n'
         if len(part.position) == 3:
-            result += f'    rotate([0, 0, {part.position[2] + 180}])\n'
+            result += f'    rotate([0, 0, {-part.position[2]}])\n'
         result += f'        {part.substract}\n'
 
     result += '    }\n\n'
 
+    result += '    if (show_pcb) {\n'
+    result += '    translate([0, 0, floor_height + standoff_height])\n'
+    result += '        pcb();\n\n'
+    result += '    }'
+
     for mount in case.pcb_mount:
         result += f'    // {mount[3]}\n'
         result += f'    translate([{mount[0][0]}, {mount[0][1]}, floor_height])\n'
         # This currently creates correct holes for the M3 threaded metal inserts I have. Not generic
         result += f'    mount({mount[1] + 0.2}, {mount[2]}, standoff_height);\n\n'
 
     for part in case.parts:
@@ -119,12 +149,12 @@
             continue
         result += f'    // {part.description}\n'
         z = 'floor_height'
         if part.offset_pcb:
             z = 'pcb_top'
         result += f'    translate([{part.position[0]}, {part.position[1]}, {z}])\n'
         if len(part.position) == 3:
-            result += f'    rotate([0, 0, {part.position[2] + 180}])\n'
+            result += f'    rotate([0, 0, {-part.position[2]}])\n'
         result += f'        {part.add}\n'
 
     result += '}\n'
     return result
```

### Comparing `turbocase-1.4.2/turbocase/vector.py` & `turbocase-1.5.0/turbocase/vector.py`

 * *Files identical despite different names*

### Comparing `turbocase-1.4.2/turbocase.egg-info/SOURCES.txt` & `turbocase-1.5.0/turbocase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

