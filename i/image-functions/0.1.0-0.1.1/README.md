# Comparing `tmp/image_functions-0.1.0.tar.gz` & `tmp/image_functions-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_functions-0.1.0.tar", last modified: Thu May  9 02:27:15 2024, max compression
+gzip compressed data, was "image_functions-0.1.1.tar", last modified: Wed May 29 03:38:37 2024, max compression
```

## Comparing `image_functions-0.1.0.tar` & `image_functions-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 02:27:15.051794 image_functions-0.1.0/
--rw-rw-rw-   0        0        0     1101 2023-05-09 16:58:11.000000 image_functions-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1101 2023-05-12 12:23:49.000000 image_functions-0.1.0/LICENSE.rst
--rw-rw-rw-   0        0        0     3714 2024-05-09 02:27:15.051794 image_functions-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1757 2024-05-08 17:47:00.000000 image_functions-0.1.0/README.md
--rw-rw-rw-   0        0        0      852 2024-05-09 01:41:07.000000 image_functions-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-09 02:27:15.051794 image_functions-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-09 02:27:15.036177 image_functions-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-09 02:27:15.051794 image_functions-0.1.0/src/image_functions.egg-info/
--rw-rw-rw-   0        0        0     3714 2024-05-09 02:27:15.000000 image_functions-0.1.0/src/image_functions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2024-05-09 02:27:15.000000 image_functions-0.1.0/src/image_functions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 02:27:15.000000 image_functions-0.1.0/src/image_functions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-09 02:27:15.000000 image_functions-0.1.0/src/image_functions.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       52 2024-05-09 02:27:15.000000 image_functions-0.1.0/src/image_functions.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-09 02:27:15.000000 image_functions-0.1.0/src/image_functions.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 02:27:15.051794 image_functions-0.1.0/src/imfun/
--rw-rw-rw-   0        0        0       40 2024-05-09 01:59:42.000000 image_functions-0.1.0/src/imfun/__init__.py
--rw-rw-rw-   0        0        0   118248 2024-05-08 17:29:20.000000 image_functions-0.1.0/src/imfun/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 03:38:37.404231 image_functions-0.1.1/
+-rw-rw-rw-   0        0        0     1101 2023-05-09 16:58:11.000000 image_functions-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1101 2023-05-12 12:23:49.000000 image_functions-0.1.1/LICENSE.rst
+-rw-rw-rw-   0        0        0     6055 2024-05-29 03:38:37.404231 image_functions-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4073 2024-05-29 03:25:27.000000 image_functions-0.1.1/README.md
+-rw-rw-rw-   0        0        0      867 2024-05-29 03:23:37.000000 image_functions-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-29 03:38:37.404231 image_functions-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 03:38:37.388600 image_functions-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 03:38:37.404231 image_functions-0.1.1/src/image_functions.egg-info/
+-rw-rw-rw-   0        0        0     6055 2024-05-29 03:38:37.000000 image_functions-0.1.1/src/image_functions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2024-05-29 03:38:37.000000 image_functions-0.1.1/src/image_functions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 03:38:37.000000 image_functions-0.1.1/src/image_functions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-29 03:38:37.000000 image_functions-0.1.1/src/image_functions.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       59 2024-05-29 03:38:37.000000 image_functions-0.1.1/src/image_functions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-29 03:38:37.000000 image_functions-0.1.1/src/image_functions.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 03:38:37.404231 image_functions-0.1.1/src/imfun/
+-rw-rw-rw-   0        0        0      113 2024-05-28 21:10:33.000000 image_functions-0.1.1/src/imfun/__init__.py
+-rw-rw-rw-   0        0        0   127519 2024-05-29 03:28:44.000000 image_functions-0.1.1/src/imfun/__main__.py
```

### Comparing `image_functions-0.1.0/LICENSE` & `image_functions-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `image_functions-0.1.0/LICENSE.rst` & `image_functions-0.1.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `image_functions-0.1.0/pyproject.toml` & `image_functions-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "image-functions"
-version = "0.1.0"
+version = "0.1.1"
 description = "Image Processing Functions"
 readme = "README.md"
 authors = [{ name = "Marlon Rodrigues Garcia", email = "marlon.garcia@unesp.br" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -19,14 +19,15 @@
 keywords = ["image processing", "digital image", "image functions"]
 dependencies = [
     "numpy",
     "opencv-contrib-python",
     "matplotlib",
     "scipy",
     "pynput",
+    "pandas",
 ]
 
 requires-python = ">=3.7"
 
 [project.urls]
 Homepage = "https://github.com/MarlonGarcia/imfun"
```

### Comparing `image_functions-0.1.0/src/imfun/__main__.py` & `image_functions-0.1.1/src/imfun/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,86 +1,129 @@
 # -*- coding: utf-8 -*-
 '''
-Imaging Functions Library
+Image Functions Library
 
-This is a library to apply simple to complex functions to treat, transform and
-prepare images. This library helps to prepare image data for machine learning,
-for example, but also helps in simple functions, like image transformation,
-loading, and printing. Next are an example of functions.
-
-
-These are an example of simple functions:
-- load_color_images: function to load all color images from a folder
-- plot_color_images: function to print all color images from a folder
-- highpass_fft: high-pass frequency filter using FFT algorithm
-- highpass_gaus: high-pass frequency filter using Gaussian equation.
-- flat2im: transform an image in flattened data, e.g. to enter machine-learning
-algorithms (like Random Forest).
-- beep: make a beep sequence to signalize.
-- good_colormaps: show different colormaps to choose one to highlight features.
-
-
-Examples of more complex functions:
-- align_ECC: align images using ECC algorithm from OpenCV
-- isoareas measure and statistics pixel's intensity by depth in a preferential
-direction.
-- im2label: transform an image to a segmented image label
-- crop_multiple: crop multiple images with the same cropping area.
-- polyroi: make a polygonal ROI in an image.
-- crop_poly_multiple: make polygonal ROI and replicate the same ROI in other
-images, changing its position.
-- choose_points: choose points in an image, and retrieve its indexes.
-
-OBS: some functions use libraries pynput and windsound, which some times are
-difficult to install and do not works on non-windows platforms. Comment on
-these imports if there are problems during installation.
+Library for image pre-processing, with functions to handle and prepare images
+for machine learning and image processing. This library accounts for functions
+to: load and plot a group of images, pre-processing, choose ROI regions (may be
+polygonal), choose points, get image properties, align and transform images
+(including rotate, scale, etc.), filter signals and images (2D data), among
+others.
+
+
+OBS: some functions use the 'pynput' and 'windsound' libraries, which may be
+difficult to install and do not works on non-windows platforms. Comment these
+library imports if there are problems during installation or loading.
 
 @author: Marlon Rodrigues Garcia
-@instit.: State University of São Paulo (Unesp)
-@contact: marlonrg@gmail.com'''
+@school: School of Engineering, Campus of Sao Joao da Boa Vista
+@instit.: Sao Paulo State University (Unesp)
+@contact: marlon.garcia@unesp.br'''
 
 import numpy as np
 import cv2
 import os
 import matplotlib.pyplot as plt
 from scipy import interpolate
 from scipy import stats
-# To use a 'beep' sound, uncomment: winsound, time.
-import winsound               # it only works on windows
 import time
 import ctypes
-from pynput import keyboard   # It does not worked on colabs
 from random import shuffle
 from scipy import fftpack     # to apply FFT and iFFT
 from scipy import signal
 from scipy.fft import fft, fftfreq
 from scipy.interpolate import interp1d
+import pandas as pd
+from pynput import keyboard   # It does not worked on Google Colab
+# To use a 'beep' sound, uncomment: winsound, time.
+import winsound               # it only works on Windows
+
+
+
+def list_folders(directory):
+    '''
+    Function to list all folders inside a directory
+
+    Parameters
+    ----------
+    directory : string
+        A string with the directory. Example: 'C:/Users/User/My Drive/Data/'.
+
+    Returns
+    -------
+    folders : list
+        A list with all folders inside the directory.
+    '''
+    # First we eliminate problems of commands with "\" (e.g. "\n", "\t", etc.)
+    bytes_string = directory.encode('unicode_escape')
+    directory = bytes_string.decode('utf-8')
+    # Then we verify if the itens inside 'directory' are really folders
+    folders = []
+    for item in os.listdir(directory):
+        path = os.path.join(directory, item)
+        if os.path.isdir(path):
+            folders.append(item)
+    return folders
+
+
+
+def list_images(directory):
+    '''
+    Function to list all images inside a folder
+
+    Parameters
+    ----------
+    directory : string
+        A string with the directory. Example: 'C:/Users/User/My Drive/Data/'.
+
+    Returns
+    -------
+    folders : list
+        A list with all the images inside the folder.
+    '''
+    # First we eliminate problems of commands with "\" (e.g. "\n", "\t", etc.)
+    bytes_string = directory.encode('unicode_escape')
+    directory = bytes_string.decode('utf-8')
+    # Defining which image to consider
+    extensions = ['.jpg', '.JPG', '.jpeg','.JPEG', '.png', '.PNG', '.gif',
+                  '.GIF', '.tif', '.TIF', '.tiff', '.TIFF', '.heic', '.HEIC',
+                  '.heif', '.HEIF', '.psd', '.PSD', '.raw', '.RAW', '.bmp',
+                  '.BMP']
+    # Then we verify if the itens inside 'directory' are really images
+    image_names = []
+    for item in os.listdir(directory):
+        path = os.path.join(directory, item)
+        if os.path.isfile(path):
+            if any(item.lower().endswith(ext) for ext in extensions):
+                image_names.append(item)
+    return image_names
 
 
-def load_gray_images(folder,colormap):
+
+def load_gray_images(folder, colormap):
     """Loading grayscale images from 'folder'
     
-    This function load all the images from 'folder' in grayscale and store in
-    variable 'I'.
+    This function loads all the images from 'folder' directory, in grayscale
+    format, and store them in the variable 'I'.
     
     if colormap = -1, no colormap is assigned
     if colormap = cv2_COLORMAP_OPTION, (being option = hsv, jet, parula, etc),
     or a colormap reference number (0, 1, 2, etc), the colormap chosen option
     is assigned.
     """
     I = []
     flag1 = cv2.IMREAD_GRAYSCALE
     if colormap == -1 or colormap == None:
         for filename in os.listdir(folder):
-            img = cv2.imread(os.path.join(folder,filename), flag1)
+            img = cv2.imread(os.path.join(folder, filename), flag1)
             if img is not None:
                 I.append(img)
     else:
         for filename in os.listdir(folder):
-            img = cv2.imread(os.path.join(folder,filename), flag1)
+            img = cv2.imread(os.path.join(folder, filename), flag1)
             if img is not None:
                 img2 = cv2.applyColorMap(img, colormap)
                 I.append(img2)
     return I
 
 
 
@@ -88,22 +131,22 @@
     """Loading colorful images from 'folder'
     
     This function load all colorful images from 'folder' in variable I.
     """
     I = []
     flag1 = cv2.IMREAD_COLOR
     for filename in os.listdir(folder):
-        img = cv2.imread(os.path.join(folder,filename), flag1)
+        img = cv2.imread(os.path.join(folder, filename), flag1)
         if img is not None:
             I.append(img)
     return I
 
 
 
-def plot_gray_images(I,n):
+def plot_gray_images(I, n):
     '''Program to plot 'n' images from 'I' using 'opencv2'
     
     This program will plot 'n' images from variable the list 'I' (a list of 
     numpy arrays). Press 'ESC' for close all the windows, or another key to 
     mantain the windows.
     '''
     I1 = np.asarray(I)
@@ -116,15 +159,15 @@
         cv2.imshow(name, I1[count])
     k = cv2.waitKey(0) & 0xFF
     if k == 27:         # Waiting for 'ESC' key before close all the windows
         cv2.destroyAllWindows()
 
 
 
-def plot_color_images(I,n):
+def plot_color_images(I, n):
     '''Program to plot 'n' color images from 'I' using 'opencv2'
     
     This program will plot 'n' color images from variable the list 'I' (a list
     of numpy arrays). Press 'ESC' for close all the windows, or another key to
     mantain the windows.
     '''
     I1 = np.asarray(I)
@@ -193,15 +236,15 @@
     freq = kwargs.get('freq')
     duration = kwargs.get('duration')
     if freq is None:
         freq = 2500  # Set Frequency To 2500 Hertz
     if duration is None:
         duration = 300  # Set Duration To 300 ms == 0.3 second
     numb = 5 # number of beeps
-    for n in range(0,numb):
+    for n in range(0, numb):
         time.sleep(0.0005)
         winsound.Beep(freq, duration)
 
 
 
 def rotate2D(pts, cnt, ang):
     '''Rotating the points about a center 'cnt' by an ang 'ang' in radians.
@@ -1924,15 +1967,15 @@
     return scale255(final)
 
 
 
 def filt_hist(hist):
     '''
     Functino to 'filter' equalized histogram, removing the zeros values 
-    between positive ones (util to process equalized historgrams).
+    between positive ones (usefull to process equalized historgrams).
     
     output = filt_hist(hist)
     
     input:
     hist (np.array): input histogram to be 'filtered' (removed the zero values)
     
     output:
@@ -1998,14 +2041,192 @@
     # Standar deviation from pixels in ROI:
     props[2] = Itemp[Itemp!=0].std()
     
     return props, Imask
 
 
 
+def roi_stats(images_dir, save_dir, experiments, colors, **kwargs):
+    ''' Easely calculate statistics of images in a given region of the images
+    
+    This function uses a interactive graphical user interface (GUI) to calcula-
+    te the statistics of multiple images, in a given region of interest (ROI)
+    inside the image. To use this function, your images have to be in a folder
+    tree like bellow. The outer folder will be 'Images Folder', that has to be
+    passed to this function in the 'images_dir' variable. Inside this folder
+    you can add as many parts of your experiment you want to (in this case
+    exemplified as animals). Inside each part (or animal) of your experiments,
+    it have to be folders corresponding to the exact experiments conducted (for
+    example different times, or differents treatments types or measurements).
+    After the processing, a '.csv' data file is saved in the folder/directory
+    specified in the variable 'save_dir'.
+    
+    Images Folder
+        |
+        |
+        |--- Animal 1
+        |       |
+        |       |--- Experiment 1
+        |       |
+        |       |--- Experiment 2
+        |       |
+        |       |--- Experiment 3
+        |
+        |
+        |--- Animal 2
+                |
+                |--- Experiment 1
+                |
+                |--- Experiment 2
+                |
+                |--- Experiment 3
+    
+    Parameters
+    ----------
+    images_dir : string
+        Root directory (outer folder) of your images. E.g. 'C:/Users/User/data'
+    save_dir : string
+        Directory to save the images.
+    experiments : list
+        Names of the experiments. Note that it has to mach the experiment names
+        e.g. ['Experiment 1', 'Experiment 2', 'Experiment 3'] in the example.
+    colors : list
+        Name of the colors (or channels) to be analized in the image, or a list
+        with the string 'gray' for grayscale images. E.g.: ['gray'] or ['red'],
+        or even all the colors ['red', 'green', 'blue']
+    
+    **kwargs (arguments that may or may not be passed to the function)
+    ----------
+        stats : list
+            A list with the statistics to be calculated. Only mean and standard
+            deviation are suported until now. E.g. ['mean'] or ['mean', 'std']
+        colormap : int
+            The colormap to use while choosing the region of interest
+            examples: cv2.COLORMAP_PINK, cv2.COLORMAP_HSV, cv2.COLORMAP_PARULA.
+    '''
+    colormap = kwargs.get('colormap', cv2.COLORMAP_PINK)
+    stats = kwargs.get('stats', ['mean', 'std'])
+    
+    if not colors or not experiments:
+        raise ValueError('\n\n- You did not choose the colors or the experiments correctly')
+
+    # Entering into the folder of images
+    folders = list_folders(images_dir)
+    
+    # Initiating the variable with the data to be saved
+    dados = {'Experiment':[]}
+    
+    # Adding all the names of experiments to be saved on 'dados'
+    for exp in experiments:
+        for color in colors:
+            for stat in stats:
+                dados[exp+' - '+stat+' '+color] = []
+    
+    # Defining the question to be asked to the user
+    question = 'OK: to continue\n\nCancel: for redo'
+    
+    
+    # Iterating between the folders with images
+    for folder in folders:
+        # Adding the experiment's name in the data to be saved
+        dados['Experiment'].append(folder)
+        # Reading all experiment names inside 'folders'
+        path = os.path.join(images_dir, folder)
+        times = list_folders(path)
+        # Iteratinf through all the experiments
+        for exp in experiments:
+            if exp in times:
+                # Reading the name of the first image inside the experiment folder
+                path = os.path.join(images_dir, folder, exp)
+                name = list_images(path)[0]
+                path = os.path.join(path, name)
+                # Reading image
+                if 'gray' in colors:
+                    Itemp = cv2.imread(path, cv2.IMREAD_GRAYSCALE)
+                else:
+                    Itemp = cv2.imread(path, cv2.IMREAD_COLOR)
+                    # Trying to change the image colors, if it is not, the image
+                    # was probably not recognized correctly, so raise an error
+                    try:
+                        Itemp = cv2.cvtColor(Itemp, cv2.COLOR_BGR2RGB)
+                    except:
+                        raise ValueError(f'\n\n- Error when opening image from {folder}, for the experiment: {exp}')
+                asw = 2
+                while asw != 1:
+                    # With the next command the user can circulate the lesion
+                    [Imask, temp] = polyroi(Itemp, cmap = colormap,
+                                                  window_name = f'Select the region of interest for {folder} / {exp}')
+                    # Then the box dialog pop up itself:
+                    asw = ctypes.windll.user32.MessageBoxW(0,question,'Question', 1)
+                # Calculating the measure defined in 'stast'
+                
+                if 'gray' in colors:
+                    if 'mean' in stats:
+                        dados[f'{exp} - mean gray'].append(np.mean(Itemp[Imask>0]))
+                    if 'std' in stats:
+                        dados[f'{exp} - std gray'].append(np.std(Itemp[Imask>0]))
+                else:
+                    if 'red' in colors:
+                        if 'mean' in stats:
+                            dados[f'{exp} - mean red'].append(np.mean(Itemp[:,:,0][Imask[:,:,0]>0]))
+                        if 'std' in stats:
+                            dados[f'{exp} - std red'].append(np.std(Itemp[:,:,0][Imask[:,:,0]>0]))
+                    if 'green' in colors:
+                        if 'mean' in stats:
+                            dados[f'{exp} - mean green'].append(np.mean(Itemp[:,:,1][Imask[:,:,1]>0]))
+                        if 'std' in stats:
+                            dados[f'{exp} - std green'].append(np.std(Itemp[:,:,1][Imask[:,:,1]>0]))
+                    if 'blue' in colors:
+                        if 'mean' in stats:
+                            dados[f'{exp} - mean blue'].append(np.mean(Itemp[:,:,2][Imask[:,:,2]>0]))
+                        if 'std' in stats:
+                            dados[f'{exp} - std blue'].append(np.std(Itemp[:,:,2][Imask[:,:,2]>0]))
+            
+            # If does not find the data, add zero to the data to be saved
+            else:
+                if 'gray' in colors:
+                    if 'mean' in stats:
+                        dados[f'{exp} - mean gray'].append(int(0))
+                    if 'std' in stats:
+                        dados[f'{exp} - std gray'].append(int(0))
+                else:
+                    if 'red' in colors:
+                        if 'mean' in stats:
+                            dados[f'{exp} - mean red'].append(int(0))
+                        if 'std' in stats:
+                            dados[f'{exp} - std red'].append(int(0))
+                    if 'green' in colors:
+                        if 'mean' in stats:
+                            dados[f'{exp} - mean green'].append(int(0))
+                        if 'std' in stats:
+                            dados[f'{exp} - std green'].append(int(0))
+                    if 'blue' in colors:
+                        if 'mean' in stats:
+                            dados[f'{exp} - mean blue'].append(int(0))
+                        if 'std' in stats:
+                            dados[f'{exp} - std blue'].append(int(0))
+    
+    ## Saving the data
+    columns = ['Experiment']
+    for exp in experiments:
+        for color in colors:
+            for stat in stats:
+                columns.append(f'{exp} - {stat} {color}')
+    
+    # Go to the directory where the data will be saved
+    os.chdir(save_dir)
+    
+    # Monting the data to be saved on a DataFrame
+    df = pd.DataFrame(dados, columns = columns)
+    
+    # Actually saving the data
+    df.to_csv('dados.csv', index = False)
+
+
+
 def imchoose(images, cmap):
     '''Function to chose images of given image set.
     
     chosen = imchoose(images, cmap)
     
     images: input images (a'list' or a 'numpy.ndarray' variable). The I shape
             has to be: 'np.shape(I)=(n, heigh, width)', with 'n' being the
@@ -2088,15 +2309,15 @@
         except: pass
     plt.close(fig)
     return np.array(chosen,np.int)
 
 
 
 def align_features(I1, I2, draw):
-    ''' Align images with Feature Based algorithm, from OpenCV
+    ''' Align images with Feature-Based algorithm, from OpenCV
     
     [Ir, warp] = align_features(I1, I2, draw)
     
     Parameters
     ----------
     I1 : numerical-array (grayscale)
         Image to be aligned (array).
@@ -2724,8 +2945,7 @@
     plt.subplot(236).set_title('BrBG')
     plt.imshow(image, cmap = "BrBG")
     plt.xticks([]), plt.yticks([])
     plt.xticks([]), plt.yticks([])
     plt.tight_layout()
     plt.subplots_adjust(top=0.92, bottom=0.08, left=0.10, right=0.95,
                         hspace=0.15, wspace=0.15)
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

