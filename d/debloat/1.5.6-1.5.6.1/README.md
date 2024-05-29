# Comparing `tmp/debloat-1.5.6.tar.gz` & `tmp/debloat-1.5.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debloat-1.5.6.tar", last modified: Sat May 18 14:00:12 2024, max compression
+gzip compressed data, was "debloat-1.5.6.1.tar", last modified: Tue May 28 12:43:25 2024, max compression
```

## Comparing `debloat-1.5.6.tar` & `debloat-1.5.6.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 14:00:12.555950 debloat-1.5.6/
--rw-rw-rw-   0        0        0     1525 2023-03-27 10:23:04.000000 debloat-1.5.6/LICENSE
--rw-rw-rw-   0        0        0     8708 2024-05-18 14:00:12.555451 debloat-1.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     8088 2024-05-18 13:59:44.000000 debloat-1.5.6/README.md
--rw-rw-rw-   0        0        0      790 2024-05-18 13:59:45.000000 debloat-1.5.6/pyproject.toml
--rw-rw-rw-   0        0        0      166 2024-05-18 14:00:12.557985 debloat-1.5.6/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-03-27 10:34:30.000000 debloat-1.5.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-18 14:00:12.408424 debloat-1.5.6/src/
-drwxrwxrwx   0        0        0        0 2024-05-18 14:00:12.477436 debloat-1.5.6/src/debloat/
--rw-rw-rw-   0        0        0        0 2023-07-11 19:08:33.000000 debloat-1.5.6/src/debloat/__init__.py
--rw-rw-rw-   0        0        0      495 2023-07-11 19:08:33.000000 debloat-1.5.6/src/debloat/auxiliary.py
--rw-rw-rw-   0        0        0     4745 2024-05-18 13:57:59.000000 debloat-1.5.6/src/debloat/gui.py
--rw-rw-rw-   0        0        0     2595 2024-05-18 13:57:59.000000 debloat-1.5.6/src/debloat/main.py
--rw-rw-rw-   0        0        0     2936 2024-05-18 13:59:45.000000 debloat-1.5.6/src/debloat/performanceTest.py
--rw-rw-rw-   0        0        0    27497 2024-05-18 13:59:45.000000 debloat-1.5.6/src/debloat/processor.py
--rw-rw-rw-   0        0        0     1486 2023-08-18 12:49:16.000000 debloat-1.5.6/src/debloat/processor.pyi
-drwxrwxrwx   0        0        0        0 2024-05-18 14:00:12.515443 debloat-1.5.6/src/debloat/tests/
--rw-rw-rw-   0        0        0        0 2023-07-11 19:08:33.000000 debloat-1.5.6/src/debloat/tests/__init__.py
--rw-rw-rw-   0        0        0      561 2023-07-11 19:08:33.000000 debloat-1.5.6/src/debloat/tests/debloat_test.py
-drwxrwxrwx   0        0        0        0 2024-05-18 14:00:12.551949 debloat-1.5.6/src/debloat/utilities/
--rw-rw-rw-   0        0        0        0 2023-07-11 19:08:33.000000 debloat-1.5.6/src/debloat/utilities/__init__.py
--rw-rw-rw-   0        0        0    51764 2024-02-21 18:11:20.000000 debloat-1.5.6/src/debloat/utilities/nsisParser.py
--rw-rw-rw-   0        0        0    23201 2024-02-21 18:11:20.000000 debloat-1.5.6/src/debloat/utilities/pyflate.py
--rw-rw-rw-   0        0        0    21202 2023-08-28 21:25:25.000000 debloat-1.5.6/src/debloat/utilities/readers.py
--rw-rw-rw-   0        0        0      746 2023-07-11 19:08:33.000000 debloat-1.5.6/src/debloat/utilities/rsrc.py
-drwxrwxrwx   0        0        0        0 2024-05-18 14:00:12.553951 debloat-1.5.6/src/debloat.egg-info/
--rw-rw-rw-   0        0        0     8708 2024-05-18 14:00:12.000000 debloat-1.5.6/src/debloat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      663 2024-05-18 14:00:12.000000 debloat-1.5.6/src/debloat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 14:00:12.000000 debloat-1.5.6/src/debloat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2024-05-18 14:00:12.000000 debloat-1.5.6/src/debloat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2024-05-18 14:00:12.000000 debloat-1.5.6/src/debloat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-18 14:00:12.000000 debloat-1.5.6/src/debloat.egg-info/top_level.txt
+drwxrwxr-x   0 kyhra     (1000) kyhra     (1000)        0 2024-05-28 12:43:25.019246 debloat-1.5.6.1/
+-rw-rw-r--   0 kyhra     (1000) kyhra     (1000)     1497 2023-07-11 19:08:33.000000 debloat-1.5.6.1/LICENSE
+-rw-r--r--   0 kyhra     (1000) kyhra     (1000)     8589 2024-05-28 12:43:25.019246 debloat-1.5.6.1/PKG-INFO
+-rw-rw-r--   0 kyhra     (1000) kyhra     (1000)     7983 2024-05-18 09:38:37.000000 debloat-1.5.6.1/README.md
+-rw-rw-r--   0 kyhra     (1000) kyhra     (1000)      761 2024-05-28 12:41:49.000000 debloat-1.5.6.1/pyproject.toml
+-rw-rw-r--   0 kyhra     (1000) kyhra     (1000)      151 2024-05-28 12:43:25.019246 debloat-1.5.6.1/setup.cfg
+-rw-rw-r--   0 kyhra     (1000) kyhra     (1000)       68 2023-07-11 19:08:33.000000 debloat-1.5.6.1/setup.py
+drwxrwxr-x   0 kyhra     (1000) kyhra     (1000)        0 2024-05-28 12:43:25.015246 debloat-1.5.6.1/src/
+drwxrwxr-x   0 kyhra     (1000) kyhra     (1000)        0 2024-05-28 12:43:25.015246 debloat-1.5.6.1/src/debloat/
+-rw-rw-r--   0 kyhra     (1000) kyhra     (1000)        0 2023-07-11 19:08:33.000000 debloat-1.5.6.1/src/debloat/__init__.py
+-rw-rw-r--   0 kyhra     (1000) kyhra     (1000)      495 2023-07-11 19:08:33.000000 debloat-1.5.6.1/src/debloat/auxiliary.py
+-rw-rw-r--   0 kyhra     (1000) kyhra     (1000)     4633 2024-04-20 10:35:56.000000 debloat-1.5.6.1/src/debloat/gui.py
+-rw-rw-r--   0 kyhra     (1000) kyhra     (1000)     2528 2024-04-20 10:37:42.000000 debloat-1.5.6.1/src/debloat/main.py
+-rw-rw-r--   0 kyhra     (1000) kyhra     (1000)     2871 2024-05-28 12:41:49.000000 debloat-1.5.6.1/src/debloat/performanceTest.py
+-rw-rw-r--   0 kyhra     (1000) kyhra     (1000)    26909 2024-05-28 12:41:49.000000 debloat-1.5.6.1/src/debloat/processor.py
+-rw-rw-r--   0 kyhra     (1000) kyhra     (1000)     1464 2023-08-13 14:50:36.000000 debloat-1.5.6.1/src/debloat/processor.pyi
+drwxrwxr-x   0 kyhra     (1000) kyhra     (1000)        0 2024-05-28 12:43:25.015246 debloat-1.5.6.1/src/debloat/tests/
+-rw-rw-r--   0 kyhra     (1000) kyhra     (1000)        0 2023-07-11 19:08:33.000000 debloat-1.5.6.1/src/debloat/tests/__init__.py
+-rw-rw-r--   0 kyhra     (1000) kyhra     (1000)      561 2023-07-11 19:08:33.000000 debloat-1.5.6.1/src/debloat/tests/debloat_test.py
+drwxrwxr-x   0 kyhra     (1000) kyhra     (1000)        0 2024-05-28 12:43:25.019246 debloat-1.5.6.1/src/debloat/utilities/
+-rw-rw-r--   0 kyhra     (1000) kyhra     (1000)        0 2023-07-11 19:08:33.000000 debloat-1.5.6.1/src/debloat/utilities/__init__.py
+-rw-rw-r--   0 kyhra     (1000) kyhra     (1000)    50428 2024-02-21 11:55:19.000000 debloat-1.5.6.1/src/debloat/utilities/nsisParser.py
+-rw-rw-r--   0 kyhra     (1000) kyhra     (1000)    22511 2024-02-19 19:41:26.000000 debloat-1.5.6.1/src/debloat/utilities/pyflate.py
+-rw-rw-r--   0 kyhra     (1000) kyhra     (1000)    20599 2023-08-28 17:17:19.000000 debloat-1.5.6.1/src/debloat/utilities/readers.py
+-rw-rw-r--   0 kyhra     (1000) kyhra     (1000)      746 2023-07-11 19:08:33.000000 debloat-1.5.6.1/src/debloat/utilities/rsrc.py
+drwxrwxr-x   0 kyhra     (1000) kyhra     (1000)        0 2024-05-28 12:43:25.019246 debloat-1.5.6.1/src/debloat.egg-info/
+-rw-r--r--   0 kyhra     (1000) kyhra     (1000)     8589 2024-05-28 12:43:25.000000 debloat-1.5.6.1/src/debloat.egg-info/PKG-INFO
+-rw-rw-r--   0 kyhra     (1000) kyhra     (1000)      663 2024-05-28 12:43:25.000000 debloat-1.5.6.1/src/debloat.egg-info/SOURCES.txt
+-rw-rw-r--   0 kyhra     (1000) kyhra     (1000)        1 2024-05-28 12:43:25.000000 debloat-1.5.6.1/src/debloat.egg-info/dependency_links.txt
+-rw-rw-r--   0 kyhra     (1000) kyhra     (1000)       77 2024-05-28 12:43:25.000000 debloat-1.5.6.1/src/debloat.egg-info/entry_points.txt
+-rw-rw-r--   0 kyhra     (1000) kyhra     (1000)       36 2024-05-28 12:43:25.000000 debloat-1.5.6.1/src/debloat.egg-info/requires.txt
+-rw-rw-r--   0 kyhra     (1000) kyhra     (1000)        8 2024-05-28 12:43:25.000000 debloat-1.5.6.1/src/debloat.egg-info/top_level.txt
```

### Comparing `debloat-1.5.6/LICENSE` & `debloat-1.5.6.1/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-BSD 3-Clause License
-
-Copyright (c) 2023, Squiblydoo
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2023, Squiblydoo
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `debloat-1.5.6/PKG-INFO` & `debloat-1.5.6.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,121 +1,105 @@
-Metadata-Version: 2.1
-Name: debloat
-Version: 1.5.6
-Summary: Debloat is an tool to remove excess garbage from bloated executables.
-Author-email: Squiblydoo <Squiblydoo@pm.me>
-Project-URL: Homepage, https://github.com/Squiblydoo/debloat
-Project-URL: Bug Tracker, https://github.com/Squiblydoo/debloat/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: tkinterdnd2>=0.3.0
-Requires-Dist: pefile>=2023.2.0
-
-![debloat](https://user-images.githubusercontent.com/77356206/215351855-9f89c298-36b4-4234-89b5-dc3f26d1f8b0.png)
-
-# Debloat
-Debloat is a GUI and CLI tool to remove excess garbage from bloated executables.
-
-By excess garbage, I mean 100 - 800 MB of junk bytes added to a binary to keep it from going into a sandbox. This method of adding junk is called "inflating" or "pumping" a binary. Debloat currently handles the 10 most common inflation tactics.
-
-Being built with Python, the application can easily be leveraged in other workflows. Currently, debloat is used by [CCCS's AssemblyLine](https://www.cyber.gc.ca/en/tools-services/assemblyline) and [CERT Polska's MWDB](https://github.com/CERT-Polska/karton-archive-extractor).
-
- The program can be compiled for Windows, MacOS, Linux. The GUI and CLI have minimal options: it is intended to be as simple as possible and the logic within the program handles the different use cases automatically.
-
-Compiled binaries have already been included in the [Releases](https://github.com/Squiblydoo/debloat/releases/).
-
-The debloat can installed using `pip install debloat`. Use `debloat` to launch the CLI and `debloat-gui` to launch the GUI.
-
-For advanced users, Debloat can also be imported into other scripts and the processing functions can be called individually.
-
-## How to use the GUI?
-The GUI of Debloat intends to be as intuitive as possible.
-When launched, you can drag and drop bloated file onto the text bar and press the "Process file" button.
-Some technical information will be printed to the scrolling textbox and the file without bloat will be written to the directory the file was pulled from.
-Sound easy? It is!
-
-Processing files will take a few seconds.<br>
-![image](https://github.com/Squiblydoo/debloat/assets/77356206/3d2756cd-bc83-44e8-b223-edd8ed464369)
-
-
-## How to use the CLI?
-After installing using `pip install debloat` use the command `debloat`.<br>
-`debloat` can take two arguments. The first argument is required: the file to debloat. The second argument is optional: the output location. When no output is provided, it will be written to the same directory as the original file.
-
-The gui can also be launched from the CLI using the command `debloat-gui`.
-
-## Does it always work?
-Not yet.
-My unscientific guess is that it should work for every 9 of 10 binaries. There are specific usecases I know where it does not work and I am working to implement solutions for those usecases. 
-
-In previous versions, `debloat` could accidentally remove too much of the binary. That is no longer the case unless you use the "--last-ditch" switch. If you ever need this switch, consider sharing the sample for additional analysis. This option has now been added to the GUI. Functionally, what the function does is it will remove the whole overlay, if there is one. In some cases this is necessary as no pattern for the junk was found---this is most commonly the case in samples that do not compress well.
-
-## Use Cases (Images from [Malcat](https://malcat.fr/))
-### Full support
-- [x] Bloat appended to the end of a Signed PE.<br>
-In the image below, the bloat has been appended to the end of the executable. <br>
-![Screenshot 2023-02-11 at 3 32 36 PM](https://user-images.githubusercontent.com/77356206/218279963-00780b59-8227-47dd-a0af-41096f6ae17b.png)
-
-- [X] Signed or Unsigned Packed executable.<br>
-In the image below, the bloat has been appended to the executable after packing. <br>
-![Screenshot 2023-02-11 at 3 44 10 PM](https://user-images.githubusercontent.com/77356206/218280433-6dbcf51a-68c8-48e1-a89a-ad0b818a0afc.png)
-
-- [X] Signed executable includes bloat in the .rsrc section of the PE.<br>
-In the image below, the bloat is identified as in the .rsrc section and is removed from the PE.<br>
-![Screenshot 2023-02-11 at 3 35 21 PM](https://user-images.githubusercontent.com/77356206/218280086-7cd548f8-e16b-4290-9283-a8a848de1419.png)
-
-- [X] Cases where bloat is added inside a PE Section.<br>
-In the image below, the bloat has been included in a PE section named [0]. <br>
-![Screenshot 2023-02-11 at 3 26 52 PM](https://user-images.githubusercontent.com/77356206/218279753-ed2c9102-482a-4639-aeb1-df8efc9c4e2e.png)
-
-- [X] Cases where the executable is a Nullsoft Scriptable Installer System executable (NSIS aka Nullsoft)
-These exe are installers that may contain one or more files. The files contained may or may not be malicious. (Sometimes actors will add files simply for increasing the file size.) All files within the installer are extracted to a new directory. The directory also contains the script for the installer which can be consulted to determine which files may be malicious.
-In the image below, Malcat has identified the executable as a NSIS installer.
-![image](https://github.com/Squiblydoo/debloat/assets/77356206/86780abc-da4b-4808-bccb-733d97fa80d8)
-
-# Partial Support
-
-- [X] Cases where the junk is too random and the entropy is too high. In these cases, a switch/option called "--last-ditch" 
-
-### Other use cases
-There are use cases where the tool does not work. However, I plan to solve for them before publishing too much about them.
-
-## Why?
-There appear to be a limited number of tools to easily process bloated executables. The two tools I have seen the most are “foremost” which is intended for recovering binaries from a disk image and “pecheck”.
-
-[Foremost](https://www.kali.org/tools/foremost/) works best in instances where the junk bytes are null (0x00) and it struggles when the binary has a fake or real signature. Its use in removing bloat from files is not its original purpose.
-
-[Pecheck](https://github.com/DidierStevens/DidierStevensSuite/blob/master/pecheck.py) has been developed over 14+ years and has some confusing commandline options. The option to remove bloated content is not the primary function of the script. Pecheck has to be combined with another tool ([disitool](https://blog.didierstevens.com/programs/disitool/)) in order to handle signed executables. In my experience, there are other times where pecheck can get confused and return an executable twice the size of the original bloated executable. All these factors seem OK if you are handling a small number of binaries, but as the number of binaries and methods increase, a tool specific to removing bloat is needed.
-
-[Binary Refinery](https://github.com/binref/refinery) is an amazing tool. It was written with the intention of being a [CyberChef](https://github.com/gchq/CyberChef) of the commandline. While both tools are amazing, they both have a shortcoming that requires the user to know what formulas should be applied. 
-
-There are good solid manual methods to remove bloat from binaries, but these methods can be tedious and not all analysts have the skills to do this. This tool removes the burden of needing to know how to manually remove bloat. Additionally, it allows for better scale. The principles used in the script allow allow for better scale if automation is desired.
-
-
-## How to build? 
-Follow the build commands appropriate to your platform. The main difference between build commands is the format of the icon.
-<br>
-MacOS<br>
-`pyinstaller --onefile --noconsole --additional-hooks-dir=./hook --icon=debloat.icns gui.py`
-
-Windows<br>
-`pyinstaller --onefile  --noconsole  --additional-hooks-dir=./hook --icon=debloat.ico gui.py`
-
-Linux<br> 
-`pyinstaller --onefile --noconsole --icon=debloat.ico --collect-all tkinterdnd2 gui.py`
-
-## Want to discuss?
-Consider joining the [debloat Discord](discord.gg/dvGXKaY5qr).
-
-## Credits
-Big shoutout to Jesko Hüttenhain creator of [Binary Refinery](https://github.com/binref/refinery). The NSIS extraction is based on his reverse engineering of the NSIS file format. Check out Binary Refinery if you have not.
-
-## Where is this project going next?
-Batch processing: process all files in a directory and produce a report.
-
-Better support for using processing methods outside of debloat.
-
-Support for debloating without unzipping.
+![debloat](https://user-images.githubusercontent.com/77356206/215351855-9f89c298-36b4-4234-89b5-dc3f26d1f8b0.png)
+
+# Debloat
+Debloat is a GUI and CLI tool to remove excess garbage from bloated executables.
+
+By excess garbage, I mean 100 - 800 MB of junk bytes added to a binary to keep it from going into a sandbox. This method of adding junk is called "inflating" or "pumping" a binary. Debloat currently handles the 10 most common inflation tactics.
+
+Being built with Python, the application can easily be leveraged in other workflows. Currently, debloat is used by [CCCS's AssemblyLine](https://www.cyber.gc.ca/en/tools-services/assemblyline) and [CERT Polska's MWDB](https://github.com/CERT-Polska/karton-archive-extractor).
+
+ The program can be compiled for Windows, MacOS, Linux. The GUI and CLI have minimal options: it is intended to be as simple as possible and the logic within the program handles the different use cases automatically.
+
+Compiled binaries have already been included in the [Releases](https://github.com/Squiblydoo/debloat/releases/).
+
+The debloat can installed using `pip install debloat`. Use `debloat` to launch the CLI and `debloat-gui` to launch the GUI.
+
+For advanced users, Debloat can also be imported into other scripts and the processing functions can be called individually.
+
+## How to use the GUI?
+The GUI of Debloat intends to be as intuitive as possible.
+When launched, you can drag and drop bloated file onto the text bar and press the "Process file" button.
+Some technical information will be printed to the scrolling textbox and the file without bloat will be written to the directory the file was pulled from.
+Sound easy? It is!
+
+Processing files will take a few seconds.<br>
+![image](https://github.com/Squiblydoo/debloat/assets/77356206/3d2756cd-bc83-44e8-b223-edd8ed464369)
+
+
+## How to use the CLI?
+After installing using `pip install debloat` use the command `debloat`.<br>
+`debloat` can take two arguments. The first argument is required: the file to debloat. The second argument is optional: the output location. When no output is provided, it will be written to the same directory as the original file.
+
+The gui can also be launched from the CLI using the command `debloat-gui`.
+
+## Does it always work?
+Not yet.
+My unscientific guess is that it should work for every 9 of 10 binaries. There are specific usecases I know where it does not work and I am working to implement solutions for those usecases. 
+
+In previous versions, `debloat` could accidentally remove too much of the binary. That is no longer the case unless you use the "--last-ditch" switch. If you ever need this switch, consider sharing the sample for additional analysis. This option has now been added to the GUI. Functionally, what the function does is it will remove the whole overlay, if there is one. In some cases this is necessary as no pattern for the junk was found---this is most commonly the case in samples that do not compress well.
+
+## Use Cases (Images from [Malcat](https://malcat.fr/))
+### Full support
+- [x] Bloat appended to the end of a Signed PE.<br>
+In the image below, the bloat has been appended to the end of the executable. <br>
+![Screenshot 2023-02-11 at 3 32 36 PM](https://user-images.githubusercontent.com/77356206/218279963-00780b59-8227-47dd-a0af-41096f6ae17b.png)
+
+- [X] Signed or Unsigned Packed executable.<br>
+In the image below, the bloat has been appended to the executable after packing. <br>
+![Screenshot 2023-02-11 at 3 44 10 PM](https://user-images.githubusercontent.com/77356206/218280433-6dbcf51a-68c8-48e1-a89a-ad0b818a0afc.png)
+
+- [X] Signed executable includes bloat in the .rsrc section of the PE.<br>
+In the image below, the bloat is identified as in the .rsrc section and is removed from the PE.<br>
+![Screenshot 2023-02-11 at 3 35 21 PM](https://user-images.githubusercontent.com/77356206/218280086-7cd548f8-e16b-4290-9283-a8a848de1419.png)
+
+- [X] Cases where bloat is added inside a PE Section.<br>
+In the image below, the bloat has been included in a PE section named [0]. <br>
+![Screenshot 2023-02-11 at 3 26 52 PM](https://user-images.githubusercontent.com/77356206/218279753-ed2c9102-482a-4639-aeb1-df8efc9c4e2e.png)
+
+- [X] Cases where the executable is a Nullsoft Scriptable Installer System executable (NSIS aka Nullsoft)
+These exe are installers that may contain one or more files. The files contained may or may not be malicious. (Sometimes actors will add files simply for increasing the file size.) All files within the installer are extracted to a new directory. The directory also contains the script for the installer which can be consulted to determine which files may be malicious.
+In the image below, Malcat has identified the executable as a NSIS installer.
+![image](https://github.com/Squiblydoo/debloat/assets/77356206/86780abc-da4b-4808-bccb-733d97fa80d8)
+
+# Partial Support
+
+- [X] Cases where the junk is too random and the entropy is too high. In these cases, a switch/option called "--last-ditch" 
+
+### Other use cases
+There are use cases where the tool does not work. However, I plan to solve for them before publishing too much about them.
+
+## Why?
+There appear to be a limited number of tools to easily process bloated executables. The two tools I have seen the most are “foremost” which is intended for recovering binaries from a disk image and “pecheck”.
+
+[Foremost](https://www.kali.org/tools/foremost/) works best in instances where the junk bytes are null (0x00) and it struggles when the binary has a fake or real signature. Its use in removing bloat from files is not its original purpose.
+
+[Pecheck](https://github.com/DidierStevens/DidierStevensSuite/blob/master/pecheck.py) has been developed over 14+ years and has some confusing commandline options. The option to remove bloated content is not the primary function of the script. Pecheck has to be combined with another tool ([disitool](https://blog.didierstevens.com/programs/disitool/)) in order to handle signed executables. In my experience, there are other times where pecheck can get confused and return an executable twice the size of the original bloated executable. All these factors seem OK if you are handling a small number of binaries, but as the number of binaries and methods increase, a tool specific to removing bloat is needed.
+
+[Binary Refinery](https://github.com/binref/refinery) is an amazing tool. It was written with the intention of being a [CyberChef](https://github.com/gchq/CyberChef) of the commandline. While both tools are amazing, they both have a shortcoming that requires the user to know what formulas should be applied. 
+
+There are good solid manual methods to remove bloat from binaries, but these methods can be tedious and not all analysts have the skills to do this. This tool removes the burden of needing to know how to manually remove bloat. Additionally, it allows for better scale. The principles used in the script allow allow for better scale if automation is desired.
+
+
+## How to build? 
+Follow the build commands appropriate to your platform. The main difference between build commands is the format of the icon.
+<br>
+MacOS<br>
+`pyinstaller --onefile --noconsole --additional-hooks-dir=./hook --icon=debloat.icns gui.py`
+
+Windows<br>
+`pyinstaller --onefile  --noconsole  --additional-hooks-dir=./hook --icon=debloat.ico gui.py`
+
+Linux<br> 
+`pyinstaller --onefile --noconsole --icon=debloat.ico --collect-all tkinterdnd2 gui.py`
+
+## Want to discuss?
+Consider joining the [debloat Discord](discord.gg/dvGXKaY5qr).
+
+## Credits
+Big shoutout to Jesko Hüttenhain creator of [Binary Refinery](https://github.com/binref/refinery). The NSIS extraction is based on his reverse engineering of the NSIS file format. Check out Binary Refinery if you have not.
+
+## Where is this project going next?
+Batch processing: process all files in a directory and produce a report.
+
+Better support for using processing methods outside of debloat.
+
+Support for debloating without unzipping.
```

### Comparing `debloat-1.5.6/README.md` & `debloat-1.5.6.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,105 +1,121 @@
-![debloat](https://user-images.githubusercontent.com/77356206/215351855-9f89c298-36b4-4234-89b5-dc3f26d1f8b0.png)
-
-# Debloat
-Debloat is a GUI and CLI tool to remove excess garbage from bloated executables.
-
-By excess garbage, I mean 100 - 800 MB of junk bytes added to a binary to keep it from going into a sandbox. This method of adding junk is called "inflating" or "pumping" a binary. Debloat currently handles the 10 most common inflation tactics.
-
-Being built with Python, the application can easily be leveraged in other workflows. Currently, debloat is used by [CCCS's AssemblyLine](https://www.cyber.gc.ca/en/tools-services/assemblyline) and [CERT Polska's MWDB](https://github.com/CERT-Polska/karton-archive-extractor).
-
- The program can be compiled for Windows, MacOS, Linux. The GUI and CLI have minimal options: it is intended to be as simple as possible and the logic within the program handles the different use cases automatically.
-
-Compiled binaries have already been included in the [Releases](https://github.com/Squiblydoo/debloat/releases/).
-
-The debloat can installed using `pip install debloat`. Use `debloat` to launch the CLI and `debloat-gui` to launch the GUI.
-
-For advanced users, Debloat can also be imported into other scripts and the processing functions can be called individually.
-
-## How to use the GUI?
-The GUI of Debloat intends to be as intuitive as possible.
-When launched, you can drag and drop bloated file onto the text bar and press the "Process file" button.
-Some technical information will be printed to the scrolling textbox and the file without bloat will be written to the directory the file was pulled from.
-Sound easy? It is!
-
-Processing files will take a few seconds.<br>
-![image](https://github.com/Squiblydoo/debloat/assets/77356206/3d2756cd-bc83-44e8-b223-edd8ed464369)
-
-
-## How to use the CLI?
-After installing using `pip install debloat` use the command `debloat`.<br>
-`debloat` can take two arguments. The first argument is required: the file to debloat. The second argument is optional: the output location. When no output is provided, it will be written to the same directory as the original file.
-
-The gui can also be launched from the CLI using the command `debloat-gui`.
-
-## Does it always work?
-Not yet.
-My unscientific guess is that it should work for every 9 of 10 binaries. There are specific usecases I know where it does not work and I am working to implement solutions for those usecases. 
-
-In previous versions, `debloat` could accidentally remove too much of the binary. That is no longer the case unless you use the "--last-ditch" switch. If you ever need this switch, consider sharing the sample for additional analysis. This option has now been added to the GUI. Functionally, what the function does is it will remove the whole overlay, if there is one. In some cases this is necessary as no pattern for the junk was found---this is most commonly the case in samples that do not compress well.
-
-## Use Cases (Images from [Malcat](https://malcat.fr/))
-### Full support
-- [x] Bloat appended to the end of a Signed PE.<br>
-In the image below, the bloat has been appended to the end of the executable. <br>
-![Screenshot 2023-02-11 at 3 32 36 PM](https://user-images.githubusercontent.com/77356206/218279963-00780b59-8227-47dd-a0af-41096f6ae17b.png)
-
-- [X] Signed or Unsigned Packed executable.<br>
-In the image below, the bloat has been appended to the executable after packing. <br>
-![Screenshot 2023-02-11 at 3 44 10 PM](https://user-images.githubusercontent.com/77356206/218280433-6dbcf51a-68c8-48e1-a89a-ad0b818a0afc.png)
-
-- [X] Signed executable includes bloat in the .rsrc section of the PE.<br>
-In the image below, the bloat is identified as in the .rsrc section and is removed from the PE.<br>
-![Screenshot 2023-02-11 at 3 35 21 PM](https://user-images.githubusercontent.com/77356206/218280086-7cd548f8-e16b-4290-9283-a8a848de1419.png)
-
-- [X] Cases where bloat is added inside a PE Section.<br>
-In the image below, the bloat has been included in a PE section named [0]. <br>
-![Screenshot 2023-02-11 at 3 26 52 PM](https://user-images.githubusercontent.com/77356206/218279753-ed2c9102-482a-4639-aeb1-df8efc9c4e2e.png)
-
-- [X] Cases where the executable is a Nullsoft Scriptable Installer System executable (NSIS aka Nullsoft)
-These exe are installers that may contain one or more files. The files contained may or may not be malicious. (Sometimes actors will add files simply for increasing the file size.) All files within the installer are extracted to a new directory. The directory also contains the script for the installer which can be consulted to determine which files may be malicious.
-In the image below, Malcat has identified the executable as a NSIS installer.
-![image](https://github.com/Squiblydoo/debloat/assets/77356206/86780abc-da4b-4808-bccb-733d97fa80d8)
-
-# Partial Support
-
-- [X] Cases where the junk is too random and the entropy is too high. In these cases, a switch/option called "--last-ditch" 
-
-### Other use cases
-There are use cases where the tool does not work. However, I plan to solve for them before publishing too much about them.
-
-## Why?
-There appear to be a limited number of tools to easily process bloated executables. The two tools I have seen the most are “foremost” which is intended for recovering binaries from a disk image and “pecheck”.
-
-[Foremost](https://www.kali.org/tools/foremost/) works best in instances where the junk bytes are null (0x00) and it struggles when the binary has a fake or real signature. Its use in removing bloat from files is not its original purpose.
-
-[Pecheck](https://github.com/DidierStevens/DidierStevensSuite/blob/master/pecheck.py) has been developed over 14+ years and has some confusing commandline options. The option to remove bloated content is not the primary function of the script. Pecheck has to be combined with another tool ([disitool](https://blog.didierstevens.com/programs/disitool/)) in order to handle signed executables. In my experience, there are other times where pecheck can get confused and return an executable twice the size of the original bloated executable. All these factors seem OK if you are handling a small number of binaries, but as the number of binaries and methods increase, a tool specific to removing bloat is needed.
-
-[Binary Refinery](https://github.com/binref/refinery) is an amazing tool. It was written with the intention of being a [CyberChef](https://github.com/gchq/CyberChef) of the commandline. While both tools are amazing, they both have a shortcoming that requires the user to know what formulas should be applied. 
-
-There are good solid manual methods to remove bloat from binaries, but these methods can be tedious and not all analysts have the skills to do this. This tool removes the burden of needing to know how to manually remove bloat. Additionally, it allows for better scale. The principles used in the script allow allow for better scale if automation is desired.
-
-
-## How to build? 
-Follow the build commands appropriate to your platform. The main difference between build commands is the format of the icon.
-<br>
-MacOS<br>
-`pyinstaller --onefile --noconsole --additional-hooks-dir=./hook --icon=debloat.icns gui.py`
-
-Windows<br>
-`pyinstaller --onefile  --noconsole  --additional-hooks-dir=./hook --icon=debloat.ico gui.py`
-
-Linux<br> 
-`pyinstaller --onefile --noconsole --icon=debloat.ico --collect-all tkinterdnd2 gui.py`
-
-## Want to discuss?
-Consider joining the [debloat Discord](discord.gg/dvGXKaY5qr).
-
-## Credits
-Big shoutout to Jesko Hüttenhain creator of [Binary Refinery](https://github.com/binref/refinery). The NSIS extraction is based on his reverse engineering of the NSIS file format. Check out Binary Refinery if you have not.
-
-## Where is this project going next?
-Batch processing: process all files in a directory and produce a report.
-
-Better support for using processing methods outside of debloat.
-
-Support for debloating without unzipping.
+Metadata-Version: 2.1
+Name: debloat
+Version: 1.5.6.1
+Summary: Debloat is an tool to remove excess garbage from bloated executables.
+Author-email: Squiblydoo <Squiblydoo@pm.me>
+Project-URL: Homepage, https://github.com/Squiblydoo/debloat
+Project-URL: Bug Tracker, https://github.com/Squiblydoo/debloat/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: tkinterdnd2>=0.3.0
+Requires-Dist: pefile>=2023.2.0
+
+![debloat](https://user-images.githubusercontent.com/77356206/215351855-9f89c298-36b4-4234-89b5-dc3f26d1f8b0.png)
+
+# Debloat
+Debloat is a GUI and CLI tool to remove excess garbage from bloated executables.
+
+By excess garbage, I mean 100 - 800 MB of junk bytes added to a binary to keep it from going into a sandbox. This method of adding junk is called "inflating" or "pumping" a binary. Debloat currently handles the 10 most common inflation tactics.
+
+Being built with Python, the application can easily be leveraged in other workflows. Currently, debloat is used by [CCCS's AssemblyLine](https://www.cyber.gc.ca/en/tools-services/assemblyline) and [CERT Polska's MWDB](https://github.com/CERT-Polska/karton-archive-extractor).
+
+ The program can be compiled for Windows, MacOS, Linux. The GUI and CLI have minimal options: it is intended to be as simple as possible and the logic within the program handles the different use cases automatically.
+
+Compiled binaries have already been included in the [Releases](https://github.com/Squiblydoo/debloat/releases/).
+
+The debloat can installed using `pip install debloat`. Use `debloat` to launch the CLI and `debloat-gui` to launch the GUI.
+
+For advanced users, Debloat can also be imported into other scripts and the processing functions can be called individually.
+
+## How to use the GUI?
+The GUI of Debloat intends to be as intuitive as possible.
+When launched, you can drag and drop bloated file onto the text bar and press the "Process file" button.
+Some technical information will be printed to the scrolling textbox and the file without bloat will be written to the directory the file was pulled from.
+Sound easy? It is!
+
+Processing files will take a few seconds.<br>
+![image](https://github.com/Squiblydoo/debloat/assets/77356206/3d2756cd-bc83-44e8-b223-edd8ed464369)
+
+
+## How to use the CLI?
+After installing using `pip install debloat` use the command `debloat`.<br>
+`debloat` can take two arguments. The first argument is required: the file to debloat. The second argument is optional: the output location. When no output is provided, it will be written to the same directory as the original file.
+
+The gui can also be launched from the CLI using the command `debloat-gui`.
+
+## Does it always work?
+Not yet.
+My unscientific guess is that it should work for every 9 of 10 binaries. There are specific usecases I know where it does not work and I am working to implement solutions for those usecases. 
+
+In previous versions, `debloat` could accidentally remove too much of the binary. That is no longer the case unless you use the "--last-ditch" switch. If you ever need this switch, consider sharing the sample for additional analysis. This option has now been added to the GUI. Functionally, what the function does is it will remove the whole overlay, if there is one. In some cases this is necessary as no pattern for the junk was found---this is most commonly the case in samples that do not compress well.
+
+## Use Cases (Images from [Malcat](https://malcat.fr/))
+### Full support
+- [x] Bloat appended to the end of a Signed PE.<br>
+In the image below, the bloat has been appended to the end of the executable. <br>
+![Screenshot 2023-02-11 at 3 32 36 PM](https://user-images.githubusercontent.com/77356206/218279963-00780b59-8227-47dd-a0af-41096f6ae17b.png)
+
+- [X] Signed or Unsigned Packed executable.<br>
+In the image below, the bloat has been appended to the executable after packing. <br>
+![Screenshot 2023-02-11 at 3 44 10 PM](https://user-images.githubusercontent.com/77356206/218280433-6dbcf51a-68c8-48e1-a89a-ad0b818a0afc.png)
+
+- [X] Signed executable includes bloat in the .rsrc section of the PE.<br>
+In the image below, the bloat is identified as in the .rsrc section and is removed from the PE.<br>
+![Screenshot 2023-02-11 at 3 35 21 PM](https://user-images.githubusercontent.com/77356206/218280086-7cd548f8-e16b-4290-9283-a8a848de1419.png)
+
+- [X] Cases where bloat is added inside a PE Section.<br>
+In the image below, the bloat has been included in a PE section named [0]. <br>
+![Screenshot 2023-02-11 at 3 26 52 PM](https://user-images.githubusercontent.com/77356206/218279753-ed2c9102-482a-4639-aeb1-df8efc9c4e2e.png)
+
+- [X] Cases where the executable is a Nullsoft Scriptable Installer System executable (NSIS aka Nullsoft)
+These exe are installers that may contain one or more files. The files contained may or may not be malicious. (Sometimes actors will add files simply for increasing the file size.) All files within the installer are extracted to a new directory. The directory also contains the script for the installer which can be consulted to determine which files may be malicious.
+In the image below, Malcat has identified the executable as a NSIS installer.
+![image](https://github.com/Squiblydoo/debloat/assets/77356206/86780abc-da4b-4808-bccb-733d97fa80d8)
+
+# Partial Support
+
+- [X] Cases where the junk is too random and the entropy is too high. In these cases, a switch/option called "--last-ditch" 
+
+### Other use cases
+There are use cases where the tool does not work. However, I plan to solve for them before publishing too much about them.
+
+## Why?
+There appear to be a limited number of tools to easily process bloated executables. The two tools I have seen the most are “foremost” which is intended for recovering binaries from a disk image and “pecheck”.
+
+[Foremost](https://www.kali.org/tools/foremost/) works best in instances where the junk bytes are null (0x00) and it struggles when the binary has a fake or real signature. Its use in removing bloat from files is not its original purpose.
+
+[Pecheck](https://github.com/DidierStevens/DidierStevensSuite/blob/master/pecheck.py) has been developed over 14+ years and has some confusing commandline options. The option to remove bloated content is not the primary function of the script. Pecheck has to be combined with another tool ([disitool](https://blog.didierstevens.com/programs/disitool/)) in order to handle signed executables. In my experience, there are other times where pecheck can get confused and return an executable twice the size of the original bloated executable. All these factors seem OK if you are handling a small number of binaries, but as the number of binaries and methods increase, a tool specific to removing bloat is needed.
+
+[Binary Refinery](https://github.com/binref/refinery) is an amazing tool. It was written with the intention of being a [CyberChef](https://github.com/gchq/CyberChef) of the commandline. While both tools are amazing, they both have a shortcoming that requires the user to know what formulas should be applied. 
+
+There are good solid manual methods to remove bloat from binaries, but these methods can be tedious and not all analysts have the skills to do this. This tool removes the burden of needing to know how to manually remove bloat. Additionally, it allows for better scale. The principles used in the script allow allow for better scale if automation is desired.
+
+
+## How to build? 
+Follow the build commands appropriate to your platform. The main difference between build commands is the format of the icon.
+<br>
+MacOS<br>
+`pyinstaller --onefile --noconsole --additional-hooks-dir=./hook --icon=debloat.icns gui.py`
+
+Windows<br>
+`pyinstaller --onefile  --noconsole  --additional-hooks-dir=./hook --icon=debloat.ico gui.py`
+
+Linux<br> 
+`pyinstaller --onefile --noconsole --icon=debloat.ico --collect-all tkinterdnd2 gui.py`
+
+## Want to discuss?
+Consider joining the [debloat Discord](discord.gg/dvGXKaY5qr).
+
+## Credits
+Big shoutout to Jesko Hüttenhain creator of [Binary Refinery](https://github.com/binref/refinery). The NSIS extraction is based on his reverse engineering of the NSIS file format. Check out Binary Refinery if you have not.
+
+## Where is this project going next?
+Batch processing: process all files in a directory and produce a report.
+
+Better support for using processing methods outside of debloat.
+
+Support for debloating without unzipping.
```

### Comparing `debloat-1.5.6/src/debloat/main.py` & `debloat-1.5.6.1/src/debloat/main.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-"""This file handles passing the CLI arguments into the processor"""
-import os
-import sys
-from pathlib import Path
-import argparse
-import pefile
-import debloat.processor
-from debloat.processor import DEBLOAT_VERSION
-from debloat.processor import RESULT_CODES
-
-
-def main() -> int:
-    parser = argparse.ArgumentParser()
-    parser.add_argument("executable", 
-                        help="Path to the executable to be debloated",
-                        type=Path)
-    parser.add_argument("--output", 
-                        help="Output location", 
-                        type=Path,
-                        required=False)
-    parser.add_argument("-yolo", "--last-ditch", dest="last_ditch_processing",
-                        help="""
-    Run last-ditch processing. In this mode Debloat may remove the
-    whole PE Overlay as a last resort if no smarter method works.
-                            """,
-                        action='store_true', default=False)
-    parser.add_argument("-c", "--cert", dest="cert_preservation", 
-                        help="""
-    Preserve the certificate on the end of the file if there is a certificate.
-    The certificate will no longer be valid.""",
-                        action='store_true',
-                        required=False,
-                        default=False)
-    parser.add_argument("-v", "--version", action='version', version='debloat version ' + DEBLOAT_VERSION, help="Prints program version")
-    args = parser.parse_args()
-
-    file_path = args.executable
-    out_path = args.output
-    file_size = os.path.getsize(file_path)
-
-    if not out_path:
-        out_path = file_path.parent \
-            / f"{file_path.stem}_patched{file_path.suffix}"
-
-    try:
-        with open(file_path, "rb") as bloated_file:
-            pe_data = bloated_file.read()
-        pe = pefile.PE(data=pe_data, fast_load=True)
-    except Exception:
-        print('''
-Provided file is not an executable! Please try again with an executable. 
-Maybe it needs unzipped?'''
-              )
-        return 1
-
-    result_code = debloat.processor.process_pe(pe, 
-                        out_path=str(out_path), 
-                        last_ditch_processing=args.last_ditch_processing,
-                        cert_preservation=args.cert_preservation,
-                        log_message=print,
-                        beginning_file_size=file_size
-                        )
-    print("Tactic identifed:", RESULT_CODES.get(result_code))
-    return 0
-
-if __name__ == "__main__":
-    sys.exit(main())
+"""This file handles passing the CLI arguments into the processor"""
+import os
+import sys
+from pathlib import Path
+import argparse
+import pefile
+import debloat.processor
+from debloat.processor import DEBLOAT_VERSION
+from debloat.processor import RESULT_CODES
+
+
+def main() -> int:
+    parser = argparse.ArgumentParser()
+    parser.add_argument("executable", 
+                        help="Path to the executable to be debloated",
+                        type=Path)
+    parser.add_argument("--output", 
+                        help="Output location", 
+                        type=Path,
+                        required=False)
+    parser.add_argument("-yolo", "--last-ditch", dest="last_ditch_processing",
+                        help="""
+    Run last-ditch processing. In this mode Debloat may remove the
+    whole PE Overlay as a last resort if no smarter method works.
+                            """,
+                        action='store_true', default=False)
+    parser.add_argument("-c", "--cert", dest="cert_preservation", 
+                        help="""
+    Preserve the certificate on the end of the file if there is a certificate.
+    The certificate will no longer be valid.""",
+                        action='store_true',
+                        required=False,
+                        default=False)
+    parser.add_argument("-v", "--version", action='version', version='debloat version ' + DEBLOAT_VERSION, help="Prints program version")
+    args = parser.parse_args()
+
+    file_path = args.executable
+    out_path = args.output
+    file_size = os.path.getsize(file_path)
+
+    if not out_path:
+        out_path = file_path.parent \
+            / f"{file_path.stem}_patched{file_path.suffix}"
+
+    try:
+        with open(file_path, "rb") as bloated_file:
+            pe_data = bloated_file.read()
+        pe = pefile.PE(data=pe_data, fast_load=True)
+    except Exception:
+        print('''
+Provided file is not an executable! Please try again with an executable. 
+Maybe it needs unzipped?'''
+              )
+        return 1
+
+    result_code = debloat.processor.process_pe(pe, 
+                        out_path=str(out_path), 
+                        last_ditch_processing=args.last_ditch_processing,
+                        cert_preservation=args.cert_preservation,
+                        log_message=print,
+                        beginning_file_size=file_size
+                        )
+    print("Tactic identifed:", RESULT_CODES.get(result_code))
+    return 0
+
+if __name__ == "__main__":
+    sys.exit(main())
```

### Comparing `debloat-1.5.6/src/debloat/performanceTest.py` & `debloat-1.5.6.1/src/debloat/performanceTest.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-## This script is for batch processing of samples and can be used for
-## measuring memory usage.
-
-import os
-import hashlib
-from memray import commands, FileReader
-from memray._memray import size_fmt
-import debloat.processor
-import timeit
-import argparse
-import cProfile
-import pstats
-import tempfile
-
-argparser = argparse.ArgumentParser(
-    prog = "Debloat Performance test",
-    description = "This program takes a test type (--mem or --cpu) and performs tests using one or more samples. If no sample or directory is specified, it defaults to a 'samples' directory in the current working directory."
-)
-argparser.add_argument("--cpu", help="Run the CPU profiler", action="store_true")
-argparser.add_argument("--mem", help="Run the memory profiler", action="store_true")
-argparser.add_argument("--sample", help="Run the debloat processor on a single sample")
-argparser.add_argument("--directory", help="Specify sample directory", default="samples")
-argparser.add_argument("--keep", help="Keeps patched copies.", action="store_true")
-args = argparser.parse_args()
-
-def process_samples(sample, directory):
-    file_size=os.path.getsize(args.directory +"/"+ sample)
-    setup = f"import pefile; import debloat; filename = '{args.directory}/{sample}'; "
-    code = f"binary = pefile.PE(filename, fast_load=True); result= debloat.processor.process_pe(binary, filename + '.patched', last_ditch_processing=False, cert_preservation=True, log_message=lambda *args, **kwargs: None, beginning_file_size={file_size}); print(result, end=' ')"
-
-    if args.mem:
-        mem_profiler(setup, code, file_size, sample, directory)
-    if args.cpu:
-        cpu_profiler()
-    if not args.keep:
-        try:
-            os.remove(args.directory + "/" + sample + ".patched")
-        except:
-            pass
-
-
-def mem_profiler(setup, code, file_size, sample, directory):
-    with tempfile.NamedTemporaryFile() as f:
-        commands.main(["run", "-f", "-q", "-o", f.name, "-c", setup+code])
-        reader = FileReader(os.fspath(f.name), report_progress=False)
-        # Uncomment to hash outputed samples.
-        #with open(directory +"/"+ sample + ".patched", "rb") as g:
-        #    out = g.read()
-        #    out_hash = hashlib.sha256(out).hexdigest()
-    times = timeit.repeat(stmt=code, setup=setup, number=1, repeat=3)
-    print(sample, size_fmt(file_size), size_fmt(reader.metadata.peak_memory), [round(x,2) for x in times])
-
-def cpu_profiler():
-    cProfile.run(setup+code, "tmp.prof")
-    p = pstats.Stats("tmp.prof")
-    p.sort_stats('tot').print_stats(10)
-    p.sort_stats('cumulative').print_stats(10)
-
-if args.sample:
-    process_samples(args.sample, args.directory)    
-
-else:
-    print("Debloat Method/ Original Filename / Disk Size /  Mem Usage / Time to process x 3")
-    for sample in os.listdir(args.directory):
-        process_samples(sample, args.directory)
-
+## This script is for batch processing of samples and can be used for
+## measuring memory usage.
+
+import os
+import hashlib
+from memray import commands, FileReader
+from memray._memray import size_fmt
+import debloat.processor
+import timeit
+import argparse
+import cProfile
+import pstats
+import tempfile
+
+argparser = argparse.ArgumentParser(
+    prog = "Debloat Performance test",
+    description = "This program takes a test type (--mem or --cpu) and performs tests using one or more samples. If no sample or directory is specified, it defaults to a 'samples' directory in the current working directory."
+)
+argparser.add_argument("--cpu", help="Run the CPU profiler", action="store_true")
+argparser.add_argument("--mem", help="Run the memory profiler", action="store_true")
+argparser.add_argument("--sample", help="Run the debloat processor on a single sample")
+argparser.add_argument("--directory", help="Specify sample directory", default="samples")
+argparser.add_argument("--keep", help="Keeps patched copies.", action="store_true")
+args = argparser.parse_args()
+
+def process_samples(sample, directory):
+    file_size=os.path.getsize(args.directory +"/"+ sample)
+    setup = f"import pefile; import debloat; filename = '{args.directory}/{sample}'; "
+    code = f"binary = pefile.PE(filename, fast_load=True); result= debloat.processor.process_pe(binary, filename + '.patched', last_ditch_processing=False, cert_preservation=False, log_message=lambda *args, **kwargs: None, beginning_file_size={file_size}); print(result, end=' ')"
+
+    if args.mem:
+        mem_profiler(setup, code, file_size, sample, directory)
+    if args.cpu:
+        cpu_profiler()
+    if not args.keep:
+        try:
+            os.remove(args.directory + "/" + sample + ".patched")
+        except:
+            pass
+
+
+def mem_profiler(setup, code, file_size, sample, directory):
+    with tempfile.NamedTemporaryFile() as f:
+        commands.main(["run", "-f", "-q", "-o", f.name, "-c", setup+code])
+        reader = FileReader(os.fspath(f.name), report_progress=False)
+        # Uncomment to hash outputed samples.
+        #with open(directory +"/"+ sample + ".patched", "rb") as g:
+        #    out = g.read()
+        #    out_hash = hashlib.sha256(out).hexdigest()
+    times = timeit.repeat(stmt=code, setup=setup, number=1, repeat=3)
+    print(sample, size_fmt(file_size), size_fmt(reader.metadata.peak_memory), [round(x,2) for x in times])
+
+def cpu_profiler():
+    cProfile.run(setup+code, "tmp.prof")
+    p = pstats.Stats("tmp.prof")
+    p.sort_stats('tot').print_stats(10)
+    p.sort_stats('cumulative').print_stats(10)
+
+if args.sample:
+    process_samples(args.sample, args.directory)    
+
+else:
+    print("Debloat Method/ Original Filename / Disk Size /  Mem Usage / Time to process x 3")
+    for sample in os.listdir(args.directory):
+        process_samples(sample, args.directory)
+
```

### Comparing `debloat-1.5.6/src/debloat/processor.py` & `debloat-1.5.6.1/src/debloat/processor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,603 +1,603 @@
-"""
-This file handles the processing of binaries and helper methods.
-
-Three methods rely heavily on parts of Binary Refinery
-https://github.com/binref/refinery
-Copyright 2019 Jesko Hüttenhain under the 3-Clause BSD License
-The methods are:
-refinery_strip()
-adjust_offsets()
-refinery_trim_resources()
-The RSRC Class is also from refinery.
-"""
-from pathlib import Path
-import re
-from typing import Tuple, Optional, Any, Callable, List
-import pefile
-import binascii
-import zlib
-from pefile import Structure, SectionStructure, DIRECTORY_ENTRY
-from typing import Generator, Iterable, Optional
-
-import debloat.utilities.nsisParser as nsisParser
-import debloat.utilities.rsrc as rsrc
-
-DEBLOAT_VERSION = "1.5.5"
-
-RESULT_CODES = {
-    0: "No Solution found.",
-    1: "Junk after signature.",
-    2: "Single repeated byte in overlay.",
-    3: "Pattern in overlay.",
-    4: "Sets of repeated bytes in overlay.",
-    5: "NSIS Installer.",
-    6: "Bloat in PE resources",
-    7: "Bloat in PE section",
-    8: "Bloat in .NET resource",
-    9: "Non-essential, high entropy overlay",
-    10: "High compression with bytes at end.",
-    11: ".NET Single File with junk",
-    12: "Packed file with bloated section"
-}
-
-
-_KB = 1000
-_MB = _KB * _KB
-
-def readable_size(value: int) -> str:
-    '''Return bytes in human readable format.'''
-    if value <= 1024:
-        return '%s bytes' % value
-    elif value < 1024 * 1024:
-        return '%.1f KB' % (float(value) / 1024.0)
-    elif value < 1024 * 1024 * 1024:
-        return '%.1f MB' % (float(value) / 1024.0 / 1024.0)
-    else:
-        return '%.1f GB' % (float(value) / 1024.0 / 1024.0 / 1024.0)
-
-def write_multiple_files(out_path: str,
-                         files: list, log_message: Callable[[str], None]) -> None:
-    '''
-    Writes multiple files to disk when applicable.
-    '''
-    log_message("Installer unpacked!\n")
-    log_message(f"The files are being written to {out_path}")
-    for file in files:
-        out_file_path = Path(out_path) / Path(file.path.replace("\\", "/"))
-        out_dir_path = out_file_path.parent
-        out_dir_path.mkdir(parents=True, exist_ok=True)
-        with open(out_file_path, "wb") as f:
-            f.write(file.data)
-            log_message("File: " + str(Path(file.path.replace("\\", "/"))))
-    log_message("")
-    log_message("The user will need to determine which file is malicious if any.")
-    log_message("If a file is bloated: resubmit it through the tool to debloat it.")
-    log_message(f"Consider reviewing the 'setup.nsis' from the installer to determine how the files were meant to be used.")
-    return 
-
-
-def write_patched_file(out_path: str,
-                        pe: pefile.PE) -> Tuple[int, str]:
-    '''Writes the patched file to disk.
-
-    Keyword Arguments:
-    out_path -- the path and file name to write
-    pe -- the pefile that is being processed
-    end_of_real_data -- an int indicating the size of bytes to write'''
-    with open(out_path, 'wb') as writer:
-        writer.write(pe.write())
-        final_filesize = len(pe.write())
-        return final_filesize, out_path
-
-def handle_signature_abnormality(signature_address: int,
-                                signature_size: int,
-                                beginning_file_size: int) -> bool:
-    '''Remove all bytes after a PE signature'''
-    # If the signature_address is 0, there was no original signature.
-    # We are setting the signature address to the filesize in order to
-    # skip the next check.
-    if signature_address == 0:
-        signature_address = beginning_file_size
-    # Check to see if there is data after the signature; if so, it is
-    #  junk data
-    if beginning_file_size > (signature_address + signature_size):
-        return True
-    return False
-
-def check_and_extract_NSIS(possible_header: bytearray, pe: pefile.PE) -> list:
-    '''Check if the PE is an NSIS installer.'''
-    extractor = nsisParser.extractNSIS()
-    confirm_if_nsis = extractor._find_archive_offset(memoryview(possible_header))
-    if confirm_if_nsis is None:
-        return
-    extracted_files = extractor.unpack(memoryview(pe.__data__))
-    return extracted_files
-
-
-def find_last_section(pe: pefile.PE) -> Optional[pefile.SectionStructure]:
-    '''Iterate through PE sections to identify the last one.'''
-    last_section = None
-    for section in pe.sections:
-        if last_section is None \
-                        or section.PointerToRawData > last_section.PointerToRawData:
-            last_section = section
-    return last_section
-
-def get_signature_info(pe: pefile.PE, cert_preservation) -> Tuple[int, int]:
-    '''Remove PE signature and update header.'''
-    signature_address = pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].VirtualAddress
-    signature_size = pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].Size
-    pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].VirtualAddress = 0
-    # If the cert is to be preservered, we do not need to modify the size in the header. 
-    if cert_preservation == False:
-        pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].Size = 0
-
-    return signature_address, signature_size
-
-
-def adjust_offsets(pe: pefile.PE, gap_offset: int, gap_size: int):
-    base = pe.OPTIONAL_HEADER.ImageBase
-    alignment = pe.OPTIONAL_HEADER.FileAlignment
-    rva_offset = pe.get_rva_from_offset(gap_offset)
-    tva_offset = rva_offset + base
-
-    section = pe.get_section_by_offset(gap_offset)
-    new_section_size = section.SizeOfRawData - gap_size
-    if new_section_size % alignment != 0:
-        raise RuntimeError(
-            F'trimming 0x{gap_size:X} bytes from section {(section.Name)} of size 0x{section.SizeOfRawData:X} '
-            F'violates required section alignment of 0x{alignment:X} bytes')
-    inside_section_offset = gap_offset - section.PointerToRawData
-    if inside_section_offset > new_section_size:
-        overlap = inside_section_offset - new_section_size
-        raise RuntimeError(F'trimming from section {(section.Name)}; data extends {overlap} beyond section')
-
-    rva_lbound = section.VirtualAddress
-    rva_ubound = section.VirtualAddress + section.Misc_VirtualSize - 1
-    tva_lbound = rva_lbound + base
-    tva_ubound = rva_ubound + base
-
-    def adjust_attributes_of_structure(
-        structure: Structure,
-        threshold: int,
-        lbound: Optional[int],
-        ubound: Optional[int],
-        attributes: Iterable[str]
-    ):
-        for attribute in attributes:
-            old_value = getattr(structure, attribute, 0)
-            if old_value <= threshold:
-                continue
-            if lbound is not None and old_value < lbound:
-                continue
-            if ubound is not None and old_value > ubound:
-                continue
-            new_value = old_value - gap_size
-            if new_value < 0:
-                raise RuntimeError(F'adjusting attribute {attribute} of {structure.name} would result in negative value: {new_value}')
-            setattr(structure, attribute, new_value)
-
-    it: Iterable[Structure] = iter(pe.__structures__)
-    remove = []
-
-    for index, structure in enumerate(it):
-        old_offset = structure.get_file_offset()
-        new_offset = old_offset - gap_offset
-
-        if old_offset > gap_offset:
-            if old_offset < gap_offset + gap_size:
-                remove.append(index)
-                continue
-            if isinstance(structure, SectionStructure) and new_offset % alignment != 0:
-                raise RuntimeError(
-                    F'section {(structure.Name)} would be moved to offset 0x{new_offset:X}, '
-                    F'violating section alignment value 0x{alignment:X}.')
-            structure.set_file_offset(new_offset)
-
-        adjust_attributes_of_structure(structure, rva_offset, rva_lbound, rva_ubound, (
-            'OffsetToData',
-            'AddressOfData',
-            'VirtualAddress',
-            'AddressOfNames',
-            'AddressOfNameOrdinals',
-            'AddressOfFunctions',
-            'AddressOfEntryPoint',
-            'AddressOfRawData',
-            'BaseOfCode',
-            'BaseOfData',
-        ))
-        adjust_attributes_of_structure(structure, tva_offset, tva_lbound, tva_ubound, (
-            'StartAddressOfRawData',
-            'EndAddressOfRawData',
-            'AddressOfIndex',
-            'AddressOfCallBacks',
-        ))
-        adjust_attributes_of_structure(structure, gap_offset, None, None, (
-            'OffsetModuleName',
-            'PointerToRawData',
-        ))
-
-        for attribute in (
-            'CvHeaderOffset',
-            'OffsetIn2Qwords',
-            'OffsetInQwords',
-            'Offset',
-            'OffsetLow',
-            'OffsetHigh'
-        ):
-            if not hasattr(structure, attribute):
-                continue
-    
-    while remove:
-        index = remove.pop()
-        pe.__structures__[index:index + 1] = []
-
-    section.SizeOfRawData = new_section_size
-    return pe
-
-
-def refinery_strip(data: memoryview, alignment=1, block_size=_MB) -> int:
-    if not data:
-        return 0
-    threshold = 0.05
-    data_overhang = len(data) % alignment
-    result = data_overhang
-
-    if 0 < threshold < 1:
-        def compression_ratio(offset: int):
-            ratio = len(zlib.compress(data[:offset], level=1)) / offset
-            return ratio
-        upper = len(data)
-        lower = result
-
-        if compression_ratio(upper) <= threshold:
-            while block_size < upper - lower:
-                pivot = (lower + upper) // 2
-                ratio = compression_ratio(pivot)
-                if ratio > threshold:
-                    lower = pivot + 1
-                    continue
-                upper = pivot
-                if abs(ratio - threshold) < 1e-10:
-                    break
-
-        result = upper
-    
-    while result > 1 and data[result - 2] == data[result -1]:
-        result -= 1
-
-    result = max(result, data_overhang)
-
-    result = result + (data_overhang - result) % alignment
-
-    if result > len(data):
-        excess = result - len(data)
-        excess = excess + (-excess % alignment)
-        result = result - excess
-
-    return result
-
-
-def refinery_trim_resources(pe: pefile.PE, data_to_delete: List) -> int:
-    size_limit = 10000
-    size_removed = 0
-
-    def find_bloated_resources(pe: pefile.PE, directory, level: int = 0, *path) -> Generator[Structure, None, None]:
-        for entry in directory.entries:
-            name = getattr(entry, 'name')
-            numeric_id = getattr(entry, 'id')
-            if not name:
-                if level == 0 and numeric_id in iter(rsrc.RSRC):
-                    name = rsrc.RSRC(entry.id)
-                elif numeric_id is not None:
-                    name = str(numeric_id)
-            name = name and str(name) or '?'
-            if entry.struct.DataIsDirectory:
-                yield from find_bloated_resources(pe, entry.directory, level + 1, *path, name)
-                continue
-            struct: Structure = entry.data.struct
-            name = '/'.join((*path, name))
-            if struct.Size <= size_limit:
-                continue
-            yield name, struct
-
-    RSRC_INDEX = DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_RESOURCE']
-    pe.parse_data_directories(directories=[RSRC_INDEX])
-
-    try:
-        resources = pe.DIRECTORY_ENTRY_RESOURCE
-    except AttributeError:
-        return 0
-    for name, resource in find_bloated_resources(pe, resources):
-        offset = pe.get_offset_from_rva(resource.OffsetToData)
-        # Offset may be modified from debloating a previous resource
-        original_offset = offset
-        for slice_start, slice_end in data_to_delete:
-            if slice_start <= original_offset:
-                original_offset += slice_end-slice_start
-        old_size = resource.Size
-        new_size = refinery_strip(memoryview(pe.__data__)[original_offset:original_offset + old_size], pe.OPTIONAL_HEADER.FileAlignment)
-        gap_size = old_size - new_size
-        if gap_size <= 0:
-            continue
-        resource.Size = new_size
-        adjust_offsets(pe, offset + new_size, gap_size)
-        size_removed += gap_size
-        data_to_delete.append((original_offset + new_size, original_offset + old_size))
-
-    pe.OPTIONAL_HEADER.DATA_DIRECTORY[RSRC_INDEX].Size -= size_removed
-
-def get_compressed_size(data: memoryview, offset: int, level: int = -1):
-    if offset <= 1024:
-        return len(zlib.compress(data[:offset], level=level))
-
-    compress_obj = zlib.compressobj(level=level)
-    compress_data_len = 0
-    index = 0
-    for index in range(offset//1024):
-        chunk = data[index*1024 : (index+1)*1024]
-        compress_data_len += len(compress_obj.compress(chunk))
-    leftover = offset%1024
-    if leftover:
-        chunk = data[(index+1)*1024 : (index+1)*1024 + leftover]
-        compress_data_len += len(compress_obj.compress(chunk))
-    compress_data_len += len(compress_obj.flush())
-    return compress_data_len
-
-def check_section_compression(pe: pefile.PE, data_to_delete: List,
-                              log_message: Callable[[str], None]) -> Tuple[pefile.PE, int, str]:
-        biggest_section = None
-        biggest_uncompressed = int
-        result = ""
-        for section in pe.sections:
-            section_name = section.Name.decode()
-            compressed_section_size = get_compressed_size(
-                memoryview(pe.__data__)[section.PointerToRawData : section.PointerToRawData+section.SizeOfRawData],
-                section.SizeOfRawData
-            )
-            section_compression_ratio = section.SizeOfRawData / compressed_section_size * 100
-            log_message("Section: "  + section_name, end="\t", flush=True)
-            log_message(" Compression Ratio: " + str(round(section_compression_ratio, 2)) +"%", end="\t",flush=True)
-            log_message("Size of section: " + readable_size(section.SizeOfRawData) +".",flush=True)
-            if biggest_section is None:
-                biggest_section = section
-                biggest_uncompressed = section_compression_ratio
-            elif section.SizeOfRawData > biggest_section.SizeOfRawData:
-                biggest_section = section
-                biggest_uncompressed = section_compression_ratio
-        # Handle specific bloated sections
-        if biggest_section.Name.decode() == ".rsrc\x00\x00\x00":
-            # Get biggest resource or resources and drop them from the
-            # Resource table
-            log_message('''
-Bloat was located in the resource section. Removing bloat..
-''')
-            refinery_trim_resources(pe, data_to_delete)
-            result_code = 6 # Bloated resource
-            return result, result_code
-
-        elif biggest_section.Name.decode() == ".text\x00\x00\x00":
-            # Data stored in the .text section is often a .NET Resource. The following checks
-            # to confirm it is .NET and then drops the resources.
-            if pe.OPTIONAL_HEADER.DATA_DIRECTORY[14].Size:
-                log_message('''
-Bloat was detected in the text section. Bloat is likely in a .NET Resource
-This use case cannot be processed at this time. ''')
-            result_code = 0 # No solution 
-            return result, result_code
-        if biggest_uncompressed > 3000:
-            log_message('''
-The compression ratio of ''' + biggest_section.Name.decode() + ''' is indicative of a bloated section.
-''', end="", flush=True)
-            # Get the size of the section.
-            biggest_section_end = biggest_section.PointerToRawData + biggest_section.SizeOfRawData
-            original_section_size = biggest_section.SizeOfRawData
-            biggest_section_data = memoryview(pe.__data__)[biggest_section.PointerToRawData:biggest_section_end]
-            delta_last_non_junk, result_code = trim_junk(pe, biggest_section_data, original_section_size)
-            # Remove the junk from the section.
-            if delta_last_non_junk > original_section_size:
-                log_message("Section was not able to be reduced.")
-                result_code = 0
-                return result
-            data_to_delete.append((biggest_section.PointerToRawData + delta_last_non_junk, biggest_section_end))
-            
-            section_bytes_to_remove = original_section_size - delta_last_non_junk
-            # Adjust all offsets for the file.
-            adjust_offsets(pe, biggest_section.PointerToRawData, section_bytes_to_remove)
-            log_message("Bloated section reduced.")
-            result_code = 7 # Bloated PE section
-            return result, result_code
-
-def find_chunk_start(targeted_regex, chunk_start, original_size_with_junk, bloated_content: memoryview, step):
-    bloated_content_len = len(bloated_content)
-    compiled_targeted_regex = re.compile(targeted_regex)
-    chunk_end = chunk_start
-    while original_size_with_junk > chunk_end:
-        chunk_end = chunk_start + step
-        targeted_regex_match = compiled_targeted_regex.search(binascii.hexlify(bytes(bloated_content[max(bloated_content_len - chunk_end, 0):bloated_content_len - chunk_start])[::-1]))
-        if targeted_regex_match:
-            chunk_start += targeted_regex_match.end(0)
-        else:
-            # If the targeted_regex_match does not
-            # return anything, that indicates the previous loop
-            # had content which did not match. We'll use that
-            # to help ensure we do not remove too much of the file.
-            chunk_start -= step * 2
-            break
-    return chunk_start
-
-def trim_junk(pe: pefile.PE, bloated_content: memoryview,
-              original_size_with_junk: int) -> int:
-    '''Attempts multiple methods to trim junk from the end of a section.'''
-    alignment = pe.OPTIONAL_HEADER.FileAlignment
-
-    # Regex Explained:
-    # Match raw bytes that are repeated more than 20 times at the end
-    # of a binary.
-    delta_last_non_junk = original_size_with_junk
-    # First Method: Trims 1 repeating byte.
-    # Check against 200 bytes, if successful, calculate full match.
-    junk_match = re.search(rb'^(..)\1{20,}', bytes(bloated_content[:-601:-1]))
-    chunk_start = 0
-    if not junk_match:
-        # Second method: remove junk using refinery_strip. This method
-        # is more efficent than a previous check that was used here.
-        delta_last_non_junk = refinery_strip(bloated_content, alignment)
-        result_code = 3 # Pattern in overlay.
-
-    # Junk was identified. A new size is assigned and returned.
-    else:
-        # First method continued...
-        bloated_content_len = len(bloated_content)
-        targeted_regex = rb"("+ binascii.hexlify(junk_match.group(1)) + rb")\1{1,}"
-        precompiled_chunk = binascii.hexlify(junk_match.group(1)) * int(1000/len(junk_match.group(1)))
-        chunk_end = chunk_start
-        while original_size_with_junk > chunk_end:
-            chunk_end = chunk_start + 1000
-            chunk = binascii.hexlify(bytes(bloated_content[max(bloated_content_len - chunk_end, 0):bloated_content_len - chunk_start])[::-1])
-            if chunk == precompiled_chunk:
-                chunk_start += 1000
-                continue
-            else:
-                # If the chunk does not match the precompiled chunk,
-                # we will return to the previous chunk_start in order
-                # to ensure important bytes are not removed.
-                if chunk_start > 1000:
-                    chunk_start -= 1000
-                break
-        junk_to_remove = chunk_start 
-
-        # Third Method: check for a series of one repeated byte.
-        # If the trimming did not remove more than half of the bytes then
-        # this suggests the attacker may have put a random series of
-        # repeated bytes. We use refinery_trim for efficiency.
-        if junk_to_remove * 2 < original_size_with_junk / 2:
-            delta_last_non_junk = refinery_strip(bloated_content, alignment)
-            result_code = 4 # Sets of repeated bytes in overlay.
-        else:
-            result_code = 2 # Single repeated byte in overlay
-        delta_last_non_junk -= junk_to_remove
-
-    # The returned size must account for the file alignment.
-    # We will make sure it is aligned by adding bytes.
-    not_aligned = alignment - (delta_last_non_junk % alignment)
-    delta_last_non_junk = delta_last_non_junk + not_aligned
-    if not result_code:
-        result_code = 0
-    return delta_last_non_junk, result_code
-
-def process_pe(pe: pefile.PE, out_path: str, last_ditch_processing: bool,
-                cert_preservation: bool,log_message: Callable[[str], None], 
-                beginning_file_size: int = 0) -> None:
-    '''Prepare PE, perform checks, remote junk, write patched binary.'''
-    result_code = 0
-    if not beginning_file_size:
-        beginning_file_size = len(pe.write())
-
-    # Remove Signature and modify size of Optional Header Security entry.
-    signature_address, signature_size = get_signature_info(pe, cert_preservation)
-    if cert_preservation == True:
-        cert = [(signature_address, signature_address + signature_size)]
-        data_to_delete = []
-    else:
-        if signature_size > 0:
-            log_message("""A certificate is being removed from this file.\n-To preserve the certificate use the Cert Preservation option.""")
-        data_to_delete = [(signature_address, signature_address + signature_size)]
-
-    signature_abnormality = handle_signature_abnormality(signature_address,
-                                                        signature_size,
-                                                        beginning_file_size)
-    if signature_abnormality:
-        data_to_delete.append((signature_address + signature_size, beginning_file_size))
-        result_code = 1  # Junk after signture
-
-    # Handle Overlays: this includes packers and overlays which are completely junk
-    elif pe.get_overlay_data_start_offset() and signature_size < len(pe.__data__) - pe.get_overlay_data_start_offset():
-        possible_header = pe.__data__[pe.get_overlay_data_start_offset():pe.get_overlay_data_start_offset() + 30]
-        # Check first to see if the file is NSIS
-        nsis_extracted = check_and_extract_NSIS(possible_header, pe)
-        if nsis_extracted:
-            write_multiple_files(out_path, nsis_extracted, log_message)
-            result_code = 5 # NSIS Installer
-            return result_code
-
-        else:
-            log_message("Attempting dynamic trim...")
-            last_section = find_last_section(pe)
-            overlay = memoryview(pe.__data__)[last_section.PointerToRawData + last_section.SizeOfRawData:signature_address or beginning_file_size]
-            
-            # The following checks a sample of the overlay to determine if it will be able to be removed.
-            overlay_compression_sample = get_compressed_size(memoryview(overlay)[-1000:], 1000)
-            sample_compression = overlay_compression_sample / 1000
-            file_size_wo_overlay = len(memoryview(pe.__data__)[:last_section.PointerToRawData + last_section.SizeOfRawData])
-            if sample_compression < 0.05:
-                end_of_real_data, result_code = trim_junk(pe, overlay, beginning_file_size)
-            else:
-                result, result_code = check_section_compression(pe, data_to_delete, log_message=log_message)
-                if len(data_to_delete) == 1:
-                    end_of_real_data = beginning_file_size
-                else:
-                    result_code = 12 # Packed with junk in section
-                    end_of_real_data = beginning_file_size - sum(slice_end-slice_start for slice_start, slice_end in data_to_delete)
-
-            if end_of_real_data > beginning_file_size * 0.9:
-                if last_ditch_processing is True:
-                    log_message("""
-"Last ditch" switch detected. Running last ditch debloat technique:\n
-This is the last resort that removes the whole overlay: this works in cases where the overlay lacks a pattern.
-However, if the file does not run after this, it is in indicator that this method removed critical data.
-                    """)
-                    end_of_real_data = last_section.PointerToRawData + last_section.SizeOfRawData
-                    data_to_delete.append((end_of_real_data, beginning_file_size))
-                else:
-                    log_message("""
-Overlay was unable to be trimmed. Try unpacking with UniExtract2 or re-running
-Debloat with the "--last-ditch" parameter."""
-                                )
-            elif result_code == 12:
-                # The end was already determined and no more data needs to be removed.
-                pass
-            else:
-                data_to_delete.append((end_of_real_data, beginning_file_size))
-    # Handle bloated sections
-    # TODO: break up into functions
-    else:
-        # In order to solve some use cases, we will find the biggest section
-        # within the binary.
-        result, result_code = check_section_compression(pe, data_to_delete, log_message=log_message)
-        log_message(result)
-    # All processing is done. Report results.
-    # There is always the signature in the list
-    if len(data_to_delete) == 0 or sum(slice_end-slice_start for slice_start, slice_end in data_to_delete) <= (beginning_file_size * 0.1):
-        log_message("""No automated method for reducing the size worked. Please consider sharing the
-sample for additional analysis.
-Email: Squiblydoo@pm.me
-Twitter: @SquiblydooBlog.
-                    """)
-        result_code = 0
-        return result_code
-    else:
-        pe_data = bytearray()
-        start = 0
-        for slice_start, slice_end in sorted(data_to_delete):
-            pe_data += bytearray(pe.__data__[start:slice_start])
-            start = slice_end
-        pe_data += bytearray(pe.__data__[start:beginning_file_size])
-        if cert_preservation == True and signature_size > 0:
-            pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].VirtualAddress = len(pe_data) - signature_size
-
-        pe.__data__ = pe_data
-        final_filesize, new_pe_name = write_patched_file(out_path,
-                                                         pe)
-        reduction_calculation = round(((beginning_file_size \
-                                        - final_filesize) \
-                                        / beginning_file_size) * 100, 2)
-        log_message("Beginning File size: " \
-                + readable_size(beginning_file_size) + ".")
-        log_message("File was reduced by " \
-                    + str(reduction_calculation) + "%.")
-        log_message("Final file size: " \
-                    + readable_size(final_filesize) + ".")
-        log_message("Processing complete.\nFile written to '" \
-                    + str(new_pe_name) + "'.")
-        return result_code
+"""
+This file handles the processing of binaries and helper methods.
+
+Three methods rely heavily on parts of Binary Refinery
+https://github.com/binref/refinery
+Copyright 2019 Jesko Hüttenhain under the 3-Clause BSD License
+The methods are:
+refinery_strip()
+adjust_offsets()
+refinery_trim_resources()
+The RSRC Class is also from refinery.
+"""
+from pathlib import Path
+import re
+from typing import Tuple, Optional, Any, Callable, List
+import pefile
+import binascii
+import zlib
+from pefile import Structure, SectionStructure, DIRECTORY_ENTRY
+from typing import Generator, Iterable, Optional
+
+import debloat.utilities.nsisParser as nsisParser
+import debloat.utilities.rsrc as rsrc
+
+DEBLOAT_VERSION = "1.5.6.1"
+
+RESULT_CODES = {
+    0: "No Solution found.",
+    1: "Junk after signature.",
+    2: "Single repeated byte in overlay.",
+    3: "Pattern in overlay.",
+    4: "Sets of repeated bytes in overlay.",
+    5: "NSIS Installer.",
+    6: "Bloat in PE resources",
+    7: "Bloat in PE section",
+    8: "Bloat in .NET resource",
+    9: "Non-essential, high entropy overlay",
+    10: "High compression with bytes at end.",
+    11: ".NET Single File with junk",
+    12: "Packed file with bloated section"
+}
+
+
+_KB = 1000
+_MB = _KB * _KB
+
+def readable_size(value: int) -> str:
+    '''Return bytes in human readable format.'''
+    if value <= 1024:
+        return '%s bytes' % value
+    elif value < 1024 * 1024:
+        return '%.1f KB' % (float(value) / 1024.0)
+    elif value < 1024 * 1024 * 1024:
+        return '%.1f MB' % (float(value) / 1024.0 / 1024.0)
+    else:
+        return '%.1f GB' % (float(value) / 1024.0 / 1024.0 / 1024.0)
+
+def write_multiple_files(out_path: str,
+                         files: list, log_message: Callable[[str], None]) -> None:
+    '''
+    Writes multiple files to disk when applicable.
+    '''
+    log_message("Installer unpacked!\n")
+    log_message(f"The files are being written to {out_path}")
+    for file in files:
+        out_file_path = Path(out_path) / Path(file.path.replace("\\", "/"))
+        out_dir_path = out_file_path.parent
+        out_dir_path.mkdir(parents=True, exist_ok=True)
+        with open(out_file_path, "wb") as f:
+            f.write(file.data)
+            log_message("File: " + str(Path(file.path.replace("\\", "/"))))
+    log_message("")
+    log_message("The user will need to determine which file is malicious if any.")
+    log_message("If a file is bloated: resubmit it through the tool to debloat it.")
+    log_message(f"Consider reviewing the 'setup.nsis' from the installer to determine how the files were meant to be used.")
+    return 
+
+
+def write_patched_file(out_path: str,
+                        pe: pefile.PE) -> Tuple[int, str]:
+    '''Writes the patched file to disk.
+
+    Keyword Arguments:
+    out_path -- the path and file name to write
+    pe -- the pefile that is being processed
+    end_of_real_data -- an int indicating the size of bytes to write'''
+    with open(out_path, 'wb') as writer:
+        writer.write(pe.write())
+        final_filesize = len(pe.write())
+        return final_filesize, out_path
+
+def handle_signature_abnormality(signature_address: int,
+                                signature_size: int,
+                                beginning_file_size: int) -> bool:
+    '''Remove all bytes after a PE signature'''
+    # If the signature_address is 0, there was no original signature.
+    # We are setting the signature address to the filesize in order to
+    # skip the next check.
+    if signature_address == 0:
+        signature_address = beginning_file_size
+    # Check to see if there is data after the signature; if so, it is
+    #  junk data
+    if beginning_file_size > (signature_address + signature_size):
+        return True
+    return False
+
+def check_and_extract_NSIS(possible_header: bytearray, pe: pefile.PE) -> list:
+    '''Check if the PE is an NSIS installer.'''
+    extractor = nsisParser.extractNSIS()
+    confirm_if_nsis = extractor._find_archive_offset(memoryview(possible_header))
+    if confirm_if_nsis is None:
+        return
+    extracted_files = extractor.unpack(memoryview(pe.__data__))
+    return extracted_files
+
+
+def find_last_section(pe: pefile.PE) -> Optional[pefile.SectionStructure]:
+    '''Iterate through PE sections to identify the last one.'''
+    last_section = None
+    for section in pe.sections:
+        if last_section is None \
+                        or section.PointerToRawData > last_section.PointerToRawData:
+            last_section = section
+    return last_section
+
+def get_signature_info(pe: pefile.PE, cert_preservation) -> Tuple[int, int]:
+    '''Remove PE signature and update header.'''
+    signature_address = pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].VirtualAddress
+    signature_size = pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].Size
+    pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].VirtualAddress = 0
+    # If the cert is to be preservered, we do not need to modify the size in the header. 
+    if cert_preservation == False:
+        pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].Size = 0
+
+    return signature_address, signature_size
+
+
+def adjust_offsets(pe: pefile.PE, gap_offset: int, gap_size: int):
+    base = pe.OPTIONAL_HEADER.ImageBase
+    alignment = pe.OPTIONAL_HEADER.FileAlignment
+    rva_offset = pe.get_rva_from_offset(gap_offset)
+    tva_offset = rva_offset + base
+
+    section = pe.get_section_by_offset(gap_offset)
+    new_section_size = section.SizeOfRawData - gap_size
+    if new_section_size % alignment != 0:
+        raise RuntimeError(
+            F'trimming 0x{gap_size:X} bytes from section {(section.Name)} of size 0x{section.SizeOfRawData:X} '
+            F'violates required section alignment of 0x{alignment:X} bytes')
+    inside_section_offset = gap_offset - section.PointerToRawData
+    if inside_section_offset > new_section_size:
+        overlap = inside_section_offset - new_section_size
+        raise RuntimeError(F'trimming from section {(section.Name)}; data extends {overlap} beyond section')
+
+    rva_lbound = section.VirtualAddress
+    rva_ubound = section.VirtualAddress + section.Misc_VirtualSize - 1
+    tva_lbound = rva_lbound + base
+    tva_ubound = rva_ubound + base
+
+    def adjust_attributes_of_structure(
+        structure: Structure,
+        threshold: int,
+        lbound: Optional[int],
+        ubound: Optional[int],
+        attributes: Iterable[str]
+    ):
+        for attribute in attributes:
+            old_value = getattr(structure, attribute, 0)
+            if old_value <= threshold:
+                continue
+            if lbound is not None and old_value < lbound:
+                continue
+            if ubound is not None and old_value > ubound:
+                continue
+            new_value = old_value - gap_size
+            if new_value < 0:
+                raise RuntimeError(F'adjusting attribute {attribute} of {structure.name} would result in negative value: {new_value}')
+            setattr(structure, attribute, new_value)
+
+    it: Iterable[Structure] = iter(pe.__structures__)
+    remove = []
+
+    for index, structure in enumerate(it):
+        old_offset = structure.get_file_offset()
+        new_offset = old_offset - gap_offset
+
+        if old_offset > gap_offset:
+            if old_offset < gap_offset + gap_size:
+                remove.append(index)
+                continue
+            if isinstance(structure, SectionStructure) and new_offset % alignment != 0:
+                raise RuntimeError(
+                    F'section {(structure.Name)} would be moved to offset 0x{new_offset:X}, '
+                    F'violating section alignment value 0x{alignment:X}.')
+            structure.set_file_offset(new_offset)
+
+        adjust_attributes_of_structure(structure, rva_offset, rva_lbound, rva_ubound, (
+            'OffsetToData',
+            'AddressOfData',
+            'VirtualAddress',
+            'AddressOfNames',
+            'AddressOfNameOrdinals',
+            'AddressOfFunctions',
+            'AddressOfEntryPoint',
+            'AddressOfRawData',
+            'BaseOfCode',
+            'BaseOfData',
+        ))
+        adjust_attributes_of_structure(structure, tva_offset, tva_lbound, tva_ubound, (
+            'StartAddressOfRawData',
+            'EndAddressOfRawData',
+            'AddressOfIndex',
+            'AddressOfCallBacks',
+        ))
+        adjust_attributes_of_structure(structure, gap_offset, None, None, (
+            'OffsetModuleName',
+            'PointerToRawData',
+        ))
+
+        for attribute in (
+            'CvHeaderOffset',
+            'OffsetIn2Qwords',
+            'OffsetInQwords',
+            'Offset',
+            'OffsetLow',
+            'OffsetHigh'
+        ):
+            if not hasattr(structure, attribute):
+                continue
+    
+    while remove:
+        index = remove.pop()
+        pe.__structures__[index:index + 1] = []
+
+    section.SizeOfRawData = new_section_size
+    return pe
+
+
+def refinery_strip(data: memoryview, alignment=1, block_size=_MB) -> int:
+    if not data:
+        return 0
+    threshold = 0.05
+    data_overhang = len(data) % alignment
+    result = data_overhang
+
+    if 0 < threshold < 1:
+        def compression_ratio(offset: int):
+            ratio = len(zlib.compress(data[:offset], level=1)) / offset
+            return ratio
+        upper = len(data)
+        lower = result
+
+        if compression_ratio(upper) <= threshold:
+            while block_size < upper - lower:
+                pivot = (lower + upper) // 2
+                ratio = compression_ratio(pivot)
+                if ratio > threshold:
+                    lower = pivot + 1
+                    continue
+                upper = pivot
+                if abs(ratio - threshold) < 1e-10:
+                    break
+
+        result = upper
+    
+    while result > 1 and data[result - 2] == data[result -1]:
+        result -= 1
+
+    result = max(result, data_overhang)
+
+    result = result + (data_overhang - result) % alignment
+
+    if result > len(data):
+        excess = result - len(data)
+        excess = excess + (-excess % alignment)
+        result = result - excess
+
+    return result
+
+
+def refinery_trim_resources(pe: pefile.PE, data_to_delete: List) -> int:
+    size_limit = 10000
+    size_removed = 0
+
+    def find_bloated_resources(pe: pefile.PE, directory, level: int = 0, *path) -> Generator[Structure, None, None]:
+        for entry in directory.entries:
+            name = getattr(entry, 'name')
+            numeric_id = getattr(entry, 'id')
+            if not name:
+                if level == 0 and numeric_id in iter(rsrc.RSRC):
+                    name = rsrc.RSRC(entry.id)
+                elif numeric_id is not None:
+                    name = str(numeric_id)
+            name = name and str(name) or '?'
+            if entry.struct.DataIsDirectory:
+                yield from find_bloated_resources(pe, entry.directory, level + 1, *path, name)
+                continue
+            struct: Structure = entry.data.struct
+            name = '/'.join((*path, name))
+            if struct.Size <= size_limit:
+                continue
+            yield name, struct
+
+    RSRC_INDEX = DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_RESOURCE']
+    pe.parse_data_directories(directories=[RSRC_INDEX])
+
+    try:
+        resources = pe.DIRECTORY_ENTRY_RESOURCE
+    except AttributeError:
+        return 0
+    for name, resource in find_bloated_resources(pe, resources):
+        offset = pe.get_offset_from_rva(resource.OffsetToData)
+        # Offset may be modified from debloating a previous resource
+        original_offset = offset
+        for slice_start, slice_end in data_to_delete:
+            if slice_start <= original_offset:
+                original_offset += slice_end-slice_start
+        old_size = resource.Size
+        new_size = refinery_strip(memoryview(pe.__data__)[original_offset:original_offset + old_size], pe.OPTIONAL_HEADER.FileAlignment)
+        gap_size = old_size - new_size
+        if gap_size <= 0:
+            continue
+        resource.Size = new_size
+        adjust_offsets(pe, offset + new_size, gap_size)
+        size_removed += gap_size
+        data_to_delete.append((original_offset + new_size, original_offset + old_size))
+
+    pe.OPTIONAL_HEADER.DATA_DIRECTORY[RSRC_INDEX].Size -= size_removed
+
+def get_compressed_size(data: memoryview, offset: int, level: int = -1):
+    if offset <= 1024:
+        return len(zlib.compress(data[:offset], level=level))
+
+    compress_obj = zlib.compressobj(level=level)
+    compress_data_len = 0
+    index = 0
+    for index in range(offset//1024):
+        chunk = data[index*1024 : (index+1)*1024]
+        compress_data_len += len(compress_obj.compress(chunk))
+    leftover = offset%1024
+    if leftover:
+        chunk = data[(index+1)*1024 : (index+1)*1024 + leftover]
+        compress_data_len += len(compress_obj.compress(chunk))
+    compress_data_len += len(compress_obj.flush())
+    return compress_data_len
+
+def check_section_compression(pe: pefile.PE, data_to_delete: List,
+                              log_message: Callable[[str], None]) -> Tuple[pefile.PE, int, str]:
+        biggest_section = None
+        biggest_uncompressed = int
+        result = ""
+        for section in pe.sections:
+            section_name = section.Name.decode()
+            compressed_section_size = get_compressed_size(
+                memoryview(pe.__data__)[section.PointerToRawData : section.PointerToRawData+section.SizeOfRawData],
+                section.SizeOfRawData
+            )
+            section_compression_ratio = section.SizeOfRawData / compressed_section_size * 100
+            log_message("Section: "  + section_name, end="\t", flush=True)
+            log_message(" Compression Ratio: " + str(round(section_compression_ratio, 2)) +"%", end="\t",flush=True)
+            log_message("Size of section: " + readable_size(section.SizeOfRawData) +".",flush=True)
+            if biggest_section is None:
+                biggest_section = section
+                biggest_uncompressed = section_compression_ratio
+            elif section.SizeOfRawData > biggest_section.SizeOfRawData:
+                biggest_section = section
+                biggest_uncompressed = section_compression_ratio
+        # Handle specific bloated sections
+        if biggest_section.Name.decode() == ".rsrc\x00\x00\x00":
+            # Get biggest resource or resources and drop them from the
+            # Resource table
+            log_message('''
+Bloat was located in the resource section. Removing bloat..
+''')
+            refinery_trim_resources(pe, data_to_delete)
+            result_code = 6 # Bloated resource
+            return result, result_code
+
+        elif biggest_section.Name.decode() == ".text\x00\x00\x00":
+            # Data stored in the .text section is often a .NET Resource. The following checks
+            # to confirm it is .NET and then drops the resources.
+            if pe.OPTIONAL_HEADER.DATA_DIRECTORY[14].Size:
+                log_message('''
+Bloat was detected in the text section. Bloat is likely in a .NET Resource
+This use case cannot be processed at this time. ''')
+            result_code = 0 # No solution 
+            return result, result_code
+        if biggest_uncompressed > 3000:
+            log_message('''
+The compression ratio of ''' + biggest_section.Name.decode() + ''' is indicative of a bloated section.
+''', end="", flush=True)
+            # Get the size of the section.
+            biggest_section_end = biggest_section.PointerToRawData + biggest_section.SizeOfRawData
+            original_section_size = biggest_section.SizeOfRawData
+            biggest_section_data = memoryview(pe.__data__)[biggest_section.PointerToRawData:biggest_section_end]
+            delta_last_non_junk, result_code = trim_junk(pe, biggest_section_data, original_section_size)
+            # Remove the junk from the section.
+            if delta_last_non_junk > original_section_size:
+                log_message("Section was not able to be reduced.")
+                result_code = 0
+                return result, result_code
+            data_to_delete.append((biggest_section.PointerToRawData + delta_last_non_junk, biggest_section_end))
+            
+            section_bytes_to_remove = original_section_size - delta_last_non_junk
+            # Adjust all offsets for the file.
+            adjust_offsets(pe, biggest_section.PointerToRawData, section_bytes_to_remove)
+            log_message("Bloated section reduced.")
+            result_code = 7 # Bloated PE section
+            return result, result_code
+
+def find_chunk_start(targeted_regex, chunk_start, original_size_with_junk, bloated_content: memoryview, step):
+    bloated_content_len = len(bloated_content)
+    compiled_targeted_regex = re.compile(targeted_regex)
+    chunk_end = chunk_start
+    while original_size_with_junk > chunk_end:
+        chunk_end = chunk_start + step
+        targeted_regex_match = compiled_targeted_regex.search(binascii.hexlify(bytes(bloated_content[max(bloated_content_len - chunk_end, 0):bloated_content_len - chunk_start])[::-1]))
+        if targeted_regex_match:
+            chunk_start += targeted_regex_match.end(0)
+        else:
+            # If the targeted_regex_match does not
+            # return anything, that indicates the previous loop
+            # had content which did not match. We'll use that
+            # to help ensure we do not remove too much of the file.
+            chunk_start -= step * 2
+            break
+    return chunk_start
+
+def trim_junk(pe: pefile.PE, bloated_content: memoryview,
+              original_size_with_junk: int) -> int:
+    '''Attempts multiple methods to trim junk from the end of a section.'''
+    alignment = pe.OPTIONAL_HEADER.FileAlignment
+
+    # Regex Explained:
+    # Match raw bytes that are repeated more than 20 times at the end
+    # of a binary.
+    delta_last_non_junk = original_size_with_junk
+    # First Method: Trims 1 repeating byte.
+    # Check against 200 bytes, if successful, calculate full match.
+    junk_match = re.search(rb'^(..)\1{20,}', bytes(bloated_content[:-601:-1]))
+    chunk_start = 0
+    if not junk_match:
+        # Second method: remove junk using refinery_strip. This method
+        # is more efficent than a previous check that was used here.
+        delta_last_non_junk = refinery_strip(bloated_content, alignment)
+        result_code = 3 # Pattern in overlay.
+
+    # Junk was identified. A new size is assigned and returned.
+    else:
+        # First method continued...
+        bloated_content_len = len(bloated_content)
+        targeted_regex = rb"("+ binascii.hexlify(junk_match.group(1)) + rb")\1{1,}"
+        precompiled_chunk = binascii.hexlify(junk_match.group(1)) * int(1000/len(junk_match.group(1)))
+        chunk_end = chunk_start
+        while original_size_with_junk > chunk_end:
+            chunk_end = chunk_start + 1000
+            chunk = binascii.hexlify(bytes(bloated_content[max(bloated_content_len - chunk_end, 0):bloated_content_len - chunk_start])[::-1])
+            if chunk == precompiled_chunk:
+                chunk_start += 1000
+                continue
+            else:
+                # If the chunk does not match the precompiled chunk,
+                # we will return to the previous chunk_start in order
+                # to ensure important bytes are not removed.
+                if chunk_start > 1000:
+                    chunk_start -= 1000
+                break
+        junk_to_remove = chunk_start 
+
+        # Third Method: check for a series of one repeated byte.
+        # If the trimming did not remove more than half of the bytes then
+        # this suggests the attacker may have put a random series of
+        # repeated bytes. We use refinery_trim for efficiency.
+        if junk_to_remove * 2 < original_size_with_junk / 2:
+            delta_last_non_junk = refinery_strip(bloated_content, alignment)
+            result_code = 4 # Sets of repeated bytes in overlay.
+        else:
+            result_code = 2 # Single repeated byte in overlay
+        delta_last_non_junk -= junk_to_remove
+
+    # The returned size must account for the file alignment.
+    # We will make sure it is aligned by adding bytes.
+    not_aligned = alignment - (delta_last_non_junk % alignment)
+    delta_last_non_junk = delta_last_non_junk + not_aligned
+    if not result_code:
+        result_code = 0
+    return delta_last_non_junk, result_code
+
+def process_pe(pe: pefile.PE, out_path: str, last_ditch_processing: bool,
+                cert_preservation: bool,log_message: Callable[[str], None], 
+                beginning_file_size: int = 0) -> None:
+    '''Prepare PE, perform checks, remote junk, write patched binary.'''
+    result_code = 0
+    if not beginning_file_size:
+        beginning_file_size = len(pe.write())
+
+    # Remove Signature and modify size of Optional Header Security entry.
+    signature_address, signature_size = get_signature_info(pe, cert_preservation)
+    if cert_preservation == True:
+        cert = [(signature_address, signature_address + signature_size)]
+        data_to_delete = []
+    else:
+        if signature_size > 0:
+            log_message("""A certificate is being removed from this file.\n-To preserve the certificate use the Cert Preservation option.""")
+        data_to_delete = [(signature_address, signature_address + signature_size)]
+
+    signature_abnormality = handle_signature_abnormality(signature_address,
+                                                        signature_size,
+                                                        beginning_file_size)
+    if signature_abnormality:
+        data_to_delete.append((signature_address + signature_size, beginning_file_size))
+        result_code = 1  # Junk after signture
+
+    # Handle Overlays: this includes packers and overlays which are completely junk
+    elif pe.get_overlay_data_start_offset() and signature_size < len(pe.__data__) - pe.get_overlay_data_start_offset():
+        possible_header = pe.__data__[pe.get_overlay_data_start_offset():pe.get_overlay_data_start_offset() + 30]
+        # Check first to see if the file is NSIS
+        nsis_extracted = check_and_extract_NSIS(possible_header, pe)
+        if nsis_extracted:
+            write_multiple_files(out_path, nsis_extracted, log_message)
+            result_code = 5 # NSIS Installer
+            return result_code
+
+        else:
+            log_message("Attempting dynamic trim...")
+            last_section = find_last_section(pe)
+            overlay = memoryview(pe.__data__)[last_section.PointerToRawData + last_section.SizeOfRawData:signature_address or beginning_file_size]
+            
+            # The following checks a sample of the overlay to determine if it will be able to be removed.
+            overlay_compression_sample = get_compressed_size(memoryview(overlay)[-1000:], 1000)
+            sample_compression = overlay_compression_sample / 1000
+            file_size_wo_overlay = len(memoryview(pe.__data__)[:last_section.PointerToRawData + last_section.SizeOfRawData])
+            if sample_compression < 0.05:
+                end_of_real_data, result_code = trim_junk(pe, overlay, beginning_file_size)
+            else:
+                result, result_code = check_section_compression(pe, data_to_delete, log_message=log_message)
+                if len(data_to_delete) == 1:
+                    end_of_real_data = beginning_file_size
+                else:
+                    result_code = 12 # Packed with junk in section
+                    end_of_real_data = beginning_file_size - sum(slice_end-slice_start for slice_start, slice_end in data_to_delete)
+
+            if end_of_real_data > beginning_file_size * 0.9:
+                if last_ditch_processing is True:
+                    log_message("""
+"Last ditch" switch detected. Running last ditch debloat technique:\n
+This is the last resort that removes the whole overlay: this works in cases where the overlay lacks a pattern.
+However, if the file does not run after this, it is in indicator that this method removed critical data.
+                    """)
+                    end_of_real_data = last_section.PointerToRawData + last_section.SizeOfRawData
+                    data_to_delete.append((end_of_real_data, beginning_file_size))
+                else:
+                    log_message("""
+Overlay was unable to be trimmed. Try unpacking with UniExtract2 or re-running
+Debloat with the "--last-ditch" parameter."""
+                                )
+            elif result_code == 12:
+                # The end was already determined and no more data needs to be removed.
+                pass
+            else:
+                data_to_delete.append((end_of_real_data, beginning_file_size))
+    # Handle bloated sections
+    # TODO: break up into functions
+    else:
+        # In order to solve some use cases, we will find the biggest section
+        # within the binary.
+        result, result_code = check_section_compression(pe, data_to_delete, log_message=log_message)
+        log_message(result)
+    # All processing is done. Report results.
+    # There is always the signature in the list
+    if len(data_to_delete) == 0 or sum(slice_end-slice_start for slice_start, slice_end in data_to_delete) <= (beginning_file_size * 0.1):
+        log_message("""No automated method for reducing the size worked. Please consider sharing the
+sample for additional analysis.
+Email: Squiblydoo@pm.me
+Twitter: @SquiblydooBlog.
+                    """)
+        result_code = 0
+        return result_code
+    else:
+        pe_data = bytearray()
+        start = 0
+        for slice_start, slice_end in sorted(data_to_delete):
+            pe_data += bytearray(pe.__data__[start:slice_start])
+            start = slice_end
+        pe_data += bytearray(pe.__data__[start:beginning_file_size])
+        if cert_preservation == True and signature_size > 0:
+            pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].VirtualAddress = len(pe_data) - signature_size
+
+        pe.__data__ = pe_data
+        final_filesize, new_pe_name = write_patched_file(out_path,
+                                                         pe)
+        reduction_calculation = round(((beginning_file_size \
+                                        - final_filesize) \
+                                        / beginning_file_size) * 100, 2)
+        log_message("Beginning File size: " \
+                + readable_size(beginning_file_size) + ".")
+        log_message("File was reduced by " \
+                    + str(reduction_calculation) + "%.")
+        log_message("Final file size: " \
+                    + readable_size(final_filesize) + ".")
+        log_message("Processing complete.\nFile written to '" \
+                    + str(new_pe_name) + "'.")
+        return result_code
```

### Comparing `debloat-1.5.6/src/debloat/processor.pyi` & `debloat-1.5.6.1/src/debloat/processor.pyi`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import pefile
-from _typeshed import Incomplete
-from pefile import Structure as Structure
-from typing import Callable, Optional, Tuple
-
-PACKER: Incomplete
-
-def readable_size(value: int) -> str: ...
-def write_multiple_files(out_path: str, files: list, log_message: Callable[[str], None]) -> None: ...
-def write_patched_file(out_path: str, pe: pefile.PE) -> Tuple[int, str]: ...
-def handle_signature_abnormality(signature_address: int, signature_size: int, beginning_file_size: int) -> bool: ...
-def check_and_extract_NSIS(possible_header: bytearray, data: bytearray) -> list: ...
-def check_for_packer(possible_header: bytearray) -> int: ...
-def find_last_section(pe: pefile.PE) -> Optional[pefile.SectionStructure]: ...
-def get_signature_info(pe: pefile.PE) -> Tuple[int, int]: ...
-def adjust_offsets(pe: pefile.PE, gap_offset: int, gap_size: int): ...
-def refinery_strip(pe: pefile.PE, data: memoryview, block_size=...) -> int: ...
-def refinery_trim_resources(pe: pefile.PE, pe_data: bytearray) -> int: ...
-def remove_resources(pe: pefile.PE, pe_data: bytearray) -> Tuple[bytearray, int]: ...
-def check_section_compression(pe: pefile.PE, pe_data: bytearray, end_of_real_data, log_message: Callable[[str], None]) -> Tuple[pefile.PE, int, str]: ...
-def trim_junk(pe: pefile.PE, bloated_content: bytes, original_size_with_junk: int) -> int: ...
-def process_pe(pe: pefile.PE, out_path: str, last_ditch_processing: bool, log_message: Callable[[str], None]) -> None: ...
+import pefile
+from _typeshed import Incomplete
+from pefile import Structure as Structure
+from typing import Callable, Optional, Tuple
+
+PACKER: Incomplete
+
+def readable_size(value: int) -> str: ...
+def write_multiple_files(out_path: str, files: list, log_message: Callable[[str], None]) -> None: ...
+def write_patched_file(out_path: str, pe: pefile.PE) -> Tuple[int, str]: ...
+def handle_signature_abnormality(signature_address: int, signature_size: int, beginning_file_size: int) -> bool: ...
+def check_and_extract_NSIS(possible_header: bytearray, data: bytearray) -> list: ...
+def check_for_packer(possible_header: bytearray) -> int: ...
+def find_last_section(pe: pefile.PE) -> Optional[pefile.SectionStructure]: ...
+def get_signature_info(pe: pefile.PE) -> Tuple[int, int]: ...
+def adjust_offsets(pe: pefile.PE, gap_offset: int, gap_size: int): ...
+def refinery_strip(pe: pefile.PE, data: memoryview, block_size=...) -> int: ...
+def refinery_trim_resources(pe: pefile.PE, pe_data: bytearray) -> int: ...
+def remove_resources(pe: pefile.PE, pe_data: bytearray) -> Tuple[bytearray, int]: ...
+def check_section_compression(pe: pefile.PE, pe_data: bytearray, end_of_real_data, log_message: Callable[[str], None]) -> Tuple[pefile.PE, int, str]: ...
+def trim_junk(pe: pefile.PE, bloated_content: bytes, original_size_with_junk: int) -> int: ...
+def process_pe(pe: pefile.PE, out_path: str, last_ditch_processing: bool, log_message: Callable[[str], None]) -> None: ...
```

### Comparing `debloat-1.5.6/src/debloat/tests/debloat_test.py` & `debloat-1.5.6.1/src/debloat/tests/debloat_test.py`

 * *Files identical despite different names*

### Comparing `debloat-1.5.6/src/debloat/utilities/nsisParser.py` & `debloat-1.5.6.1/src/debloat/utilities/nsisParser.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,1336 +1,1336 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-# Most of this code was repurposed from Binary Refinery (https://github.com/binref/refinery), used under the 3-Clause BSD License
-
-from collections import namedtuple
-import struct
-
-import enum
-
-import itertools
-import re
-import io
-import dataclasses
-
-import zlib
-import lzma
-
-from datetime import datetime
-
-import logging
-from debloat.utilities.readers import StructReader, Struct, StreamDetour, MemoryFile
-from debloat.utilities.pyflate import BZip2File
-from typing import (
-    BinaryIO, 
-    NamedTuple, 
-    Iterable, 
-    Iterator, 
-    Callable, 
-    Union, 
-    ByteString, 
-    Optional, 
-    List, 
-    Dict,
-    Type)
-
-logging.basicConfig(level=logging.WARN)
-
-class UnpackResult:
-
-    def get_data(self) -> ByteString:
-        if Callable(self.data):
-            self.data = self.data()
-        return self.data
-
-    def __init__(self, _br__path: str, _br__data: Union[ByteString, Callable[[], ByteString]], **_br__meta):
-        self.path = _br__path
-        self.data = _br__data
-        self.meta = _br__meta
-        for key in [key for key, value in _br__meta.items() if value is None]:
-            del _br__meta[key]   
-
-class ArchiveUnit:
-    def __init__(self, *paths, 
-                 list=False, join_path=False, 
-                 drop_path=False, fuzzy=0, exact=False, 
-                 regex=False, 
-                 date=b'date', 
-                 path=b'path', **kwargs):
-        self.paths = paths
-        self.list = list
-        self.join_path = join_path
-        self.drop_path = drop_path
-        self.fuzzy = fuzzy
-        self.exact = exact
-        self.regex = regex
-        self.path = path
-        self.date = date,
-        self.kwargs = kwargs
-
-    def _pack(
-        self,
-        path: str,
-        date: Optional[Union[datetime, str]],
-        data: Union[ByteString, Callable[[], ByteString]],
-        **meta
-    ) -> UnpackResult:
-        if isinstance(date, datetime):
-            date = date.isoformat(' ', 'seconds')
-        if isinstance(date, str):
-            meta[self.args.date.decode(self.codec)] = date
-        return UnpackResult(path, data, **meta)
-
-class DeflateFile(io.RawIOBase):
-
-    data: MemoryFile
-    dc: zlib.decompress
-
-    def __new__(cls, data: MemoryFile):
-        self = super().__new__(cls)
-        self.data = data
-        self.dc = zlib.decompressobj(-15)
-        return io.BufferedReader(self)
-
-    def readall(self) -> bytes:
-        return self.read()
-
-    def readinto(self, __buffer):
-        data = self.read(len(__buffer))
-        size = len(data)
-        __buffer[:size] = data
-        return size
-
-    def read(self, size=-1):
-        buffer = self.dc.unconsumed_tail or self.data.read(size)
-        kwargs = {}
-        if size > 0:
-            kwargs.update(max_length=size)
-        return self.dc.decompress(buffer, **kwargs)
-
-    def readable(self) -> bool:
-        return True
-
-    def seekable(self) -> bool:
-        return False
-
-    def writable(self) -> bool:
-        return False
-
-    def write(self, __b):
-        raise NotImplementedError
-
-class LZMAOptions(NamedTuple):
-    filter_flag: bool
-    dictionary_size: int
-
-class NSBlockHeaderOffset(Struct):
-    def __init__(self, reader: StructReader, is64bit: bool):
-        self.offset = reader.u64() if is64bit else reader.u32()
-        self.size = reader.u32()
-
-class NSMethod(str, enum.Enum):
-    Copy = 'COPY'
-    LZMA = 'LZMA'
-    BZip2 = 'BZIP2'
-    Deflate = 'DEFLATE'
-
-class Op(enum.IntEnum):
-    INVALID_OPCODE     = 0              # noqa
-    RET                = enum.auto()    # noqa; Return
-    NOP                = enum.auto()    # noqa; Nop, Goto
-    ABORT              = enum.auto()    # noqa; Abort
-    QUIT               = enum.auto()    # noqa; Quit
-    CALL               = enum.auto()    # noqa; Call, InitPluginsDir
-    UPDATETEXT         = enum.auto()    # noqa; DetailPrint
-    SLEEP              = enum.auto()    # noqa; Sleep
-    BRINGTOFRONT       = enum.auto()    # noqa; BringToFront
-    CHDETAILSVIEW      = enum.auto()    # noqa; SetDetailsView
-    SETFILEATTRIBUTES  = enum.auto()    # noqa; SetFileAttributes
-    CREATEDIR          = enum.auto()    # noqa; CreateDirectory, SetOutPath
-    IFFILEEXISTS       = enum.auto()    # noqa; IfFileExists
-    SETFLAG            = enum.auto()    # noqa; SetRebootFlag, ...
-    IFFLAG             = enum.auto()    # noqa; IfAbort, IfSilent, IfErrors, IfRebootFlag
-    GETFLAG            = enum.auto()    # noqa; GetInstDirError, GetErrorLevel
-    RENAME             = enum.auto()    # noqa; Rename
-    GETFULLPATHNAME    = enum.auto()    # noqa; GetFullPathName
-    SEARCHPATH         = enum.auto()    # noqa; SearchPath
-    GETTEMPFILENAME    = enum.auto()    # noqa; GetTempFileName
-    EXTRACTFILE        = enum.auto()    # noqa; File
-    DELETEFILE         = enum.auto()    # noqa; Delete
-    MESSAGEBOX         = enum.auto()    # noqa; MessageBox
-    RMDIR              = enum.auto()    # noqa; RMDir
-    STRLEN             = enum.auto()    # noqa; StrLen
-    ASSIGNVAR          = enum.auto()    # noqa; StrCpy
-    STRCMP             = enum.auto()    # noqa; StrCmp
-    READENVSTR         = enum.auto()    # noqa; ReadEnvStr, ExpandEnvStrings
-    INTCMP             = enum.auto()    # noqa; IntCmp, IntCmpU
-    INTOP              = enum.auto()    # noqa; IntOp
-    INTFMT             = enum.auto()    # noqa; IntFmt/Int64Fmt
-    PUSHPOP            = enum.auto()    # noqa; Push/Pop/Exchange
-    FINDWINDOW         = enum.auto()    # noqa; FindWindow
-    SENDMESSAGE        = enum.auto()    # noqa; SendMessage
-    ISWINDOW           = enum.auto()    # noqa; IsWindow
-    GETDLGITEM         = enum.auto()    # noqa; GetDlgItem
-    SETCTLCOLORS       = enum.auto()    # noqa; SetCtlColors
-    SETBRANDINGIMAGE   = enum.auto()    # noqa; SetBrandingImage / LoadAndSetImage
-    CREATEFONT         = enum.auto()    # noqa; CreateFont
-    SHOWWINDOW         = enum.auto()    # noqa; ShowWindow, EnableWindow, HideWindow
-    SHELLEXEC          = enum.auto()    # noqa; ExecShell
-    EXECUTE            = enum.auto()    # noqa; Exec, ExecWait
-    GETFILETIME        = enum.auto()    # noqa; GetFileTime
-    GETDLLVERSION      = enum.auto()    # noqa; GetDLLVersion
-#   GETFONTVERSION     = enum.auto()    # noqa; Park : 2.46.2
-#   GETFONTNAME        = enum.auto()    # noqa; Park : 2.46.3
-    REGISTERDLL        = enum.auto()    # noqa; RegDLL, UnRegDLL, CallInstDLL
-    CREATESHORTCUT     = enum.auto()    # noqa; CreateShortCut
-    COPYFILES          = enum.auto()    # noqa; CopyFiles
-    REBOOT             = enum.auto()    # noqa; Reboot
-    WRITEINI           = enum.auto()    # noqa; WriteINIStr, DeleteINISec, DeleteINIStr, FlushINI
-    READINISTR         = enum.auto()    # noqa; ReadINIStr
-    DELREG             = enum.auto()    # noqa; DeleteRegValue, DeleteRegKey
-    WRITEREG           = enum.auto()    # noqa; WriteRegStr, WriteRegExpandStr, WriteRegBin, WriteRegDWORD
-    READREGSTR         = enum.auto()    # noqa; ReadRegStr, ReadRegDWORD
-    REGENUM            = enum.auto()    # noqa; EnumRegKey, EnumRegValue
-    FCLOSE             = enum.auto()    # noqa; FileClose
-    FOPEN              = enum.auto()    # noqa; FileOpen
-    FPUTS              = enum.auto()    # noqa; FileWrite, FileWriteByte
-    FGETS              = enum.auto()    # noqa; FileRead, FileReadByte
-#   Park:
-#   FPUTWS             = enum.auto()    # noqa; FileWriteUTF16LE, FileWriteWord
-#   FGETWS             = enum.auto()    # noqa; FileReadUTF16LE, FileReadWord
-    FSEEK              = enum.auto()    # noqa; FileSeek
-    FINDCLOSE          = enum.auto()    # noqa; FindClose
-    FINDNEXT           = enum.auto()    # noqa; FindNext
-    FINDFIRST          = enum.auto()    # noqa; FindFirst
-    WRITEUNINSTALLER   = enum.auto()    # noqa; WriteUninstaller
-#   Park : since 2.46.3 the log is enabled in main Park version
-#   LOG                = enum.auto()    # noqa; LogSet, LogText
-    SECTIONSET         = enum.auto()    # noqa; Get*, Set*
-    INSTTYPESET        = enum.auto()    # noqa; InstTypeSetText, InstTypeGetText, SetCurInstType, GetCurInstType
-#   Before NSIS v3.06: Instructions not actually implemented in exehead, but used in compiler.
-#   GETLABELADDR       = enum.auto()    # noqa; both of these get converted to ASSIGNVAR
-#   GETFUNCTIONADDR    = enum.auto()    # noqa
-#   In NSIS v3.06 and later it was changed to:
-    GETOSINFO          = enum.auto()    # noqa
-    RESERVEDOPCODE     = enum.auto()    # noqa
-    LOCKWINDOW         = enum.auto()    # noqa; LockWindow
-#   Two unicode commands available only in Unicode archive:
-    FPUTWS             = enum.auto()    # noqa; FileWriteUTF16LE, FileWriteWord
-    FGETWS             = enum.auto()    # noqa; FileReadUTF16LE, FileReadWord
-#   Since NSIS v3.06 the fllowing IDs codes was moved here:
-#   Opcodes listed here are not actually used in exehead.
-#   No exehead opcodes should be present after these!
-#   GETLABELADDR       = enum.auto()    # noqa; ASSIGNVAR
-#   GETFUNCTIONADDR    = enum.auto()    # noqa; ASSIGNVAR
-#   The following IDs are not IDs in real order.
-#   We just need some IDs to translate eny extended layout to main layout:
-    LOG                = enum.auto()    # noqa; LogSet, LogText
-#   Park
-    FINDPROC           = enum.auto()    # noqa; FindProc
-    GETFONTVERSION     = enum.auto()    # noqa; GetFontVersion
-    GETFONTNAME        = enum.auto()    # noqa; GetFontName
-
-    @classmethod
-    def from_int(cls, value: int) -> 'Op':
-        try:
-            return cls(value)
-        except ValueError:
-            return cls.INVALID_OPCODE
-_Op_PARAMETER_COUNT = {
-    Op.INVALID_OPCODE   : 0,
-    Op.RET              : 0,
-    Op.NOP              : 1,
-    Op.ABORT            : 1,
-    Op.QUIT             : 0,
-    Op.CALL             : 2,
-    Op.UPDATETEXT       : 6,
-    Op.SLEEP            : 1,
-    Op.BRINGTOFRONT     : 0,
-    Op.CHDETAILSVIEW    : 2,
-    Op.SETFILEATTRIBUTES: 2,
-    Op.CREATEDIR        : 3,
-    Op.IFFILEEXISTS     : 3,
-    Op.SETFLAG          : 3,
-    Op.IFFLAG           : 4,
-    Op.GETFLAG          : 2,
-    Op.RENAME           : 4,
-    Op.GETFULLPATHNAME  : 3,
-    Op.SEARCHPATH       : 2,
-    Op.GETTEMPFILENAME  : 2,
-    Op.EXTRACTFILE      : 6,
-    Op.DELETEFILE       : 2,
-    Op.MESSAGEBOX       : 6,
-    Op.RMDIR            : 2,
-    Op.STRLEN           : 2,
-    Op.ASSIGNVAR        : 4,
-    Op.STRCMP           : 5,
-    Op.READENVSTR       : 3,
-    Op.INTCMP           : 6,
-    Op.INTOP            : 4,
-    Op.INTFMT           : 4,
-    Op.PUSHPOP          : 6,
-    Op.FINDWINDOW       : 5,
-    Op.SENDMESSAGE      : 6,
-    Op.ISWINDOW         : 3,
-    Op.GETDLGITEM       : 3,
-    Op.SETCTLCOLORS     : 2,
-    Op.SETBRANDINGIMAGE : 4,
-    Op.CREATEFONT       : 5,
-    Op.SHOWWINDOW       : 4,
-    Op.SHELLEXEC        : 6,
-    Op.EXECUTE          : 3,
-    Op.GETFILETIME      : 3,
-    Op.GETDLLVERSION    : 4,
-    Op.REGISTERDLL      : 6,
-    Op.CREATESHORTCUT   : 6,
-    Op.COPYFILES        : 4,
-    Op.REBOOT           : 1,
-    Op.WRITEINI         : 5,
-    Op.READINISTR       : 4,
-    Op.DELREG           : 5,
-    Op.WRITEREG         : 6,
-    Op.READREGSTR       : 5,
-    Op.REGENUM          : 5,
-    Op.FCLOSE           : 1,
-    Op.FOPEN            : 4,
-    Op.FPUTS            : 3,
-    Op.FGETS            : 4,
-    Op.FSEEK            : 4,
-    Op.FINDCLOSE        : 1,
-    Op.FINDNEXT         : 2,
-    Op.FINDFIRST        : 3,
-    Op.WRITEUNINSTALLER : 4,
-    Op.SECTIONSET       : 5,
-    Op.INSTTYPESET      : 4,
-    Op.GETOSINFO        : 6,
-    Op.RESERVEDOPCODE   : 2,
-    Op.LOCKWINDOW       : 1,
-    Op.FPUTWS           : 4,
-    Op.FGETWS           : 4,
-    Op.LOG              : 2,
-    Op.FINDPROC         : 2,
-    Op.GETFONTVERSION   : 2,
-    Op.GETFONTNAME      : 2,
-}
-
-NS_SHELL_STRINGS = {
-    0x00: 'DESKTOP',
-    0x01: 'INTERNET',
-    0x02: 'SMPROGRAMS',
-    0x03: 'CONTROLS',
-    0x04: 'PRINTERS',
-    0x05: 'DOCUMENTS',
-    0x06: 'FAVORITES',
-    0x07: 'SMSTARTUP',
-    0x08: 'RECENT',
-    0x09: 'SENDTO',
-    0x0A: 'BITBUCKET',
-    0x0B: 'STARTMENU',
-    0x0D: 'MUSIC',
-    0x0E: 'VIDEOS',
-    0x10: 'DESKTOP',
-    0x11: 'DRIVES',
-    0x12: 'NETWORK',
-    0x13: 'NETHOOD',
-    0x14: 'FONTS',
-    0x15: 'TEMPLATES',
-    0x16: 'STARTMENU',
-    0x17: 'SMPROGRAMS',
-    0x18: 'SMSTARTUP',
-    0x19: 'DESKTOP',
-    0x1A: 'APPDATA',
-    0x1B: 'PRINTHOOD',
-    0x1C: 'LOCALAPPDATA',
-    0x1D: 'ALTSTARTUP',
-    0x1E: 'ALTSTARTUP',
-    0x1F: 'FAVORITES',
-    0x20: 'INTERNET_CACHE',
-    0x21: 'COOKIES',
-    0x22: 'HISTORY',
-    0x23: 'APPDATA',
-    0x24: 'WINDIR',
-    0x25: 'SYSDIR',
-    0x26: 'PROGRAM_FILES',
-    0x27: 'PICTURES',
-    0x28: 'PROFILE',
-    0x29: 'SYSTEMX86',
-    0x2A: 'PROGRAM_FILESX86',
-    0x2B: 'PROGRAM_FILES_COMMON',
-    0x2C: 'PROGRAM_FILES_COMMONX8',
-    0x2D: 'TEMPLATES',
-    0x2E: 'DOCUMENTS',
-    0x2F: 'ADMINTOOLS',
-    0x30: 'ADMINTOOLS',
-    0x31: 'CONNECTIONS',
-    0x35: 'MUSIC',
-    0x36: 'PICTURES',
-    0x37: 'VIDEOS',
-    0x38: 'RESOURCES',
-    0x39: 'RESOURCES_LOCALIZED',
-    0x3A: 'COMMON_OEM_LINKS',
-    0x3B: 'CDBURN_AREA',
-    0x3D: 'COMPUTERSNEARME',
-}
-
-NS_VARIABLE_STRINGS = (
-    "CMDLINE",
-    "INSTDIR",
-    "OUTDIR",
-    "EXEDIR",
-    "LANGUAGE",
-    "TEMP",
-    "PLUGINSDIR",
-    "EXEPATH",  # NSIS 2.26+
-    "EXEFILE",  # NSIS 2.26+
-    "HWNDPARENT",
-    "CLICK",    # set from page->clicknext
-    "OUTDIR",   # NSIS 2.04+
-)
-
-class NSHeaderFlags(enum.IntFlag):
-    Undefined = 0
-    Uninstall = 1
-    Silent = 2
-    NoCrc = 4
-    ForceCrc = 8
-    LongOffset = 16
-    ExternalFileSupport = 32
-    ExternalFile = 64
-    IsStubInstaller = 128
-
-
-
-class NSType(enum.IntEnum):
-    Nsis2 = 0
-    Nsis3 = enum.auto()
-    Park1 = enum.auto()
-    Park2 = enum.auto()
-    Park3 = enum.auto()
-
-class NSScriptInstruction(Struct):
-    def __init__(self, reader: StructReader):
-        self.opcode = reader.u32()
-        self.arguments = [reader.u32() for _ in range(6)]
-
-class NSCharCode(enum.IntEnum):
-    NONE = 0
-    CHAR = enum.auto()
-    SKIP = enum.auto()
-    SHELL = enum.auto()
-    VAR = enum.auto()
-    LANG = enum.auto()
-
-    @property
-    def special(self):
-        return self > NSCharCode.CHAR
-    
-@dataclasses.dataclass(eq=True)
-class NSItem:
-    offset: int
-    name: Optional[str] = None
-    mtime: Optional[datetime] = None
-    is_compressed: bool = True
-    is_uninstaller: bool = False
-    attributes: Optional[int] = None
-    size: Optional[int] = None
-    compressed_size: Optional[int] = None
-    estimated_size: Optional[int] = None
-    dictionary_size: int = 1
-    patch_size: int = 0
-    prefix: Optional[str] = None
-
-    @property
-    def path(self) -> str:
-        path = self.name
-        if self.prefix:
-            path = F'{self.prefix}\\{path}'
-        return path
-    
-    def __str__(self) -> str:
-        return self.name
-
-
-class NSHeader(Struct):
-    BACKSLASH           = ord('\\')  # noqa
-    NS_CMDLINE          = 20         # noqa
-    NS_INSTDIR          = 21         # noqa
-    NS_OUTDIR           = 22         # noqa
-    NS_EXEDIR           = 23         # noqa
-    NS_LANGUAGE         = 24         # noqa
-    NS_TEMP             = 25         # noqa
-    NS_PLUGINSDIR       = 26         # noqa
-    NS_EXEPATH          = 27         # noqa NSIS 2.26+
-    NS_EXEFILE          = 28         # noqa NSIS 2.26+
-    NS_HWNDPARENT_225   = 27         # noqa
-    NS_HWNDPARENT_226   = 29         # noqa
-    NS_CLICK            = 30         # noqa
-    NS_OUTDIR_225       = 29         # noqa NSIS 2.04 - 2.25
-    NS_OUTDIR_226       = 31         # noqa NSIS 2.26+
-
-    def _string_args_to_single_arg(self, arg1: int, 
-                                   arg2: Optional[int] = None) -> int:
-        if self.type >= NSType.Park1:
-            return arg1 & 0x7FFF
-        else:
-            if arg2 is None:
-                arg2 = arg1 >> 8
-            arg1 &= 0x7F
-            arg2 &= 0x7F
-            return arg1 | arg2 << 7
-
-    def _get_char_code(self, char: int) -> NSCharCode:
-        if self.type >= NSType.Park1:
-            if char < 0x80:
-                return NSCharCode.CHAR
-            lookup = {
-                0xE000: NSCharCode.SKIP,
-                0xE001: NSCharCode.VAR,
-                0xE002: NSCharCode.SHELL,
-                0xE003: NSCharCode.LANG,
-            }
-        elif self.type is NSType.Nsis3:
-            if char > 4:
-                return NSCharCode.CHAR
-            lookup = {
-                0x0002: NSCharCode.SHELL,
-                0x0003: NSCharCode.VAR,
-                0x0004: NSCharCode.SKIP,
-            }
-        elif self.type is NSType.Nsis2:
-            lookup = {
-                0x00FC: NSCharCode.SKIP,
-                0x00FD: NSCharCode.VAR,
-                0x00FE: NSCharCode.SHELL,
-            }
-        else:
-            raise ValueError(F'Unknown NSIS type {self.type}.')
-        return lookup.get(char, NSCharCode.NONE)
-
-    def _string_code_shell(self, index1: int, 
-                           index2: Optional[int] = None) -> str:
-        if index2 is None:
-            index2 = index1 >> 8
-            index1 &= 0xFF
-        if index1 & 0x80 != 0:
-            offset = index1 & 0x3F
-            with StreamDetour(self.strings, offset):
-                if self.strings.tell() != offset:
-                    raise ValueError(F'Failed to detour to offset 0x{offset:02X}.')
-                path = self._read_current_string()
-                if path.startswith('ProgramFilesDir'):
-                    return '$PROGRAMFILES'
-                if path.startswith('CommonFilesDir'):
-                    return '$COMMONFILES'
-                suffix = 32 * (index1 >> 5 & 2)
-                return F'$REG{suffix}({path})'
-        for index in (index1, index2):
-            shell = NS_SHELL_STRINGS.get(index)
-            if shell is not None:
-                return F'$SHELL:{shell}'
-        else:
-            return F'Error:$SHELL:{index1:02X}{index2:02X}'
-
-    def _string_code_variable(self, index: int) -> str:
-        varcount = 20 + len(NS_VARIABLE_STRINGS)
-        if self._is_nsis200:
-            varcount -= 3
-        elif self._is_nsis225:
-            varcount -= 2
-        if index < 20:
-            if index >= 10:
-                return F'$R{index - 10}'
-            return F'$V{index}'
-        else:
-            if index < varcount:
-                if self._is_nsis225 and index >= self.NS_EXEPATH:
-                    index += 2
-                try:
-                    variable = NS_VARIABLE_STRINGS[index - 20]
-                except IndexError:
-                    return F'Error:$V:{index}'
-                else:
-                    return F'${variable}'
-            return F'Error:$V:{index}'
-        
-    def _string_code_language(self, index: int) -> str:
-        return F'$LANGUAGE:{index}'
-
-    @property
-    def _read_char(self) -> str:
-        return self.strings.u16 if self.unicode else self.strings.u8
-    
-    def _seek_to_string(self, position: int) -> bool:
-        pos = position * self.charsize
-        return self.strings.seek(pos) == pos
-    
-    def _read_string(self, position: int) -> Optional[str]:
-        if position < 0:
-            return self._string_code_language(-(position + 1))
-        if not self._seek_to_string(position):
-            return None
-        return self._read_current_string()
-
-    def _read_string_raw(self, position: int) -> Optional[str]:
-        if not self._seek_to_string(position):
-            return None
-        if self.unicode:
-            return self.strings.read_w_string()
-        else:
-            return self.strings.read_c_string()
-        
-    def _is_var_absolute_path(self, position: int) -> bool:
-        var = self._get_var_index(position)
-        if var is None:
-            return False
-        return var in (
-            self.NS_INSTDIR,
-            self.NS_EXEDIR,
-            self.NS_TEMP,
-            self.NS_PLUGINSDIR,
-        )
-    
-    def _is_good_string(self, position: int) -> bool:
-        if position == 0:
-            return False
-        if not self._seek_to_string(position - 1):
-            return False
-        prefix = self._read_char()
-        return prefix == 0 or prefix == self.BACKSLASH
-
-    def _is_var_str(self, position: int, index: int) -> bool:
-        if index > 0x7FFF:
-            return False
-        var_index = self._get_var_index(position)
-        if var_index is None:
-            return False
-        if self._get_resource_finished(position, 0) is None:
-            return False
-        return var_index == index
-
-    def _get_var_index(self, position: int) -> Optional[int]:
-        if not self._seek_to_string(position):
-            raise LookupError(F'Failed to seek to string at position 0x{position:08X}.')
-        try:
-            code = self._read_char()
-            if self._get_char_code(code) is not NSCharCode.VAR:
-                return None
-            arg1 = self._read_char()
-            if arg1 == 0:
-                return None
-            if self.unicode:
-                args = arg1,
-            else:
-                arg2 = self._read_char()
-                if arg2 == 0:
-                    return None
-                args = arg1, arg2
-            return self._string_args_to_single_arg(*args)
-        except EOFError:
-            return None
-        
-    def _get_resource(self, position: int) -> Optional[int]:
-        if self.unicode:
-            if len(self.strings) - position >= 4:
-                return 2
-        else:
-            if len(self.strings) - position >= 3:
-                return 3
-        return None
-
-    def _get_resource_finished(self, position: int, 
-                          terminator: int) -> Optional[int]:
-        if not self._seek_to_string(position):
-            return None
-        self.strings.seek_relative(3)
-        if self.unicode:
-            self.strings.seek_relative(1)
-        if self.strings.remaining_bytes < self.charsize:
-            return None
-        if self._read_char() != terminator:
-            return None
-        return 3 if self.unicode else 4
-
-
-    @property
-    def charsize(self) -> int:
-        return 2 if self.unicode else 1
-
-    def _read_current_string(self) -> str:
-        string = io.StringIO()
-        chars = iter(self._read_char, 0)
-        for letter in chars:
-            code = self._get_char_code(letter)
-            if code is NSCharCode.CHAR:
-                string.write(chr(letter))
-                continue
-            if code.special:
-                try:
-                    var1 = next(chars)
-                except StopIteration:
-                    break
-                if var1 == 0:
-                    break
-                if code is NSCharCode.SKIP:
-                    letter = var1
-                else:
-                    if not self.unicode:
-                        try:
-                            var2 = next(chars)
-                        except StopIteration:
-                                break
-                        if var2 == 0:
-                            break
-                        vars = var1, var2
-                    else:
-                        vars = var1,
-                    if code is NSCharCode.SHELL:
-                        string.write(self._string_code_shell(*vars))
-                        continue
-                    else:
-                        var = self._string_args_to_single_arg(*vars)
-                        if code is NSCharCode.VAR:
-                            string.write(self._string_code_variable(var))
-                        if code is NSCharCode.LANG:
-                            string.write(self._string_code_language(var))
-                        continue
-            string.write(chr(letter))
-        return string.getvalue()
-
-    def opcode(self, cmd: NSScriptInstruction) -> Op:
-        code = cmd.opcode
-        if self.type < NSType.Park1:
-            if self._log_cmd_is_enabled:
-                return Op.from_int(code)
-            if code < Op.SECTIONSET:
-                return Op.from_int(code)
-            if code is Op.SECTIONSET:
-                return Op.LOG
-            return Op.from_int(code - 1)
-        if code < Op.REGISTERDLL:
-            return Op.from_int(code)
-        if self.type >= NSType.Park2:
-            if code == Op.REGISTERDLL:
-                return Op.GETFONTVERSION
-            code -= 1
-        if self.type >= NSType.Park3:
-            if code == Op.REGISTERDLL:
-                return Op.GETFONTNAME
-            code -= 1
-        if code >= Op.FSEEK:
-            if self.unicode:
-                if code == Op.FSEEK:
-                    return Op.FPUTWS
-                if code == Op.FSEEK + 1:
-                    return Op.FGETWS
-                code -= 2
-            if code >= Op.SECTIONSET and self._log_cmd_is_enabled:
-                if code == Op.SECTIONSET:
-                    return Op.LOG
-                return Op.from_int(code - 1)
-            if code == Op.FPUTWS:
-                return Op.FINDPROC
-        return Op.from_int(code)
-
-    def _find_bad_cmd(self) -> None:
-        self._bad_cmd = -1
-        for instruction in self.instructions:
-            cmd = self.opcode(instruction)
-            arg = instruction.arguments
-            if cmd is Op.INVALID_OPCODE:
-                continue
-            if cmd >= self._bad_cmd >= 0:
-                continue
-            if self.type is NSType.Nsis3:
-                if cmd == Op.RESERVEDOPCODE:
-                    self._bad_cmd = cmd
-                    continue
-            else:
-                if cmd == Op.RESERVEDOPCODE or cmd == Op.GETOSINFO:
-                    self._bad_cmd = cmd
-                    continue
-            last_non_empty_index = max((k for k, a in enumerate(arg, 1) if a), default=0)
-            if cmd == Op.FINDPROC and last_non_empty_index == 0:
-                continue
-            if _Op_PARAMETER_COUNT[cmd] < last_non_empty_index:
-                self._bad_cmd = cmd
-
-    def _guess_nsis_version(self):
-        self.strong_nsis = False
-        self.strong_park = False
-        char_mask = 0x8080 if self.unicode else 0x80
-        self.strings.seek(0)
-        while not self.strings.is_eof:
-            string = self._read_current_string()
-            if string is None:
-                continue
-            if len(string) < 2:
-                continue
-            if ord(string[0]) != 3:
-                continue
-            if ord(string[1]) & char_mask == char_mask:
-                self.type = NSType.Nsis3
-                self.strong_nsis = True
-                break
-        if self.unicode:
-            if not self.strong_nsis:
-                self.type = NSType.Park1
-                self.strong_park = True
-        elif self.type is NSType.Nsis2:
-            for instruction in self.instructions:
-                cmd = self.opcode(instruction)
-                arg = instruction.arguments
-                if cmd is Op.GETDLGITEM:
-                    if self._is_var_str(arg[1], self.NS_HWNDPARENT_225):
-                        self._is_nsis225 = True
-                        if arg[0] == self.NS_OUTDIR_225:
-                            self._is_nsis200 = True
-                            break
-                if cmd is Op.ASSIGNVAR:
-                    if arg[0] == self.NS_OUTDIR_225 and arg[2] == 0 and arg[3] == 0:
-                        self._is_nsis225 = self._is_var_str(arg[1], self.NS_OUTDIR)
-        got_park_version = False
-        mask = 0
-        IN = 4 if self.unicode else 2
-        if not self.strong_nsis and not self._is_nsis225 and not self._is_nsis200:
-            for instruction in self.instructions:
-                cmd = instruction.opcode
-                arg = instruction.arguments
-                alt = arg[3]
-                if cmd < Op.WRITEUNINSTALLER or cmd > Op.WRITEUNINSTALLER + IN:
-                    continue
-                if arg[4] != 0 or arg[5] != 0 or arg[0] <= 1 or alt <= 1:
-                    continue
-                if not self._is_good_string(arg[0]) or not self._is_good_string(alt):
-                    continue
-                index = self._get_var_index(alt)
-                if index is None:
-                    continue
-                additional = self._get_resource_finished(alt, self.BACKSLASH)
-                if index != self.NS_INSTDIR:
-                    continue
-                if self._read_string_raw(alt + additional) == self._read_string_raw(arg[0]):
-                    inserts = cmd - Op.WRITEUNINSTALLER.value
-                    mask |= 1 << inserts
-            if mask == 1:
-                got_park_version = True
-            elif mask:
-                shift = 0
-                nt = self.type
-                if self.unicode:
-                    shift = 2
-                if mask == 1 << (shift + 1):
-                    nt = NSType.Park2
-                if mask == 1 << (shift + 2):
-                    nt = NSType.Park3
-                if nt != self.type:
-                    self.type = nt
-                    got_park_version = True
-        self._find_bad_cmd()
-        if self._bad_cmd < Op.REGISTERDLL:
-            return
-        if self.strong_park and not got_park_version:
-            if self._bad_cmd < Op.SECTIONSET:
-                self.type = NSType.Park3
-                self._log_cmd_is_enabled = True
-                self._find_bad_cmd()
-                if self._bad_cmd in range(Op.SECTIONSET):
-                    self.type = NSType.Park2
-                    self._log_cmd_is_enabled = False
-                    self._find_bad_cmd()
-                    if self._bad_cmd in range(Op.SECTIONSET):
-                        self.type = NSType.Park1
-                        self._find_bad_cmd()
-        if self._bad_cmd >= Op.SECTIONSET:
-            self._log_cmd_is_enabled = not self._log_cmd_is_enabled
-            self._find_bad_cmd()
-            if self._bad_cmd >= Op.SECTIONSET and self._log_cmd_is_enabled:
-                self._log_cmd_is_enabled = False
-                self._find_bad_cmd()   
-
-    def _read_items(self) -> List[NSItem]:
-        prefixes = ['$INSTDIR']
-        out_dir = ''
-        out_dir_index = (
-            self.NS_OUTDIR_225
-        ) if self._is_nsis225 else (
-            self.NS_OUTDIR_226
-        )
-        items: List[NSItem] = []
-
-        for cmd_index, instruction in enumerate(self.instructions):
-            def set_path(index:int) -> None:
-                item.prefix = None
-                item.name = self._read_string(index)
-                if not self._is_var_absolute_path(index):
-                    item.prefix = prefixes[-1]
-            
-            cmd = self.opcode(instruction)
-            arg = instruction.arguments
-
-            if cmd is Op.INVALID_OPCODE:
-                continue
-            elif cmd is Op.CREATEDIR:
-                if not arg[1]:
-                    continue
-                _path = arg[0]
-                index = self._get_var_index(_path)
-                if index in (out_dir_index, self.NS_OUTDIR):
-                    _path += self._get_resource(_path)
-                path = self._read_string(_path)
-                if index == out_dir_index:
-                    path = out_dir + path
-                elif index == self.NS_OUTDIR:
-                    path = prefixes[-1] + path
-                prefixes.append(path)
-            elif cmd is Op.ASSIGNVAR:
-                if arg[0] != out_dir_index:
-                    continue
-                if self._is_var_str(arg[1], self.NS_OUTDIR) and arg[2] == 0 and arg[3] == 0:
-                    out_dir = prefixes[-1]
-            elif cmd is Op.EXTRACTFILE:
-                try:
-                    time = datetime.fromtimestamp(arg[4] << 32 | arg[3])
-                except Exception:
-                    time = None
-                item = NSItem(arg[2], mtime=time)
-                set_path(arg[1])
-                items.append(item)
-                if not self._is_var_str(arg[1], 10):
-                    continue
-                cmd_back_offset = 28
-                if cmd_index > 1:
-                    previous = self.instructions[cmd_index - 1]
-                    if self.opcode(previous) is Op.NOP:
-                        cmd_back_offset -= 2
-                if cmd_index <= cmd_back_offset:
-                    continue
-                previous = self.instructions[cmd_index - cmd_back_offset]
-                if self.opcode(previous) is Op.ASSIGNVAR:
-                    previous_arguments = previous.arguments
-                    if previous_arguments[0] == 14 and previous_arguments[2] == 0 and previous_arguments[3] == 0:
-                        set_path(previous_arguments[1])
-            elif cmd is Op.SETFILEATTRIBUTES:
-                if cmd_index > 0:
-                    previous = self.instructions[cmd_index - 1]
-                    previous_arguments = previous.arguments
-                    if self.opcode(previous) is Op.EXTRACTFILE and arg[0] == previous_arguments[1]:
-                        item = items[-1]
-                        item.attributes = arg[1]
-            elif cmd is Op.WRITEUNINSTALLER:
-                if arg[4] or arg[5] or arg[0] <=1 or arg[3] <= 1:
-                    continue
-                if not self._is_good_string(arg[0]):
-                    continue
-                if self._bad_cmd in range(Op.WRITEUNINSTALLER):
-                    continue
-                item = NSItem(arg[1])
-                set_path(arg[0])
-                item.patch_size = arg[2]
-                item.is_uninstaller = True
-                items.append(item)
-        return items
-                
-    @property
-    def script(self):
-        script = io.StringIO()
-        name_width = max(len(op.name) for op in Op)
-        addr_width = len(F'{len(self.instructions):X}')
-        for k, instruction in enumerate(self.instructions):
-            if k > 0:
-                script.write('\n')
-            opcode = self.opcode(instruction)
-            script.write(F'{k:0{addr_width}X} {opcode.name:{name_width}}')
-            for j, arg in enumerate(instruction.arguments[:_Op_PARAMETER_COUNT.get(opcode, 6)]):
-                if j > 0:
-                    script.write(', ')
-                if arg > 20 and self._is_good_string(arg):
-                    script.write(repr(self._read_string(arg)))
-                elif arg < 0x100:
-                    script.write(str(arg))
-                elif arg < 0x10000:
-                    script.write(F'${arg:04X}')
-                else:
-                    script.write(F'${arg:08X}')
-        return script.getvalue()
-
-    def _string_code_language(self, index: int) -> str:
-        return F'$LANGUAGE:{index:04X}'
-
-
-    def __init__(self, reader: StructReader[bytearray], size: int):
-        self.is64bit = size >= 100 and not any(
-            struct.unpack('8xI' * 8, reader.peek(12 * 8)))
-        block_header_offset_size = 12 if self.is64bit else 8
-        required_size = block_header_offset_size * 8 + 4
-        if size < required_size:
-            raise ValueError(F'Header size 0x{size:08X} is too small. Minimum required size is 0x{required_size:08X}.')
-        # TODO: Confirm role of unknown value. Copilot believes it to be
-        # a signature indicating the end of the NSIS installer header.
-        self.unknown_value = reader.u32()
-        self.block_header_offsets = [NSBlockHeaderOffset(
-            reader.read(block_header_offset_size), 
-            is64bit=self.is64bit) for _ in range(8)]
-        self.block_header_entries = self.block_header_offsets[2]
-        self.block_header_strings = self.block_header_offsets[3]
-        self.block_header_langtables = self.block_header_offsets[4]
-        
-        for key, offset in enumerate(self.block_header_offsets):
-            width = 0x10 if self.is64bit else 8
-            table = {2: 'entries', 3: 'strings', 4: 'langtables'}.get(key)
-            message = F'Block {key}: offset=0x{offset.offset:0{width}X}, size=0x{offset.size:0{width}X}'
-            if table is not None:
-                message += F'{message} ({table})'
-            logging.debug(message)
-
-        self.type = NSType.Nsis2 # Default to NSIS 2
-        
-        reader.seek_set(self.block_header_entries.offset)
-        self.instructions: List[NSScriptInstruction] = [NSScriptInstruction(reader) for _ in range(self.block_header_entries.size)]
-
-        if self.block_header_entries.offset > size:
-            raise ValueError(F'Header indicates {self.block_header_entries.size} entries, but only {size} bytes remain.')
-        if self.block_header_strings.offset > size:
-            raise ValueError(F'Header indicates {self.block_header_strings.size} strings, but only {size} bytes remain.')
-        if self.block_header_langtables.offset > size:
-            raise ValueError(F'Header indicates {self.block_header_langtables.size} langtables, but only {size} bytes remain.')
-        if self.block_header_langtables.offset < self.block_header_strings.offset:
-            raise ValueError(F'Langtables block is before strings block.')
-        string_table_size = self.block_header_langtables.offset - self.block_header_strings.offset
-        if string_table_size < 2:
-            raise ValueError(F'String table size is too small.')
-        reader.seek_set(self.block_header_strings.offset)
-        strings = reader.read(string_table_size)
-        self.unicode = strings[:2] == B'\0\0'
-        if strings[-1] != 0 or (self.unicode and strings[-2] != 0):
-            raise ValueError(F'String table is not null-terminated.')
-        if self.unicode and string_table_size % 2 != 0:
-            raise ValueError(F'String table is not even-sized.')
-
-        self.strings = StructReader(strings)
-        if self.block_header_entries.size > (1 << 25):
-            raise ValueError(F'Header indicates {self.block_header_entries.size} entries, which is too large.')
-        
-        self._log_cmd_is_enabled = False
-        self._is_nsis225 = False
-        self._is_nsis200 = False
-        self_bad_cmd = -1
-
-        self._guess_nsis_version()
-
-        items: Dict[(str, int), NSItem] = {}
-        for item in self._read_items():
-            if items.setdefault((item.path, item.offset), item) != item:
-                raise ValueError(F'Duplicate item: {item.path} at 0x{item.offset:08X}')
-        
-        self.items = [items[t] for t in sorted(items.keys())]
-        
-
-
-class NSArchive(Struct):
-    MAGICS = [
-        # https://nsis.sourceforge.io/Can_I_decompile_an_existing_installer
-        B'\xEF\xBE\xAD\xDE' B'Null' B'soft' B'Inst',   # v1.6
-        B'\xEF\xBE\xAD\xDE' B'Null' B'Soft' B'Inst',   # v1.3
-        B'\xED\xBE\xAD\xDE' B'Null' B'Soft' B'Inst',   # v1.1
-        B'\xEF\xBE\xAD\xDE' B'nsis' B'inst' B'all\0',  # v1.0
-    ]
-
-    @dataclasses.dataclass
-    class Entry:
-        offset: int
-        data: bytearray
-        compressed_size: int
-        decompression_failed: bool = False
-
-
-    def __init__(self, reader: StructReader[bytearray]):
-        self.flags = NSHeaderFlags(reader.u32())
-        self.signature = reader.read(0x10)
-        header_data = None
-        header_size = reader.u32()
-        header_data_length = None
-        archive_size = reader.u32()
-        self.archive_offset = reader.tell()
-        body_size = archive_size - self.archive_offset
-        if body_size < 0:
-            raise ValueError("Invalid archive size")
-        if header_size < self.archive_offset:
-            raise ValueError("Invalid header size")
-        if reader.remaining_bytes < body_size:
-            raise ValueError(
-                F'Header indicates archive size 0x{archive_size:08X}, '
-                F'but only 0x{reader.remaining_bytes:08X} bytes remain.')
-    
-        # Prepare to check compression format. This takes
-        # a few bytes and checks the header to determine the format
-        preview_bytes = bytes(reader.peek(4))
-        preview_value = int.from_bytes(preview_bytes, byteorder='little')
-        
-        # The default "solid" value is True and default method is deflate.
-        # Regarding Solid:
-        # "If /SOLID is used, all of the installer data is compressed in one block. This results in greater compression ratios."
-        # We determine if the compression is solid or not by checking the headers.
-        # https://nsis.sourceforge.io/Docs/Chapter4.html#
-        
-        self.solid = True
-        self.lzma_options: Optional[LZMAOptions] = None
-        self.method = NSMethod.Deflate
-
-        # Header Matching Logic:
-        #  X is the header size as given by the first header
-        #  T is a value less than 0xE
-        #  Y is a value different from 0x80
-        # XX XX XX XX __ __ __ __ __ __ __  non-solid, uncompressed
-        # 5D 00 00 DD DD 00 __ __ __ __ __  solid LZMA
-        # 00 5D 00 00 DD DD 00 __ __ __ __  solid LZMA, empty filter
-        # 01 5D 00 00 DD DD 00 __ __ __ __  solid LZMA, BCJ filter
-         # __ __ __ 80 5D 00 00 DD DD 00 __  non-solid LZMA
-        # __ __ __ 80 00 5D 00 00 DD DD 00  non-solid LZMA, empty filter
-        # __ __ __ 80 01 5D 00 00 DD DD 00  non-solid LZMA, BCJ filter
-        # __ __ __ 80 01 0T __ __ __ __ __  non-solid BZip
-        # __ __ __ 80 __ __ __ __ __ __ __  non-solid deflate
-        # 01 0T __ YY __ __ __ __ __ __ __  solid BZip
-        # __ __ __ YY __ __ __ __ __ __ __  solid Deflate
-        
-        def lzmacheck(preview):
-            if B'\x5D\0\0' not in preview:
-                return False
-            filter_flag = preview_bytes[0] <= 1
-            reader.seek_relative(3 + int(filter_flag))
-            self.lzma_options = LZMAOptions(filter_flag, reader.u32())
-            return True
-        
-        def bzipcheck(preview):
-            return preview[0] == 0x31 and preview[1] < 14
-        
-        if preview_value == header_size:
-            self.solid = False
-            header_data = reader.read_exactly(header_size)
-            self.method = NSMethod.Copy
-        elif lzmacheck(preview_bytes):
-            self.method = NSMethod.LZMA
-        elif preview_bytes[3] == 0x80:
-            self.solid = False
-            reader.seek_relative(4)
-            second_preview = bytes(reader.peek(4))
-            if lzmacheck(second_preview):
-                self.method = NSMethod.LZMA
-            elif bzipcheck(second_preview):
-                self.method = NSMethod.BZip2
-        elif bzipcheck(preview_bytes):
-            self.method = NSMethod.BZip2
-
-        reader.seek_set(self.archive_offset)
-        self.entries: Dict[int, bytearray] = {}
-        self.entry_offset_delta = 0
-        self._solid_iter = None
-
-        if header_data is None:
-            item = self._decompress_items(reader)
-            try:
-                header_entry = next(item)
-            except zlib.error as ZLERR:
-                raise NotImplementedError(
-                    'This archive seems to use an NSIS-specific deflate '
-                    'algorithm which has not been implemented yet.'
-                ) from ZLERR
-            if self.solid:
-                self._solid_iter = item 
-            self.entry_offset_delta = header_entry.compressed_size + 4
-            header_data = header_entry.data
-        else:
-            self.entry_offset_delta = len(header_data)
-
-        if not header_data:
-            raise ValueError("Empty header")
-        logging.debug(F'Header size: 0x{header_size:08X}')
-
-        self.header = NSHeader(header_data, size=header_size)
-        self.reader = reader
-        
-    @property
-    def script(self):
-        return self.header.script
-    
-    @property
-    def offset_items(self):
-        return self.archive_offset + self.entry_offset_delta
-    
-    def _extract_item_data(self, item: NSItem) -> Entry:
-        if self.solid:
-            while True:
-                try:
-                    entry = self.entries[item.offset]
-                except KeyError:
-                    try:
-                        entry = next(self._solid_iter)
-                    except StopIteration:
-                        raise LookupError(F'Failed to find item at offset 0x{item.offset:08X}.')
-                    self.entries[entry.offset - self.entry_offset_delta] = entry.data
-                else: 
-                    return entry
-        else:
-            self.reader.seek(self.offset_items + item.offset)
-            decompressed = self._decompress_items(self.reader)
-            entry = next(decompressed).data
-            return entry
-
-    class PartsReader(Iterable[Entry]):
-        def __init__(self, src: BinaryIO):
-            self.src = src
-            self.pos = 0
-
-        def __iter__(self):
-            return self
-        
-        def __next__(self):
-            offset = self.pos
-            size = self.src.read(4)
-            if len(size) != 4:
-                raise StopIteration
-            size = int.from_bytes(size, byteorder='little')
-            read = size & 0x7FFFFFFF
-            data = self.src.read(read)
-            if len(data) != read:
-                raise EOFError('Unexpected end of stream while decompressing archive entries.')
-            self.pos = offset + size + 4
-            return NSArchive.Entry(offset, data, size)
-
-    class SolidReader(PartsReader):
-        def __init__(self, src: BinaryIO, decompressor: Type[BinaryIO]):
-            super().__init__(src)
-            self._dc = decompressor
-
-        def __next__(self):
-            item = super().__next__()
-            is_compressed = bool(item.compressed_size & 0x80000000)
-            item.compressed_size &= 0x7FFFFFFF
-            if is_compressed:
-                try:
-                    dc = self._dc(MemoryFile(item.data))
-                    item.data = dc.read()
-                except Exception:
-                    item.decompression_failed = True
-            return item              
-        
-    class LZMAFix:
-        ''' Creates a wrapper to compensate for how NSIS handles LZMA'''
-        def __init__(self, src: MemoryFile):
-            self._src = src
-            self._fix = MemoryFile(bytes(src.read(5)) + B'\xFF' * 8)
-
-        def __getattr__(self, key):
-            return getattr(self._src, key)
-        
-        def read(self, size: int = -1):
-            src = self._src
-            fix = self._fix
-            if not fix.remaining_bytes:
-                return src.read(size)
-            if size < 0:
-                size = fix.remaining_bytes + src.remaining_bytes
-            data = bytearray(size)
-            wrapper = fix.read(size)
-            data[:len(wrapper)] = wrapper
-            data[len(wrapper):] = src.read(size - len(wrapper))
-            return data
-    
-
-
-    def _decompress_items(self, reader: StructReader[bytearray]) -> Iterator[Entry]:
-        """ Decompresses the items in the archive. """
-        def NSISLZMAFile(d):
-            return lzma.LZMAFile(self.LZMAFix(d))
-        decompressor: Type[BinaryIO]= {
-            NSMethod.Deflate : DeflateFile,
-            NSMethod.LZMA    : NSISLZMAFile,
-            NSMethod.BZip2   : BZip2File,
-        }[self.method]
-        if self.solid:
-            return self.PartsReader(decompressor(reader))
-        return self.SolidReader(reader, decompressor)
-        
-
-class extractNSIS(ArchiveUnit):
-    """
-    A class to extract an NSIS file.
-    """
-    @classmethod
-    def _find_archive_offset(cls, data: memoryview, before: int = -1, flaw_max=2) -> int:
-        def signatures(*magics):
-            for changes in range(flaw_max + 1):
-                for magic in magics:
-                    if not changes:
-                        yield 0, magic
-                        continue
-                    for positions in itertools.permutations(range(len(magic)), r=changes):
-                        signature = bytearray(magic)
-                        for position in positions:
-                            signature[position] = 0x2E
-                        yield changes, bytes(signature)
-        best_guess = None
-        search_space = memoryview(data)
-        for flaws, sig in signatures(*NSArchive.MAGICS):
-            if flaws > 1:
-                search_space = search_space[:0x20_000]
-            matches = [m.start() - 4 for m in re.finditer(sig, 
-                                                          search_space, 
-                                                          flags=re.DOTALL)]
-            if before >= 0:
-                matches = [match for match in matches if match < before]
-            matches.reverse()
-            archive = None
-            for match in matches:
-                if match % 0x200 == 0:
-                    archive = match
-                    break
-            if not archive:
-                if matches and not best_guess:
-                    best_guess = matches[-1]
-            else:
-                message = F'Archive signature was found at offset 0x{archive:08X}.'
-                if flaws > 0:
-                    message += F' the signature has {flaws} flaws and was likely modified.'
-                logging.debug(message)
-                return archive
-        if best_guess:
-            message = F'Archive signature was found at offset 0x{best_guess:08X}, but it has too many flaws to be reliable.'
-            logging.debug(message)
-        return best_guess
-
-    def unpack(self, data: memoryview):
-        memory = memoryview(data)
-        before = -1
-        _error = None
-        while True:
-            offset = self._find_archive_offset(data, before)
-            if offset is None:
-                _error = _error or ValueError("Unable to find NSIS archive marker")
-                raise _error
-            try:
-                archive = NSArchive(memory[offset:])
-            except Exception as e:
-                _error = e
-                before = offset
-            else:
-                break
-
-        def info():
-            yield F'{archive.header.type.name} archive'
-            yield F'{archive.method.name.lower()} compression'
-            yield F'Mystery value 0x{archive.header.unknown_value:X}'
-            yield 'solid archive' if archive.solid else 'non-solid archive'
-            yield '64-bit archive' if archive.header.is64bit else '32-bit archive'
-            yield 'unicode' if archive.header.unicode else 'ansi'
-        
-        logging.info(', '.join(info()))
-        unpacked_items = []
-        for item in archive.header.items:
-            unpacked_items.append(self._pack(item.path, item.mtime, archive._extract_item_data(item)))
-            #data = archive._extract_item_data(item)
-            logging.info(F'{item.path} at 0x{item.offset:08X}, {len(data)} bytes')
-        unpacked_items.append(self._pack('setup.nsis', None, archive.script.encode('utf-8'))) 
-        return unpacked_items
-
-
-
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+# Most of this code was repurposed from Binary Refinery (https://github.com/binref/refinery), used under the 3-Clause BSD License
+
+from collections import namedtuple
+import struct
+
+import enum
+
+import itertools
+import re
+import io
+import dataclasses
+
+import zlib
+import lzma
+
+from datetime import datetime
+
+import logging
+from debloat.utilities.readers import StructReader, Struct, StreamDetour, MemoryFile
+from debloat.utilities.pyflate import BZip2File
+from typing import (
+    BinaryIO, 
+    NamedTuple, 
+    Iterable, 
+    Iterator, 
+    Callable, 
+    Union, 
+    ByteString, 
+    Optional, 
+    List, 
+    Dict,
+    Type)
+
+logging.basicConfig(level=logging.WARN)
+
+class UnpackResult:
+
+    def get_data(self) -> ByteString:
+        if Callable(self.data):
+            self.data = self.data()
+        return self.data
+
+    def __init__(self, _br__path: str, _br__data: Union[ByteString, Callable[[], ByteString]], **_br__meta):
+        self.path = _br__path
+        self.data = _br__data
+        self.meta = _br__meta
+        for key in [key for key, value in _br__meta.items() if value is None]:
+            del _br__meta[key]   
+
+class ArchiveUnit:
+    def __init__(self, *paths, 
+                 list=False, join_path=False, 
+                 drop_path=False, fuzzy=0, exact=False, 
+                 regex=False, 
+                 date=b'date', 
+                 path=b'path', **kwargs):
+        self.paths = paths
+        self.list = list
+        self.join_path = join_path
+        self.drop_path = drop_path
+        self.fuzzy = fuzzy
+        self.exact = exact
+        self.regex = regex
+        self.path = path
+        self.date = date,
+        self.kwargs = kwargs
+
+    def _pack(
+        self,
+        path: str,
+        date: Optional[Union[datetime, str]],
+        data: Union[ByteString, Callable[[], ByteString]],
+        **meta
+    ) -> UnpackResult:
+        if isinstance(date, datetime):
+            date = date.isoformat(' ', 'seconds')
+        if isinstance(date, str):
+            meta[self.args.date.decode(self.codec)] = date
+        return UnpackResult(path, data, **meta)
+
+class DeflateFile(io.RawIOBase):
+
+    data: MemoryFile
+    dc: zlib.decompress
+
+    def __new__(cls, data: MemoryFile):
+        self = super().__new__(cls)
+        self.data = data
+        self.dc = zlib.decompressobj(-15)
+        return io.BufferedReader(self)
+
+    def readall(self) -> bytes:
+        return self.read()
+
+    def readinto(self, __buffer):
+        data = self.read(len(__buffer))
+        size = len(data)
+        __buffer[:size] = data
+        return size
+
+    def read(self, size=-1):
+        buffer = self.dc.unconsumed_tail or self.data.read(size)
+        kwargs = {}
+        if size > 0:
+            kwargs.update(max_length=size)
+        return self.dc.decompress(buffer, **kwargs)
+
+    def readable(self) -> bool:
+        return True
+
+    def seekable(self) -> bool:
+        return False
+
+    def writable(self) -> bool:
+        return False
+
+    def write(self, __b):
+        raise NotImplementedError
+
+class LZMAOptions(NamedTuple):
+    filter_flag: bool
+    dictionary_size: int
+
+class NSBlockHeaderOffset(Struct):
+    def __init__(self, reader: StructReader, is64bit: bool):
+        self.offset = reader.u64() if is64bit else reader.u32()
+        self.size = reader.u32()
+
+class NSMethod(str, enum.Enum):
+    Copy = 'COPY'
+    LZMA = 'LZMA'
+    BZip2 = 'BZIP2'
+    Deflate = 'DEFLATE'
+
+class Op(enum.IntEnum):
+    INVALID_OPCODE     = 0              # noqa
+    RET                = enum.auto()    # noqa; Return
+    NOP                = enum.auto()    # noqa; Nop, Goto
+    ABORT              = enum.auto()    # noqa; Abort
+    QUIT               = enum.auto()    # noqa; Quit
+    CALL               = enum.auto()    # noqa; Call, InitPluginsDir
+    UPDATETEXT         = enum.auto()    # noqa; DetailPrint
+    SLEEP              = enum.auto()    # noqa; Sleep
+    BRINGTOFRONT       = enum.auto()    # noqa; BringToFront
+    CHDETAILSVIEW      = enum.auto()    # noqa; SetDetailsView
+    SETFILEATTRIBUTES  = enum.auto()    # noqa; SetFileAttributes
+    CREATEDIR          = enum.auto()    # noqa; CreateDirectory, SetOutPath
+    IFFILEEXISTS       = enum.auto()    # noqa; IfFileExists
+    SETFLAG            = enum.auto()    # noqa; SetRebootFlag, ...
+    IFFLAG             = enum.auto()    # noqa; IfAbort, IfSilent, IfErrors, IfRebootFlag
+    GETFLAG            = enum.auto()    # noqa; GetInstDirError, GetErrorLevel
+    RENAME             = enum.auto()    # noqa; Rename
+    GETFULLPATHNAME    = enum.auto()    # noqa; GetFullPathName
+    SEARCHPATH         = enum.auto()    # noqa; SearchPath
+    GETTEMPFILENAME    = enum.auto()    # noqa; GetTempFileName
+    EXTRACTFILE        = enum.auto()    # noqa; File
+    DELETEFILE         = enum.auto()    # noqa; Delete
+    MESSAGEBOX         = enum.auto()    # noqa; MessageBox
+    RMDIR              = enum.auto()    # noqa; RMDir
+    STRLEN             = enum.auto()    # noqa; StrLen
+    ASSIGNVAR          = enum.auto()    # noqa; StrCpy
+    STRCMP             = enum.auto()    # noqa; StrCmp
+    READENVSTR         = enum.auto()    # noqa; ReadEnvStr, ExpandEnvStrings
+    INTCMP             = enum.auto()    # noqa; IntCmp, IntCmpU
+    INTOP              = enum.auto()    # noqa; IntOp
+    INTFMT             = enum.auto()    # noqa; IntFmt/Int64Fmt
+    PUSHPOP            = enum.auto()    # noqa; Push/Pop/Exchange
+    FINDWINDOW         = enum.auto()    # noqa; FindWindow
+    SENDMESSAGE        = enum.auto()    # noqa; SendMessage
+    ISWINDOW           = enum.auto()    # noqa; IsWindow
+    GETDLGITEM         = enum.auto()    # noqa; GetDlgItem
+    SETCTLCOLORS       = enum.auto()    # noqa; SetCtlColors
+    SETBRANDINGIMAGE   = enum.auto()    # noqa; SetBrandingImage / LoadAndSetImage
+    CREATEFONT         = enum.auto()    # noqa; CreateFont
+    SHOWWINDOW         = enum.auto()    # noqa; ShowWindow, EnableWindow, HideWindow
+    SHELLEXEC          = enum.auto()    # noqa; ExecShell
+    EXECUTE            = enum.auto()    # noqa; Exec, ExecWait
+    GETFILETIME        = enum.auto()    # noqa; GetFileTime
+    GETDLLVERSION      = enum.auto()    # noqa; GetDLLVersion
+#   GETFONTVERSION     = enum.auto()    # noqa; Park : 2.46.2
+#   GETFONTNAME        = enum.auto()    # noqa; Park : 2.46.3
+    REGISTERDLL        = enum.auto()    # noqa; RegDLL, UnRegDLL, CallInstDLL
+    CREATESHORTCUT     = enum.auto()    # noqa; CreateShortCut
+    COPYFILES          = enum.auto()    # noqa; CopyFiles
+    REBOOT             = enum.auto()    # noqa; Reboot
+    WRITEINI           = enum.auto()    # noqa; WriteINIStr, DeleteINISec, DeleteINIStr, FlushINI
+    READINISTR         = enum.auto()    # noqa; ReadINIStr
+    DELREG             = enum.auto()    # noqa; DeleteRegValue, DeleteRegKey
+    WRITEREG           = enum.auto()    # noqa; WriteRegStr, WriteRegExpandStr, WriteRegBin, WriteRegDWORD
+    READREGSTR         = enum.auto()    # noqa; ReadRegStr, ReadRegDWORD
+    REGENUM            = enum.auto()    # noqa; EnumRegKey, EnumRegValue
+    FCLOSE             = enum.auto()    # noqa; FileClose
+    FOPEN              = enum.auto()    # noqa; FileOpen
+    FPUTS              = enum.auto()    # noqa; FileWrite, FileWriteByte
+    FGETS              = enum.auto()    # noqa; FileRead, FileReadByte
+#   Park:
+#   FPUTWS             = enum.auto()    # noqa; FileWriteUTF16LE, FileWriteWord
+#   FGETWS             = enum.auto()    # noqa; FileReadUTF16LE, FileReadWord
+    FSEEK              = enum.auto()    # noqa; FileSeek
+    FINDCLOSE          = enum.auto()    # noqa; FindClose
+    FINDNEXT           = enum.auto()    # noqa; FindNext
+    FINDFIRST          = enum.auto()    # noqa; FindFirst
+    WRITEUNINSTALLER   = enum.auto()    # noqa; WriteUninstaller
+#   Park : since 2.46.3 the log is enabled in main Park version
+#   LOG                = enum.auto()    # noqa; LogSet, LogText
+    SECTIONSET         = enum.auto()    # noqa; Get*, Set*
+    INSTTYPESET        = enum.auto()    # noqa; InstTypeSetText, InstTypeGetText, SetCurInstType, GetCurInstType
+#   Before NSIS v3.06: Instructions not actually implemented in exehead, but used in compiler.
+#   GETLABELADDR       = enum.auto()    # noqa; both of these get converted to ASSIGNVAR
+#   GETFUNCTIONADDR    = enum.auto()    # noqa
+#   In NSIS v3.06 and later it was changed to:
+    GETOSINFO          = enum.auto()    # noqa
+    RESERVEDOPCODE     = enum.auto()    # noqa
+    LOCKWINDOW         = enum.auto()    # noqa; LockWindow
+#   Two unicode commands available only in Unicode archive:
+    FPUTWS             = enum.auto()    # noqa; FileWriteUTF16LE, FileWriteWord
+    FGETWS             = enum.auto()    # noqa; FileReadUTF16LE, FileReadWord
+#   Since NSIS v3.06 the fllowing IDs codes was moved here:
+#   Opcodes listed here are not actually used in exehead.
+#   No exehead opcodes should be present after these!
+#   GETLABELADDR       = enum.auto()    # noqa; ASSIGNVAR
+#   GETFUNCTIONADDR    = enum.auto()    # noqa; ASSIGNVAR
+#   The following IDs are not IDs in real order.
+#   We just need some IDs to translate eny extended layout to main layout:
+    LOG                = enum.auto()    # noqa; LogSet, LogText
+#   Park
+    FINDPROC           = enum.auto()    # noqa; FindProc
+    GETFONTVERSION     = enum.auto()    # noqa; GetFontVersion
+    GETFONTNAME        = enum.auto()    # noqa; GetFontName
+
+    @classmethod
+    def from_int(cls, value: int) -> 'Op':
+        try:
+            return cls(value)
+        except ValueError:
+            return cls.INVALID_OPCODE
+_Op_PARAMETER_COUNT = {
+    Op.INVALID_OPCODE   : 0,
+    Op.RET              : 0,
+    Op.NOP              : 1,
+    Op.ABORT            : 1,
+    Op.QUIT             : 0,
+    Op.CALL             : 2,
+    Op.UPDATETEXT       : 6,
+    Op.SLEEP            : 1,
+    Op.BRINGTOFRONT     : 0,
+    Op.CHDETAILSVIEW    : 2,
+    Op.SETFILEATTRIBUTES: 2,
+    Op.CREATEDIR        : 3,
+    Op.IFFILEEXISTS     : 3,
+    Op.SETFLAG          : 3,
+    Op.IFFLAG           : 4,
+    Op.GETFLAG          : 2,
+    Op.RENAME           : 4,
+    Op.GETFULLPATHNAME  : 3,
+    Op.SEARCHPATH       : 2,
+    Op.GETTEMPFILENAME  : 2,
+    Op.EXTRACTFILE      : 6,
+    Op.DELETEFILE       : 2,
+    Op.MESSAGEBOX       : 6,
+    Op.RMDIR            : 2,
+    Op.STRLEN           : 2,
+    Op.ASSIGNVAR        : 4,
+    Op.STRCMP           : 5,
+    Op.READENVSTR       : 3,
+    Op.INTCMP           : 6,
+    Op.INTOP            : 4,
+    Op.INTFMT           : 4,
+    Op.PUSHPOP          : 6,
+    Op.FINDWINDOW       : 5,
+    Op.SENDMESSAGE      : 6,
+    Op.ISWINDOW         : 3,
+    Op.GETDLGITEM       : 3,
+    Op.SETCTLCOLORS     : 2,
+    Op.SETBRANDINGIMAGE : 4,
+    Op.CREATEFONT       : 5,
+    Op.SHOWWINDOW       : 4,
+    Op.SHELLEXEC        : 6,
+    Op.EXECUTE          : 3,
+    Op.GETFILETIME      : 3,
+    Op.GETDLLVERSION    : 4,
+    Op.REGISTERDLL      : 6,
+    Op.CREATESHORTCUT   : 6,
+    Op.COPYFILES        : 4,
+    Op.REBOOT           : 1,
+    Op.WRITEINI         : 5,
+    Op.READINISTR       : 4,
+    Op.DELREG           : 5,
+    Op.WRITEREG         : 6,
+    Op.READREGSTR       : 5,
+    Op.REGENUM          : 5,
+    Op.FCLOSE           : 1,
+    Op.FOPEN            : 4,
+    Op.FPUTS            : 3,
+    Op.FGETS            : 4,
+    Op.FSEEK            : 4,
+    Op.FINDCLOSE        : 1,
+    Op.FINDNEXT         : 2,
+    Op.FINDFIRST        : 3,
+    Op.WRITEUNINSTALLER : 4,
+    Op.SECTIONSET       : 5,
+    Op.INSTTYPESET      : 4,
+    Op.GETOSINFO        : 6,
+    Op.RESERVEDOPCODE   : 2,
+    Op.LOCKWINDOW       : 1,
+    Op.FPUTWS           : 4,
+    Op.FGETWS           : 4,
+    Op.LOG              : 2,
+    Op.FINDPROC         : 2,
+    Op.GETFONTVERSION   : 2,
+    Op.GETFONTNAME      : 2,
+}
+
+NS_SHELL_STRINGS = {
+    0x00: 'DESKTOP',
+    0x01: 'INTERNET',
+    0x02: 'SMPROGRAMS',
+    0x03: 'CONTROLS',
+    0x04: 'PRINTERS',
+    0x05: 'DOCUMENTS',
+    0x06: 'FAVORITES',
+    0x07: 'SMSTARTUP',
+    0x08: 'RECENT',
+    0x09: 'SENDTO',
+    0x0A: 'BITBUCKET',
+    0x0B: 'STARTMENU',
+    0x0D: 'MUSIC',
+    0x0E: 'VIDEOS',
+    0x10: 'DESKTOP',
+    0x11: 'DRIVES',
+    0x12: 'NETWORK',
+    0x13: 'NETHOOD',
+    0x14: 'FONTS',
+    0x15: 'TEMPLATES',
+    0x16: 'STARTMENU',
+    0x17: 'SMPROGRAMS',
+    0x18: 'SMSTARTUP',
+    0x19: 'DESKTOP',
+    0x1A: 'APPDATA',
+    0x1B: 'PRINTHOOD',
+    0x1C: 'LOCALAPPDATA',
+    0x1D: 'ALTSTARTUP',
+    0x1E: 'ALTSTARTUP',
+    0x1F: 'FAVORITES',
+    0x20: 'INTERNET_CACHE',
+    0x21: 'COOKIES',
+    0x22: 'HISTORY',
+    0x23: 'APPDATA',
+    0x24: 'WINDIR',
+    0x25: 'SYSDIR',
+    0x26: 'PROGRAM_FILES',
+    0x27: 'PICTURES',
+    0x28: 'PROFILE',
+    0x29: 'SYSTEMX86',
+    0x2A: 'PROGRAM_FILESX86',
+    0x2B: 'PROGRAM_FILES_COMMON',
+    0x2C: 'PROGRAM_FILES_COMMONX8',
+    0x2D: 'TEMPLATES',
+    0x2E: 'DOCUMENTS',
+    0x2F: 'ADMINTOOLS',
+    0x30: 'ADMINTOOLS',
+    0x31: 'CONNECTIONS',
+    0x35: 'MUSIC',
+    0x36: 'PICTURES',
+    0x37: 'VIDEOS',
+    0x38: 'RESOURCES',
+    0x39: 'RESOURCES_LOCALIZED',
+    0x3A: 'COMMON_OEM_LINKS',
+    0x3B: 'CDBURN_AREA',
+    0x3D: 'COMPUTERSNEARME',
+}
+
+NS_VARIABLE_STRINGS = (
+    "CMDLINE",
+    "INSTDIR",
+    "OUTDIR",
+    "EXEDIR",
+    "LANGUAGE",
+    "TEMP",
+    "PLUGINSDIR",
+    "EXEPATH",  # NSIS 2.26+
+    "EXEFILE",  # NSIS 2.26+
+    "HWNDPARENT",
+    "CLICK",    # set from page->clicknext
+    "OUTDIR",   # NSIS 2.04+
+)
+
+class NSHeaderFlags(enum.IntFlag):
+    Undefined = 0
+    Uninstall = 1
+    Silent = 2
+    NoCrc = 4
+    ForceCrc = 8
+    LongOffset = 16
+    ExternalFileSupport = 32
+    ExternalFile = 64
+    IsStubInstaller = 128
+
+
+
+class NSType(enum.IntEnum):
+    Nsis2 = 0
+    Nsis3 = enum.auto()
+    Park1 = enum.auto()
+    Park2 = enum.auto()
+    Park3 = enum.auto()
+
+class NSScriptInstruction(Struct):
+    def __init__(self, reader: StructReader):
+        self.opcode = reader.u32()
+        self.arguments = [reader.u32() for _ in range(6)]
+
+class NSCharCode(enum.IntEnum):
+    NONE = 0
+    CHAR = enum.auto()
+    SKIP = enum.auto()
+    SHELL = enum.auto()
+    VAR = enum.auto()
+    LANG = enum.auto()
+
+    @property
+    def special(self):
+        return self > NSCharCode.CHAR
+    
+@dataclasses.dataclass(eq=True)
+class NSItem:
+    offset: int
+    name: Optional[str] = None
+    mtime: Optional[datetime] = None
+    is_compressed: bool = True
+    is_uninstaller: bool = False
+    attributes: Optional[int] = None
+    size: Optional[int] = None
+    compressed_size: Optional[int] = None
+    estimated_size: Optional[int] = None
+    dictionary_size: int = 1
+    patch_size: int = 0
+    prefix: Optional[str] = None
+
+    @property
+    def path(self) -> str:
+        path = self.name
+        if self.prefix:
+            path = F'{self.prefix}\\{path}'
+        return path
+    
+    def __str__(self) -> str:
+        return self.name
+
+
+class NSHeader(Struct):
+    BACKSLASH           = ord('\\')  # noqa
+    NS_CMDLINE          = 20         # noqa
+    NS_INSTDIR          = 21         # noqa
+    NS_OUTDIR           = 22         # noqa
+    NS_EXEDIR           = 23         # noqa
+    NS_LANGUAGE         = 24         # noqa
+    NS_TEMP             = 25         # noqa
+    NS_PLUGINSDIR       = 26         # noqa
+    NS_EXEPATH          = 27         # noqa NSIS 2.26+
+    NS_EXEFILE          = 28         # noqa NSIS 2.26+
+    NS_HWNDPARENT_225   = 27         # noqa
+    NS_HWNDPARENT_226   = 29         # noqa
+    NS_CLICK            = 30         # noqa
+    NS_OUTDIR_225       = 29         # noqa NSIS 2.04 - 2.25
+    NS_OUTDIR_226       = 31         # noqa NSIS 2.26+
+
+    def _string_args_to_single_arg(self, arg1: int, 
+                                   arg2: Optional[int] = None) -> int:
+        if self.type >= NSType.Park1:
+            return arg1 & 0x7FFF
+        else:
+            if arg2 is None:
+                arg2 = arg1 >> 8
+            arg1 &= 0x7F
+            arg2 &= 0x7F
+            return arg1 | arg2 << 7
+
+    def _get_char_code(self, char: int) -> NSCharCode:
+        if self.type >= NSType.Park1:
+            if char < 0x80:
+                return NSCharCode.CHAR
+            lookup = {
+                0xE000: NSCharCode.SKIP,
+                0xE001: NSCharCode.VAR,
+                0xE002: NSCharCode.SHELL,
+                0xE003: NSCharCode.LANG,
+            }
+        elif self.type is NSType.Nsis3:
+            if char > 4:
+                return NSCharCode.CHAR
+            lookup = {
+                0x0002: NSCharCode.SHELL,
+                0x0003: NSCharCode.VAR,
+                0x0004: NSCharCode.SKIP,
+            }
+        elif self.type is NSType.Nsis2:
+            lookup = {
+                0x00FC: NSCharCode.SKIP,
+                0x00FD: NSCharCode.VAR,
+                0x00FE: NSCharCode.SHELL,
+            }
+        else:
+            raise ValueError(F'Unknown NSIS type {self.type}.')
+        return lookup.get(char, NSCharCode.NONE)
+
+    def _string_code_shell(self, index1: int, 
+                           index2: Optional[int] = None) -> str:
+        if index2 is None:
+            index2 = index1 >> 8
+            index1 &= 0xFF
+        if index1 & 0x80 != 0:
+            offset = index1 & 0x3F
+            with StreamDetour(self.strings, offset):
+                if self.strings.tell() != offset:
+                    raise ValueError(F'Failed to detour to offset 0x{offset:02X}.')
+                path = self._read_current_string()
+                if path.startswith('ProgramFilesDir'):
+                    return '$PROGRAMFILES'
+                if path.startswith('CommonFilesDir'):
+                    return '$COMMONFILES'
+                suffix = 32 * (index1 >> 5 & 2)
+                return F'$REG{suffix}({path})'
+        for index in (index1, index2):
+            shell = NS_SHELL_STRINGS.get(index)
+            if shell is not None:
+                return F'$SHELL:{shell}'
+        else:
+            return F'Error:$SHELL:{index1:02X}{index2:02X}'
+
+    def _string_code_variable(self, index: int) -> str:
+        varcount = 20 + len(NS_VARIABLE_STRINGS)
+        if self._is_nsis200:
+            varcount -= 3
+        elif self._is_nsis225:
+            varcount -= 2
+        if index < 20:
+            if index >= 10:
+                return F'$R{index - 10}'
+            return F'$V{index}'
+        else:
+            if index < varcount:
+                if self._is_nsis225 and index >= self.NS_EXEPATH:
+                    index += 2
+                try:
+                    variable = NS_VARIABLE_STRINGS[index - 20]
+                except IndexError:
+                    return F'Error:$V:{index}'
+                else:
+                    return F'${variable}'
+            return F'Error:$V:{index}'
+        
+    def _string_code_language(self, index: int) -> str:
+        return F'$LANGUAGE:{index}'
+
+    @property
+    def _read_char(self) -> str:
+        return self.strings.u16 if self.unicode else self.strings.u8
+    
+    def _seek_to_string(self, position: int) -> bool:
+        pos = position * self.charsize
+        return self.strings.seek(pos) == pos
+    
+    def _read_string(self, position: int) -> Optional[str]:
+        if position < 0:
+            return self._string_code_language(-(position + 1))
+        if not self._seek_to_string(position):
+            return None
+        return self._read_current_string()
+
+    def _read_string_raw(self, position: int) -> Optional[str]:
+        if not self._seek_to_string(position):
+            return None
+        if self.unicode:
+            return self.strings.read_w_string()
+        else:
+            return self.strings.read_c_string()
+        
+    def _is_var_absolute_path(self, position: int) -> bool:
+        var = self._get_var_index(position)
+        if var is None:
+            return False
+        return var in (
+            self.NS_INSTDIR,
+            self.NS_EXEDIR,
+            self.NS_TEMP,
+            self.NS_PLUGINSDIR,
+        )
+    
+    def _is_good_string(self, position: int) -> bool:
+        if position == 0:
+            return False
+        if not self._seek_to_string(position - 1):
+            return False
+        prefix = self._read_char()
+        return prefix == 0 or prefix == self.BACKSLASH
+
+    def _is_var_str(self, position: int, index: int) -> bool:
+        if index > 0x7FFF:
+            return False
+        var_index = self._get_var_index(position)
+        if var_index is None:
+            return False
+        if self._get_resource_finished(position, 0) is None:
+            return False
+        return var_index == index
+
+    def _get_var_index(self, position: int) -> Optional[int]:
+        if not self._seek_to_string(position):
+            raise LookupError(F'Failed to seek to string at position 0x{position:08X}.')
+        try:
+            code = self._read_char()
+            if self._get_char_code(code) is not NSCharCode.VAR:
+                return None
+            arg1 = self._read_char()
+            if arg1 == 0:
+                return None
+            if self.unicode:
+                args = arg1,
+            else:
+                arg2 = self._read_char()
+                if arg2 == 0:
+                    return None
+                args = arg1, arg2
+            return self._string_args_to_single_arg(*args)
+        except EOFError:
+            return None
+        
+    def _get_resource(self, position: int) -> Optional[int]:
+        if self.unicode:
+            if len(self.strings) - position >= 4:
+                return 2
+        else:
+            if len(self.strings) - position >= 3:
+                return 3
+        return None
+
+    def _get_resource_finished(self, position: int, 
+                          terminator: int) -> Optional[int]:
+        if not self._seek_to_string(position):
+            return None
+        self.strings.seek_relative(3)
+        if self.unicode:
+            self.strings.seek_relative(1)
+        if self.strings.remaining_bytes < self.charsize:
+            return None
+        if self._read_char() != terminator:
+            return None
+        return 3 if self.unicode else 4
+
+
+    @property
+    def charsize(self) -> int:
+        return 2 if self.unicode else 1
+
+    def _read_current_string(self) -> str:
+        string = io.StringIO()
+        chars = iter(self._read_char, 0)
+        for letter in chars:
+            code = self._get_char_code(letter)
+            if code is NSCharCode.CHAR:
+                string.write(chr(letter))
+                continue
+            if code.special:
+                try:
+                    var1 = next(chars)
+                except StopIteration:
+                    break
+                if var1 == 0:
+                    break
+                if code is NSCharCode.SKIP:
+                    letter = var1
+                else:
+                    if not self.unicode:
+                        try:
+                            var2 = next(chars)
+                        except StopIteration:
+                                break
+                        if var2 == 0:
+                            break
+                        vars = var1, var2
+                    else:
+                        vars = var1,
+                    if code is NSCharCode.SHELL:
+                        string.write(self._string_code_shell(*vars))
+                        continue
+                    else:
+                        var = self._string_args_to_single_arg(*vars)
+                        if code is NSCharCode.VAR:
+                            string.write(self._string_code_variable(var))
+                        if code is NSCharCode.LANG:
+                            string.write(self._string_code_language(var))
+                        continue
+            string.write(chr(letter))
+        return string.getvalue()
+
+    def opcode(self, cmd: NSScriptInstruction) -> Op:
+        code = cmd.opcode
+        if self.type < NSType.Park1:
+            if self._log_cmd_is_enabled:
+                return Op.from_int(code)
+            if code < Op.SECTIONSET:
+                return Op.from_int(code)
+            if code is Op.SECTIONSET:
+                return Op.LOG
+            return Op.from_int(code - 1)
+        if code < Op.REGISTERDLL:
+            return Op.from_int(code)
+        if self.type >= NSType.Park2:
+            if code == Op.REGISTERDLL:
+                return Op.GETFONTVERSION
+            code -= 1
+        if self.type >= NSType.Park3:
+            if code == Op.REGISTERDLL:
+                return Op.GETFONTNAME
+            code -= 1
+        if code >= Op.FSEEK:
+            if self.unicode:
+                if code == Op.FSEEK:
+                    return Op.FPUTWS
+                if code == Op.FSEEK + 1:
+                    return Op.FGETWS
+                code -= 2
+            if code >= Op.SECTIONSET and self._log_cmd_is_enabled:
+                if code == Op.SECTIONSET:
+                    return Op.LOG
+                return Op.from_int(code - 1)
+            if code == Op.FPUTWS:
+                return Op.FINDPROC
+        return Op.from_int(code)
+
+    def _find_bad_cmd(self) -> None:
+        self._bad_cmd = -1
+        for instruction in self.instructions:
+            cmd = self.opcode(instruction)
+            arg = instruction.arguments
+            if cmd is Op.INVALID_OPCODE:
+                continue
+            if cmd >= self._bad_cmd >= 0:
+                continue
+            if self.type is NSType.Nsis3:
+                if cmd == Op.RESERVEDOPCODE:
+                    self._bad_cmd = cmd
+                    continue
+            else:
+                if cmd == Op.RESERVEDOPCODE or cmd == Op.GETOSINFO:
+                    self._bad_cmd = cmd
+                    continue
+            last_non_empty_index = max((k for k, a in enumerate(arg, 1) if a), default=0)
+            if cmd == Op.FINDPROC and last_non_empty_index == 0:
+                continue
+            if _Op_PARAMETER_COUNT[cmd] < last_non_empty_index:
+                self._bad_cmd = cmd
+
+    def _guess_nsis_version(self):
+        self.strong_nsis = False
+        self.strong_park = False
+        char_mask = 0x8080 if self.unicode else 0x80
+        self.strings.seek(0)
+        while not self.strings.is_eof:
+            string = self._read_current_string()
+            if string is None:
+                continue
+            if len(string) < 2:
+                continue
+            if ord(string[0]) != 3:
+                continue
+            if ord(string[1]) & char_mask == char_mask:
+                self.type = NSType.Nsis3
+                self.strong_nsis = True
+                break
+        if self.unicode:
+            if not self.strong_nsis:
+                self.type = NSType.Park1
+                self.strong_park = True
+        elif self.type is NSType.Nsis2:
+            for instruction in self.instructions:
+                cmd = self.opcode(instruction)
+                arg = instruction.arguments
+                if cmd is Op.GETDLGITEM:
+                    if self._is_var_str(arg[1], self.NS_HWNDPARENT_225):
+                        self._is_nsis225 = True
+                        if arg[0] == self.NS_OUTDIR_225:
+                            self._is_nsis200 = True
+                            break
+                if cmd is Op.ASSIGNVAR:
+                    if arg[0] == self.NS_OUTDIR_225 and arg[2] == 0 and arg[3] == 0:
+                        self._is_nsis225 = self._is_var_str(arg[1], self.NS_OUTDIR)
+        got_park_version = False
+        mask = 0
+        IN = 4 if self.unicode else 2
+        if not self.strong_nsis and not self._is_nsis225 and not self._is_nsis200:
+            for instruction in self.instructions:
+                cmd = instruction.opcode
+                arg = instruction.arguments
+                alt = arg[3]
+                if cmd < Op.WRITEUNINSTALLER or cmd > Op.WRITEUNINSTALLER + IN:
+                    continue
+                if arg[4] != 0 or arg[5] != 0 or arg[0] <= 1 or alt <= 1:
+                    continue
+                if not self._is_good_string(arg[0]) or not self._is_good_string(alt):
+                    continue
+                index = self._get_var_index(alt)
+                if index is None:
+                    continue
+                additional = self._get_resource_finished(alt, self.BACKSLASH)
+                if index != self.NS_INSTDIR:
+                    continue
+                if self._read_string_raw(alt + additional) == self._read_string_raw(arg[0]):
+                    inserts = cmd - Op.WRITEUNINSTALLER.value
+                    mask |= 1 << inserts
+            if mask == 1:
+                got_park_version = True
+            elif mask:
+                shift = 0
+                nt = self.type
+                if self.unicode:
+                    shift = 2
+                if mask == 1 << (shift + 1):
+                    nt = NSType.Park2
+                if mask == 1 << (shift + 2):
+                    nt = NSType.Park3
+                if nt != self.type:
+                    self.type = nt
+                    got_park_version = True
+        self._find_bad_cmd()
+        if self._bad_cmd < Op.REGISTERDLL:
+            return
+        if self.strong_park and not got_park_version:
+            if self._bad_cmd < Op.SECTIONSET:
+                self.type = NSType.Park3
+                self._log_cmd_is_enabled = True
+                self._find_bad_cmd()
+                if self._bad_cmd in range(Op.SECTIONSET):
+                    self.type = NSType.Park2
+                    self._log_cmd_is_enabled = False
+                    self._find_bad_cmd()
+                    if self._bad_cmd in range(Op.SECTIONSET):
+                        self.type = NSType.Park1
+                        self._find_bad_cmd()
+        if self._bad_cmd >= Op.SECTIONSET:
+            self._log_cmd_is_enabled = not self._log_cmd_is_enabled
+            self._find_bad_cmd()
+            if self._bad_cmd >= Op.SECTIONSET and self._log_cmd_is_enabled:
+                self._log_cmd_is_enabled = False
+                self._find_bad_cmd()   
+
+    def _read_items(self) -> List[NSItem]:
+        prefixes = ['$INSTDIR']
+        out_dir = ''
+        out_dir_index = (
+            self.NS_OUTDIR_225
+        ) if self._is_nsis225 else (
+            self.NS_OUTDIR_226
+        )
+        items: List[NSItem] = []
+
+        for cmd_index, instruction in enumerate(self.instructions):
+            def set_path(index:int) -> None:
+                item.prefix = None
+                item.name = self._read_string(index)
+                if not self._is_var_absolute_path(index):
+                    item.prefix = prefixes[-1]
+            
+            cmd = self.opcode(instruction)
+            arg = instruction.arguments
+
+            if cmd is Op.INVALID_OPCODE:
+                continue
+            elif cmd is Op.CREATEDIR:
+                if not arg[1]:
+                    continue
+                _path = arg[0]
+                index = self._get_var_index(_path)
+                if index in (out_dir_index, self.NS_OUTDIR):
+                    _path += self._get_resource(_path)
+                path = self._read_string(_path)
+                if index == out_dir_index:
+                    path = out_dir + path
+                elif index == self.NS_OUTDIR:
+                    path = prefixes[-1] + path
+                prefixes.append(path)
+            elif cmd is Op.ASSIGNVAR:
+                if arg[0] != out_dir_index:
+                    continue
+                if self._is_var_str(arg[1], self.NS_OUTDIR) and arg[2] == 0 and arg[3] == 0:
+                    out_dir = prefixes[-1]
+            elif cmd is Op.EXTRACTFILE:
+                try:
+                    time = datetime.fromtimestamp(arg[4] << 32 | arg[3])
+                except Exception:
+                    time = None
+                item = NSItem(arg[2], mtime=time)
+                set_path(arg[1])
+                items.append(item)
+                if not self._is_var_str(arg[1], 10):
+                    continue
+                cmd_back_offset = 28
+                if cmd_index > 1:
+                    previous = self.instructions[cmd_index - 1]
+                    if self.opcode(previous) is Op.NOP:
+                        cmd_back_offset -= 2
+                if cmd_index <= cmd_back_offset:
+                    continue
+                previous = self.instructions[cmd_index - cmd_back_offset]
+                if self.opcode(previous) is Op.ASSIGNVAR:
+                    previous_arguments = previous.arguments
+                    if previous_arguments[0] == 14 and previous_arguments[2] == 0 and previous_arguments[3] == 0:
+                        set_path(previous_arguments[1])
+            elif cmd is Op.SETFILEATTRIBUTES:
+                if cmd_index > 0:
+                    previous = self.instructions[cmd_index - 1]
+                    previous_arguments = previous.arguments
+                    if self.opcode(previous) is Op.EXTRACTFILE and arg[0] == previous_arguments[1]:
+                        item = items[-1]
+                        item.attributes = arg[1]
+            elif cmd is Op.WRITEUNINSTALLER:
+                if arg[4] or arg[5] or arg[0] <=1 or arg[3] <= 1:
+                    continue
+                if not self._is_good_string(arg[0]):
+                    continue
+                if self._bad_cmd in range(Op.WRITEUNINSTALLER):
+                    continue
+                item = NSItem(arg[1])
+                set_path(arg[0])
+                item.patch_size = arg[2]
+                item.is_uninstaller = True
+                items.append(item)
+        return items
+                
+    @property
+    def script(self):
+        script = io.StringIO()
+        name_width = max(len(op.name) for op in Op)
+        addr_width = len(F'{len(self.instructions):X}')
+        for k, instruction in enumerate(self.instructions):
+            if k > 0:
+                script.write('\n')
+            opcode = self.opcode(instruction)
+            script.write(F'{k:0{addr_width}X} {opcode.name:{name_width}}')
+            for j, arg in enumerate(instruction.arguments[:_Op_PARAMETER_COUNT.get(opcode, 6)]):
+                if j > 0:
+                    script.write(', ')
+                if arg > 20 and self._is_good_string(arg):
+                    script.write(repr(self._read_string(arg)))
+                elif arg < 0x100:
+                    script.write(str(arg))
+                elif arg < 0x10000:
+                    script.write(F'${arg:04X}')
+                else:
+                    script.write(F'${arg:08X}')
+        return script.getvalue()
+
+    def _string_code_language(self, index: int) -> str:
+        return F'$LANGUAGE:{index:04X}'
+
+
+    def __init__(self, reader: StructReader[bytearray], size: int):
+        self.is64bit = size >= 100 and not any(
+            struct.unpack('8xI' * 8, reader.peek(12 * 8)))
+        block_header_offset_size = 12 if self.is64bit else 8
+        required_size = block_header_offset_size * 8 + 4
+        if size < required_size:
+            raise ValueError(F'Header size 0x{size:08X} is too small. Minimum required size is 0x{required_size:08X}.')
+        # TODO: Confirm role of unknown value. Copilot believes it to be
+        # a signature indicating the end of the NSIS installer header.
+        self.unknown_value = reader.u32()
+        self.block_header_offsets = [NSBlockHeaderOffset(
+            reader.read(block_header_offset_size), 
+            is64bit=self.is64bit) for _ in range(8)]
+        self.block_header_entries = self.block_header_offsets[2]
+        self.block_header_strings = self.block_header_offsets[3]
+        self.block_header_langtables = self.block_header_offsets[4]
+        
+        for key, offset in enumerate(self.block_header_offsets):
+            width = 0x10 if self.is64bit else 8
+            table = {2: 'entries', 3: 'strings', 4: 'langtables'}.get(key)
+            message = F'Block {key}: offset=0x{offset.offset:0{width}X}, size=0x{offset.size:0{width}X}'
+            if table is not None:
+                message += F'{message} ({table})'
+            logging.debug(message)
+
+        self.type = NSType.Nsis2 # Default to NSIS 2
+        
+        reader.seek_set(self.block_header_entries.offset)
+        self.instructions: List[NSScriptInstruction] = [NSScriptInstruction(reader) for _ in range(self.block_header_entries.size)]
+
+        if self.block_header_entries.offset > size:
+            raise ValueError(F'Header indicates {self.block_header_entries.size} entries, but only {size} bytes remain.')
+        if self.block_header_strings.offset > size:
+            raise ValueError(F'Header indicates {self.block_header_strings.size} strings, but only {size} bytes remain.')
+        if self.block_header_langtables.offset > size:
+            raise ValueError(F'Header indicates {self.block_header_langtables.size} langtables, but only {size} bytes remain.')
+        if self.block_header_langtables.offset < self.block_header_strings.offset:
+            raise ValueError(F'Langtables block is before strings block.')
+        string_table_size = self.block_header_langtables.offset - self.block_header_strings.offset
+        if string_table_size < 2:
+            raise ValueError(F'String table size is too small.')
+        reader.seek_set(self.block_header_strings.offset)
+        strings = reader.read(string_table_size)
+        self.unicode = strings[:2] == B'\0\0'
+        if strings[-1] != 0 or (self.unicode and strings[-2] != 0):
+            raise ValueError(F'String table is not null-terminated.')
+        if self.unicode and string_table_size % 2 != 0:
+            raise ValueError(F'String table is not even-sized.')
+
+        self.strings = StructReader(strings)
+        if self.block_header_entries.size > (1 << 25):
+            raise ValueError(F'Header indicates {self.block_header_entries.size} entries, which is too large.')
+        
+        self._log_cmd_is_enabled = False
+        self._is_nsis225 = False
+        self._is_nsis200 = False
+        self_bad_cmd = -1
+
+        self._guess_nsis_version()
+
+        items: Dict[(str, int), NSItem] = {}
+        for item in self._read_items():
+            if items.setdefault((item.path, item.offset), item) != item:
+                raise ValueError(F'Duplicate item: {item.path} at 0x{item.offset:08X}')
+        
+        self.items = [items[t] for t in sorted(items.keys())]
+        
+
+
+class NSArchive(Struct):
+    MAGICS = [
+        # https://nsis.sourceforge.io/Can_I_decompile_an_existing_installer
+        B'\xEF\xBE\xAD\xDE' B'Null' B'soft' B'Inst',   # v1.6
+        B'\xEF\xBE\xAD\xDE' B'Null' B'Soft' B'Inst',   # v1.3
+        B'\xED\xBE\xAD\xDE' B'Null' B'Soft' B'Inst',   # v1.1
+        B'\xEF\xBE\xAD\xDE' B'nsis' B'inst' B'all\0',  # v1.0
+    ]
+
+    @dataclasses.dataclass
+    class Entry:
+        offset: int
+        data: bytearray
+        compressed_size: int
+        decompression_failed: bool = False
+
+
+    def __init__(self, reader: StructReader[bytearray]):
+        self.flags = NSHeaderFlags(reader.u32())
+        self.signature = reader.read(0x10)
+        header_data = None
+        header_size = reader.u32()
+        header_data_length = None
+        archive_size = reader.u32()
+        self.archive_offset = reader.tell()
+        body_size = archive_size - self.archive_offset
+        if body_size < 0:
+            raise ValueError("Invalid archive size")
+        if header_size < self.archive_offset:
+            raise ValueError("Invalid header size")
+        if reader.remaining_bytes < body_size:
+            raise ValueError(
+                F'Header indicates archive size 0x{archive_size:08X}, '
+                F'but only 0x{reader.remaining_bytes:08X} bytes remain.')
+    
+        # Prepare to check compression format. This takes
+        # a few bytes and checks the header to determine the format
+        preview_bytes = bytes(reader.peek(4))
+        preview_value = int.from_bytes(preview_bytes, byteorder='little')
+        
+        # The default "solid" value is True and default method is deflate.
+        # Regarding Solid:
+        # "If /SOLID is used, all of the installer data is compressed in one block. This results in greater compression ratios."
+        # We determine if the compression is solid or not by checking the headers.
+        # https://nsis.sourceforge.io/Docs/Chapter4.html#
+        
+        self.solid = True
+        self.lzma_options: Optional[LZMAOptions] = None
+        self.method = NSMethod.Deflate
+
+        # Header Matching Logic:
+        #  X is the header size as given by the first header
+        #  T is a value less than 0xE
+        #  Y is a value different from 0x80
+        # XX XX XX XX __ __ __ __ __ __ __  non-solid, uncompressed
+        # 5D 00 00 DD DD 00 __ __ __ __ __  solid LZMA
+        # 00 5D 00 00 DD DD 00 __ __ __ __  solid LZMA, empty filter
+        # 01 5D 00 00 DD DD 00 __ __ __ __  solid LZMA, BCJ filter
+         # __ __ __ 80 5D 00 00 DD DD 00 __  non-solid LZMA
+        # __ __ __ 80 00 5D 00 00 DD DD 00  non-solid LZMA, empty filter
+        # __ __ __ 80 01 5D 00 00 DD DD 00  non-solid LZMA, BCJ filter
+        # __ __ __ 80 01 0T __ __ __ __ __  non-solid BZip
+        # __ __ __ 80 __ __ __ __ __ __ __  non-solid deflate
+        # 01 0T __ YY __ __ __ __ __ __ __  solid BZip
+        # __ __ __ YY __ __ __ __ __ __ __  solid Deflate
+        
+        def lzmacheck(preview):
+            if B'\x5D\0\0' not in preview:
+                return False
+            filter_flag = preview_bytes[0] <= 1
+            reader.seek_relative(3 + int(filter_flag))
+            self.lzma_options = LZMAOptions(filter_flag, reader.u32())
+            return True
+        
+        def bzipcheck(preview):
+            return preview[0] == 0x31 and preview[1] < 14
+        
+        if preview_value == header_size:
+            self.solid = False
+            header_data = reader.read_exactly(header_size)
+            self.method = NSMethod.Copy
+        elif lzmacheck(preview_bytes):
+            self.method = NSMethod.LZMA
+        elif preview_bytes[3] == 0x80:
+            self.solid = False
+            reader.seek_relative(4)
+            second_preview = bytes(reader.peek(4))
+            if lzmacheck(second_preview):
+                self.method = NSMethod.LZMA
+            elif bzipcheck(second_preview):
+                self.method = NSMethod.BZip2
+        elif bzipcheck(preview_bytes):
+            self.method = NSMethod.BZip2
+
+        reader.seek_set(self.archive_offset)
+        self.entries: Dict[int, bytearray] = {}
+        self.entry_offset_delta = 0
+        self._solid_iter = None
+
+        if header_data is None:
+            item = self._decompress_items(reader)
+            try:
+                header_entry = next(item)
+            except zlib.error as ZLERR:
+                raise NotImplementedError(
+                    'This archive seems to use an NSIS-specific deflate '
+                    'algorithm which has not been implemented yet.'
+                ) from ZLERR
+            if self.solid:
+                self._solid_iter = item 
+            self.entry_offset_delta = header_entry.compressed_size + 4
+            header_data = header_entry.data
+        else:
+            self.entry_offset_delta = len(header_data)
+
+        if not header_data:
+            raise ValueError("Empty header")
+        logging.debug(F'Header size: 0x{header_size:08X}')
+
+        self.header = NSHeader(header_data, size=header_size)
+        self.reader = reader
+        
+    @property
+    def script(self):
+        return self.header.script
+    
+    @property
+    def offset_items(self):
+        return self.archive_offset + self.entry_offset_delta
+    
+    def _extract_item_data(self, item: NSItem) -> Entry:
+        if self.solid:
+            while True:
+                try:
+                    entry = self.entries[item.offset]
+                except KeyError:
+                    try:
+                        entry = next(self._solid_iter)
+                    except StopIteration:
+                        raise LookupError(F'Failed to find item at offset 0x{item.offset:08X}.')
+                    self.entries[entry.offset - self.entry_offset_delta] = entry.data
+                else: 
+                    return entry
+        else:
+            self.reader.seek(self.offset_items + item.offset)
+            decompressed = self._decompress_items(self.reader)
+            entry = next(decompressed).data
+            return entry
+
+    class PartsReader(Iterable[Entry]):
+        def __init__(self, src: BinaryIO):
+            self.src = src
+            self.pos = 0
+
+        def __iter__(self):
+            return self
+        
+        def __next__(self):
+            offset = self.pos
+            size = self.src.read(4)
+            if len(size) != 4:
+                raise StopIteration
+            size = int.from_bytes(size, byteorder='little')
+            read = size & 0x7FFFFFFF
+            data = self.src.read(read)
+            if len(data) != read:
+                raise EOFError('Unexpected end of stream while decompressing archive entries.')
+            self.pos = offset + size + 4
+            return NSArchive.Entry(offset, data, size)
+
+    class SolidReader(PartsReader):
+        def __init__(self, src: BinaryIO, decompressor: Type[BinaryIO]):
+            super().__init__(src)
+            self._dc = decompressor
+
+        def __next__(self):
+            item = super().__next__()
+            is_compressed = bool(item.compressed_size & 0x80000000)
+            item.compressed_size &= 0x7FFFFFFF
+            if is_compressed:
+                try:
+                    dc = self._dc(MemoryFile(item.data))
+                    item.data = dc.read()
+                except Exception:
+                    item.decompression_failed = True
+            return item              
+        
+    class LZMAFix:
+        ''' Creates a wrapper to compensate for how NSIS handles LZMA'''
+        def __init__(self, src: MemoryFile):
+            self._src = src
+            self._fix = MemoryFile(bytes(src.read(5)) + B'\xFF' * 8)
+
+        def __getattr__(self, key):
+            return getattr(self._src, key)
+        
+        def read(self, size: int = -1):
+            src = self._src
+            fix = self._fix
+            if not fix.remaining_bytes:
+                return src.read(size)
+            if size < 0:
+                size = fix.remaining_bytes + src.remaining_bytes
+            data = bytearray(size)
+            wrapper = fix.read(size)
+            data[:len(wrapper)] = wrapper
+            data[len(wrapper):] = src.read(size - len(wrapper))
+            return data
+    
+
+
+    def _decompress_items(self, reader: StructReader[bytearray]) -> Iterator[Entry]:
+        """ Decompresses the items in the archive. """
+        def NSISLZMAFile(d):
+            return lzma.LZMAFile(self.LZMAFix(d))
+        decompressor: Type[BinaryIO]= {
+            NSMethod.Deflate : DeflateFile,
+            NSMethod.LZMA    : NSISLZMAFile,
+            NSMethod.BZip2   : BZip2File,
+        }[self.method]
+        if self.solid:
+            return self.PartsReader(decompressor(reader))
+        return self.SolidReader(reader, decompressor)
+        
+
+class extractNSIS(ArchiveUnit):
+    """
+    A class to extract an NSIS file.
+    """
+    @classmethod
+    def _find_archive_offset(cls, data: memoryview, before: int = -1, flaw_max=2) -> int:
+        def signatures(*magics):
+            for changes in range(flaw_max + 1):
+                for magic in magics:
+                    if not changes:
+                        yield 0, magic
+                        continue
+                    for positions in itertools.permutations(range(len(magic)), r=changes):
+                        signature = bytearray(magic)
+                        for position in positions:
+                            signature[position] = 0x2E
+                        yield changes, bytes(signature)
+        best_guess = None
+        search_space = memoryview(data)
+        for flaws, sig in signatures(*NSArchive.MAGICS):
+            if flaws > 1:
+                search_space = search_space[:0x20_000]
+            matches = [m.start() - 4 for m in re.finditer(sig, 
+                                                          search_space, 
+                                                          flags=re.DOTALL)]
+            if before >= 0:
+                matches = [match for match in matches if match < before]
+            matches.reverse()
+            archive = None
+            for match in matches:
+                if match % 0x200 == 0:
+                    archive = match
+                    break
+            if not archive:
+                if matches and not best_guess:
+                    best_guess = matches[-1]
+            else:
+                message = F'Archive signature was found at offset 0x{archive:08X}.'
+                if flaws > 0:
+                    message += F' the signature has {flaws} flaws and was likely modified.'
+                logging.debug(message)
+                return archive
+        if best_guess:
+            message = F'Archive signature was found at offset 0x{best_guess:08X}, but it has too many flaws to be reliable.'
+            logging.debug(message)
+        return best_guess
+
+    def unpack(self, data: memoryview):
+        memory = memoryview(data)
+        before = -1
+        _error = None
+        while True:
+            offset = self._find_archive_offset(data, before)
+            if offset is None:
+                _error = _error or ValueError("Unable to find NSIS archive marker")
+                raise _error
+            try:
+                archive = NSArchive(memory[offset:])
+            except Exception as e:
+                _error = e
+                before = offset
+            else:
+                break
+
+        def info():
+            yield F'{archive.header.type.name} archive'
+            yield F'{archive.method.name.lower()} compression'
+            yield F'Mystery value 0x{archive.header.unknown_value:X}'
+            yield 'solid archive' if archive.solid else 'non-solid archive'
+            yield '64-bit archive' if archive.header.is64bit else '32-bit archive'
+            yield 'unicode' if archive.header.unicode else 'ansi'
+        
+        logging.info(', '.join(info()))
+        unpacked_items = []
+        for item in archive.header.items:
+            unpacked_items.append(self._pack(item.path, item.mtime, archive._extract_item_data(item)))
+            #data = archive._extract_item_data(item)
+            logging.info(F'{item.path} at 0x{item.offset:08X}, {len(data)} bytes')
+        unpacked_items.append(self._pack('setup.nsis', None, archive.script.encode('utf-8'))) 
+        return unpacked_items
+
+
+
```

### Comparing `debloat-1.5.6/src/debloat/utilities/pyflate.py` & `debloat-1.5.6.1/src/debloat/utilities/pyflate.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,690 +1,690 @@
-#!/usr/bin/env python
-# ============================ MOTIFICATION NOTE ============================
-# The content of this file has been modified for use in binary refinery; it
-# has been ported from Python2 to Python3 and the BZip2 implementation was
-# rewritten to support NSIS-specific BZip stream and block headers, which are
-# different from the official standard values. The original code was taken
-# from the following location:
-#  https://github.com/pfalcon/pyflate/blob/master/pyflate.py
-
-# ============================ ORIGINAL LICENSING ============================
-# Copyright 2006--2007-01-21 Paul Sladen
-#  http://www.paul.sladen.org/projects/compression/
-#
-# You may use and distribute this code under any DFSG-compatible license (eg.
-# BSD, GNU GPLv2).
-#
-# Stand-alone pure-Python DEFLATE (gzip) and bzip2 decoder/decompressor. This
-# is probably most useful for research purposes/index building; there is
-# certainly some room for improvement in the Huffman bit-matcher.
-#
-# With the as-written implementation, there was a known bug in BWT decoding
-# to do with repeated strings. This has been worked around; see bwt_reverse().
-# Correct output is produced in all test cases but ideally the problem would
-# be found...
-# ============================================================================
-from __future__ import annotations
-from typing import List, Tuple, Iterable, Optional, BinaryIO
-
-import itertools
-import abc
-
-
-class BitfieldBase(abc.ABC):
-
-    def __init__(self, x):
-        if isinstance(x, BitfieldBase):
-            self.f = x.f
-            self.bits = x.bits
-            self.bitfield = x.bitfield
-            self.count = x.bitfield
-        else:
-            self.f = x
-            self.bits = 0
-            self.bitfield = 0x0
-            self.count = 0
-
-    def _read(self, n):
-        s = self.f.read(n)
-        if not s:
-            raise RuntimeError('length error')
-        self.count += len(s)
-        return s
-
-    def needbits(self, n):
-        while self.bits < n:
-            self._more()
-
-    def _mask(self, n):
-        return (1 << n) - 1
-
-    def toskip(self):
-        return self.bits & 0x7
-
-    def align(self):
-        self.readbits(self.toskip())
-
-    def dropbits(self, n=8):
-        while n >= self.bits and n > 7:
-            n -= self.bits
-            self.bits = 0
-            n -= len(self.f._read(n >> 3)) << 3
-        if n:
-            self.readbits(n)
-
-    def dropbytes(self, n=1):
-        self.dropbits(n << 3)
-
-    def tell(self):
-        return self.count - ((self.bits + 7) >> 3), 7 - ((self.bits - 1) & 0x7)
-
-    def tellbits(self):
-        bytes, bits = self.tell()
-        return (bytes << 3) + bits
-
-    @abc.abstractmethod
-    def _more(self):
-        pass
-
-    @abc.abstractmethod
-    def snoopbits(self, n=8):
-        pass
-
-    @abc.abstractmethod
-    def readbits(self, n=8):
-        pass
-
-
-class LBitfield(BitfieldBase):
-
-    def _more(self):
-        c = self._read(1)
-        self.bitfield += c[0] << self.bits
-        self.bits += 8
-
-    def snoopbits(self, n=8):
-        if n > self.bits:
-            self.needbits(n)
-        return self.bitfield & self._mask(n)
-
-    def readbits(self, n=8):
-        if n > self.bits:
-            self.needbits(n)
-        r = self.bitfield & self._mask(n)
-        self.bits -= n
-        self.bitfield >>= n
-        return r
-
-
-class RBitfield(BitfieldBase):
-
-    def _more(self):
-        c = self._read(1)
-        self.bitfield <<= 8
-        self.bitfield += c[0]
-        self.bits += 8
-
-    def snoopbits(self, n=8):
-        if n > self.bits:
-            self.needbits(n)
-        return (self.bitfield >> (self.bits - n)) & self._mask(n)
-
-    def readbits(self, n=8):
-        if n > self.bits:
-            self.needbits(n)
-        r = (self.bitfield >> (self.bits - n)) & self._mask(n)
-        self.bits -= n
-        self.bitfield &= ~(self._mask(n) << self.bits)
-        return r
-
-
-class HuffmanLength:
-    code: int
-    bits: int
-    symbol: Optional[int]
-    reverse_symbol: Optional[int]
-
-    def __init__(self, code, bits=0):
-        self.code = code
-        self.bits = bits
-        self.symbol = None
-        self.reverse_symbol = None
-
-    def __lt__(self, other):
-        return self.__cmp(other) < 0
-
-    def __gt__(self, other):
-        return self.__cmp(other) > 0
-
-    def __eq__(self, other):
-        return self.__cmp(other) == 0
-
-    def __le__(self, other):
-        return self.__cmp(other) <= 0
-
-    def __ge__(self, other):
-        return self.__cmp(other) >= 0
-
-    def __ne__(self, other):
-        return self.__cmp(other) != 0
-
-    def __cmp(self, other):
-        a, b = self.bits, other.bits
-        if a == b:
-            a, b = self.code, other.code
-        return (a > b) - (a < b)
-
-
-def reverse_bits(v: int, n: int):
-    a = 1 << 0
-    b = 1 << (n - 1)
-    z = 0
-    for i in range(n - 1, -1, -2):
-        z |= (v >> i) & a
-        z |= (v << i) & b
-        a <<= 1
-        b >>= 1
-    return z
-
-
-def reverse_bytes(v, n):
-    a = 0xff << 0
-    b = 0xff << (n - 8)
-    z = 0
-    for i in range(n - 8, -8, -16):
-        z |= (v >> i) & a
-        z |= (v << i) & b
-        a <<= 8
-        b >>= 8
-    return z
-
-
-class HuffmanTable:
-    table: List[HuffmanLength]
-
-    def __init__(self, bootstrap):
-        table = []
-        start, bits = bootstrap[0]
-        for finish, endbits in bootstrap[1:]:
-            if bits:
-                for code in range(start, finish):
-                    table.append(HuffmanLength(code, bits))
-            start, bits = finish, endbits
-            if endbits == -1:
-                break
-        table.sort()
-        self.table = table
-
-    def populate_huffman_symbols(self):
-        bits, symbol = -1, -1
-        for x in self.table:
-            symbol += 1
-            if x.bits != bits:
-                symbol <<= (x.bits - bits)
-                bits = x.bits
-            x.symbol = symbol
-            x.reverse_symbol = reverse_bits(symbol, bits)
-
-    def min_max_bits(self):
-        self.min_bits, self.max_bits = 16, -1
-        for x in self.table:
-            if x.bits < self.min_bits: self.min_bits = x.bits
-            if x.bits > self.max_bits: self.max_bits = x.bits
-
-    def _find_symbol(self, bits: int, symbol: int, table: Iterable[HuffmanLength]) -> int:
-        for h in table:
-            if h.bits == bits and h.reverse_symbol == symbol:
-                return h.code
-        return -1
-
-    def find_next_symbol(self, field: LBitfield, reversed=True):
-        cached_length = -1
-        cached = None
-        for x in self.table:
-            if cached_length != x.bits:
-                cached = field.snoopbits(x.bits)
-                cached_length = x.bits
-            if (reversed and x.reverse_symbol == cached) or (not reversed and x.symbol == cached):
-                field.readbits(x.bits)
-                return x.code
-        raise RuntimeError(F'symbol not found even after end of table at {field.tell()}')
-
-
-class OrderedHuffmanTable(HuffmanTable):
-    def __init__(self, lengths):
-        _ordered_lengths = list(enumerate(lengths))
-        _ordered_lengths.append((len(lengths), -1))
-        super().__init__(_ordered_lengths)
-
-
-CODE_LENGTH_ORDERS = (
-    0x10, 0x11, 0x12, 0x00, 0x08, 0x07, 0x09, 0x06, 0x0A, 0x05,
-    0x0B, 0x04, 0x0C, 0x03, 0x0D, 0x02, 0x0E, 0x01, 0x0F)
-
-DISTANCE_BASE = (
-    0x0001, 0x0002, 0x0003, 0x0004, 0x0005, 0x0007, 0x0009, 0x000D, 0x0011, 0x0019,
-    0x0021, 0x0031, 0x0041, 0x0061, 0x0081, 0x00C1, 0x0101, 0x0181, 0x0201, 0x0301,
-    0x0401, 0x0601, 0x0801, 0x0C01, 0x1001, 0x1801, 0x2001, 0x3001, 0x4001, 0x6001)
-
-LENGTH_BASE = (
-    0x0003, 0x0004, 0x0005, 0x0006, 0x0007, 0x0008, 0x0009, 0x000A, 0x000B, 0x000D,
-    0x000F, 0x0011, 0x0013, 0x0017, 0x001B, 0x001F, 0x0023, 0x002B, 0x0033, 0x003B,
-    0x0043, 0x0053, 0x0063, 0x0073, 0x0083, 0x00A3, 0x00C3, 0x00E3, 0x0102)
-
-
-def extra_distance_bits(n):
-    if 0 <= n <= 1:
-        return 0
-    elif 2 <= n <= 29:
-        return (n >> 1) - 1
-    else:
-        raise RuntimeError('illegal distance code')
-
-
-def extra_length_bits(n):
-    if 257 <= n <= 260 or n == 285:
-        return 0
-    elif 261 <= n <= 284:
-        return ((n - 257) >> 2) - 1
-    else:
-        raise RuntimeError('illegal length code')
-
-
-def move_to_front(array: list, index):
-    array[:] = itertools.chain(
-        itertools.islice(array, index, index + 1),
-        itertools.islice(array, 0, index),
-        itertools.islice(array, index + 1, None)
-    )
-
-
-def bwt_transform(data):
-    tmp = bytearray(sorted(data))
-    base = list(map(tmp.find, range(256)))
-    pointers = [-1] * len(data)
-    for i, symbol in enumerate(data):
-        pointers[base[symbol]] = i
-        base[symbol] += 1
-    return pointers
-
-
-def bwt_reverse(data, end):
-    out = bytearray(len(data))
-    transform = bwt_transform(data)
-
-    # STRAGENESS WARNING: There was a bug somewhere here in that
-    # if the output of the BWT resolves to a perfect copy of N
-    # identical strings (think exact multiples of 255 'X' here),
-    # then a loop is formed.  When decoded, the output string would
-    # be cut off after the first loop, typically '\0\0\0\0\xfb'.
-    # The previous loop construct was:
-    #
-    #  next = T[end]
-    #  while next != end:
-    #      out += L[next]
-    #      next = T[next]
-    #  out += L[next]
-    #
-    # For the moment, I've instead replaced it with a check to see
-    # if there has been enough output generated.  I didn't figured
-    # out where the off-by-one-ism is yet---that actually produced
-    # the cyclic loop.
-
-    for i in range(len(data)):
-        end = transform[end]
-        out[i] = data[end]
-
-    return out
-
-
-class _DecompressionFile(abc.ABC):
-
-    def readable(self) -> bool:
-        return True
-
-    def seekable(self) -> bool:
-        return False
-
-    def writable(self) -> bool:
-        return False
-
-    def write(self, __b):
-        raise NotImplementedError
-
-    data: BinaryIO
-    bits: BitfieldBase
-    nsis: bool
-    done: bool
-    current_block: bytearray
-
-    def __init__(self, data: BinaryIO, nsis: bool = True):
-        self.data = data
-        self.nsis = nsis
-        self.done = False
-        self.current_block = bytearray()
-
-    def readall(self) -> bytes:
-        return self.read()
-
-    def readinto(self, __buffer):
-        data = self.read(len(__buffer))
-        size = len(data)
-        __buffer[:size] = data
-        return size
-
-    def read(self, size=-1):
-        while size not in range(len(self.current_block)):
-            if not self._readblock():
-                break
-        block = self.current_block
-        if size < 0 or size >= len(block):
-            self.current_block = bytearray()
-            return block
-        else:
-            out = block[:size]
-            del block[:size]
-            return out
-
-    @abc.abstractmethod
-    def _readblock(self) -> bool:
-        pass
-
-
-class BZip2File(_DecompressionFile):
-
-    blocksize: int
-    block_header_size: int
-    block_header_type: Tuple[int, int]
-    current_block: bytearray
-
-    def __init__(self, data: BinaryIO, nsis: bool = True):
-        super().__init__(data, nsis)
-        self.bits = RBitfield(data)
-
-        if nsis:
-            self.blocksize = 9
-            self.block_header_size = 8
-            self.block_header_type = (0x31, 0x17)
-        else:
-            if data.read(2) != b'BZ':
-                raise RuntimeError('BZip2 header magic is missing')
-            if self.bits.readbits(8) != ord('h'):
-                raise RuntimeError('BZip2 header contains unknown compression method')
-            blocksize = self.bits.readbits(8)
-            if 0x31 <= blocksize <= 0x39:
-                blocksize = blocksize - 0x30
-            else:
-                raise RuntimeError('BZip2 header specifies invalid block size')
-            self.blocksize = blocksize
-            self.block_header_size = 48
-            self.block_header_type = (0x314159265359, 0x177245385090)
-
-        self.blocksize *= 100_000
-
-    def _readblock(self):
-        out = self.current_block
-        if self.done:
-            return False
-        br = self.bits
-        blocktype = br.readbits(self.block_header_size)
-        if not self.nsis:
-            _ = br.readbits(32) # crc
-        if blocktype == self.block_header_type[0]:
-            if not self.nsis and br.readbits(1):
-                raise RuntimeError('BZip2 randomised support not implemented')
-            pointer = br.readbits(24)
-            huffman_used_map = br.readbits(16)
-            map_mask = 1 << 15
-            used = []
-            while map_mask > 0:
-                if huffman_used_map & map_mask:
-                    huffman_used_bitmap = br.readbits(16)
-                    bit_mask = 1 << 15
-                    while bit_mask > 0:
-                        if huffman_used_bitmap & bit_mask:
-                            pass
-                        used += [bool(huffman_used_bitmap & bit_mask)]
-                        bit_mask >>= 1
-                else:
-                    used += [False] * 16
-                map_mask >>= 1
-            huffman_groups = br.readbits(3)
-            if not 2 <= huffman_groups <= 6:
-                raise RuntimeError('BZip2 number of Huffman groups not in range 2..6')
-            selectors_used = br.readbits(15)
-            mtf = list(range(huffman_groups))
-            selectors_list = []
-            for i in range(selectors_used):
-                c = 0
-                while br.readbits(1):
-                    c += 1
-                    if c >= huffman_groups:
-                        raise RuntimeError('BZip2 chosen selector greater than number of groups (max 6)')
-                if c >= 0:
-                    move_to_front(mtf, c)
-                selectors_list += mtf[0:1]
-            groups_lengths = []
-            symbols_in_use = sum(used) + 2  # remember RUN[AB] RLE symbols
-            for _ in range(huffman_groups):
-                length = br.readbits(5)
-                lengths = []
-                for i in range(symbols_in_use):
-                    if not 0 <= length <= 20:
-                        raise RuntimeError('BZip2 Huffman length code outside range 0..20')
-                    while br.readbits(1):
-                        length -= (br.readbits(1) * 2) - 1
-                    lengths += [length]
-                groups_lengths += [lengths]
-
-            tables = []
-            for g in groups_lengths:
-                codes = OrderedHuffmanTable(g)
-                codes.populate_huffman_symbols()
-                codes.min_max_bits()
-                tables.append(codes)
-
-            favourites = [y for y, x in enumerate(used) if x]
-            selector_pointer = 0
-            decoded = 0
-            repeat = repeat_power = 0
-            buffer = bytearray()
-            t = None
-            while True:
-                decoded -= 1
-                if decoded <= 0:
-                    decoded = 50
-                    if selector_pointer <= len(selectors_list):
-                        t = tables[selectors_list[selector_pointer]]
-                        selector_pointer += 1
-                r = t.find_next_symbol(br, False)
-                if 0 <= r <= 1:
-                    if repeat == 0:
-                        repeat_power = 1
-                    repeat += repeat_power << r
-                    repeat_power <<= 1
-                    continue
-                elif repeat > 0:
-                    buffer.extend(itertools.repeat(favourites[0], repeat))
-                    repeat = 0
-                if r == symbols_in_use - 1:
-                    break
-                else:
-                    o = favourites[r - 1]
-                    move_to_front(favourites, r - 1)
-                    buffer.append(o)
-            # RLE step
-            nt = bwt_reverse(buffer, pointer)
-            done = bytearray()
-            n = len(nt)
-            i = 0
-            while i < n:
-                if i < n - 4 and nt[i] == nt[i + 1] == nt[i + 2] == nt[i + 3]:
-                    done.extend(itertools.repeat(nt[i], nt[i + 4] + 4))
-                    i += 5
-                else:
-                    done.append(nt[i])
-                    i += 1
-            out.extend(done)
-            return True
-        elif blocktype == self.block_header_type[1]:
-            br.align()
-            self.done = True
-            return False
-        else:
-            raise RuntimeError(
-                F'unknown BZip2 block value 0x{blocktype:0{self.block_header_size // 4}X}')
-
-
-class GZipFile(_DecompressionFile):
-
-    def __init__(self, data: BinaryIO, nsis: bool = True):
-        super().__init__(data, nsis)
-        br = self.bits = LBitfield(data)
-        if self.data.read(2) != b'\x1F\x8B':
-            raise RuntimeError('Unknown (not 1F8B) header')
-        if br.readbits(8) != 8:
-            raise RuntimeError('Unknown (not type 8 DEFLATE) compression method')
-        self.flags = br.readbits(8)
-        self.mtime = br.readbits(32)
-        self.extra_flags = br.readbits(8)
-        self.os_type = br.readbits(8)
-        self.file_name = ''
-        self.comment = ''
-
-        if self.flags & 0x04:
-            # structured GZ_FEXTRA miscellaneous data
-            xlen = br.readbits(16)
-            br.dropbytes(xlen)
-        while self.flags & 0x08:
-            # original GZ_FNAME filename
-            cc = br.readbits(8)
-            if not cc:
-                break
-            self.file_name += chr(cc)
-        while self.flags & 0x10:
-            # human readable GZ_FCOMMENT
-            cc = br.readbits(8)
-            if not cc:
-                break
-            self.comment += chr(cc)
-        if self.flags & 0x02:
-            # header-only GZ_FHCRC checksum
-            br.readbits(16)
-
-    def _readblock(self) -> bool:
-        if self.done:
-            return False
-        br = self.bits
-        out = self.current_block
-        lastbit = br.readbits(1)
-        blocktype = br.readbits(2)
-
-        def _error_unused(msg):
-            return RuntimeError(F'illegal unused {msg} in use at {br.tell()}')
-
-        if blocktype == 0:
-            br.align()
-            length = br.readbits(16)
-            if length & br.readbits(16):
-                raise RuntimeError('stored block lengths do not match each other')
-            if not br.bits:
-                it = self.data.read(length)
-            else:
-                it = (br.readbits(8) for _ in range(length))
-            out.extend(it)
-
-        elif blocktype == 1 or blocktype == 2:
-            main_literals, main_distances = None, None
-
-            if blocktype == 1: # Static Huffman
-                static_huffman_bootstrap = [(0, 8), (144, 9), (256, 7), (280, 8), (288, -1)]
-                static_huffman_lengths_bootstrap = [(0, 5), (32, -1)]
-                main_literals = HuffmanTable(static_huffman_bootstrap)
-                main_distances = HuffmanTable(static_huffman_lengths_bootstrap)
-
-            elif blocktype == 2: # Dynamic Huffman
-                len_codes = br.readbits(5)
-                literals = len_codes + 257
-                distances = br.readbits(5) + 1
-                code_lengths_length = br.readbits(4) + 4
-                table = [0] * 19
-                for i in range(code_lengths_length):
-                    table[CODE_LENGTH_ORDERS[i]] = br.readbits(3)
-                dynamic_codes = OrderedHuffmanTable(table)
-                dynamic_codes.populate_huffman_symbols()
-                dynamic_codes.min_max_bits()
-
-                # Decode the code_lengths for both tables at once,
-                # then split the list later
-
-                code_lengths = []
-                n = 0
-                while n < (literals + distances):
-                    r = dynamic_codes.find_next_symbol(br)
-                    if 0 <= r <= 15: # literal bitlength for this code
-                        count = 1
-                        what = r
-                    elif r == 16: # repeat last code
-                        count = 3 + br.readbits(2)
-                        # Is this supposed to default to '0' if in the zeroth position?
-                        what = code_lengths[-1]
-                    elif r == 17: # repeat zero
-                        count = 3 + br.readbits(3)
-                        what = 0
-                    elif r == 18: # repeat zero lots
-                        count = 11 + br.readbits(7)
-                        what = 0
-                    else:
-                        raise RuntimeError('next code length is outside of the range 0 <= r <= 18')
-                    code_lengths += [what] * count
-                    n += count
-
-                main_literals = OrderedHuffmanTable(code_lengths[:literals])
-                main_distances = OrderedHuffmanTable(code_lengths[literals:])
-
-            main_literals.populate_huffman_symbols()
-            main_distances.populate_huffman_symbols()
-            main_literals.min_max_bits()
-            main_distances.min_max_bits()
-            literal_count = 0
-
-            while True:
-                r = main_literals.find_next_symbol(br)
-                if 0 <= r <= 255:
-                    literal_count += 1
-                    out.append(r)
-                elif r == 256:
-                    if literal_count > 0:
-                        literal_count = 0
-                    break
-                elif 257 <= r <= 285: # dictionary lookup
-                    if literal_count > 0:
-                        literal_count = 0
-                    length_extra = br.readbits(extra_length_bits(r))
-                    length = LENGTH_BASE[r - 257] + length_extra
-
-                    r1 = main_distances.find_next_symbol(br)
-                    if 0 <= r1 <= 29:
-                        distance = DISTANCE_BASE[r1] + br.readbits(extra_distance_bits(r1))
-                        while length > distance:
-                            out += out[-distance:]
-                            length -= distance
-                        if length == distance:
-                            out += out[-distance:]
-                        else:
-                            out += out[-distance:length - distance]
-                    elif 30 <= r1 <= 31:
-                        raise _error_unused('distance symbol')
-                elif 286 <= r <= 287:
-                    raise _error_unused('literal/length symbol')
-        elif blocktype == 3:
-            raise _error_unused('blocktype')
-
-        if lastbit:
-            self.done = True
-            br.align()
-            _ = br.readbits(32) # crc
-            _ = br.readbits(32) # length
-            return False
-        else:
-            return True
+#!/usr/bin/env python
+# ============================ MOTIFICATION NOTE ============================
+# The content of this file has been modified for use in binary refinery; it
+# has been ported from Python2 to Python3 and the BZip2 implementation was
+# rewritten to support NSIS-specific BZip stream and block headers, which are
+# different from the official standard values. The original code was taken
+# from the following location:
+#  https://github.com/pfalcon/pyflate/blob/master/pyflate.py
+
+# ============================ ORIGINAL LICENSING ============================
+# Copyright 2006--2007-01-21 Paul Sladen
+#  http://www.paul.sladen.org/projects/compression/
+#
+# You may use and distribute this code under any DFSG-compatible license (eg.
+# BSD, GNU GPLv2).
+#
+# Stand-alone pure-Python DEFLATE (gzip) and bzip2 decoder/decompressor. This
+# is probably most useful for research purposes/index building; there is
+# certainly some room for improvement in the Huffman bit-matcher.
+#
+# With the as-written implementation, there was a known bug in BWT decoding
+# to do with repeated strings. This has been worked around; see bwt_reverse().
+# Correct output is produced in all test cases but ideally the problem would
+# be found...
+# ============================================================================
+from __future__ import annotations
+from typing import List, Tuple, Iterable, Optional, BinaryIO
+
+import itertools
+import abc
+
+
+class BitfieldBase(abc.ABC):
+
+    def __init__(self, x):
+        if isinstance(x, BitfieldBase):
+            self.f = x.f
+            self.bits = x.bits
+            self.bitfield = x.bitfield
+            self.count = x.bitfield
+        else:
+            self.f = x
+            self.bits = 0
+            self.bitfield = 0x0
+            self.count = 0
+
+    def _read(self, n):
+        s = self.f.read(n)
+        if not s:
+            raise RuntimeError('length error')
+        self.count += len(s)
+        return s
+
+    def needbits(self, n):
+        while self.bits < n:
+            self._more()
+
+    def _mask(self, n):
+        return (1 << n) - 1
+
+    def toskip(self):
+        return self.bits & 0x7
+
+    def align(self):
+        self.readbits(self.toskip())
+
+    def dropbits(self, n=8):
+        while n >= self.bits and n > 7:
+            n -= self.bits
+            self.bits = 0
+            n -= len(self.f._read(n >> 3)) << 3
+        if n:
+            self.readbits(n)
+
+    def dropbytes(self, n=1):
+        self.dropbits(n << 3)
+
+    def tell(self):
+        return self.count - ((self.bits + 7) >> 3), 7 - ((self.bits - 1) & 0x7)
+
+    def tellbits(self):
+        bytes, bits = self.tell()
+        return (bytes << 3) + bits
+
+    @abc.abstractmethod
+    def _more(self):
+        pass
+
+    @abc.abstractmethod
+    def snoopbits(self, n=8):
+        pass
+
+    @abc.abstractmethod
+    def readbits(self, n=8):
+        pass
+
+
+class LBitfield(BitfieldBase):
+
+    def _more(self):
+        c = self._read(1)
+        self.bitfield += c[0] << self.bits
+        self.bits += 8
+
+    def snoopbits(self, n=8):
+        if n > self.bits:
+            self.needbits(n)
+        return self.bitfield & self._mask(n)
+
+    def readbits(self, n=8):
+        if n > self.bits:
+            self.needbits(n)
+        r = self.bitfield & self._mask(n)
+        self.bits -= n
+        self.bitfield >>= n
+        return r
+
+
+class RBitfield(BitfieldBase):
+
+    def _more(self):
+        c = self._read(1)
+        self.bitfield <<= 8
+        self.bitfield += c[0]
+        self.bits += 8
+
+    def snoopbits(self, n=8):
+        if n > self.bits:
+            self.needbits(n)
+        return (self.bitfield >> (self.bits - n)) & self._mask(n)
+
+    def readbits(self, n=8):
+        if n > self.bits:
+            self.needbits(n)
+        r = (self.bitfield >> (self.bits - n)) & self._mask(n)
+        self.bits -= n
+        self.bitfield &= ~(self._mask(n) << self.bits)
+        return r
+
+
+class HuffmanLength:
+    code: int
+    bits: int
+    symbol: Optional[int]
+    reverse_symbol: Optional[int]
+
+    def __init__(self, code, bits=0):
+        self.code = code
+        self.bits = bits
+        self.symbol = None
+        self.reverse_symbol = None
+
+    def __lt__(self, other):
+        return self.__cmp(other) < 0
+
+    def __gt__(self, other):
+        return self.__cmp(other) > 0
+
+    def __eq__(self, other):
+        return self.__cmp(other) == 0
+
+    def __le__(self, other):
+        return self.__cmp(other) <= 0
+
+    def __ge__(self, other):
+        return self.__cmp(other) >= 0
+
+    def __ne__(self, other):
+        return self.__cmp(other) != 0
+
+    def __cmp(self, other):
+        a, b = self.bits, other.bits
+        if a == b:
+            a, b = self.code, other.code
+        return (a > b) - (a < b)
+
+
+def reverse_bits(v: int, n: int):
+    a = 1 << 0
+    b = 1 << (n - 1)
+    z = 0
+    for i in range(n - 1, -1, -2):
+        z |= (v >> i) & a
+        z |= (v << i) & b
+        a <<= 1
+        b >>= 1
+    return z
+
+
+def reverse_bytes(v, n):
+    a = 0xff << 0
+    b = 0xff << (n - 8)
+    z = 0
+    for i in range(n - 8, -8, -16):
+        z |= (v >> i) & a
+        z |= (v << i) & b
+        a <<= 8
+        b >>= 8
+    return z
+
+
+class HuffmanTable:
+    table: List[HuffmanLength]
+
+    def __init__(self, bootstrap):
+        table = []
+        start, bits = bootstrap[0]
+        for finish, endbits in bootstrap[1:]:
+            if bits:
+                for code in range(start, finish):
+                    table.append(HuffmanLength(code, bits))
+            start, bits = finish, endbits
+            if endbits == -1:
+                break
+        table.sort()
+        self.table = table
+
+    def populate_huffman_symbols(self):
+        bits, symbol = -1, -1
+        for x in self.table:
+            symbol += 1
+            if x.bits != bits:
+                symbol <<= (x.bits - bits)
+                bits = x.bits
+            x.symbol = symbol
+            x.reverse_symbol = reverse_bits(symbol, bits)
+
+    def min_max_bits(self):
+        self.min_bits, self.max_bits = 16, -1
+        for x in self.table:
+            if x.bits < self.min_bits: self.min_bits = x.bits
+            if x.bits > self.max_bits: self.max_bits = x.bits
+
+    def _find_symbol(self, bits: int, symbol: int, table: Iterable[HuffmanLength]) -> int:
+        for h in table:
+            if h.bits == bits and h.reverse_symbol == symbol:
+                return h.code
+        return -1
+
+    def find_next_symbol(self, field: LBitfield, reversed=True):
+        cached_length = -1
+        cached = None
+        for x in self.table:
+            if cached_length != x.bits:
+                cached = field.snoopbits(x.bits)
+                cached_length = x.bits
+            if (reversed and x.reverse_symbol == cached) or (not reversed and x.symbol == cached):
+                field.readbits(x.bits)
+                return x.code
+        raise RuntimeError(F'symbol not found even after end of table at {field.tell()}')
+
+
+class OrderedHuffmanTable(HuffmanTable):
+    def __init__(self, lengths):
+        _ordered_lengths = list(enumerate(lengths))
+        _ordered_lengths.append((len(lengths), -1))
+        super().__init__(_ordered_lengths)
+
+
+CODE_LENGTH_ORDERS = (
+    0x10, 0x11, 0x12, 0x00, 0x08, 0x07, 0x09, 0x06, 0x0A, 0x05,
+    0x0B, 0x04, 0x0C, 0x03, 0x0D, 0x02, 0x0E, 0x01, 0x0F)
+
+DISTANCE_BASE = (
+    0x0001, 0x0002, 0x0003, 0x0004, 0x0005, 0x0007, 0x0009, 0x000D, 0x0011, 0x0019,
+    0x0021, 0x0031, 0x0041, 0x0061, 0x0081, 0x00C1, 0x0101, 0x0181, 0x0201, 0x0301,
+    0x0401, 0x0601, 0x0801, 0x0C01, 0x1001, 0x1801, 0x2001, 0x3001, 0x4001, 0x6001)
+
+LENGTH_BASE = (
+    0x0003, 0x0004, 0x0005, 0x0006, 0x0007, 0x0008, 0x0009, 0x000A, 0x000B, 0x000D,
+    0x000F, 0x0011, 0x0013, 0x0017, 0x001B, 0x001F, 0x0023, 0x002B, 0x0033, 0x003B,
+    0x0043, 0x0053, 0x0063, 0x0073, 0x0083, 0x00A3, 0x00C3, 0x00E3, 0x0102)
+
+
+def extra_distance_bits(n):
+    if 0 <= n <= 1:
+        return 0
+    elif 2 <= n <= 29:
+        return (n >> 1) - 1
+    else:
+        raise RuntimeError('illegal distance code')
+
+
+def extra_length_bits(n):
+    if 257 <= n <= 260 or n == 285:
+        return 0
+    elif 261 <= n <= 284:
+        return ((n - 257) >> 2) - 1
+    else:
+        raise RuntimeError('illegal length code')
+
+
+def move_to_front(array: list, index):
+    array[:] = itertools.chain(
+        itertools.islice(array, index, index + 1),
+        itertools.islice(array, 0, index),
+        itertools.islice(array, index + 1, None)
+    )
+
+
+def bwt_transform(data):
+    tmp = bytearray(sorted(data))
+    base = list(map(tmp.find, range(256)))
+    pointers = [-1] * len(data)
+    for i, symbol in enumerate(data):
+        pointers[base[symbol]] = i
+        base[symbol] += 1
+    return pointers
+
+
+def bwt_reverse(data, end):
+    out = bytearray(len(data))
+    transform = bwt_transform(data)
+
+    # STRAGENESS WARNING: There was a bug somewhere here in that
+    # if the output of the BWT resolves to a perfect copy of N
+    # identical strings (think exact multiples of 255 'X' here),
+    # then a loop is formed.  When decoded, the output string would
+    # be cut off after the first loop, typically '\0\0\0\0\xfb'.
+    # The previous loop construct was:
+    #
+    #  next = T[end]
+    #  while next != end:
+    #      out += L[next]
+    #      next = T[next]
+    #  out += L[next]
+    #
+    # For the moment, I've instead replaced it with a check to see
+    # if there has been enough output generated.  I didn't figured
+    # out where the off-by-one-ism is yet---that actually produced
+    # the cyclic loop.
+
+    for i in range(len(data)):
+        end = transform[end]
+        out[i] = data[end]
+
+    return out
+
+
+class _DecompressionFile(abc.ABC):
+
+    def readable(self) -> bool:
+        return True
+
+    def seekable(self) -> bool:
+        return False
+
+    def writable(self) -> bool:
+        return False
+
+    def write(self, __b):
+        raise NotImplementedError
+
+    data: BinaryIO
+    bits: BitfieldBase
+    nsis: bool
+    done: bool
+    current_block: bytearray
+
+    def __init__(self, data: BinaryIO, nsis: bool = True):
+        self.data = data
+        self.nsis = nsis
+        self.done = False
+        self.current_block = bytearray()
+
+    def readall(self) -> bytes:
+        return self.read()
+
+    def readinto(self, __buffer):
+        data = self.read(len(__buffer))
+        size = len(data)
+        __buffer[:size] = data
+        return size
+
+    def read(self, size=-1):
+        while size not in range(len(self.current_block)):
+            if not self._readblock():
+                break
+        block = self.current_block
+        if size < 0 or size >= len(block):
+            self.current_block = bytearray()
+            return block
+        else:
+            out = block[:size]
+            del block[:size]
+            return out
+
+    @abc.abstractmethod
+    def _readblock(self) -> bool:
+        pass
+
+
+class BZip2File(_DecompressionFile):
+
+    blocksize: int
+    block_header_size: int
+    block_header_type: Tuple[int, int]
+    current_block: bytearray
+
+    def __init__(self, data: BinaryIO, nsis: bool = True):
+        super().__init__(data, nsis)
+        self.bits = RBitfield(data)
+
+        if nsis:
+            self.blocksize = 9
+            self.block_header_size = 8
+            self.block_header_type = (0x31, 0x17)
+        else:
+            if data.read(2) != b'BZ':
+                raise RuntimeError('BZip2 header magic is missing')
+            if self.bits.readbits(8) != ord('h'):
+                raise RuntimeError('BZip2 header contains unknown compression method')
+            blocksize = self.bits.readbits(8)
+            if 0x31 <= blocksize <= 0x39:
+                blocksize = blocksize - 0x30
+            else:
+                raise RuntimeError('BZip2 header specifies invalid block size')
+            self.blocksize = blocksize
+            self.block_header_size = 48
+            self.block_header_type = (0x314159265359, 0x177245385090)
+
+        self.blocksize *= 100_000
+
+    def _readblock(self):
+        out = self.current_block
+        if self.done:
+            return False
+        br = self.bits
+        blocktype = br.readbits(self.block_header_size)
+        if not self.nsis:
+            _ = br.readbits(32) # crc
+        if blocktype == self.block_header_type[0]:
+            if not self.nsis and br.readbits(1):
+                raise RuntimeError('BZip2 randomised support not implemented')
+            pointer = br.readbits(24)
+            huffman_used_map = br.readbits(16)
+            map_mask = 1 << 15
+            used = []
+            while map_mask > 0:
+                if huffman_used_map & map_mask:
+                    huffman_used_bitmap = br.readbits(16)
+                    bit_mask = 1 << 15
+                    while bit_mask > 0:
+                        if huffman_used_bitmap & bit_mask:
+                            pass
+                        used += [bool(huffman_used_bitmap & bit_mask)]
+                        bit_mask >>= 1
+                else:
+                    used += [False] * 16
+                map_mask >>= 1
+            huffman_groups = br.readbits(3)
+            if not 2 <= huffman_groups <= 6:
+                raise RuntimeError('BZip2 number of Huffman groups not in range 2..6')
+            selectors_used = br.readbits(15)
+            mtf = list(range(huffman_groups))
+            selectors_list = []
+            for i in range(selectors_used):
+                c = 0
+                while br.readbits(1):
+                    c += 1
+                    if c >= huffman_groups:
+                        raise RuntimeError('BZip2 chosen selector greater than number of groups (max 6)')
+                if c >= 0:
+                    move_to_front(mtf, c)
+                selectors_list += mtf[0:1]
+            groups_lengths = []
+            symbols_in_use = sum(used) + 2  # remember RUN[AB] RLE symbols
+            for _ in range(huffman_groups):
+                length = br.readbits(5)
+                lengths = []
+                for i in range(symbols_in_use):
+                    if not 0 <= length <= 20:
+                        raise RuntimeError('BZip2 Huffman length code outside range 0..20')
+                    while br.readbits(1):
+                        length -= (br.readbits(1) * 2) - 1
+                    lengths += [length]
+                groups_lengths += [lengths]
+
+            tables = []
+            for g in groups_lengths:
+                codes = OrderedHuffmanTable(g)
+                codes.populate_huffman_symbols()
+                codes.min_max_bits()
+                tables.append(codes)
+
+            favourites = [y for y, x in enumerate(used) if x]
+            selector_pointer = 0
+            decoded = 0
+            repeat = repeat_power = 0
+            buffer = bytearray()
+            t = None
+            while True:
+                decoded -= 1
+                if decoded <= 0:
+                    decoded = 50
+                    if selector_pointer <= len(selectors_list):
+                        t = tables[selectors_list[selector_pointer]]
+                        selector_pointer += 1
+                r = t.find_next_symbol(br, False)
+                if 0 <= r <= 1:
+                    if repeat == 0:
+                        repeat_power = 1
+                    repeat += repeat_power << r
+                    repeat_power <<= 1
+                    continue
+                elif repeat > 0:
+                    buffer.extend(itertools.repeat(favourites[0], repeat))
+                    repeat = 0
+                if r == symbols_in_use - 1:
+                    break
+                else:
+                    o = favourites[r - 1]
+                    move_to_front(favourites, r - 1)
+                    buffer.append(o)
+            # RLE step
+            nt = bwt_reverse(buffer, pointer)
+            done = bytearray()
+            n = len(nt)
+            i = 0
+            while i < n:
+                if i < n - 4 and nt[i] == nt[i + 1] == nt[i + 2] == nt[i + 3]:
+                    done.extend(itertools.repeat(nt[i], nt[i + 4] + 4))
+                    i += 5
+                else:
+                    done.append(nt[i])
+                    i += 1
+            out.extend(done)
+            return True
+        elif blocktype == self.block_header_type[1]:
+            br.align()
+            self.done = True
+            return False
+        else:
+            raise RuntimeError(
+                F'unknown BZip2 block value 0x{blocktype:0{self.block_header_size // 4}X}')
+
+
+class GZipFile(_DecompressionFile):
+
+    def __init__(self, data: BinaryIO, nsis: bool = True):
+        super().__init__(data, nsis)
+        br = self.bits = LBitfield(data)
+        if self.data.read(2) != b'\x1F\x8B':
+            raise RuntimeError('Unknown (not 1F8B) header')
+        if br.readbits(8) != 8:
+            raise RuntimeError('Unknown (not type 8 DEFLATE) compression method')
+        self.flags = br.readbits(8)
+        self.mtime = br.readbits(32)
+        self.extra_flags = br.readbits(8)
+        self.os_type = br.readbits(8)
+        self.file_name = ''
+        self.comment = ''
+
+        if self.flags & 0x04:
+            # structured GZ_FEXTRA miscellaneous data
+            xlen = br.readbits(16)
+            br.dropbytes(xlen)
+        while self.flags & 0x08:
+            # original GZ_FNAME filename
+            cc = br.readbits(8)
+            if not cc:
+                break
+            self.file_name += chr(cc)
+        while self.flags & 0x10:
+            # human readable GZ_FCOMMENT
+            cc = br.readbits(8)
+            if not cc:
+                break
+            self.comment += chr(cc)
+        if self.flags & 0x02:
+            # header-only GZ_FHCRC checksum
+            br.readbits(16)
+
+    def _readblock(self) -> bool:
+        if self.done:
+            return False
+        br = self.bits
+        out = self.current_block
+        lastbit = br.readbits(1)
+        blocktype = br.readbits(2)
+
+        def _error_unused(msg):
+            return RuntimeError(F'illegal unused {msg} in use at {br.tell()}')
+
+        if blocktype == 0:
+            br.align()
+            length = br.readbits(16)
+            if length & br.readbits(16):
+                raise RuntimeError('stored block lengths do not match each other')
+            if not br.bits:
+                it = self.data.read(length)
+            else:
+                it = (br.readbits(8) for _ in range(length))
+            out.extend(it)
+
+        elif blocktype == 1 or blocktype == 2:
+            main_literals, main_distances = None, None
+
+            if blocktype == 1: # Static Huffman
+                static_huffman_bootstrap = [(0, 8), (144, 9), (256, 7), (280, 8), (288, -1)]
+                static_huffman_lengths_bootstrap = [(0, 5), (32, -1)]
+                main_literals = HuffmanTable(static_huffman_bootstrap)
+                main_distances = HuffmanTable(static_huffman_lengths_bootstrap)
+
+            elif blocktype == 2: # Dynamic Huffman
+                len_codes = br.readbits(5)
+                literals = len_codes + 257
+                distances = br.readbits(5) + 1
+                code_lengths_length = br.readbits(4) + 4
+                table = [0] * 19
+                for i in range(code_lengths_length):
+                    table[CODE_LENGTH_ORDERS[i]] = br.readbits(3)
+                dynamic_codes = OrderedHuffmanTable(table)
+                dynamic_codes.populate_huffman_symbols()
+                dynamic_codes.min_max_bits()
+
+                # Decode the code_lengths for both tables at once,
+                # then split the list later
+
+                code_lengths = []
+                n = 0
+                while n < (literals + distances):
+                    r = dynamic_codes.find_next_symbol(br)
+                    if 0 <= r <= 15: # literal bitlength for this code
+                        count = 1
+                        what = r
+                    elif r == 16: # repeat last code
+                        count = 3 + br.readbits(2)
+                        # Is this supposed to default to '0' if in the zeroth position?
+                        what = code_lengths[-1]
+                    elif r == 17: # repeat zero
+                        count = 3 + br.readbits(3)
+                        what = 0
+                    elif r == 18: # repeat zero lots
+                        count = 11 + br.readbits(7)
+                        what = 0
+                    else:
+                        raise RuntimeError('next code length is outside of the range 0 <= r <= 18')
+                    code_lengths += [what] * count
+                    n += count
+
+                main_literals = OrderedHuffmanTable(code_lengths[:literals])
+                main_distances = OrderedHuffmanTable(code_lengths[literals:])
+
+            main_literals.populate_huffman_symbols()
+            main_distances.populate_huffman_symbols()
+            main_literals.min_max_bits()
+            main_distances.min_max_bits()
+            literal_count = 0
+
+            while True:
+                r = main_literals.find_next_symbol(br)
+                if 0 <= r <= 255:
+                    literal_count += 1
+                    out.append(r)
+                elif r == 256:
+                    if literal_count > 0:
+                        literal_count = 0
+                    break
+                elif 257 <= r <= 285: # dictionary lookup
+                    if literal_count > 0:
+                        literal_count = 0
+                    length_extra = br.readbits(extra_length_bits(r))
+                    length = LENGTH_BASE[r - 257] + length_extra
+
+                    r1 = main_distances.find_next_symbol(br)
+                    if 0 <= r1 <= 29:
+                        distance = DISTANCE_BASE[r1] + br.readbits(extra_distance_bits(r1))
+                        while length > distance:
+                            out += out[-distance:]
+                            length -= distance
+                        if length == distance:
+                            out += out[-distance:]
+                        else:
+                            out += out[-distance:length - distance]
+                    elif 30 <= r1 <= 31:
+                        raise _error_unused('distance symbol')
+                elif 286 <= r <= 287:
+                    raise _error_unused('literal/length symbol')
+        elif blocktype == 3:
+            raise _error_unused('blocktype')
+
+        if lastbit:
+            self.done = True
+            br.align()
+            _ = br.readbits(32) # crc
+            _ = br.readbits(32) # length
+            return False
+        else:
+            return True
```

### Comparing `debloat-1.5.6/src/debloat/utilities/readers.py` & `debloat-1.5.6.1/src/debloat/utilities/readers.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,604 +1,604 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-# Most of this code was repurposed from Binary Refinery (https://github.com/binref/refinery), used under the 3-Clause BSD License
-
-from __future__ import annotations
-import io
-import itertools
-import enum
-import struct
-import re
-import functools
-from types import TracebackType
-from typing import List, Union, Tuple, Optional, Iterable, ByteString, TypeVar, Generic, Any, Dict
-
-T = TypeVar('T', bound=Union[bytearray, bytes, memoryview])
-UnpackType = Union[int, bool, float, bytes]
-
-def signed(k: int, bits: int):
-    M = 1 << bits
-    k = k & (M - 1)
-    return k - M if k >> (bits - 1) else k
-
-class StreamDetour:
-    def __init__(self, stream: io.IOBase, 
-                 offset=None, whence=io.SEEK_SET) -> None:
-        self.stream = stream
-        self.offset = offset
-        self.whence = whence
-
-    def __enter__(self) -> io.IOBase:
-        self.cursor = self.stream.tell()
-        if self.offset is not None:
-            self.stream.seek(self.offset, self.whence)
-        return self.stream
-    
-    def __exit__(self, *args) -> None:
-        self.stream.seek(self.cursor, io.SEEK_SET)
-
-class MemoryFile(Generic[T], io.IOBase):
-
-    closed: bool
-    read_as_bytes: bool
-
-    _data: T
-    _cursor: int   # Defines where in the file we are currently reading from
-    _closed: bool
-
-    class SEEK(int, enum.Enum):
-        CUR = io.SEEK_CUR
-        END = io.SEEK_END
-        SET = io.SEEK_SET
-
-    def __init__(self, data: T, read_as_bytes: bool = False, 
-                 file_number: Optional[int] = None) -> None:
-        self._data = data
-        self._cursor = 0
-        self._closed = False
-        self.read_as_bytes = read_as_bytes
-        self.file_number = file_number
-
-    def close(self) -> None:
-        self._closed = True
-
-    @property
-    def closed(self) -> bool:
-        return self._closed
-    
-    # Enter and exit methods for context manager
-    def __enter__(self) -> 'MemoryFile':
-        return self
-    
-    def __exit__(self, exc_type: type[BaseException] | None, exc_val: BaseException | None, exc_tb: TracebackType | None) -> None:
-        return super().__exit__(exc_type, exc_val, exc_tb)
-    
-    def flush(self) -> None:
-        return super().flush()
-    
-    def isatty(self) -> bool:
-        return super().isatty()
-
-    def __iter__(self) -> Iterable[bytes]:
-        return self
-    
-    def __len__(self) -> int:
-        return len(self._data)
-    
-    def __next__(self) -> bytes:
-        if self._cursor >= len(self._data):
-            raise StopIteration
-        else:
-            return self.readline()
-        
-    def file_number(self) -> Optional[int]:
-        if self.file_number is None:
-            return None
-        return self.file_number
-    
-    def readable(self) -> bool:
-        return super().readable()
-    
-    def seekable(self) -> bool:
-        return super().seekable()
-    
-    @property
-    def is_eof(self) -> bool:
-        return self._closed or self._cursor >= len(self._data)
-    
-    @property
-    def remaining_bytes(self) -> int:
-        return len(self._data) - self.tell()
-    
-    def writable(self) -> bool:
-        if self._closed:
-            return False
-        # Readonly for memoryview?
-        return isinstance(self._data, bytearray)
-
-    def read(self, size: int = -1, peek: bool = False) -> T:
-        beginning = self._cursor
-        if size is None or size < 0:
-            end = len(self._data)
-        else:
-            end = min(self._cursor + size, len(self._data))
-        result = self._data[beginning:end]
-        if self.read_as_bytes and not isinstance(result, bytes):
-            result = bytes(result)
-        if not peek:
-            self._cursor = end
-        return result
-    
-    def peek(self, size: int = -1) -> memoryview:
-        cursor = self._cursor
-        mv = memoryview(self._data)
-        if size is None or size < 0:
-            return mv[cursor:]
-        return mv[cursor:cursor + size]
-    
-    def read1(self, size: int = -1, peek: bool = False) -> T:
-        return self.read(size, peek)
-    
-    def _find_linebreak(self, beginning: int, end: int) -> int:
-        if not isinstance(self._data, memoryview):
-            return self._data.find(b'\n', beginning, end)
-        for k in range(beginning, end):
-            if self._data[k] == 0xA: return k
-        return -1
-    
-    def readline(self, size: int = -1) -> T:
-        beginning, end = self._cursor, len(self._data)
-        if size is not None and size >= 0:
-            end = beginning + size
-        p = self._find_linebreak(beginning, end)
-        self._cursor = end if p < 0 else p + 1
-        result = self._data[beginning:self._cursor]
-        if self.read_as_bytes and not isinstance(result, bytes):
-            result = bytes(result)
-        return result
-    
-    def readlines(self, size: int = -1) -> Iterable[T]:
-        if size is None or size < 0:
-            yield from self
-        else:
-            total = 0
-            while total < size:
-                line = next(self)
-                total += len(line)
-                yield line
-    
-    def readinto1(self, buffer: Any) -> int:
-        data = self.read(len(buffer))
-        size = len(data)
-        buffer[:size] = data
-        return size
-    
-    def readinto(self, buffer: Any) -> int: 
-        return self.readinto1(buffer)
-
-    def tell(self) -> int:
-        return self._cursor
-    
-    def seek_relative(self, offset: int) -> int:
-        return self.seek(self._cursor + offset)
-        
-    def seek_set(self, offset: int) -> int:
-        if offset < 0:
-            return self.seek(offset, self.SEEK.END)
-        else:
-            return self.seek(offset, self.SEEK.SET)
-        
-    def get_buffer(self) -> T:
-        return self._data
-    
-    def get_value(self) -> T:
-        return self._data
-    
-    def seek(self, offset: int, whence=io.SEEK_SET) -> int:
-        if whence == io.SEEK_SET:
-            if offset < 0:
-                raise ValueError('Negative seek position {}'.format(offset))    
-            self._cursor = offset
-        elif whence == io.SEEK_CUR:
-            self._cursor += offset
-        elif whence == io.SEEK_END:
-            self._cursor = len(self._data) + offset
-        self._cursor = max(0, min(self._cursor, len(self._data)))
-        return self._cursor
-    
-    def write_lines(self, lines: Iterable[ByteString]) -> None:
-        for line in lines:
-            self.append(line)
-
-    def truncate(self, size=None) -> None:
-        if size is not None:
-            if not (0 <= size <= len(self._data)):
-                raise ValueError('Invalid size {}'.format(size))
-            self._cursor = size
-        del self._data[self._cursor:]
-
-    def append_byte(self, byte: int) -> None:
-        try:
-            cursor = self._cursor
-            if cursor < len(self._data):
-                self._data[cursor] = byte
-            else:
-                self._data.append(byte)
-        except Exception as T:
-            raise io.UnsupportedOperation('append_byte') from T
-        else:
-            self._cursor += 1
-
-    def append(self, data: Iterable[int]) -> int:
-        output_data = self._data
-        end = len(output_data)
-        beginning = self._cursor
-        if beginning == end:
-            output_data.extend(data)
-            self._cursor = end = len(output_data)
-            return end - beginning
-        try:
-            size = len(data)
-        except Exception as T:
-            it = iter(data)
-            for cursor, byte in enumerate(it, end - beginning):
-                output_data[cursor] = byte
-                if cursor >= end - 1:
-                    break
-            else:
-                cursor += 1
-                self._cursor = cursor
-                return cursor - beginning
-            output_data.extend(it)
-        else:
-            self._cursor += size
-            try:
-                self._data[beginning:self._cursor] = data
-            except Exception as T:
-                self._cursor = beginning
-                raise io.UnsupportedOperation('append') from T
-            return size
-        self._cursor = end = len(output_data)
-        return end - beginning
-
-    def __getitem__(self, slice: Any) -> T:
-        result = self._data[slice]
-        if isinstance(result, bytes) and not self.read_as_bytes:
-            result = bytes(result)
-        return result
-
-    def replay(self, offset: int, length: int) -> None:
-        if offset not in range(self._cursor + 1):
-            raise ValueError('Invalid offset {}'.format(offset))
-        rep, r = divmod(length, offset)
-        offset = -offset - len(self) + self._cursor
-        replay = self._data[offset:offset + r]
-        if rep > 0:
-            replay = bytes(self._data[offset:self._cursor]) * rep + replay
-        self.append(replay)
-
-
-class order(str, enum.Enum):
-    big = 'big'
-    little = 'little'
-
-class StructReader(MemoryFile[T]):
-
-    class Unaligned(RuntimeError):
-        pass
-
-    def __init__(self, data: T, bigendian: bool = False):
-        super().__init__(data)
-        self._number_of_bits = 0
-        self._buffer_bits = 0
-        self._bigendian = bigendian
-    
-    def __enter__(self) -> 'StructReader':
-        return self
-    
-    def __exit__(self) -> None:
-        return super().__exit__()
-
-    @property
-    def bigendian(self):
-        self.bigendian = True
-        try:
-            yield self
-        finally:
-            self.bigendian = False
-    
-    @property
-    def byteorder_format(self) -> str:
-        return '>' if self.bigendian else '<'
-    
-    @property
-    def byteorder_name(self) -> str:
-        return 'big' if self._bigendian else 'little'
-
-    def readinto(self, buffer: Any) -> int:
-        return super().readinto(buffer)
-    
-    def seek(self, offset: int, whence: int = io.SEEK_SET) -> int:
-        return super().seek(offset, whence)
-    
-    def read_exactly(self, size: Optional[int] = None,
-                      peek: bool = False) -> T:
-        if not self.byte_aligned:
-            raise StructReader.Unaligned('Buffer is not byte aligned')
-        data = self.read1(size, peek)
-        if size and len(data) < size:
-            raise EOF(data)
-        return data
-        
-    @property
-    def byte_aligned(self) -> bool:
-        return not self._number_of_bits
-    
-    def byte_align(self, blocksize: int = 1) -> Tuple[int, int]:
-        if self.byte_aligned:
-            return 0, 0
-        number_of_bits = self._number_of_bits
-        buffer_bits = self._buffer_bits
-        self._number_of_bits = 0
-        self._buffer_bits = 0
-        mod = self._cursor % blocksize
-        self.seek_relative(mod and blocksize - mod)
-        return number_of_bits, buffer_bits
-    
-    # TODO: Review Read Integer if needed
-    def read_integer(self, length: int, peek: bool = False) -> int:
-        """
-        Read `length` many bits from the underlying stream as an integer.
-        """
-        if length < self._number_of_bits:
-            new_count = self._number_of_bits - length
-            if self.bigendian:
-                result = self._buffer_bist >> new_count
-                if not peek:
-                    self._buffer_bist ^= result << new_count
-            else:
-                result = self._buffer_bist & 2 ** length - 1
-                if not peek:
-                    self._buffer_bist >>= length
-            if not peek:
-                self._number_of_bits = new_count
-            return result
-
-
-        number_of_bits, buffer_bits = self.byte_align()
-        number_of_missing_bits = length - number_of_bits
-        bytecount, rest = divmod(number_of_missing_bits, 8)
-        if rest:
-            bytecount += 1
-            rest = 8 - rest
-        if bytecount == 1:
-            result, = self.read_exactly(1, peek)
-        else:
-            result = int.from_bytes(self.read_exactly(bytecount, peek), self.byteorder_name)
-        if not number_of_bits and not rest:
-            return result
-        if self.bigendian:
-            rbmask   = 2 ** rest - 1       # noqa
-            excess   = result & rbmask     # noqa
-            result >>= rest                # noqa
-            result  ^= buffer_bits << number_of_missing_bits   # noqa
-        else:
-            excess   = result >> number_of_missing_bits  # noqa
-            result  ^= excess << number_of_missing_bits  # noqa
-            result <<= number_of_bits               # noqa
-            result  |= buffer_bits               # noqa
-        assert excess.bit_length() <= rest
-        if not peek:
-            self._number_of_bits = rest
-            self._buffer_bist = excess
-        return result
-        
-    def read_bytes(self, size: int, peek: bool = False) -> bytes:
-        if self.byte_aligned:
-            data = self.read_exactly(size, peek)
-            if not isinstance(data, bytes):
-                data = bytes(data)
-            return data
-        else:
-            return self.read_bits(size * 8, peek).tobytes()
-        
-    def read_bit(self) -> int:
-        return self.read_integer(1)
-    
-    def read_bits(self, number_of_bits: int) -> Iterable[int]:
-        chunk = self.read_integrer(number_of_bits) 
-        for k in range(number_of_bits -1, -1, -1):
-            yield chunk >> k & 1
-
-    def read_flags(self, number_of_bits: int, reverse=False) -> Iterable[bool]:
-        bits = list(self.read_bits(number_of_bits))
-        if reverse:
-            bits.reverse()
-        for bit in bits:
-            yield bool(bit)
-
-    def read_struct(self, spec: str, unwrap=False, 
-                    peek=False) -> Union[List[UnpackType], UnpackType]:
-        if not spec:
-            raise ValueError('No format specified')
-        byte_order = spec[:1]
-        if byte_order in '<!=@>':
-            spec = spec[1:]
-        else:
-            byte_order = self.byteorder_format
-        data = []
-        current_cursor = self.tell()
-
-        for k, part in enumerate(re.split('(\\d*[auwE])', spec)):
-            if k % 2 == 1:
-                count = 1 if len(part) == 1 else int(part[:~0])
-                part = part[~0]
-                for _ in range(count):
-                    if part == 'a':
-                        size = self.read_integer(8)
-                        data.append(self.read_bytes(size))
-                    elif part == 'u':
-                        data.append(self.read_integer(8))
-                    elif part == 'w':
-                        data.append(self.read_integer(16))
-                    elif part == 'E':
-                        data.append(self.read_integer(32))
-                    else:
-                        raise ValueError('Invalid format {}'.format(part))
-                continue
-            else:
-                part = F'{byte_order}{part}'
-                data.extend(struct.unpack(part, self.read_exactly(struct.calcsize(part))))
-        if unwrap and len(data) == 1:
-            return data[0]
-        if peek:
-            self.seek_set(current_cursor)
-        return data
-
-    def read_nibble(self, peek: bool = False) -> int:
-        return self.read_integer(4, peek)
-
-
-    def u8(self, peek: bool = False) -> int: 
-        return self.read_integer(8, peek)
-    def i8(self, peek: bool = False) -> int: 
-        return signed(self.read_integer(8, peek), 8)
-    def u16(self, peek: bool = False) -> int: 
-        return self.read_integer(16, peek)
-    def u32(self, peek: bool = False) -> int: 
-        return self.read_integer(32, peek)
-    def u64(self, peek: bool = False) -> int: 
-        return self.read_integer(64, peek)
-    def i16(self, peek: bool = False) -> int: 
-        return signed(self.read_integer(16, peek), 16)
-    def i32(self, peek: bool = False) -> int: 
-        return signed(self.read_integer(32, peek), 32)
-    def i64(self, peek: bool = False) -> int: 
-        return signed(self.read_integer(64, peek), 64)
-    def f32(self, peek: bool = False) -> float: 
-        return self.read_struct('f', unwrap=True, peek=peek)
-    def f64(self, peek: bool = False) -> float: 
-        return self.read_struct('d', unwrap=True, peek=peek)
-    def read_byte(self, peek: bool = False) -> int: 
-        return self.read_integer(8, peek)
-    def read_char(self, peek: bool = False) -> int:
-        return signed(self.read_integer(8, peek), 8)
-
-    def read_terminated_array(self, terminator: bytes, 
-                              alignment: int = 1) -> bytearray:
-        pos = self.tell()
-        buffer = self.get_buffer()
-        try:
-            end = pos - 1
-            while True:
-                end = buffer.find(terminator, end + 1)
-                if end < 0 or not (end - pos) % alignment:
-                    break
-        except AttributeError:
-            result = bytearray()
-            while not self.is_eof:
-                result.extend(self.read_bytes(alignment))
-                if result.endswith(terminator):
-                    return result[:-len(terminator)]
-            self.seek(pos)
-            raise EOF
-        else:
-            data = self.read_exactly(end - pos)
-            self.seek_relative(len(terminator))
-            return bytearray(data)
-    
-    def read_c_string(self, encoding=None) -> Union[str, bytearray]:
-        data = self.read_terminated_array(b'\0')
-        if encoding is not None:
-            data = data.decode(encoding)
-        return data
-    
-    def read_w_string(self, encoding=None) -> Union[str, bytearray]:
-        data = self.read_terminated_array(b'\0\0', 2)
-        if encoding is not None:
-            data = data.decode(encoding)
-        return data
-    
-    def read_length_prefixed(self, 
-                             prefix_size: int = 32, 
-                             encoding: Optional[str] = None,
-                             block_size: int = 1) -> Union[T, str]:
-        prefix = self.read_integer(prefix_size) * block_size
-        data = self.read(prefix)
-        if encoding is not None:
-            data = data.decode(encoding)
-        return data
-
-    def read_length_prefixed_ascii(self, 
-                                   prefix_size: int = 32) -> Union[T, str]:
-        return self.read_length_prefixed(prefix_size, 'ascii')
-    
-    def read_length_prefixed_utf8(self, 
-                                  prefix_size: int = 32) -> Union[T, str]:
-        return self.read_length_prefixed(prefix_size, 'utf-8')
-    
-    def read_length_prefixed_utf16(self, 
-                                   prefix_size: int = 32,
-                                   bytecount: bool = False) -> Union[T, str]:
-        block_size = 1 if bytecount else 2
-        return self.read_length_prefixed(prefix_size, 'utf-16le', block_size)
-    
-    # TODO: Review function if needed
-    def read_7bit_encoded_int(self, max_bits: int = 0) -> int:
-        result = 0
-        for k in itertools.count():
-            if k == max_bits:
-                raise ValueError('Invalid 7-bit encoded integer')
-            byte = self.read_byte()
-            result |= (byte & 0x7F) << (7 * k)
-            if not byte & 0x80:
-                break
-        return result
-
-class StructMeta(type):
-    def __new__(mcls, name, bases, nmspc, parser=StructReader):
-        return type.__new__(mcls, name, bases, nmspc)
-    
-    def __init__(cls, name, bases, nmspc, parser=StructReader):
-        super(StructMeta, cls).__init__(name, bases, nmspc)
-        original__init__ = cls.__init__
-
-        @functools.wraps(original__init__)
-        def wrapped__init__(self: Struct, reader, *args, **kwargs):
-            if not isinstance(reader, parser):
-                if issubclass(parser, reader.__class__):
-                    raise ValueError(
-                        F'A reader of type {reader.__class__.__name__} was passed to {cls.__name__}, '
-                        F'but a {parser.__name__} is required.')
-                reader = parser(reader)
-            start = reader.tell()
-            view = memoryview(reader.get_buffer())
-            original__init__(self, reader, *args, **kwargs)
-            self.__data = view[start:reader.tell()]
-
-        cls.__init__ = wrapped__init__
-
-class Struct(metaclass=StructMeta):
-
-    _data: Union[memoryview, bytearray]
-
-    def __len__(self):
-        return len(self._data)
-    
-    def __bytes__(self):
-        return bytes(self._data)   
-    
-    def get_data(self, decouple=False):
-        if decouple and isinstance(self._data, memoryview):
-            self._data = bytearray(self._data)
-        return self._data
-    
-    def __init__(self, reader: StructReader):
-        pass
-
-    
-
-
-class EOF(EOFError):
-    def __init__(self, rest: ByteString = B''):
-        super().__init__('End of File')
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+# Most of this code was repurposed from Binary Refinery (https://github.com/binref/refinery), used under the 3-Clause BSD License
+
+from __future__ import annotations
+import io
+import itertools
+import enum
+import struct
+import re
+import functools
+from types import TracebackType
+from typing import List, Union, Tuple, Optional, Iterable, ByteString, TypeVar, Generic, Any, Dict
+
+T = TypeVar('T', bound=Union[bytearray, bytes, memoryview])
+UnpackType = Union[int, bool, float, bytes]
+
+def signed(k: int, bits: int):
+    M = 1 << bits
+    k = k & (M - 1)
+    return k - M if k >> (bits - 1) else k
+
+class StreamDetour:
+    def __init__(self, stream: io.IOBase, 
+                 offset=None, whence=io.SEEK_SET) -> None:
+        self.stream = stream
+        self.offset = offset
+        self.whence = whence
+
+    def __enter__(self) -> io.IOBase:
+        self.cursor = self.stream.tell()
+        if self.offset is not None:
+            self.stream.seek(self.offset, self.whence)
+        return self.stream
+    
+    def __exit__(self, *args) -> None:
+        self.stream.seek(self.cursor, io.SEEK_SET)
+
+class MemoryFile(Generic[T], io.IOBase):
+
+    closed: bool
+    read_as_bytes: bool
+
+    _data: T
+    _cursor: int   # Defines where in the file we are currently reading from
+    _closed: bool
+
+    class SEEK(int, enum.Enum):
+        CUR = io.SEEK_CUR
+        END = io.SEEK_END
+        SET = io.SEEK_SET
+
+    def __init__(self, data: T, read_as_bytes: bool = False, 
+                 file_number: Optional[int] = None) -> None:
+        self._data = data
+        self._cursor = 0
+        self._closed = False
+        self.read_as_bytes = read_as_bytes
+        self.file_number = file_number
+
+    def close(self) -> None:
+        self._closed = True
+
+    @property
+    def closed(self) -> bool:
+        return self._closed
+    
+    # Enter and exit methods for context manager
+    def __enter__(self) -> 'MemoryFile':
+        return self
+    
+    def __exit__(self, exc_type: type[BaseException] | None, exc_val: BaseException | None, exc_tb: TracebackType | None) -> None:
+        return super().__exit__(exc_type, exc_val, exc_tb)
+    
+    def flush(self) -> None:
+        return super().flush()
+    
+    def isatty(self) -> bool:
+        return super().isatty()
+
+    def __iter__(self) -> Iterable[bytes]:
+        return self
+    
+    def __len__(self) -> int:
+        return len(self._data)
+    
+    def __next__(self) -> bytes:
+        if self._cursor >= len(self._data):
+            raise StopIteration
+        else:
+            return self.readline()
+        
+    def file_number(self) -> Optional[int]:
+        if self.file_number is None:
+            return None
+        return self.file_number
+    
+    def readable(self) -> bool:
+        return super().readable()
+    
+    def seekable(self) -> bool:
+        return super().seekable()
+    
+    @property
+    def is_eof(self) -> bool:
+        return self._closed or self._cursor >= len(self._data)
+    
+    @property
+    def remaining_bytes(self) -> int:
+        return len(self._data) - self.tell()
+    
+    def writable(self) -> bool:
+        if self._closed:
+            return False
+        # Readonly for memoryview?
+        return isinstance(self._data, bytearray)
+
+    def read(self, size: int = -1, peek: bool = False) -> T:
+        beginning = self._cursor
+        if size is None or size < 0:
+            end = len(self._data)
+        else:
+            end = min(self._cursor + size, len(self._data))
+        result = self._data[beginning:end]
+        if self.read_as_bytes and not isinstance(result, bytes):
+            result = bytes(result)
+        if not peek:
+            self._cursor = end
+        return result
+    
+    def peek(self, size: int = -1) -> memoryview:
+        cursor = self._cursor
+        mv = memoryview(self._data)
+        if size is None or size < 0:
+            return mv[cursor:]
+        return mv[cursor:cursor + size]
+    
+    def read1(self, size: int = -1, peek: bool = False) -> T:
+        return self.read(size, peek)
+    
+    def _find_linebreak(self, beginning: int, end: int) -> int:
+        if not isinstance(self._data, memoryview):
+            return self._data.find(b'\n', beginning, end)
+        for k in range(beginning, end):
+            if self._data[k] == 0xA: return k
+        return -1
+    
+    def readline(self, size: int = -1) -> T:
+        beginning, end = self._cursor, len(self._data)
+        if size is not None and size >= 0:
+            end = beginning + size
+        p = self._find_linebreak(beginning, end)
+        self._cursor = end if p < 0 else p + 1
+        result = self._data[beginning:self._cursor]
+        if self.read_as_bytes and not isinstance(result, bytes):
+            result = bytes(result)
+        return result
+    
+    def readlines(self, size: int = -1) -> Iterable[T]:
+        if size is None or size < 0:
+            yield from self
+        else:
+            total = 0
+            while total < size:
+                line = next(self)
+                total += len(line)
+                yield line
+    
+    def readinto1(self, buffer: Any) -> int:
+        data = self.read(len(buffer))
+        size = len(data)
+        buffer[:size] = data
+        return size
+    
+    def readinto(self, buffer: Any) -> int: 
+        return self.readinto1(buffer)
+
+    def tell(self) -> int:
+        return self._cursor
+    
+    def seek_relative(self, offset: int) -> int:
+        return self.seek(self._cursor + offset)
+        
+    def seek_set(self, offset: int) -> int:
+        if offset < 0:
+            return self.seek(offset, self.SEEK.END)
+        else:
+            return self.seek(offset, self.SEEK.SET)
+        
+    def get_buffer(self) -> T:
+        return self._data
+    
+    def get_value(self) -> T:
+        return self._data
+    
+    def seek(self, offset: int, whence=io.SEEK_SET) -> int:
+        if whence == io.SEEK_SET:
+            if offset < 0:
+                raise ValueError('Negative seek position {}'.format(offset))    
+            self._cursor = offset
+        elif whence == io.SEEK_CUR:
+            self._cursor += offset
+        elif whence == io.SEEK_END:
+            self._cursor = len(self._data) + offset
+        self._cursor = max(0, min(self._cursor, len(self._data)))
+        return self._cursor
+    
+    def write_lines(self, lines: Iterable[ByteString]) -> None:
+        for line in lines:
+            self.append(line)
+
+    def truncate(self, size=None) -> None:
+        if size is not None:
+            if not (0 <= size <= len(self._data)):
+                raise ValueError('Invalid size {}'.format(size))
+            self._cursor = size
+        del self._data[self._cursor:]
+
+    def append_byte(self, byte: int) -> None:
+        try:
+            cursor = self._cursor
+            if cursor < len(self._data):
+                self._data[cursor] = byte
+            else:
+                self._data.append(byte)
+        except Exception as T:
+            raise io.UnsupportedOperation('append_byte') from T
+        else:
+            self._cursor += 1
+
+    def append(self, data: Iterable[int]) -> int:
+        output_data = self._data
+        end = len(output_data)
+        beginning = self._cursor
+        if beginning == end:
+            output_data.extend(data)
+            self._cursor = end = len(output_data)
+            return end - beginning
+        try:
+            size = len(data)
+        except Exception as T:
+            it = iter(data)
+            for cursor, byte in enumerate(it, end - beginning):
+                output_data[cursor] = byte
+                if cursor >= end - 1:
+                    break
+            else:
+                cursor += 1
+                self._cursor = cursor
+                return cursor - beginning
+            output_data.extend(it)
+        else:
+            self._cursor += size
+            try:
+                self._data[beginning:self._cursor] = data
+            except Exception as T:
+                self._cursor = beginning
+                raise io.UnsupportedOperation('append') from T
+            return size
+        self._cursor = end = len(output_data)
+        return end - beginning
+
+    def __getitem__(self, slice: Any) -> T:
+        result = self._data[slice]
+        if isinstance(result, bytes) and not self.read_as_bytes:
+            result = bytes(result)
+        return result
+
+    def replay(self, offset: int, length: int) -> None:
+        if offset not in range(self._cursor + 1):
+            raise ValueError('Invalid offset {}'.format(offset))
+        rep, r = divmod(length, offset)
+        offset = -offset - len(self) + self._cursor
+        replay = self._data[offset:offset + r]
+        if rep > 0:
+            replay = bytes(self._data[offset:self._cursor]) * rep + replay
+        self.append(replay)
+
+
+class order(str, enum.Enum):
+    big = 'big'
+    little = 'little'
+
+class StructReader(MemoryFile[T]):
+
+    class Unaligned(RuntimeError):
+        pass
+
+    def __init__(self, data: T, bigendian: bool = False):
+        super().__init__(data)
+        self._number_of_bits = 0
+        self._buffer_bits = 0
+        self._bigendian = bigendian
+    
+    def __enter__(self) -> 'StructReader':
+        return self
+    
+    def __exit__(self) -> None:
+        return super().__exit__()
+
+    @property
+    def bigendian(self):
+        self.bigendian = True
+        try:
+            yield self
+        finally:
+            self.bigendian = False
+    
+    @property
+    def byteorder_format(self) -> str:
+        return '>' if self.bigendian else '<'
+    
+    @property
+    def byteorder_name(self) -> str:
+        return 'big' if self._bigendian else 'little'
+
+    def readinto(self, buffer: Any) -> int:
+        return super().readinto(buffer)
+    
+    def seek(self, offset: int, whence: int = io.SEEK_SET) -> int:
+        return super().seek(offset, whence)
+    
+    def read_exactly(self, size: Optional[int] = None,
+                      peek: bool = False) -> T:
+        if not self.byte_aligned:
+            raise StructReader.Unaligned('Buffer is not byte aligned')
+        data = self.read1(size, peek)
+        if size and len(data) < size:
+            raise EOF(data)
+        return data
+        
+    @property
+    def byte_aligned(self) -> bool:
+        return not self._number_of_bits
+    
+    def byte_align(self, blocksize: int = 1) -> Tuple[int, int]:
+        if self.byte_aligned:
+            return 0, 0
+        number_of_bits = self._number_of_bits
+        buffer_bits = self._buffer_bits
+        self._number_of_bits = 0
+        self._buffer_bits = 0
+        mod = self._cursor % blocksize
+        self.seek_relative(mod and blocksize - mod)
+        return number_of_bits, buffer_bits
+    
+    # TODO: Review Read Integer if needed
+    def read_integer(self, length: int, peek: bool = False) -> int:
+        """
+        Read `length` many bits from the underlying stream as an integer.
+        """
+        if length < self._number_of_bits:
+            new_count = self._number_of_bits - length
+            if self.bigendian:
+                result = self._buffer_bist >> new_count
+                if not peek:
+                    self._buffer_bist ^= result << new_count
+            else:
+                result = self._buffer_bist & 2 ** length - 1
+                if not peek:
+                    self._buffer_bist >>= length
+            if not peek:
+                self._number_of_bits = new_count
+            return result
+
+
+        number_of_bits, buffer_bits = self.byte_align()
+        number_of_missing_bits = length - number_of_bits
+        bytecount, rest = divmod(number_of_missing_bits, 8)
+        if rest:
+            bytecount += 1
+            rest = 8 - rest
+        if bytecount == 1:
+            result, = self.read_exactly(1, peek)
+        else:
+            result = int.from_bytes(self.read_exactly(bytecount, peek), self.byteorder_name)
+        if not number_of_bits and not rest:
+            return result
+        if self.bigendian:
+            rbmask   = 2 ** rest - 1       # noqa
+            excess   = result & rbmask     # noqa
+            result >>= rest                # noqa
+            result  ^= buffer_bits << number_of_missing_bits   # noqa
+        else:
+            excess   = result >> number_of_missing_bits  # noqa
+            result  ^= excess << number_of_missing_bits  # noqa
+            result <<= number_of_bits               # noqa
+            result  |= buffer_bits               # noqa
+        assert excess.bit_length() <= rest
+        if not peek:
+            self._number_of_bits = rest
+            self._buffer_bist = excess
+        return result
+        
+    def read_bytes(self, size: int, peek: bool = False) -> bytes:
+        if self.byte_aligned:
+            data = self.read_exactly(size, peek)
+            if not isinstance(data, bytes):
+                data = bytes(data)
+            return data
+        else:
+            return self.read_bits(size * 8, peek).tobytes()
+        
+    def read_bit(self) -> int:
+        return self.read_integer(1)
+    
+    def read_bits(self, number_of_bits: int) -> Iterable[int]:
+        chunk = self.read_integrer(number_of_bits) 
+        for k in range(number_of_bits -1, -1, -1):
+            yield chunk >> k & 1
+
+    def read_flags(self, number_of_bits: int, reverse=False) -> Iterable[bool]:
+        bits = list(self.read_bits(number_of_bits))
+        if reverse:
+            bits.reverse()
+        for bit in bits:
+            yield bool(bit)
+
+    def read_struct(self, spec: str, unwrap=False, 
+                    peek=False) -> Union[List[UnpackType], UnpackType]:
+        if not spec:
+            raise ValueError('No format specified')
+        byte_order = spec[:1]
+        if byte_order in '<!=@>':
+            spec = spec[1:]
+        else:
+            byte_order = self.byteorder_format
+        data = []
+        current_cursor = self.tell()
+
+        for k, part in enumerate(re.split('(\\d*[auwE])', spec)):
+            if k % 2 == 1:
+                count = 1 if len(part) == 1 else int(part[:~0])
+                part = part[~0]
+                for _ in range(count):
+                    if part == 'a':
+                        size = self.read_integer(8)
+                        data.append(self.read_bytes(size))
+                    elif part == 'u':
+                        data.append(self.read_integer(8))
+                    elif part == 'w':
+                        data.append(self.read_integer(16))
+                    elif part == 'E':
+                        data.append(self.read_integer(32))
+                    else:
+                        raise ValueError('Invalid format {}'.format(part))
+                continue
+            else:
+                part = F'{byte_order}{part}'
+                data.extend(struct.unpack(part, self.read_exactly(struct.calcsize(part))))
+        if unwrap and len(data) == 1:
+            return data[0]
+        if peek:
+            self.seek_set(current_cursor)
+        return data
+
+    def read_nibble(self, peek: bool = False) -> int:
+        return self.read_integer(4, peek)
+
+
+    def u8(self, peek: bool = False) -> int: 
+        return self.read_integer(8, peek)
+    def i8(self, peek: bool = False) -> int: 
+        return signed(self.read_integer(8, peek), 8)
+    def u16(self, peek: bool = False) -> int: 
+        return self.read_integer(16, peek)
+    def u32(self, peek: bool = False) -> int: 
+        return self.read_integer(32, peek)
+    def u64(self, peek: bool = False) -> int: 
+        return self.read_integer(64, peek)
+    def i16(self, peek: bool = False) -> int: 
+        return signed(self.read_integer(16, peek), 16)
+    def i32(self, peek: bool = False) -> int: 
+        return signed(self.read_integer(32, peek), 32)
+    def i64(self, peek: bool = False) -> int: 
+        return signed(self.read_integer(64, peek), 64)
+    def f32(self, peek: bool = False) -> float: 
+        return self.read_struct('f', unwrap=True, peek=peek)
+    def f64(self, peek: bool = False) -> float: 
+        return self.read_struct('d', unwrap=True, peek=peek)
+    def read_byte(self, peek: bool = False) -> int: 
+        return self.read_integer(8, peek)
+    def read_char(self, peek: bool = False) -> int:
+        return signed(self.read_integer(8, peek), 8)
+
+    def read_terminated_array(self, terminator: bytes, 
+                              alignment: int = 1) -> bytearray:
+        pos = self.tell()
+        buffer = self.get_buffer()
+        try:
+            end = pos - 1
+            while True:
+                end = buffer.find(terminator, end + 1)
+                if end < 0 or not (end - pos) % alignment:
+                    break
+        except AttributeError:
+            result = bytearray()
+            while not self.is_eof:
+                result.extend(self.read_bytes(alignment))
+                if result.endswith(terminator):
+                    return result[:-len(terminator)]
+            self.seek(pos)
+            raise EOF
+        else:
+            data = self.read_exactly(end - pos)
+            self.seek_relative(len(terminator))
+            return bytearray(data)
+    
+    def read_c_string(self, encoding=None) -> Union[str, bytearray]:
+        data = self.read_terminated_array(b'\0')
+        if encoding is not None:
+            data = data.decode(encoding)
+        return data
+    
+    def read_w_string(self, encoding=None) -> Union[str, bytearray]:
+        data = self.read_terminated_array(b'\0\0', 2)
+        if encoding is not None:
+            data = data.decode(encoding)
+        return data
+    
+    def read_length_prefixed(self, 
+                             prefix_size: int = 32, 
+                             encoding: Optional[str] = None,
+                             block_size: int = 1) -> Union[T, str]:
+        prefix = self.read_integer(prefix_size) * block_size
+        data = self.read(prefix)
+        if encoding is not None:
+            data = data.decode(encoding)
+        return data
+
+    def read_length_prefixed_ascii(self, 
+                                   prefix_size: int = 32) -> Union[T, str]:
+        return self.read_length_prefixed(prefix_size, 'ascii')
+    
+    def read_length_prefixed_utf8(self, 
+                                  prefix_size: int = 32) -> Union[T, str]:
+        return self.read_length_prefixed(prefix_size, 'utf-8')
+    
+    def read_length_prefixed_utf16(self, 
+                                   prefix_size: int = 32,
+                                   bytecount: bool = False) -> Union[T, str]:
+        block_size = 1 if bytecount else 2
+        return self.read_length_prefixed(prefix_size, 'utf-16le', block_size)
+    
+    # TODO: Review function if needed
+    def read_7bit_encoded_int(self, max_bits: int = 0) -> int:
+        result = 0
+        for k in itertools.count():
+            if k == max_bits:
+                raise ValueError('Invalid 7-bit encoded integer')
+            byte = self.read_byte()
+            result |= (byte & 0x7F) << (7 * k)
+            if not byte & 0x80:
+                break
+        return result
+
+class StructMeta(type):
+    def __new__(mcls, name, bases, nmspc, parser=StructReader):
+        return type.__new__(mcls, name, bases, nmspc)
+    
+    def __init__(cls, name, bases, nmspc, parser=StructReader):
+        super(StructMeta, cls).__init__(name, bases, nmspc)
+        original__init__ = cls.__init__
+
+        @functools.wraps(original__init__)
+        def wrapped__init__(self: Struct, reader, *args, **kwargs):
+            if not isinstance(reader, parser):
+                if issubclass(parser, reader.__class__):
+                    raise ValueError(
+                        F'A reader of type {reader.__class__.__name__} was passed to {cls.__name__}, '
+                        F'but a {parser.__name__} is required.')
+                reader = parser(reader)
+            start = reader.tell()
+            view = memoryview(reader.get_buffer())
+            original__init__(self, reader, *args, **kwargs)
+            self.__data = view[start:reader.tell()]
+
+        cls.__init__ = wrapped__init__
+
+class Struct(metaclass=StructMeta):
+
+    _data: Union[memoryview, bytearray]
+
+    def __len__(self):
+        return len(self._data)
+    
+    def __bytes__(self):
+        return bytes(self._data)   
+    
+    def get_data(self, decouple=False):
+        if decouple and isinstance(self._data, memoryview):
+            self._data = bytearray(self._data)
+        return self._data
+    
+    def __init__(self, reader: StructReader):
+        pass
+
+    
+
+
+class EOF(EOFError):
+    def __init__(self, rest: ByteString = B''):
+        super().__init__('End of File')
         self.rest = rest
```

### Comparing `debloat-1.5.6/src/debloat/utilities/rsrc.py` & `debloat-1.5.6.1/src/debloat/utilities/rsrc.py`

 * *Files identical despite different names*

### Comparing `debloat-1.5.6/src/debloat.egg-info/PKG-INFO` & `debloat-1.5.6.1/src/debloat.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-Metadata-Version: 2.1
-Name: debloat
-Version: 1.5.6
-Summary: Debloat is an tool to remove excess garbage from bloated executables.
-Author-email: Squiblydoo <Squiblydoo@pm.me>
-Project-URL: Homepage, https://github.com/Squiblydoo/debloat
-Project-URL: Bug Tracker, https://github.com/Squiblydoo/debloat/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: tkinterdnd2>=0.3.0
-Requires-Dist: pefile>=2023.2.0
-
-![debloat](https://user-images.githubusercontent.com/77356206/215351855-9f89c298-36b4-4234-89b5-dc3f26d1f8b0.png)
-
-# Debloat
-Debloat is a GUI and CLI tool to remove excess garbage from bloated executables.
-
-By excess garbage, I mean 100 - 800 MB of junk bytes added to a binary to keep it from going into a sandbox. This method of adding junk is called "inflating" or "pumping" a binary. Debloat currently handles the 10 most common inflation tactics.
-
-Being built with Python, the application can easily be leveraged in other workflows. Currently, debloat is used by [CCCS's AssemblyLine](https://www.cyber.gc.ca/en/tools-services/assemblyline) and [CERT Polska's MWDB](https://github.com/CERT-Polska/karton-archive-extractor).
-
- The program can be compiled for Windows, MacOS, Linux. The GUI and CLI have minimal options: it is intended to be as simple as possible and the logic within the program handles the different use cases automatically.
-
-Compiled binaries have already been included in the [Releases](https://github.com/Squiblydoo/debloat/releases/).
-
-The debloat can installed using `pip install debloat`. Use `debloat` to launch the CLI and `debloat-gui` to launch the GUI.
-
-For advanced users, Debloat can also be imported into other scripts and the processing functions can be called individually.
-
-## How to use the GUI?
-The GUI of Debloat intends to be as intuitive as possible.
-When launched, you can drag and drop bloated file onto the text bar and press the "Process file" button.
-Some technical information will be printed to the scrolling textbox and the file without bloat will be written to the directory the file was pulled from.
-Sound easy? It is!
-
-Processing files will take a few seconds.<br>
-![image](https://github.com/Squiblydoo/debloat/assets/77356206/3d2756cd-bc83-44e8-b223-edd8ed464369)
-
-
-## How to use the CLI?
-After installing using `pip install debloat` use the command `debloat`.<br>
-`debloat` can take two arguments. The first argument is required: the file to debloat. The second argument is optional: the output location. When no output is provided, it will be written to the same directory as the original file.
-
-The gui can also be launched from the CLI using the command `debloat-gui`.
-
-## Does it always work?
-Not yet.
-My unscientific guess is that it should work for every 9 of 10 binaries. There are specific usecases I know where it does not work and I am working to implement solutions for those usecases. 
-
-In previous versions, `debloat` could accidentally remove too much of the binary. That is no longer the case unless you use the "--last-ditch" switch. If you ever need this switch, consider sharing the sample for additional analysis. This option has now been added to the GUI. Functionally, what the function does is it will remove the whole overlay, if there is one. In some cases this is necessary as no pattern for the junk was found---this is most commonly the case in samples that do not compress well.
-
-## Use Cases (Images from [Malcat](https://malcat.fr/))
-### Full support
-- [x] Bloat appended to the end of a Signed PE.<br>
-In the image below, the bloat has been appended to the end of the executable. <br>
-![Screenshot 2023-02-11 at 3 32 36 PM](https://user-images.githubusercontent.com/77356206/218279963-00780b59-8227-47dd-a0af-41096f6ae17b.png)
-
-- [X] Signed or Unsigned Packed executable.<br>
-In the image below, the bloat has been appended to the executable after packing. <br>
-![Screenshot 2023-02-11 at 3 44 10 PM](https://user-images.githubusercontent.com/77356206/218280433-6dbcf51a-68c8-48e1-a89a-ad0b818a0afc.png)
-
-- [X] Signed executable includes bloat in the .rsrc section of the PE.<br>
-In the image below, the bloat is identified as in the .rsrc section and is removed from the PE.<br>
-![Screenshot 2023-02-11 at 3 35 21 PM](https://user-images.githubusercontent.com/77356206/218280086-7cd548f8-e16b-4290-9283-a8a848de1419.png)
-
-- [X] Cases where bloat is added inside a PE Section.<br>
-In the image below, the bloat has been included in a PE section named [0]. <br>
-![Screenshot 2023-02-11 at 3 26 52 PM](https://user-images.githubusercontent.com/77356206/218279753-ed2c9102-482a-4639-aeb1-df8efc9c4e2e.png)
-
-- [X] Cases where the executable is a Nullsoft Scriptable Installer System executable (NSIS aka Nullsoft)
-These exe are installers that may contain one or more files. The files contained may or may not be malicious. (Sometimes actors will add files simply for increasing the file size.) All files within the installer are extracted to a new directory. The directory also contains the script for the installer which can be consulted to determine which files may be malicious.
-In the image below, Malcat has identified the executable as a NSIS installer.
-![image](https://github.com/Squiblydoo/debloat/assets/77356206/86780abc-da4b-4808-bccb-733d97fa80d8)
-
-# Partial Support
-
-- [X] Cases where the junk is too random and the entropy is too high. In these cases, a switch/option called "--last-ditch" 
-
-### Other use cases
-There are use cases where the tool does not work. However, I plan to solve for them before publishing too much about them.
-
-## Why?
-There appear to be a limited number of tools to easily process bloated executables. The two tools I have seen the most are “foremost” which is intended for recovering binaries from a disk image and “pecheck”.
-
-[Foremost](https://www.kali.org/tools/foremost/) works best in instances where the junk bytes are null (0x00) and it struggles when the binary has a fake or real signature. Its use in removing bloat from files is not its original purpose.
-
-[Pecheck](https://github.com/DidierStevens/DidierStevensSuite/blob/master/pecheck.py) has been developed over 14+ years and has some confusing commandline options. The option to remove bloated content is not the primary function of the script. Pecheck has to be combined with another tool ([disitool](https://blog.didierstevens.com/programs/disitool/)) in order to handle signed executables. In my experience, there are other times where pecheck can get confused and return an executable twice the size of the original bloated executable. All these factors seem OK if you are handling a small number of binaries, but as the number of binaries and methods increase, a tool specific to removing bloat is needed.
-
-[Binary Refinery](https://github.com/binref/refinery) is an amazing tool. It was written with the intention of being a [CyberChef](https://github.com/gchq/CyberChef) of the commandline. While both tools are amazing, they both have a shortcoming that requires the user to know what formulas should be applied. 
-
-There are good solid manual methods to remove bloat from binaries, but these methods can be tedious and not all analysts have the skills to do this. This tool removes the burden of needing to know how to manually remove bloat. Additionally, it allows for better scale. The principles used in the script allow allow for better scale if automation is desired.
-
-
-## How to build? 
-Follow the build commands appropriate to your platform. The main difference between build commands is the format of the icon.
-<br>
-MacOS<br>
-`pyinstaller --onefile --noconsole --additional-hooks-dir=./hook --icon=debloat.icns gui.py`
-
-Windows<br>
-`pyinstaller --onefile  --noconsole  --additional-hooks-dir=./hook --icon=debloat.ico gui.py`
-
-Linux<br> 
-`pyinstaller --onefile --noconsole --icon=debloat.ico --collect-all tkinterdnd2 gui.py`
-
-## Want to discuss?
-Consider joining the [debloat Discord](discord.gg/dvGXKaY5qr).
-
-## Credits
-Big shoutout to Jesko Hüttenhain creator of [Binary Refinery](https://github.com/binref/refinery). The NSIS extraction is based on his reverse engineering of the NSIS file format. Check out Binary Refinery if you have not.
-
-## Where is this project going next?
-Batch processing: process all files in a directory and produce a report.
-
-Better support for using processing methods outside of debloat.
-
-Support for debloating without unzipping.
+Metadata-Version: 2.1
+Name: debloat
+Version: 1.5.6.1
+Summary: Debloat is an tool to remove excess garbage from bloated executables.
+Author-email: Squiblydoo <Squiblydoo@pm.me>
+Project-URL: Homepage, https://github.com/Squiblydoo/debloat
+Project-URL: Bug Tracker, https://github.com/Squiblydoo/debloat/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: tkinterdnd2>=0.3.0
+Requires-Dist: pefile>=2023.2.0
+
+![debloat](https://user-images.githubusercontent.com/77356206/215351855-9f89c298-36b4-4234-89b5-dc3f26d1f8b0.png)
+
+# Debloat
+Debloat is a GUI and CLI tool to remove excess garbage from bloated executables.
+
+By excess garbage, I mean 100 - 800 MB of junk bytes added to a binary to keep it from going into a sandbox. This method of adding junk is called "inflating" or "pumping" a binary. Debloat currently handles the 10 most common inflation tactics.
+
+Being built with Python, the application can easily be leveraged in other workflows. Currently, debloat is used by [CCCS's AssemblyLine](https://www.cyber.gc.ca/en/tools-services/assemblyline) and [CERT Polska's MWDB](https://github.com/CERT-Polska/karton-archive-extractor).
+
+ The program can be compiled for Windows, MacOS, Linux. The GUI and CLI have minimal options: it is intended to be as simple as possible and the logic within the program handles the different use cases automatically.
+
+Compiled binaries have already been included in the [Releases](https://github.com/Squiblydoo/debloat/releases/).
+
+The debloat can installed using `pip install debloat`. Use `debloat` to launch the CLI and `debloat-gui` to launch the GUI.
+
+For advanced users, Debloat can also be imported into other scripts and the processing functions can be called individually.
+
+## How to use the GUI?
+The GUI of Debloat intends to be as intuitive as possible.
+When launched, you can drag and drop bloated file onto the text bar and press the "Process file" button.
+Some technical information will be printed to the scrolling textbox and the file without bloat will be written to the directory the file was pulled from.
+Sound easy? It is!
+
+Processing files will take a few seconds.<br>
+![image](https://github.com/Squiblydoo/debloat/assets/77356206/3d2756cd-bc83-44e8-b223-edd8ed464369)
+
+
+## How to use the CLI?
+After installing using `pip install debloat` use the command `debloat`.<br>
+`debloat` can take two arguments. The first argument is required: the file to debloat. The second argument is optional: the output location. When no output is provided, it will be written to the same directory as the original file.
+
+The gui can also be launched from the CLI using the command `debloat-gui`.
+
+## Does it always work?
+Not yet.
+My unscientific guess is that it should work for every 9 of 10 binaries. There are specific usecases I know where it does not work and I am working to implement solutions for those usecases. 
+
+In previous versions, `debloat` could accidentally remove too much of the binary. That is no longer the case unless you use the "--last-ditch" switch. If you ever need this switch, consider sharing the sample for additional analysis. This option has now been added to the GUI. Functionally, what the function does is it will remove the whole overlay, if there is one. In some cases this is necessary as no pattern for the junk was found---this is most commonly the case in samples that do not compress well.
+
+## Use Cases (Images from [Malcat](https://malcat.fr/))
+### Full support
+- [x] Bloat appended to the end of a Signed PE.<br>
+In the image below, the bloat has been appended to the end of the executable. <br>
+![Screenshot 2023-02-11 at 3 32 36 PM](https://user-images.githubusercontent.com/77356206/218279963-00780b59-8227-47dd-a0af-41096f6ae17b.png)
+
+- [X] Signed or Unsigned Packed executable.<br>
+In the image below, the bloat has been appended to the executable after packing. <br>
+![Screenshot 2023-02-11 at 3 44 10 PM](https://user-images.githubusercontent.com/77356206/218280433-6dbcf51a-68c8-48e1-a89a-ad0b818a0afc.png)
+
+- [X] Signed executable includes bloat in the .rsrc section of the PE.<br>
+In the image below, the bloat is identified as in the .rsrc section and is removed from the PE.<br>
+![Screenshot 2023-02-11 at 3 35 21 PM](https://user-images.githubusercontent.com/77356206/218280086-7cd548f8-e16b-4290-9283-a8a848de1419.png)
+
+- [X] Cases where bloat is added inside a PE Section.<br>
+In the image below, the bloat has been included in a PE section named [0]. <br>
+![Screenshot 2023-02-11 at 3 26 52 PM](https://user-images.githubusercontent.com/77356206/218279753-ed2c9102-482a-4639-aeb1-df8efc9c4e2e.png)
+
+- [X] Cases where the executable is a Nullsoft Scriptable Installer System executable (NSIS aka Nullsoft)
+These exe are installers that may contain one or more files. The files contained may or may not be malicious. (Sometimes actors will add files simply for increasing the file size.) All files within the installer are extracted to a new directory. The directory also contains the script for the installer which can be consulted to determine which files may be malicious.
+In the image below, Malcat has identified the executable as a NSIS installer.
+![image](https://github.com/Squiblydoo/debloat/assets/77356206/86780abc-da4b-4808-bccb-733d97fa80d8)
+
+# Partial Support
+
+- [X] Cases where the junk is too random and the entropy is too high. In these cases, a switch/option called "--last-ditch" 
+
+### Other use cases
+There are use cases where the tool does not work. However, I plan to solve for them before publishing too much about them.
+
+## Why?
+There appear to be a limited number of tools to easily process bloated executables. The two tools I have seen the most are “foremost” which is intended for recovering binaries from a disk image and “pecheck”.
+
+[Foremost](https://www.kali.org/tools/foremost/) works best in instances where the junk bytes are null (0x00) and it struggles when the binary has a fake or real signature. Its use in removing bloat from files is not its original purpose.
+
+[Pecheck](https://github.com/DidierStevens/DidierStevensSuite/blob/master/pecheck.py) has been developed over 14+ years and has some confusing commandline options. The option to remove bloated content is not the primary function of the script. Pecheck has to be combined with another tool ([disitool](https://blog.didierstevens.com/programs/disitool/)) in order to handle signed executables. In my experience, there are other times where pecheck can get confused and return an executable twice the size of the original bloated executable. All these factors seem OK if you are handling a small number of binaries, but as the number of binaries and methods increase, a tool specific to removing bloat is needed.
+
+[Binary Refinery](https://github.com/binref/refinery) is an amazing tool. It was written with the intention of being a [CyberChef](https://github.com/gchq/CyberChef) of the commandline. While both tools are amazing, they both have a shortcoming that requires the user to know what formulas should be applied. 
+
+There are good solid manual methods to remove bloat from binaries, but these methods can be tedious and not all analysts have the skills to do this. This tool removes the burden of needing to know how to manually remove bloat. Additionally, it allows for better scale. The principles used in the script allow allow for better scale if automation is desired.
+
+
+## How to build? 
+Follow the build commands appropriate to your platform. The main difference between build commands is the format of the icon.
+<br>
+MacOS<br>
+`pyinstaller --onefile --noconsole --additional-hooks-dir=./hook --icon=debloat.icns gui.py`
+
+Windows<br>
+`pyinstaller --onefile  --noconsole  --additional-hooks-dir=./hook --icon=debloat.ico gui.py`
+
+Linux<br> 
+`pyinstaller --onefile --noconsole --icon=debloat.ico --collect-all tkinterdnd2 gui.py`
+
+## Want to discuss?
+Consider joining the [debloat Discord](discord.gg/dvGXKaY5qr).
+
+## Credits
+Big shoutout to Jesko Hüttenhain creator of [Binary Refinery](https://github.com/binref/refinery). The NSIS extraction is based on his reverse engineering of the NSIS file format. Check out Binary Refinery if you have not.
+
+## Where is this project going next?
+Batch processing: process all files in a directory and produce a report.
+
+Better support for using processing methods outside of debloat.
+
+Support for debloating without unzipping.
```

### Comparing `debloat-1.5.6/src/debloat.egg-info/SOURCES.txt` & `debloat-1.5.6.1/src/debloat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

