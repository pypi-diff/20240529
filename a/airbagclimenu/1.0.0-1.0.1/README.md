# Comparing `tmp/airbagclimenu-1.0.0.tar.gz` & `tmp/airbagclimenu-1.0.1.tar.gz`

## Comparing `airbagclimenu-1.0.0.tar` & `airbagclimenu-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    64770 2020-02-02 00:00:00.000000 airbagclimenu-1.0.0/qrcode.png
--rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 airbagclimenu-1.0.0/src/airbagclimenu/Menu.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airbagclimenu-1.0.0/src/airbagclimenu/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 airbagclimenu-1.0.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 airbagclimenu-1.0.0/LICENSE
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 airbagclimenu-1.0.0/README.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 airbagclimenu-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 airbagclimenu-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    64770 2020-02-02 00:00:00.000000 airbagclimenu-1.0.1/qrcode.png
+-rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 airbagclimenu-1.0.1/src/airbagclimenu/Menu.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airbagclimenu-1.0.1/src/airbagclimenu/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 airbagclimenu-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 airbagclimenu-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 airbagclimenu-1.0.1/README.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 airbagclimenu-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 airbagclimenu-1.0.1/PKG-INFO
```

### Comparing `airbagclimenu-1.0.0/qrcode.png` & `airbagclimenu-1.0.1/qrcode.png`

 * *Files identical despite different names*

### Comparing `airbagclimenu-1.0.0/src/airbagclimenu/Menu.py` & `airbagclimenu-1.0.1/src/airbagclimenu/Menu.py`

 * *Files identical despite different names*

### Comparing `airbagclimenu-1.0.0/LICENSE` & `airbagclimenu-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `airbagclimenu-1.0.0/README.md` & `airbagclimenu-1.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -24,31 +24,40 @@
 source <name-of-venv>/bin/activate
 ```
 
 When you have activated the virtual environment and running from within it, you can install ```airbagclimenu```, with one of the following commands: 
 
 Windows:
 ```bat
-py -m pip install --index-url https://test.pypi.org/simple/ --no-deps airbagclimenu
+pip3 install airbagclimenu
 ```
 MacOS / Linux: 
 ```Bash
-python3 -m pip install --index-url https://test.pypi.org/simple/ --no-deps airbagclimenu
+pip install airbagclimenu
 ```
 
 ## Usage
 Make sure to use this exact ```import``` statement for the following to work:
 ```Python
 from airbagclimenu import Menu
 ```
 To create and run the menu, you do as follows:
 ```Python
 menu = Menu.CLIMenu()
 menu.run()
 ```
+The construcor for the menu takes an optional argument ```quit_stmt``` which is ```True``` by default. It provides an option to quit the menu that you don't have to add yourself. 
+When the quit option is present, the menu will run indefinitly, meaning you don't have to restart it for each time after choosing an option. This loop is however not present if 
+the quit statement is not there. If you which not to have the quit statement, you simply pass the argument ```False``` into the construcor when creating the object. 
+
+
+The ```run``` method also takes an optional argument ```clear_screen```, which determines whether the screen should clear after each option. It's default value is
+```True``` but can easily be switched of by giving the argument ```False``` to the ```run``` method.
+
+
 To add alternatives in the menu you have two options. You can add a function that will execute when that option is chosen, or you can add a submenu, which reveals more options when chosen. 
 ### add_menu_option(menu_option: MenuOption)
 This method takes one parameter which should be of type ```MenuOption```. See example usecase below:
 ```Python
 menu = Menu.CLIMenu()
 # You can add a submenu directly by creating it as a parameter like this
 menu.add_menu_option(Menu.MenuOption("Submenu 1"))
```

### Comparing `airbagclimenu-1.0.0/pyproject.toml` & `airbagclimenu-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "airbagclimenu"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name = "Anton Norman", email="normananton03@gmail.com" },
 ]
 description = "A python package that makes it easy and intuitive to create good looking CLI menus"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `airbagclimenu-1.0.0/PKG-INFO` & `airbagclimenu-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: airbagclimenu
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python package that makes it easy and intuitive to create good looking CLI menus
 Project-URL: Homepage, https://github.com/Airbag65/CLI-Menu
 Project-URL: Issues, https://github.com/Airbag65/CLI-Menu/issues
 Author-email: Anton Norman <normananton03@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -38,31 +38,40 @@
 source <name-of-venv>/bin/activate
 ```
 
 When you have activated the virtual environment and running from within it, you can install ```airbagclimenu```, with one of the following commands: 
 
 Windows:
 ```bat
-py -m pip install --index-url https://test.pypi.org/simple/ --no-deps airbagclimenu
+pip3 install airbagclimenu
 ```
 MacOS / Linux: 
 ```Bash
-python3 -m pip install --index-url https://test.pypi.org/simple/ --no-deps airbagclimenu
+pip install airbagclimenu
 ```
 
 ## Usage
 Make sure to use this exact ```import``` statement for the following to work:
 ```Python
 from airbagclimenu import Menu
 ```
 To create and run the menu, you do as follows:
 ```Python
 menu = Menu.CLIMenu()
 menu.run()
 ```
+The construcor for the menu takes an optional argument ```quit_stmt``` which is ```True``` by default. It provides an option to quit the menu that you don't have to add yourself. 
+When the quit option is present, the menu will run indefinitly, meaning you don't have to restart it for each time after choosing an option. This loop is however not present if 
+the quit statement is not there. If you which not to have the quit statement, you simply pass the argument ```False``` into the construcor when creating the object. 
+
+
+The ```run``` method also takes an optional argument ```clear_screen```, which determines whether the screen should clear after each option. It's default value is
+```True``` but can easily be switched of by giving the argument ```False``` to the ```run``` method.
+
+
 To add alternatives in the menu you have two options. You can add a function that will execute when that option is chosen, or you can add a submenu, which reveals more options when chosen. 
 ### add_menu_option(menu_option: MenuOption)
 This method takes one parameter which should be of type ```MenuOption```. See example usecase below:
 ```Python
 menu = Menu.CLIMenu()
 # You can add a submenu directly by creating it as a parameter like this
 menu.add_menu_option(Menu.MenuOption("Submenu 1"))
```

