# Comparing `tmp/rye_tui-0.2.1.tar.gz` & `tmp/rye_tui-0.2.2.tar.gz`

## Comparing `rye_tui-0.2.1.tar` & `rye_tui-0.2.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 rye_tui-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 rye_tui-0.2.1/.python-version
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 rye_tui-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 rye_tui-0.2.1/requirements-dev.lock
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 rye_tui-0.2.1/requirements.lock
--rw-r--r--   0        0        0   102536 2020-02-02 00:00:00.000000 rye_tui-0.2.1/images/image_rye_add.png
--rw-r--r--   0        0        0    53894 2020-02-02 00:00:00.000000 rye_tui-0.2.1/images/image_rye_config.png
--rw-r--r--   0        0        0    61490 2020-02-02 00:00:00.000000 rye_tui-0.2.1/images/image_rye_demo_preview.png
--rw-r--r--   0        0        0    51791 2020-02-02 00:00:00.000000 rye_tui-0.2.1/images/image_rye_general.png
--rw-r--r--   0        0        0    92020 2020-02-02 00:00:00.000000 rye_tui-0.2.1/images/image_rye_project.png
--rw-r--r--   0        0        0    56573 2020-02-02 00:00:00.000000 rye_tui-0.2.1/images/modals_screen_sketches.excalidraw
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 rye_tui-0.2.1/images/rye_favicon.svg
--rw-r--r--   0        0        0    69488 2020-02-02 00:00:00.000000 rye_tui-0.2.1/images/sketch.png
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 rye_tui-0.2.1/src/rye_tui/__init__.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 rye_tui-0.2.1/src/rye_tui/app.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 rye_tui-0.2.1/src/rye_tui/cli_parser.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 rye_tui-0.2.1/src/rye_tui/config.py
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 rye_tui-0.2.1/src/rye_tui/constants.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 rye_tui-0.2.1/src/rye_tui/tooltips.py
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 rye_tui-0.2.1/src/rye_tui/tui.py
--rw-r--r--   0        0        0     6864 2020-02-02 00:00:00.000000 rye_tui-0.2.1/src/rye_tui/utils.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 rye_tui-0.2.1/src/rye_tui/assets/modal_screens.css
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 rye_tui-0.2.1/src/rye_tui/assets/tui.css
--rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 rye_tui-0.2.1/src/rye_tui/components/config_tab.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 rye_tui-0.2.1/src/rye_tui/components/general_tab.py
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 rye_tui-0.2.1/src/rye_tui/components/helper_widgets.py
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 rye_tui-0.2.1/src/rye_tui/components/mainframe.py
--rw-r--r--   0        0        0    12970 2020-02-02 00:00:00.000000 rye_tui-0.2.1/src/rye_tui/components/modals.py
--rw-r--r--   0        0        0     7821 2020-02-02 00:00:00.000000 rye_tui-0.2.1/src/rye_tui/components/projects_tab.py
--rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 rye_tui-0.2.1/src/rye_tui/static/rye_image.jpg
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 rye_tui-0.2.1/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 rye_tui-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 rye_tui-0.2.1/README.md
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 rye_tui-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 rye_tui-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 rye_tui-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 rye_tui-0.2.2/.python-version
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 rye_tui-0.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 rye_tui-0.2.2/requirements-dev.lock
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 rye_tui-0.2.2/requirements.lock
+-rw-r--r--   0        0        0   102536 2020-02-02 00:00:00.000000 rye_tui-0.2.2/images/image_rye_add.png
+-rw-r--r--   0        0        0    53894 2020-02-02 00:00:00.000000 rye_tui-0.2.2/images/image_rye_config.png
+-rw-r--r--   0        0        0    61490 2020-02-02 00:00:00.000000 rye_tui-0.2.2/images/image_rye_demo_preview.png
+-rw-r--r--   0        0        0    51791 2020-02-02 00:00:00.000000 rye_tui-0.2.2/images/image_rye_general.png
+-rw-r--r--   0        0        0    92020 2020-02-02 00:00:00.000000 rye_tui-0.2.2/images/image_rye_project.png
+-rw-r--r--   0        0        0    56573 2020-02-02 00:00:00.000000 rye_tui-0.2.2/images/modals_screen_sketches.excalidraw
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 rye_tui-0.2.2/images/rye_favicon.svg
+-rw-r--r--   0        0        0    69488 2020-02-02 00:00:00.000000 rye_tui-0.2.2/images/sketch.png
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 rye_tui-0.2.2/src/rye_tui/__init__.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 rye_tui-0.2.2/src/rye_tui/app.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 rye_tui-0.2.2/src/rye_tui/cli_parser.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 rye_tui-0.2.2/src/rye_tui/config.py
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 rye_tui-0.2.2/src/rye_tui/constants.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 rye_tui-0.2.2/src/rye_tui/tooltips.py
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 rye_tui-0.2.2/src/rye_tui/tui.py
+-rw-r--r--   0        0        0     6864 2020-02-02 00:00:00.000000 rye_tui-0.2.2/src/rye_tui/utils.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 rye_tui-0.2.2/src/rye_tui/assets/modal_screens.css
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 rye_tui-0.2.2/src/rye_tui/assets/tui.css
+-rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 rye_tui-0.2.2/src/rye_tui/components/config_tab.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 rye_tui-0.2.2/src/rye_tui/components/general_tab.py
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 rye_tui-0.2.2/src/rye_tui/components/helper_widgets.py
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 rye_tui-0.2.2/src/rye_tui/components/mainframe.py
+-rw-r--r--   0        0        0    12983 2020-02-02 00:00:00.000000 rye_tui-0.2.2/src/rye_tui/components/modals.py
+-rw-r--r--   0        0        0     7821 2020-02-02 00:00:00.000000 rye_tui-0.2.2/src/rye_tui/components/projects_tab.py
+-rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 rye_tui-0.2.2/src/rye_tui/static/rye_image.jpg
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 rye_tui-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 rye_tui-0.2.2/LICENSE.txt
+-rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 rye_tui-0.2.2/README.md
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 rye_tui-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5048 2020-02-02 00:00:00.000000 rye_tui-0.2.2/PKG-INFO
```

### Comparing `rye_tui-0.2.1/requirements-dev.lock` & `rye_tui-0.2.2/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/requirements.lock` & `rye_tui-0.2.2/requirements.lock`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/images/image_rye_add.png` & `rye_tui-0.2.2/images/image_rye_add.png`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/images/image_rye_config.png` & `rye_tui-0.2.2/images/image_rye_config.png`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/images/image_rye_demo_preview.png` & `rye_tui-0.2.2/images/image_rye_demo_preview.png`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/images/image_rye_general.png` & `rye_tui-0.2.2/images/image_rye_general.png`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/images/image_rye_project.png` & `rye_tui-0.2.2/images/image_rye_project.png`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/images/modals_screen_sketches.excalidraw` & `rye_tui-0.2.2/images/modals_screen_sketches.excalidraw`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/images/rye_favicon.svg` & `rye_tui-0.2.2/images/rye_favicon.svg`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/images/sketch.png` & `rye_tui-0.2.2/images/sketch.png`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/src/rye_tui/cli_parser.py` & `rye_tui-0.2.2/src/rye_tui/cli_parser.py`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/src/rye_tui/config.py` & `rye_tui-0.2.2/src/rye_tui/config.py`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/src/rye_tui/constants.py` & `rye_tui-0.2.2/src/rye_tui/constants.py`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/src/rye_tui/tooltips.py` & `rye_tui-0.2.2/src/rye_tui/tooltips.py`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/src/rye_tui/tui.py` & `rye_tui-0.2.2/src/rye_tui/tui.py`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/src/rye_tui/utils.py` & `rye_tui-0.2.2/src/rye_tui/utils.py`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/src/rye_tui/assets/modal_screens.css` & `rye_tui-0.2.2/src/rye_tui/assets/modal_screens.css`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/src/rye_tui/assets/tui.css` & `rye_tui-0.2.2/src/rye_tui/assets/tui.css`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/src/rye_tui/components/config_tab.py` & `rye_tui-0.2.2/src/rye_tui/components/config_tab.py`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/src/rye_tui/components/general_tab.py` & `rye_tui-0.2.2/src/rye_tui/components/general_tab.py`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/src/rye_tui/components/helper_widgets.py` & `rye_tui-0.2.2/src/rye_tui/components/helper_widgets.py`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/src/rye_tui/components/mainframe.py` & `rye_tui-0.2.2/src/rye_tui/components/mainframe.py`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/src/rye_tui/components/modals.py` & `rye_tui-0.2.2/src/rye_tui/components/modals.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,16 +114,16 @@
 class ModalRyePin(ModalScreen):
     CSS_PATH: Path = Path("../assets/modal_screens.css")
 
     def compose(self) -> Iterable[Widget]:
         with Vertical():
             yield Label(f"Pin Python Version of [blue]{self.app.project['name']}[/]")
             self.pin_input = Input(
-                placeholder="enter python version to pin",
-                validators=[Regex("^3\.(?:[89]|1[012])$")],
+                placeholder="enter python version to pin (e.g. 3.11)",
+                validators=[Regex(r"^3\.(?:[89]|1[012])$")],
                 id="input_pin_python",
             )
             yield self.pin_input
             with Horizontal(classes="horizontal-conf-cancel"):
                 yield Button(
                     "continue", variant="success", classes="btn-continue", disabled=True
                 )
```

### Comparing `rye_tui-0.2.1/src/rye_tui/components/projects_tab.py` & `rye_tui-0.2.2/src/rye_tui/components/projects_tab.py`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/src/rye_tui/static/rye_image.jpg` & `rye_tui-0.2.2/src/rye_tui/static/rye_image.jpg`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/LICENSE.txt` & `rye_tui-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rye_tui-0.2.1/README.md` & `rye_tui-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -70,17 +70,19 @@
 ![general_image](https://raw.githubusercontent.com/Zaloog/rye-tui/main/images/image_rye_general.png)
 
 ### Config Tab
 The Config Tab can be used to change rye's underlying config.
 `default` and `sources` sections functionality is still missing currently
 ![config_image](https://raw.githubusercontent.com/Zaloog/rye-tui/main/images/image_rye_config.png)
 
+## Feedback and Issues
+Feel free to reach out and share your feedback, or open an Issue, if something doesnt work as expected.
+Also check the [Changelog](https://github.com/Zaloog/rye-tui/blob/main/CHANGELOG.md) for new updates.
 
-
-# Open Points:
+## Open Points:
 - projects tab
     - project_list
         - [ ] further check if folder is actually a rye project
         - [ ] edit button functionality
     - button functionalities
         - [ ] Add Flags to Rye Init and Rye add
         - [ ] publish when wheels in dist/*
@@ -90,14 +92,13 @@
     - [ ] source adding/removing
 - other/general stuff
     - [ ] Add more tooltips
     - [ ] focus widget color?
     - [ ] Docs/Readme
     - [ ] Input Validators for Path
 
-
 [XDG]: https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html
 [platformdirs]: https://platformdirs.readthedocs.io/en/latest/
 [textual]: https://textual.textualize.io
 [pipx]: https://github.com/pypa/pipx
 [rye]: https://rye-up.com
 [PyPi]: https://pypi.org/project/rye-tui/
```

### Comparing `rye_tui-0.2.1/pyproject.toml` & `rye_tui-0.2.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rye-tui"
-version = "0.2.1"
+version = "0.2.2"
 description = "Rye meets Textual. Manage your python projects with a Tui"
 authors = [
     { name = "Zaloog", email = "gramslars@gmail.com" }
 ]
 dependencies = [
     "textual>=0.63.0",
     "rich-pixels>=3.0.1",
```

### Comparing `rye_tui-0.2.1/PKG-INFO` & `rye_tui-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rye-tui
-Version: 0.2.1
+Version: 0.2.2
 Summary: Rye meets Textual. Manage your python projects with a Tui
 Project-URL: Repository, https://github.com/Zaloog/rye-tui
 Project-URL: Changelog, https://github.com/Zaloog/rye-tui/blob/main/CHANGELOG.md
 Author-email: Zaloog <gramslars@gmail.com>
 License: MIT
 License-File: LICENSE.txt
 Keywords: python,rye,textual,tui
@@ -96,17 +96,19 @@
 ![general_image](https://raw.githubusercontent.com/Zaloog/rye-tui/main/images/image_rye_general.png)
 
 ### Config Tab
 The Config Tab can be used to change rye's underlying config.
 `default` and `sources` sections functionality is still missing currently
 ![config_image](https://raw.githubusercontent.com/Zaloog/rye-tui/main/images/image_rye_config.png)
 
+## Feedback and Issues
+Feel free to reach out and share your feedback, or open an Issue, if something doesnt work as expected.
+Also check the [Changelog](https://github.com/Zaloog/rye-tui/blob/main/CHANGELOG.md) for new updates.
 
-
-# Open Points:
+## Open Points:
 - projects tab
     - project_list
         - [ ] further check if folder is actually a rye project
         - [ ] edit button functionality
     - button functionalities
         - [ ] Add Flags to Rye Init and Rye add
         - [ ] publish when wheels in dist/*
@@ -116,14 +118,13 @@
     - [ ] source adding/removing
 - other/general stuff
     - [ ] Add more tooltips
     - [ ] focus widget color?
     - [ ] Docs/Readme
     - [ ] Input Validators for Path
 
-
 [XDG]: https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html
 [platformdirs]: https://platformdirs.readthedocs.io/en/latest/
 [textual]: https://textual.textualize.io
 [pipx]: https://github.com/pypa/pipx
 [rye]: https://rye-up.com
 [PyPi]: https://pypi.org/project/rye-tui/
```

