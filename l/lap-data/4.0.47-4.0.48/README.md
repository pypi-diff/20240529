# Comparing `tmp/lap_data-4.0.47.tar.gz` & `tmp/lap_data-4.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lap_data-4.0.47.tar", last modified: Wed May 15 12:19:14 2024, max compression
+gzip compressed data, was "lap_data-4.0.48.tar", last modified: Wed May 29 08:07:46 2024, max compression
```

## Comparing `lap_data-4.0.47.tar` & `lap_data-4.0.48.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 12:19:14.856734 lap_data-4.0.47/
--rw-rw-rw-   0        0        0    35821 2022-10-20 13:06:49.000000 lap_data-4.0.47/LICENSE
--rw-rw-rw-   0        0        0      709 2024-05-15 12:19:14.856734 lap_data-4.0.47/PKG-INFO
--rw-rw-rw-   0        0        0      329 2022-10-20 13:06:49.000000 lap_data-4.0.47/README.md
--rw-rw-rw-   0        0        0       97 2022-10-20 13:06:49.000000 lap_data-4.0.47/pyproject.toml
--rw-rw-rw-   0        0        0       81 2024-05-15 12:19:14.860151 lap_data-4.0.47/setup.cfg
--rw-rw-rw-   0        0        0     1518 2024-05-04 22:11:23.000000 lap_data-4.0.47/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 12:19:14.794184 lap_data-4.0.47/src/
-drwxrwxrwx   0        0        0        0 2024-05-15 12:19:14.828795 lap_data-4.0.47/src/lap_data/
--rw-rw-rw-   0        0        0      197 2024-04-16 08:00:23.000000 lap_data-4.0.47/src/lap_data/__init__.py
--rw-rw-rw-   0        0        0    19940 2024-04-16 08:00:15.000000 lap_data-4.0.47/src/lap_data/lcmodel.py
-drwxrwxrwx   0        0        0        0 2024-05-15 12:19:14.855754 lap_data-4.0.47/src/lap_data.egg-info/
--rw-rw-rw-   0        0        0      709 2024-05-15 12:19:14.000000 lap_data-4.0.47/src/lap_data.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2024-05-15 12:19:14.000000 lap_data-4.0.47/src/lap_data.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 12:19:14.000000 lap_data-4.0.47/src/lap_data.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-15 12:19:14.000000 lap_data-4.0.47/src/lap_data.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-15 12:19:14.000000 lap_data-4.0.47/src/lap_data.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 08:07:46.036930 lap_data-4.0.48/
+-rw-rw-rw-   0        0        0    35821 2022-10-20 13:06:49.000000 lap_data-4.0.48/LICENSE
+-rw-rw-rw-   0        0        0      709 2024-05-29 08:07:46.036930 lap_data-4.0.48/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2022-10-20 13:06:49.000000 lap_data-4.0.48/README.md
+-rw-rw-rw-   0        0        0       97 2022-10-20 13:06:49.000000 lap_data-4.0.48/pyproject.toml
+-rw-rw-rw-   0        0        0       81 2024-05-29 08:07:46.036930 lap_data-4.0.48/setup.cfg
+-rw-rw-rw-   0        0        0     1518 2024-05-29 07:53:13.000000 lap_data-4.0.48/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:07:45.990058 lap_data-4.0.48/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 08:07:46.005697 lap_data-4.0.48/src/lap_data/
+-rw-rw-rw-   0        0        0      197 2024-05-29 07:51:59.000000 lap_data-4.0.48/src/lap_data/__init__.py
+-rw-rw-rw-   0        0        0    20274 2024-05-29 06:19:54.000000 lap_data-4.0.48/src/lap_data/lcmodel.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:07:46.036930 lap_data-4.0.48/src/lap_data.egg-info/
+-rw-rw-rw-   0        0        0      709 2024-05-29 08:07:45.000000 lap_data-4.0.48/src/lap_data.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2024-05-29 08:07:45.000000 lap_data-4.0.48/src/lap_data.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 08:07:45.000000 lap_data-4.0.48/src/lap_data.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-29 08:07:45.000000 lap_data-4.0.48/src/lap_data.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-29 08:07:45.000000 lap_data-4.0.48/src/lap_data.egg-info/top_level.txt
```

### Comparing `lap_data-4.0.47/LICENSE` & `lap_data-4.0.48/LICENSE`

 * *Files identical despite different names*

### Comparing `lap_data-4.0.47/PKG-INFO` & `lap_data-4.0.48/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: lap_data
-Version: 4.0.47
+Version: 4.0.48
 Summary: Laser Aided Profiler Data Access Library
 Author: Peter Demján
 Author-email: peter.demjan@gmail.com
 Keywords: database,graph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Database
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: deposit_gui<1.5,>=1.4.41
+Requires-Dist: deposit_gui<1.5,>=1.4.47
 
 Laser Aided Profiler Data Access Library
```

### Comparing `lap_data-4.0.47/setup.py` & `lap_data-4.0.48/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,11 +43,11 @@
 		"Operating System :: Microsoft :: Windows :: Windows 10",
 	],
 	keywords="database, graph",
 	package_dir={"": "src"},
 	packages=find_packages(where="src"),
 	python_requires=">=3.10, <4",
 	install_requires=[
-		'deposit_gui>=1.4.41, <1.5',
+		'deposit_gui>=1.4.47, <1.5',
 	],
 	cmdclass={'bdist_wheel': bdist_wheel},
 )
```

### Comparing `lap_data-4.0.47/src/lap_data/lcmodel.py` & `lap_data-4.0.48/src/lap_data/lcmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,14 +201,27 @@
 					classes.append(class1)
 				if class2 not in classes:
 					classes.append(class2)
 				if (name, class2, descr) not in descriptors:
 					descriptors.append((name, class2, descr))
 				relations.add((class1, rel, class2))
 		
+		# add class relations to relations
+		for class1 in classes:
+			cls1 = self.get_class(class1)
+			if cls1 is None:
+				continue
+			for cls2, label in cls1.get_relations():
+				if cls2.name not in classes:
+					continue
+				row = (class1, label, cls2.name)
+				if row in relations:
+					continue
+				relations.add(row)
+		
 		return classes, descriptors, relations
 	
 	def get_arc_structure(self):
 		
 		arc_cls, arc_descr, arc_rel = None, None, None
 		_, descriptors, relations = self.get_data_structure()
 		for name, cls, descr in descriptors:
```

### Comparing `lap_data-4.0.47/src/lap_data.egg-info/PKG-INFO` & `lap_data-4.0.48/src/lap_data.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: lap_data
-Version: 4.0.47
+Version: 4.0.48
 Summary: Laser Aided Profiler Data Access Library
 Author: Peter Demján
 Author-email: peter.demjan@gmail.com
 Keywords: database,graph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Database
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: deposit_gui<1.5,>=1.4.41
+Requires-Dist: deposit_gui<1.5,>=1.4.47
 
 Laser Aided Profiler Data Access Library
```

