# Comparing `tmp/CTG_Utils-1.2.1.tar.gz` & `tmp/CTG_Utils-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTG_Utils-1.2.1.tar", last modified: Sat May 25 08:14:12 2024, max compression
+gzip compressed data, was "CTG_Utils-1.2.2.tar", last modified: Wed May 29 14:00:34 2024, max compression
```

## Comparing `CTG_Utils-1.2.1.tar` & `CTG_Utils-1.2.2.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 08:14:12.644664 CTG_Utils-1.2.1/
-drwxrwxrwx   0        0        0        0 2024-05-25 08:14:12.571807 CTG_Utils-1.2.1/CTG_Utils/
-drwxrwxrwx   0        0        0        0 2024-05-25 08:14:12.595795 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/
--rw-rw-rw-   0        0        0     9766 2024-05-17 09:17:02.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTGClasses.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:14:12.612749 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/
--rw-rw-rw-   0        0        0       41 2024-04-03 06:31:10.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/CTG.yaml
--rw-rw-rw-   0        0        0      605 2023-09-01 12:09:43.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml
--rw-rw-rw-   0        0        0      194 2024-05-15 10:03:47.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/help.txt
--rw-rw-rw-   0        0        0     1920 2024-05-15 10:17:54.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/help_config.txt
--rw-rw-rw-   0        0        0   228969 2024-05-05 16:57:27.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico
--rw-rw-rw-   0        0        0    34827 2024-05-05 14:03:57.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png
--rw-rw-rw-   0        0        0    26973 2024-05-06 17:53:49.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG
--rw-rw-rw-   0        0        0   100526 2024-05-06 17:57:15.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico
--rw-rw-rw-   0        0        0     1576 2024-05-10 18:06:52.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml
--rw-rw-rw-   0        0        0      574 2024-04-15 12:33:24.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml
--rw-rw-rw-   0        0        0  9545867 2024-04-03 11:27:38.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv
--rw-rw-rw-   0        0        0      488 2024-05-09 07:18:30.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_config.py
--rw-rw-rw-   0        0        0    18737 2024-05-20 06:33:57.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_effectif.py
--rw-rw-rw-   0        0        0    11562 2024-05-17 09:25:57.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_plot.py
--rw-rw-rw-   0        0        0    15836 2024-05-20 06:57:30.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_synthese.py
--rw-rw-rw-   0        0        0     4661 2024-05-20 06:33:57.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_utility.py
--rw-rw-rw-   0        0        0      214 2024-05-15 06:16:14.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_Func/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:14:12.641673 CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/
--rw-rw-rw-   0        0        0    16076 2024-05-20 07:00:54.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/GUI_Globals.py
--rw-rw-rw-   0        0        0    10886 2024-05-10 12:46:38.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/PageDivers.py
--rw-rw-rw-   0        0        0    11530 2024-05-07 13:39:45.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/PageEffectif.py
--rw-rw-rw-   0        0        0    11820 2024-05-20 06:52:52.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/PageSorties.py
--rw-rw-rw-   0        0        0    10763 2024-05-09 13:49:41.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/PageSynthese.py
--rw-rw-rw-   0        0        0    10944 2024-05-13 07:34:59.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/PageTendance.py
--rw-rw-rw-   0        0        0    32252 2024-05-15 06:32:08.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/Page_Classes.py
--rw-rw-rw-   0        0        0    13687 2024-04-26 08:07:42.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/Useful_Classes.py
--rw-rw-rw-   0        0        0    11454 2024-05-12 12:03:55.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/Useful_Functions.py
--rw-rw-rw-   0        0        0      221 2024-05-15 06:17:11.000000 CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:14:12.586819 CTG_Utils-1.2.1/CTG_Utils.egg-info/
--rw-rw-rw-   0        0        0      670 2024-05-25 08:14:11.000000 CTG_Utils-1.2.1/CTG_Utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1331 2024-05-25 08:14:11.000000 CTG_Utils-1.2.1/CTG_Utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 08:14:11.000000 CTG_Utils-1.2.1/CTG_Utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2024-05-25 08:14:11.000000 CTG_Utils-1.2.1/CTG_Utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       37 2024-05-25 08:14:11.000000 CTG_Utils-1.2.1/CTG_Utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2022-03-26 14:35:29.000000 CTG_Utils-1.2.1/LICENSE
--rw-rw-rw-   0        0        0       90 2024-05-18 08:06:39.000000 CTG_Utils-1.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0      670 2024-05-25 08:14:12.643667 CTG_Utils-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-05-18 08:07:37.000000 CTG_Utils-1.2.1/README.md
--rwxrwxrwx   0        0        0     1031 2024-05-20 08:04:44.000000 CTG_Utils-1.2.1/make_exe.bat
--rwxrwxrwx   0        0        0      107 2024-05-20 07:59:16.000000 CTG_Utils-1.2.1/make_venv.bat
--rw-rw-rw-   0        0        0       42 2024-05-25 08:14:12.644664 CTG_Utils-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1367 2024-05-25 08:07:10.000000 CTG_Utils-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:00:34.257589 CTG_Utils-1.2.2/
+drwxrwxrwx   0        0        0        0 2024-05-29 14:00:34.211421 CTG_Utils-1.2.2/CTG_Utils.egg-info/
+-rw-rw-rw-   0        0        0      670 2024-05-29 14:00:34.000000 CTG_Utils-1.2.2/CTG_Utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1280 2024-05-29 14:00:34.000000 CTG_Utils-1.2.2/CTG_Utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 14:00:34.000000 CTG_Utils-1.2.2/CTG_Utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2024-05-29 14:00:34.000000 CTG_Utils-1.2.2/CTG_Utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       35 2024-05-29 14:00:34.000000 CTG_Utils-1.2.2/CTG_Utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2022-03-26 14:35:29.000000 CTG_Utils-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0       71 2024-05-29 13:37:31.000000 CTG_Utils-1.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      670 2024-05-29 14:00:34.256588 CTG_Utils-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-05-18 08:07:37.000000 CTG_Utils-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 14:00:34.196169 CTG_Utils-1.2.2/ctgutils/
+drwxrwxrwx   0        0        0        0 2024-05-29 14:00:34.220111 CTG_Utils-1.2.2/ctgutils/ctgFuncts/
+drwxrwxrwx   0        0        0        0 2024-05-29 14:00:34.234074 CTG_Utils-1.2.2/ctgutils/ctgFuncts/CTG_RefFiles/
+-rw-rw-rw-   0        0        0       41 2024-04-03 06:31:10.000000 CTG_Utils-1.2.2/ctgutils/ctgFuncts/CTG_RefFiles/CTG.yaml
+-rw-rw-rw-   0        0        0      605 2023-09-01 12:09:43.000000 CTG_Utils-1.2.2/ctgutils/ctgFuncts/CTG_RefFiles/CTG_correction.yaml
+-rw-rw-rw-   0        0        0      194 2024-05-15 10:03:47.000000 CTG_Utils-1.2.2/ctgutils/ctgFuncts/CTG_RefFiles/help.txt
+-rw-rw-rw-   0        0        0     1920 2024-05-15 10:17:54.000000 CTG_Utils-1.2.2/ctgutils/ctgFuncts/CTG_RefFiles/help_config.txt
+-rw-rw-rw-   0        0        0   228969 2024-05-05 16:57:27.000000 CTG_Utils-1.2.2/ctgutils/ctgFuncts/CTG_RefFiles/logo_ffvelo.ico
+-rw-rw-rw-   0        0        0    26973 2024-05-06 17:53:49.000000 CTG_Utils-1.2.2/ctgutils/ctgFuncts/CTG_RefFiles/logoctg4.PNG
+-rw-rw-rw-   0        0        0   100526 2024-05-06 17:57:15.000000 CTG_Utils-1.2.2/ctgutils/ctgFuncts/CTG_RefFiles/logoctg4.ico
+-rw-rw-rw-   0        0        0     1576 2024-05-10 18:06:52.000000 CTG_Utils-1.2.2/ctgutils/ctgFuncts/CTG_RefFiles/memory_sorties.yml
+-rw-rw-rw-   0        0        0      574 2024-04-15 12:33:24.000000 CTG_Utils-1.2.2/ctgutils/ctgFuncts/CTG_RefFiles/memory_sorties_old.yml
+-rw-rw-rw-   0        0        0  9545867 2024-04-03 11:27:38.000000 CTG_Utils-1.2.2/ctgutils/ctgFuncts/CTG_RefFiles/villes_france_premium.csv
+-rw-rw-rw-   0        0        0      297 2024-05-29 13:31:30.000000 CTG_Utils-1.2.2/ctgutils/ctgFuncts/__init__.py
+-rw-rw-rw-   0        0        0     2141 2024-05-29 09:12:30.000000 CTG_Utils-1.2.2/ctgutils/ctgFuncts/club38.py
+-rw-rw-rw-   0        0        0     9375 2024-05-29 13:27:01.000000 CTG_Utils-1.2.2/ctgutils/ctgFuncts/ctg_classes.py
+-rw-rw-rw-   0        0        0    17250 2024-05-29 13:27:01.000000 CTG_Utils-1.2.2/ctgutils/ctgFuncts/ctg_effectif.py
+-rw-rw-rw-   0        0        0     7231 2024-05-29 13:27:01.000000 CTG_Utils-1.2.2/ctgutils/ctgFuncts/ctg_plot.py
+-rw-rw-rw-   0        0        0    14501 2024-05-29 13:27:01.000000 CTG_Utils-1.2.2/ctgutils/ctgFuncts/ctg_synthese.py
+-rw-rw-rw-   0        0        0     5947 2024-05-29 09:12:30.000000 CTG_Utils-1.2.2/ctgutils/ctgFuncts/ctg_tools.py
+-rw-rw-rw-   0        0        0     4861 2024-05-29 09:12:30.000000 CTG_Utils-1.2.2/ctgutils/ctgFuncts/ctg_utils.py
+-rw-rw-rw-   0        0        0    10267 2024-05-29 13:18:52.000000 CTG_Utils-1.2.2/ctgutils/ctgFuncts/pagesynthese.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:00:34.255591 CTG_Utils-1.2.2/ctgutils/ctggui/
+-rw-rw-rw-   0        0        0      431 2024-05-29 13:21:13.000000 CTG_Utils-1.2.2/ctgutils/ctggui/__init__.py
+-rw-rw-rw-   0        0        0    15953 2024-05-29 10:42:46.000000 CTG_Utils-1.2.2/ctgutils/ctggui/guiglobals.py
+-rw-rw-rw-   0        0        0    10891 2024-05-29 13:21:13.000000 CTG_Utils-1.2.2/ctgutils/ctggui/page_effectif.py
+-rw-rw-rw-   0        0        0    27828 2024-05-29 13:21:13.000000 CTG_Utils-1.2.2/ctgutils/ctggui/pageclasses.py
+-rw-rw-rw-   0        0        0    10330 2024-05-29 13:21:13.000000 CTG_Utils-1.2.2/ctgutils/ctggui/pagedivers.py
+-rw-rw-rw-   0        0        0    11080 2024-05-29 13:21:13.000000 CTG_Utils-1.2.2/ctgutils/ctggui/pagesorties.py
+-rw-rw-rw-   0        0        0    10267 2024-05-29 13:21:13.000000 CTG_Utils-1.2.2/ctgutils/ctggui/pagesynthese.py
+-rw-rw-rw-   0        0        0    10369 2024-05-29 13:21:13.000000 CTG_Utils-1.2.2/ctgutils/ctggui/pagetendance.py
+-rw-rw-rw-   0        0        0    10594 2024-05-29 13:21:13.000000 CTG_Utils-1.2.2/ctgutils/ctggui/useful_functions.py
+-rwxrwxrwx   0        0        0     2709 2024-05-29 13:39:26.000000 CTG_Utils-1.2.2/make_ctg_exe.bat
+-rw-rw-rw-   0        0        0       42 2024-05-29 14:00:34.257589 CTG_Utils-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1365 2024-05-29 13:59:35.000000 CTG_Utils-1.2.2/setup.py
```

### Comparing `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTGClasses.py` & `CTG_Utils-1.2.2/ctgutils/ctgFuncts/ctg_classes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+# Standard library imports
+import os
+from pathlib import Path
+from math import asin, cos, radians, sin, sqrt
+from tkinter import messagebox
+
+# Third party imports
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
+
+# Internal imports
+from ctgutils.ctgfuncts.ctg_tools import built_lat_long  
 
 class EffectifCtg():
     
     
     def __init__(self,year,ctg_path):
         
-        # Standard library imports
-        from pathlib import Path
-
-        # Third party imports
-        import pandas as pd
-
-        # Internal imports
-        from CTG_Utils.CTG_Func.CTG_plot import built_lat_long
-
         self.year = year
         self.ctg_path = ctg_path
         df = pd.read_excel(self.ctg_path / Path(str(year))/ Path('DATA')/Path(str(year)+'.xlsx'))
         
         year_1 = int(year)-1
         df_1 = pd.read_excel(self.ctg_path / Path(str(year_1))/ Path('DATA')/Path(str(year_1)+'.xlsx'))
 
@@ -38,34 +42,24 @@
         
         self.cotisation_licence,self.cotisation_totale, self.cotisation_ctg = self.cotisation()
         
         self.membres_sympathisants, self.nbr_membres_sympathisants = self.membres_sympathisants()
         
     @staticmethod
     def distance_(row,dh):
-    
-        # Standard library imports
-        from math import asin, cos, radians, sin, sqrt
-        
-        # Third party imports        
-        import numpy as np
         
         phi1, lon1 = dh.query("Ville=='GRENOBLE'")[['long','lat']].values.flatten()
         phi1, lon1 = radians(phi1), radians(lon1)
         phi2, lon2 = radians(row['long']), radians(row['lat'])
         rad = 6371
         dist = 2 * rad * asin(sqrt(sin((phi2 - phi1) / 2) ** 2
                                  + cos(phi1) * cos(phi2) * sin((lon2 - lon1) / 2) ** 2))
         return np.round(dist,1)
     
     def stat(self):
-    
-        # Standard library imports
-        from pathlib import Path
-        from tkinter import messagebox
 
         da = self.effectif.groupby('Sexe')['Age'].agg(['count','median','max','min'])
         res = self.effectif['Age'].agg(['count','median','max','min']).tolist()
         stat = []
         stat.append(f"Année : {self.year}")
         stat.append(" ")
         nbr_membres = round(res[0],0)
@@ -141,19 +135,15 @@
             nouveaux_licenciés_list.append(f"{row['Prénom'][0]}. {row['Nom']}")
         nouveaux_licenciés_noms = '; '.join(nouveaux_licenciés_list)
         nbr_nouveaux_licencié = len(dg)
 
         return moy_age_entrants, nbr_nouveaux_licencié, nouveaux_licenciés_noms
         
     def membres_sympathisants(self):
-    
-        import os
-        from pathlib import Path
-        import pandas as pd 
-        
+           
         file_path = self.ctg_path / Path(str(self.year))/Path('DATA')/ Path('membres_sympatisants.xlsx')
         if os.path.isfile(file_path):
             membres_sympathisants_df = pd.read_excel(file_path)
             membres_sympathisants_df['Nom_Prenom'] = membres_sympathisants_df['Nom']+" "+membres_sympathisants_df['Prénom'].str[0]
             membres_sympathisants = ', '.join(membres_sympathisants_df['Nom_Prenom'].tolist())
             nbr_membres_sympathisants = len(membres_sympathisants_df)
         else:
@@ -188,18 +178,14 @@
         
         cotisation_ctg = 15*len(self.effectif)
         return cotisation_licence,cotisation_totale, cotisation_ctg
         
  
     def plot_histo(self):
     
-        # Third party imports
-        import matplotlib.pyplot as plt
-        import pandas as pd
-        
         fig, ax = plt.subplots(figsize=(10,10))
         self.effectif['age group'] = pd.cut(self.effectif.Age, bins=range(0, 95, 5), right=False)
         result_hist = self.effectif.groupby('Sexe')['age group'].value_counts().unstack().T.plot.bar(width=1, stacked=False,ax=ax)
         
         plt.tick_params(axis='x', labelsize=20)
         plt.tick_params(axis='y', labelsize=20)
         plt.title(self.year,fontsize=20)
```

### Comparing `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml` & `CTG_Utils-1.2.2/ctgutils/ctgFuncts/CTG_RefFiles/CTG_correction.yaml`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/help_config.txt` & `CTG_Utils-1.2.2/ctgutils/ctgFuncts/CTG_RefFiles/help_config.txt`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico` & `CTG_Utils-1.2.2/ctgutils/ctgFuncts/CTG_RefFiles/logo_ffvelo.ico`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG` & `CTG_Utils-1.2.2/ctgutils/ctgFuncts/CTG_RefFiles/logoctg4.PNG`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico` & `CTG_Utils-1.2.2/ctgutils/ctgFuncts/CTG_RefFiles/logoctg4.ico`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml` & `CTG_Utils-1.2.2/ctgutils/ctgFuncts/CTG_RefFiles/memory_sorties.yml`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml` & `CTG_Utils-1.2.2/ctgutils/ctgFuncts/CTG_RefFiles/memory_sorties_old.yml`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv` & `CTG_Utils-1.2.2/ctgutils/ctgFuncts/CTG_RefFiles/villes_france_premium.csv`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_effectif.py` & `CTG_Utils-1.2.2/ctgutils/ctgFuncts/ctg_effectif.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,76 +1,80 @@
-__all__ = ['count_participation',
+__all__ = ['anciennete_au_club',
+           'builds_excel_presence_au_club',
+           'count_participation',
+           'evolution_effectif',
            'inscrit_sejour',
            'parse_date',
            'read_effectif',
            'read_effectif_corrected',
-           'evolution_effectif',
-           'builds_excel_presence_au_club',
            'statistique_vae',
-           'anciennete_au_club',]
-                      
+           ]
+
+# Standard library imports
+import datetime
+import functools
+import os
+import re
+import unicodedata
+from collections import Counter
+from math import asin, cos, radians, sin, sqrt
+from pathlib import Path
+
+# 3rd party imports
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
+
+# Internal imports
+from ctgutils.ctgfuncts.ctg_tools import built_lat_long
 
 def read_effectif_corrected(ctg_path, year=None):
-    
+
     '''Lecture du fichier effectif et correction
     '''
-    # Standard library imports
-    from pathlib import Path
-    import datetime
-   
-    # 3rd party imports
-    import pandas as pd
-    
+
+
     if year is not None:
         file_effectif = str(year) + '.xlsx'
     else:
         currentDateTime = datetime.datetime.now()
         date = currentDateTime.date()
         year = date.strftime("%Y")
         file_effectif = year + '.xlsx'
-        
+
     effectif_df = pd.read_excel(ctg_path / Path(str(year))/Path('DATA')/ Path(file_effectif))
     effectif_df = effectif_df[['N° Licencié', 'Nom','Prénom','Sexe','Pratique VAE']]
-    
+
     correction_effectif = pd.read_excel(ctg_path / Path(str(year))/Path('DATA')/ Path('correction_effectif.xlsx'))
     correction_effectif.index = correction_effectif['N° Licencié']
     membres_sympathisants_df = pd.read_excel(ctg_path / Path(str(year))/Path('DATA')/ Path('membres_sympatisants.xlsx'))
     membres_sympathisants_df = membres_sympathisants_df[['N° Licencié', 'Nom','Prénom','Sexe','Pratique VAE']]
-    
+
     for num_licence in correction_effectif.index:
         idx = effectif_df[effectif_df["N° Licencié"]==num_licence].index
         effectif_df.loc[idx,'Prénom'] = correction_effectif.loc[num_licence,'Prénom']
         effectif_df.loc[idx,'Nom'] = correction_effectif.loc[num_licence,'Nom']
-    
+
     effectif_df = pd.concat([effectif_df, membres_sympathisants_df], ignore_index=True, axis=0)
     effectif_df['Prénom1'] = effectif_df['Prénom'].str[0]
     effectif_df['Prénom'] = effectif_df['Prénom'].str.replace(' ','-')
-    
+
     return effectif_df
 
 def inscrit_sejour(file,no_match,df_effectif):
 
-    # Standard library import
-    import functools
-    import os
-    import unicodedata
-    
-    # 3rd party import
-    import pandas as pd
-
-
     nfc = functools.partial(unicodedata.normalize,'NFD')
     convert_to_ascii = lambda text : nfc(text). \
                                      encode('ascii', 'ignore'). \
                                      decode('utf-8').\
                                      strip()
-                                     
-    df = pd.read_csv(file) 
+
+    df = pd.read_csv(file)
     sejour = os.path.splitext(os.path.basename(file))[0]
-    
+
     if len(df) != 0:
         dg = df['Unnamed: 0'].str.upper()
         dg = dg.dropna()
         dg = dg.str.replace(' \t?','',regex=False)
         dg = dg.str.replace('.',' ',regex=False)
         dg = dg.str.replace(' - ','-',regex=False)
         dg = dg.apply(convert_to_ascii)
@@ -105,261 +109,227 @@
                          dic[idx] =dr.iloc[0].tolist()[:-1]+[sejour]
                     else:
                         print(f'{sejour} : no match, prénom/prénom:{row.name2}, nom/prénom: {row.name1}')
                         no_match.append((file,row.name2,row.name1))
             else:
                 print(f'WARNING: incorrect name {row.name1}, {row.name2}, {row.name3} in sejour {sejour}')
 
-        dg = pd.DataFrame.from_dict(dic).T 
+        dg = pd.DataFrame.from_dict(dic).T
         if len(dg) !=0:
             dg.columns = ['N° Licencié','Nom','Prénom','Sexe','Pratique VAE','sejour',]
         else:
             dg = pd.DataFrame([[None,None,None,None,sejour,]], columns=['N° Licencié','Nom','Prénom','Sexe','sejour',])
     else:
         dg = pd.DataFrame([[None,None,None,None,sejour,]], columns=['N° Licencié','Nom','Prénom','Sexe','sejour',])
-    
+
     return dg
 
-    
+
 def count_participation(path,ctg_path,year,info_rando):
-    
-    # Standard library imports
-    import os
-    import re
-    from pathlib import Path
-    
-    # Third party imports
-    import pandas as pd
-    
+
     flag_sejour = False
-    if os.path.split(path)[-1] == 'SEJOUR' : 
+    if os.path.split(path)[-1] == 'SEJOUR' :
         flag_sejour = True
 
     type_sortie_default = os.path.basename(path)
     type_sortie_default = type_sortie_default.split('.', 1)[0]
 
     df_effectif = read_effectif_corrected(ctg_path,year)
 
     no_match = []
-    df_list = [] 
+    df_list = []
     info_sejours = []
     sejours = [x for x in os.listdir( path / Path('CSV')) if x.endswith('.csv')]
-    
+
     sejours_xlsx = [x for x in os.listdir( path / Path('EXCEL')) if x.endswith('.xlsx')]
     for sejours_xlsx in sejours_xlsx:
         path_file_xlsx = path / Path('EXCEL') / Path(sejours_xlsx)
         os.remove(path_file_xlsx)
-        
+
     nbr_moyen_participants = 0
     counter = 1
     for sejour in sejours:
         dg = inscrit_sejour( path / Path('CSV') /Path(sejour),no_match,df_effectif)
-        
+
         if re.findall(r'^\d{4}[-_]',sejour):
             date = sejour[2:10].replace('_','-')
         else:
             date = str(year)[2:4] + '-' +sejour[0:5].replace('_','-')
-            
-        dg['nbr_jours'] = 0    
+
+        dg['nbr_jours'] = 0
         if date in info_rando['date'].tolist():
             dh = info_rando.query('type=="randonnee" and date==@date')
-            if not flag_sejour and len(dh) != 0 : 
+            if not flag_sejour and len(dh) != 0 :
                 dg['Type'] = "RANDONNEE"
             else:
                 dg['Type'] = type_sortie_default
-            
+
             dg['nbr_jours'] = 1
             dh = info_rando.query('type=="sejour" and date==@date')
             if flag_sejour and len(dh) != 0:
-                dg['nbr_jours'] = dh['nbr_jours'].tolist()[0]    
-            
+                dg['nbr_jours'] = dh['nbr_jours'].tolist()[0]
+
         if dg.reset_index().loc[0,'Nom'] is not None:
             nbr_inscrits = len(dg)
             if nbr_inscrits != 0:
                 nbr_moyen_participants = nbr_moyen_participants + (nbr_inscrits - nbr_moyen_participants)/counter
                 counter += 1
-                info_sejours.append(f"{os.path.split(path)[-1]} :{sejour}, Nombre d'inscrits : {nbr_inscrits}")   
-        
+                info_sejours.append(f"{os.path.split(path)[-1]} :{sejour}, Nombre d'inscrits : {nbr_inscrits}")
+
         df_list.append(dg)
         file_store = os.path.splitext(sejour)[0]+'.xlsx'
         dg.to_excel(path / Path('EXCEL') / Path(file_store))
-       
+
     info_sejours.append(f"Nombre d'évènenements : {counter-1}. Nombre moyen de participants : {nbr_moyen_participants}")
     info_sejours = '\n'.join(info_sejours)
     info_sejours_path = ctg_path / Path(str(year)) / Path('STATISTIQUES')/ Path(type_sortie_default+'.txt')
     with open(info_sejours_path,'w') as f:
         f.write(info_sejours)
-        
-    nbr_evenement = counter-1 
+
+    nbr_evenement = counter-1
     if counter-1 > 0 :  #
         df_total = pd.concat(df_list,ignore_index=True)
     else:
         return (None, None, None)
 
 
     liste_licence = df_effectif['N° Licencié']
     liste_licence_sejour = df_total['N° Licencié']
     index = list(set(liste_licence)-set(liste_licence_sejour))
 
     df_non_inscrits = df_effectif.copy()
     df_non_inscrits = df_non_inscrits[df_non_inscrits['N° Licencié'].isin(index)]
     df_non_inscrits['sejour'] = 'aucun'
     df_total = pd.concat([df_total,df_non_inscrits],ignore_index=True)
-    
+
 
     return(no_match,df_total,index)
 
 def parse_date(s,year):
-    
-    import re
-    from datetime import datetime 
 
-    convert_to_date = lambda s: datetime.strptime(s,"%Y_%m_%d")
+    convert_to_date = lambda s: datetime.datetime.strptime(s,"%Y_%m_%d")
     s = re.sub(r"-","_",s)
-    
+
     try:
         pattern = re.compile(r"(?P<year>\b\d{4}_)(?P<month>\d{1,2}_)(?P<day>\d{1,2})")
         match = pattern.search(s)
         date = convert_to_date(match.group("year")+match.group("month")+match.group("day"))
     except:
         pattern = re.compile(r"(?P<month>\d{1,2}_)(?P<day>\d{1,2})")
         match = pattern.search(s)
         date = convert_to_date(str(year)+'_'+match.group("month")+match.group("day"))
-    
+
     return date
 
-    
+
 def read_effectif(ctg_path,year):
-    
-    from pathlib import Path
-    
-    import numpy as np
-    import pandas as pd
-    
-    from CTG_Utils.CTG_Func.CTG_plot import built_lat_long
 
-        
     def distance_(row):
-        from math import asin, cos, radians, sin, sqrt
+
         phi1, lon1 = dh.query("Ville=='GRENOBLE'")[['long','lat']].values.flatten()
         phi1, lon1 = radians(phi1), radians(lon1)
         phi2, lon2 = radians(row['long']), radians(row['lat'])
         rad = 6371
         dist = 2 * rad * asin(
                                 sqrt(
                                     sin((phi2 - phi1) / 2) ** 2
                                     + cos(phi1) * cos(phi2) * sin((lon2 - lon1) / 2) ** 2
                                 ))
         return np.round(dist,1)
 
-    
+
     df = pd.read_excel(ctg_path / Path(str(year))/ Path('DATA')/Path(str(year)+'.xlsx'))
-        
+
     df['Date de naissance'] = pd.to_datetime(df['Date de naissance'], format="%d/%m/%Y")
-    
+
     df['Age']  = df['Date de naissance'].apply(lambda x : (pd.Timestamp(year, 9, 30)-x).days/365)
 
     df,dh = built_lat_long(df)
 
     df['distance'] = df.apply(distance_,axis=1)
-    
+
     return df
-    
+
 def evolution_effectif(ctg_path):
 
     # Evolution des effectifs hommes et femme de 2016 à 2022
-    import os
-    import re
-    
-    import matplotlib.pyplot as plt
-    import numpy as np
-    
+
     def addlabels(x,y,z=None):
         for i in range(len(x)):
             if z is None:
                 plt.text(x[i]-0.4,y[i]+5,y[i],size=10)
             else:
                 plt.text(x[i]-0.4,y[i]+5,z[i],size=10,rotation='vertical')
-    
-    
+
+
     def _evolution_effectif(years):
         nbr_hommes = []
         nbr_femmes = []
         nbr_total = []
         ratio_femmes = []
         for year in years:
             if year == 2006:
                 nbr_femmes.append(41)
                 nbr_hommes.append(100)
                 nbr_total.append(141)
                 ratio_femmes.append(str(29)+'%')
-            else:  
+            else:
                 df_effectif = read_effectif(ctg_path,year)
                 nh = len(df_effectif.query('Sexe =="M"'))
                 nbr_hommes.append(nh)
                 nf = len(df_effectif.query('Sexe =="F"'))
                 nbr_femmes.append(nf)
                 nbr_total.append(nh + nf)
                 ratio_femmes.append(str(int(100*nf/(nh+nf)))+'%')
         return nbr_hommes, nbr_femmes,nbr_total,ratio_femmes
-    
+
     years = [2006] + [int(x) for x in os.listdir(ctg_path) if re.findall('^\d{4}$',x)]
     nbr_hommes, nbr_femmes,nbr_total,ratio_femmes = _evolution_effectif(years)
-    
+
     title='Evolution du nombre de licenciés CTG'
-    
-    ax = plt.axes() 
+
+    ax = plt.axes()
     plt.bar(years, nbr_femmes,label= 'Femme')
     addlabels(years, nbr_femmes)
     plt.bar(years, nbr_hommes,bottom=nbr_femmes,label= 'Hommes')
     plt.legend()
     addlabels(years, nbr_total)
     ax.set_xticks(years)
-    plt.xticks(rotation=90)    
+    plt.xticks(rotation=90)
     plt.tight_layout()
     plt.show()
-    
+
 def evolution_age_median(ctg_path):
 
-    from pathlib import Path
-    from collections import Counter
-    import os
-    import re
-    
-    import matplotlib.pyplot as plt
-    import numpy as np 
-    import pandas as pd
-    
-    
     def addlabels(x,y,z=None):
         for i in range(len(x)):
             if z is None:
                 plt.text(x[i]-0.3,y[i]+0.1,y[i],size=10)
             else:
                 plt.text(x[i]-0.2,y[i]+0.1,z[i],size=10,rotation='vertical')
-        
+
     xt = range(55,90)
     years = [int(x) for x in os.listdir(ctg_path) if re.findall('^\d{4}$',x)]
     nbr_femmes = []
     ratio_femmes = []
     nbr_total = []
-    age_mean = [] 
+    age_mean = []
     age_naturel = []
     for idx,year in enumerate(years):
         df_effectif = pd.read_excel(ctg_path / Path(str(year)) / Path('DATA') / Path(str(year)+'.xlsx'))
         df_effectif['Date de naissance'] = pd.to_datetime(df_effectif['Date de naissance'], format="%d/%m/%Y")
         df_effectif['Age']  = df_effectif['Date de naissance'].apply(lambda x : (pd.Timestamp(year, 9, 30)-x).days/365)#.astype(int)
         age_median = df_effectif['Age'].median()
         age_mean.append(age_median)
         if idx == 0:
            age_median_0 = age_median
            age_naturel.append(age_median_0)
         else:
            age_naturel.append(age_median_0+idx)
-        
+
     fig, ax = plt.subplots()
     plt.bar(years,age_mean)
     plt.plot(years,age_naturel,"--r")
     plt.ylabel('Age moyen')
     plt.ylim(50,1.1*max(age_naturel))
     addlabels(years,[round(x,1) for x in age_mean])
     linear_model = np.polyfit(years,age_mean,1)
@@ -369,79 +339,64 @@
     plt.tick_params(axis='y', labelsize=20)
     plt.ylabel('Age median',size=20)
     x_s =[years[0]-1] + years + [years[-1]+1]
     plt.plot(x_s,linear_model_fn(x_s),"--g")
     plt.title(f'Pente vieillissement : {round(linear_model[0]*12,1)} mois par ans')
     plt.tight_layout()
     plt.show()
-    
+
 def builds_excel_presence_au_club(ctg_path):
-    import os
-    import re
-    from pathlib import Path
-    
-    import pandas as pd
-    
-    import CTG_Utils as ctg
-    
+
     list_date = [int(x) for x in os.listdir(ctg_path) if re.findall('^\d{4}$',x)]
     list_df = []
-    
+
     for date in list_date:
         df = pd.read_excel(ctg_path /Path(str(date)) / Path('DATA') / Path(str(date)+'.xlsx'))
         df['date'] = date
         list_df.append(df[['N° Licencié','Nom','Prénom','date']])
-        
+
     df = pd.concat(list_df) #.to_excel(file / Path('effectif_total.xlsx'),index=False)
-    
+
     dic = {}
     list_num_licence = []
     list_nom = []
     list_prenom = []
     list_date_ = []
     for licence in df.groupby('N° Licencié'):
         list_c = [x if x in licence[1]['date'].to_list() else None for x in list_date]
         #if len(list_c) - list_c.count(None) == 1: singleton
         list_num_licence.append(licence[0])
         list_nom.append(licence[1]['Nom'].unique()[0])
         list_prenom.append(licence[1]['Prénom'].unique()[0])
         list_date_.append(list_c)
-    
-        
+
+
     dic['N° Licencié'] = list_num_licence
     dic['Nom'] = list_nom
     dic['Prénom'] = list_prenom
     dic['date'] = list_date_
-    
+
     df = pd.DataFrame.from_dict(dic)
     split_df = pd.DataFrame(df['date'].tolist(), columns=list_date)
-    
+
     df = pd.concat([df, split_df], axis=1)
     df = df.drop('date',axis=1)
     out_path = ctg_path / Path(str(list_date[-1])) / Path('STATISTIQUES') / Path('effectif_history.xlsx')
     df.to_excel(out_path)
     return out_path
-    
+
 def statistique_vae(ctg_path):
 
-    from datetime import datetime
-    from pathlib import Path
-    
-    import matplotlib.pyplot as plt
-    import pandas as pd
-    
-    # Internal import
-    import CTG_Utils as ctg
     # function to add value labels
     def addlabels(x,y):
         for i in range(1,len(x)):
             plt.text(x[i]-0.2,y[i]+0.5,y[i],size=10)
-    
-    current_year = datetime.now().year
-    
+
+    current_year = datetime.datetime.now().year
+
     last_year = 2018
     years =[]
     nb_vae_m = []
     nb_vae_f = []
     nb_vae_tot = []
     for year in range(last_year,current_year+1):
         df_N1 = pd.read_excel(ctg_path / Path(str(year)) / Path('DATA') /Path(str(year)+'.xlsx'))
@@ -461,46 +416,37 @@
     addlabels(years, nb_vae_m)
     addlabels(years, [x+y for x,y in zip(nb_vae_m,nb_vae_f)])
     plt.tight_layout()
     plt.show()
 
 def anciennete_au_club(ctg_path):
 
-    import datetime
-    from pathlib import Path
-    
-    import numpy as np
-    import matplotlib.pyplot as plt
-    import pandas as pd
-    
-    import CTG_Utils as ctg
-    
     def addlabels(x,y,offset):
         for i in range(len(x)):
             if y[i] != 0:
                 plt.text(x[i]-0.2,y[i]+offset,round(y[i],1),size=15)
-                
+
     currentDateTime = datetime.datetime.now()
     date = currentDateTime.date()
     current_year = int(date.strftime("%Y"))
-    
+
     in_path = ctg_path / Path(str(current_year)) / Path('STATISTIQUES') / Path('effectif_history.xlsx')
     df = pd.read_excel(in_path)
     eff = []
-    
+
     years = list(range(2012,current_year+1))
     for year in years:
         dg = df.dropna(subset=[year,current_year])
         eff.append(len(dg))
     eff = [eff[0]] + list(np.diff(eff))
-    
+
     # creating the bar plot
     fig = plt.figure(figsize = (10, 5))
-    plt.bar(years, eff, color ='maroon', 
+    plt.bar(years, eff, color ='maroon',
             width = 0.4)
-     
+
     plt.xlabel("")
     plt.ylabel("# adhérents")
     plt.title("Ancienneté au CTG")
     addlabels(list(range(2012,2025)), eff,0)
     plt.tight_layout()
     plt.show()
```

### Comparing `CTG_Utils-1.2.1/CTG_Utils/CTG_Func/CTG_synthese.py` & `CTG_Utils-1.2.2/ctgutils/ctgFuncts/ctg_synthese.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,990 +1,907 @@
-00000000: 0d0a 6465 6620 7379 6e74 6865 7365 2879  ..def synthese(y
-00000010: 6561 722c 6374 675f 7061 7468 293a 0d0a  ear,ctg_path):..
-00000020: 0d0a 2020 2020 2320 5374 616e 6461 7264  ..    # Standard
-00000030: 206c 6962 7261 7279 2069 6d70 6f72 7473   library imports
-00000040: 0d0a 2020 2020 696d 706f 7274 206f 730d  ..    import os.
-00000050: 0a20 2020 2066 726f 6d20 7061 7468 6c69  .    from pathli
-00000060: 6220 696d 706f 7274 2050 6174 680d 0a0d  b import Path...
-00000070: 0a20 2020 2023 2054 6869 7264 2070 6172  .    # Third par
-00000080: 7479 2069 6d70 6f72 7473 2020 2020 0d0a  ty imports    ..
-00000090: 2020 2020 696d 706f 7274 2070 616e 6461      import panda
-000000a0: 7320 6173 2070 640d 0a20 2020 200d 0a20  s as pd..    .. 
-000000b0: 2020 2023 2049 6e74 6572 6e61 6c20 696d     # Internal im
-000000c0: 706f 7274 730d 0a20 2020 2066 726f 6d20  ports..    from 
-000000d0: 4354 475f 5574 696c 732e 4354 475f 4675  CTG_Utils.CTG_Fu
-000000e0: 6e63 2e43 5447 5f65 6666 6563 7469 6620  nc.CTG_effectif 
-000000f0: 696d 706f 7274 2072 6561 645f 6566 6665  import read_effe
-00000100: 6374 6966 5f63 6f72 7265 6374 6564 0d0a  ctif_corrected..
-00000110: 2020 2020 0d0a 0d0a 2020 2020 0d0a 2020      ....    ..  
-00000120: 2020 0d0a 2020 2020 7061 7468 5f64 6972    ..    path_dir
-00000130: 5f6c 6973 7420 3d20 5b63 7467 5f70 6174  _list = [ctg_pat
-00000140: 6820 2f20 5061 7468 2873 7472 2879 6561  h / Path(str(yea
-00000150: 7229 2920 2f20 5061 7468 2827 534f 5254  r)) / Path('SORT
-00000160: 4945 5320 4455 2053 414d 4544 4927 2920  IES DU SAMEDI') 
-00000170: 2f20 5061 7468 2827 4558 4345 4c27 292c  / Path('EXCEL'),
-00000180: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000190: 2020 2020 2020 2063 7467 5f70 6174 6820         ctg_path 
-000001a0: 2f20 5061 7468 2873 7472 2879 6561 7229  / Path(str(year)
-000001b0: 2920 2f20 5061 7468 2827 534f 5254 4945  ) / Path('SORTIE
-000001c0: 5320 4455 2044 494d 414e 4348 4527 2920  S DU DIMANCHE') 
-000001d0: 2f20 5061 7468 2827 4558 4345 4c27 292c  / Path('EXCEL'),
-000001e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000001f0: 2020 2020 2020 2063 7467 5f70 6174 6820         ctg_path 
-00000200: 2f20 5061 7468 2873 7472 2879 6561 7229  / Path(str(year)
-00000210: 2920 2f20 5061 7468 2827 534f 5254 4945  ) / Path('SORTIE
-00000220: 5320 4455 204a 4555 4449 2729 202f 2050  S DU JEUDI') / P
-00000230: 6174 6828 2745 5843 454c 2729 2c0d 0a20  ath('EXCEL'),.. 
-00000240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000250: 2020 2020 6374 675f 7061 7468 202f 2050      ctg_path / P
-00000260: 6174 6828 7374 7228 7965 6172 2929 202f  ath(str(year)) /
-00000270: 2050 6174 6828 2753 4f52 5449 4553 2048   Path('SORTIES H
-00000280: 4956 4552 2729 202f 2050 6174 6828 2745  IVER') / Path('E
-00000290: 5843 454c 2729 2c0d 0a20 2020 2020 2020  XCEL'),..       
-000002a0: 2020 2020 2020 2020 2020 2020 2020 6374                ct
-000002b0: 675f 7061 7468 202f 2050 6174 6828 7374  g_path / Path(st
-000002c0: 7228 7965 6172 2929 202f 2050 6174 6828  r(year)) / Path(
-000002d0: 2753 4f52 5449 4553 2044 5520 4c55 4e44  'SORTIES DU LUND
-000002e0: 4927 292f 2050 6174 6828 2745 5843 454c  I')/ Path('EXCEL
-000002f0: 2729 2c0d 0a20 2020 2020 2020 2020 2020  '),..           
-00000300: 2020 2020 2020 2020 2020 6374 675f 7061            ctg_pa
-00000310: 7468 202f 2050 6174 6828 7374 7228 7965  th / Path(str(ye
-00000320: 6172 2929 202f 2050 6174 6828 2753 454a  ar)) / Path('SEJ
-00000330: 4f55 5227 2920 2f20 5061 7468 2827 4558  OUR') / Path('EX
-00000340: 4345 4c27 295d 0d0a 0d0a 2020 2020 6c69  CEL')]....    li
-00000350: 7374 5f64 6620 3d20 5b5d 0d0a 2020 2020  st_df = []..    
-00000360: 666f 7220 7061 7468 5f64 6972 2069 6e20  for path_dir in 
-00000370: 7061 7468 5f64 6972 5f6c 6973 743a 0d0a  path_dir_list:..
-00000380: 2020 2020 2020 2020 6966 206f 732e 7061          if os.pa
-00000390: 7468 2e69 7364 6972 2870 6174 685f 6469  th.isdir(path_di
-000003a0: 7229 3a0d 0a20 2020 2020 2020 2020 2020  r):..           
-000003b0: 2066 696c 6573 203d 205b 7820 666f 7220   files = [x for 
-000003c0: 7820 696e 206f 732e 6c69 7374 6469 7228  x in os.listdir(
-000003d0: 7061 7468 5f64 6972 2920 6966 2078 2e65  path_dir) if x.e
-000003e0: 6e64 7377 6974 6828 272e 786c 7378 2729  ndswith('.xlsx')
-000003f0: 2061 6e64 2022 7e24 2220 6e6f 7420 696e   and "~$" not in
-00000400: 2078 5d20 0d0a 2020 2020 2020 2020 2020   x] ..          
-00000410: 2020 6c69 7374 5f64 662e 6578 7465 6e64    list_df.extend
-00000420: 285b 7064 2e72 6561 645f 6578 6365 6c28  ([pd.read_excel(
-00000430: 7061 7468 5f64 6972 202f 2050 6174 6828  path_dir / Path(
-00000440: 6669 6c65 292c 2065 6e67 696e 653d 276f  file), engine='o
-00000450: 7065 6e70 7978 6c27 2920 666f 7220 6669  penpyxl') for fi
-00000460: 6c65 2069 6e20 6669 6c65 735d 290d 0a20  le in files]).. 
-00000470: 2020 200d 0a20 2020 2064 665f 746f 7461     ..    df_tota
-00000480: 6c20 3d20 7064 2e63 6f6e 6361 7428 6c69  l = pd.concat(li
-00000490: 7374 5f64 662c 2069 676e 6f72 655f 696e  st_df, ignore_in
-000004a0: 6465 783d 5472 7565 290d 0a20 2020 200d  dex=True)..    .
-000004b0: 0a20 2020 2064 665f 6566 6665 6374 6966  .    df_effectif
-000004c0: 203d 2072 6561 645f 6566 6665 6374 6966   = read_effectif
-000004d0: 5f63 6f72 7265 6374 6564 2863 7467 5f70  _corrected(ctg_p
-000004e0: 6174 6829 0d0a 2020 2020 0d0a 2020 2020  ath)..    ..    
-000004f0: 6466 5f74 6f74 616c 5b27 5072 6174 6971  df_total['Pratiq
-00000500: 7565 2056 4145 275d 2e66 696c 6c6e 6128  ue VAE'].fillna(
-00000510: 274e 6f6e 272c 696e 706c 6163 653d 5472  'Non',inplace=Tr
-00000520: 7565 290d 0a20 2020 200d 0a20 2020 2023  ue)..    ..    #
-00000530: 206e 6f6d 6272 6520 6d6f 7965 6e20 6465   nombre moyen de
-00000540: 2070 6172 7469 6369 7061 6e74 2070 6172   participant par
-00000550: 2061 6374 6976 6974 c3a9 0d0a 2020 2020   activit....    
-00000560: 666f 7220 7820 696e 2064 665f 746f 7461  for x in df_tota
-00000570: 6c2e 6772 6f75 7062 7928 5b27 5479 7065  l.groupby(['Type
-00000580: 275d 293a 0d0a 2020 2020 2020 2020 7072  ']):..        pr
-00000590: 696e 7428 785b 305d 2c6c 656e 2878 5b31  int(x[0],len(x[1
-000005a0: 5d29 2c6c 656e 2873 6574 2878 5b31 5d5b  ]),len(set(x[1][
-000005b0: 2773 656a 6f75 7227 5d29 292c 6c65 6e28  'sejour'])),len(
-000005c0: 785b 315d 292f 6c65 6e28 7365 7428 785b  x[1])/len(set(x[
-000005d0: 315d 5b27 7365 6a6f 7572 275d 2929 290d  1]['sejour']))).
-000005e0: 0a20 2020 200d 0a20 2020 2066 696c 6520  .    ..    file 
-000005f0: 3d20 6374 675f 7061 7468 202f 2050 6174  = ctg_path / Pat
-00000600: 6828 7374 7228 7965 6172 2929 202f 2050  h(str(year)) / P
-00000610: 6174 6828 2753 5441 5449 5354 4951 5545  ath('STATISTIQUE
-00000620: 5327 2920 2f20 5061 7468 2827 7379 6e74  S') / Path('synt
-00000630: 6865 7365 2e78 6c73 7827 290d 0a20 2020  hese.xlsx')..   
-00000640: 2064 665f 746f 7461 6c2e 746f 5f65 7863   df_total.to_exc
-00000650: 656c 2866 696c 6529 0d0a 0d0a 6465 6620  el(file)....def 
-00000660: 706c 6f74 5f70 6965 5f73 796e 7468 6573  plot_pie_synthes
-00000670: 6528 7965 6172 2c63 7467 5f70 6174 6829  e(year,ctg_path)
-00000680: 3a0d 0a20 2020 200d 0a20 2020 2023 2053  :..    ..    # S
-00000690: 7461 6e64 6172 6420 6c69 6272 6172 7920  tandard library 
-000006a0: 696d 706f 7274 730d 0a20 2020 2066 726f  imports..    fro
-000006b0: 6d20 7061 7468 6c69 6220 696d 706f 7274  m pathlib import
-000006c0: 2050 6174 680d 0a20 2020 200d 0a20 2020   Path..    ..   
-000006d0: 2023 2054 6869 7264 2070 6172 7479 2069   # Third party i
-000006e0: 6d70 6f72 7473 0d0a 2020 2020 696d 706f  mports..    impo
-000006f0: 7274 206e 756d 7079 2061 7320 6e70 0d0a  rt numpy as np..
-00000700: 2020 2020 696d 706f 7274 206d 6174 706c      import matpl
-00000710: 6f74 6c69 622e 7079 706c 6f74 2061 7320  otlib.pyplot as 
-00000720: 706c 740d 0a20 2020 2069 6d70 6f72 7420  plt..    import 
-00000730: 7061 6e64 6173 2061 7320 7064 0d0a 2020  pandas as pd..  
-00000740: 2020 0d0a 2020 2020 6465 6620 6675 6e63    ..    def func
-00000750: 2870 6374 2c20 616c 6c76 616c 7565 7329  (pct, allvalues)
-00000760: 3a0d 0a20 2020 2020 2020 2061 6273 6f6c  :..        absol
-00000770: 7574 6520 3d20 726f 756e 6428 7063 7420  ute = round(pct 
-00000780: 2f20 3130 302e 2a6e 702e 7375 6d28 616c  / 100.*np.sum(al
-00000790: 6c76 616c 7565 7329 2c30 290d 0a20 2020  lvalues),0)..   
-000007a0: 2020 2020 2023 7265 7475 726e 2022 7b3a       #return "{:
-000007b0: 2e31 667d 255c 6e28 7b3a 647d 2922 2e66  .1f}%\n({:d})".f
-000007c0: 6f72 6d61 7428 7063 742c 2061 6273 6f6c  ormat(pct, absol
-000007d0: 7574 6529 0d0a 2020 2020 2020 2020 7265  ute)..        re
-000007e0: 7475 726e 2020 6622 7b69 6e74 2872 6f75  turn  f"{int(rou
-000007f0: 6e64 2861 6273 6f6c 7574 652c 3129 297d  nd(absolute,1))}
-00000800: 5c6e 7b72 6f75 6e64 2870 6374 2c31 297d  \n{round(pct,1)}
-00000810: 2025 220d 0a20 2020 2020 2020 200d 0a20   %"..        .. 
-00000820: 2020 2066 696c 655f 696e 203d 2063 7467     file_in = ctg
-00000830: 5f70 6174 6820 2f20 5061 7468 2873 7472  _path / Path(str
-00000840: 2879 6561 7229 2920 2f20 5061 7468 2827  (year)) / Path('
-00000850: 5354 4154 4953 5449 5155 4553 2729 202f  STATISTIQUES') /
-00000860: 2050 6174 6828 2773 796e 7468 6573 652e   Path('synthese.
-00000870: 786c 7378 2729 0d0a 2020 2020 6466 5f74  xlsx')..    df_t
-00000880: 6f74 616c 203d 2070 642e 7265 6164 5f65  otal = pd.read_e
-00000890: 7863 656c 2866 696c 655f 696e 290d 0a20  xcel(file_in).. 
-000008a0: 2020 2064 665f 746f 7461 6c20 3d20 6466     df_total = df
-000008b0: 5f74 6f74 616c 2e64 726f 706e 6128 7375  _total.dropna(su
-000008c0: 6273 6574 3d5b 2754 7970 6527 5d29 200d  bset=['Type']) .
-000008d0: 0a20 2020 2064 665f 746f 7461 6c20 3d20  .    df_total = 
-000008e0: 6466 5f74 6f74 616c 2e64 726f 706e 6128  df_total.dropna(
-000008f0: 7375 6273 6574 3d5b 274e 6f6d 275d 290d  subset=['Nom']).
-00000900: 0a0d 0a20 2020 2064 6167 6720 3d20 6466  ...    dagg = df
-00000910: 5f74 6f74 616c 2e67 726f 7570 6279 2827  _total.groupby('
-00000920: 5479 7065 2729 5b27 6e62 725f 6a6f 7572  Type')['nbr_jour
-00000930: 7327 5d2e 6167 6728 7375 6d29 0d0a 0d0a  s'].agg(sum)....
-00000940: 2020 2020 0d0a 2020 2020 0d0a 2020 2020      ..    ..    
-00000950: 6578 706c 6f64 655f 6469 6320 3d20 7b27  explode_dic = {'
-00000960: 5241 4e44 4f4e 4e45 4527 3a30 2e31 2c0d  RANDONNEE':0.1,.
-00000970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000980: 2020 2020 2753 454a 4f55 5227 3a30 2e30      'SEJOUR':0.0
-00000990: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
-000009a0: 2020 2020 2020 2027 534f 5254 4945 5320         'SORTIES 
-000009b0: 4455 2044 494d 414e 4348 4527 3a30 2e32  DU DIMANCHE':0.2
-000009c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000009d0: 2020 2020 2020 2753 4f52 5449 4553 2044        'SORTIES D
-000009e0: 5520 4a45 5544 4927 3a30 2e32 2c0d 0a20  U JEUDI':0.2,.. 
-000009f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a00: 2020 2753 4f52 5449 4553 2044 5520 4c55    'SORTIES DU LU
-00000a10: 4e44 4927 3a30 2e32 2c20 0d0a 2020 2020  NDI':0.2, ..    
-00000a20: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00000a30: 534f 5254 4945 5320 4455 2053 414d 4544  SORTIES DU SAMED
-00000a40: 4927 3a30 2e32 2c0d 0a20 2020 2020 2020  I':0.2,..       
-00000a50: 2020 2020 2020 2020 2020 2020 2753 4f52              'SOR
-00000a60: 5449 4553 2048 4956 4552 273a 302e 327d  TIES HIVER':0.2}
-00000a70: 0d0a 0d0a 2020 2020 6461 7461 203d 205b  ....    data = [
-00000a80: 5d0d 0a20 2020 2073 6f72 7469 6573 203d  ]..    sorties =
-00000a90: 205b 5d0d 0a20 2020 2066 6f72 2074 7970   []..    for typ
-00000aa0: 655f 7365 6a6f 7572 2c20 6e62 7220 696e  e_sejour, nbr in
-00000ab0: 207a 6970 2864 6167 672e 696e 6465 782c   zip(dagg.index,
-00000ac0: 6461 6767 2e74 6f6c 6973 7428 2929 3a0d  dagg.tolist()):.
-00000ad0: 0a20 2020 2020 2020 2069 6620 6e62 7221  .        if nbr!
-00000ae0: 3d30 3a0d 0a20 2020 2020 2020 2020 2020  =0:..           
-00000af0: 2064 6174 612e 6170 7065 6e64 286e 6272   data.append(nbr
-00000b00: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-00000b10: 6f72 7469 6573 2e61 7070 656e 6428 7479  orties.append(ty
-00000b20: 7065 5f73 656a 6f75 7229 0d0a 0d0a 2020  pe_sejour)....  
-00000b30: 2020 6578 706c 6f64 6520 3d20 5b65 7870    explode = [exp
-00000b40: 6c6f 6465 5f64 6963 5b74 7970 5d20 666f  lode_dic[typ] fo
-00000b50: 7220 7479 7020 696e 2073 6f72 7469 6573  r typ in sorties
-00000b60: 5d0d 0a20 2020 200d 0a20 2020 200d 0a20  ]..    ..    .. 
-00000b70: 2020 2023 2043 7265 6174 696e 6720 706c     # Creating pl
-00000b80: 6f74 0d0a 2020 2020 6669 6720 3d20 706c  ot..    fig = pl
-00000b90: 742e 6669 6775 7265 2866 6967 7369 7a65  t.figure(figsize
-00000ba0: 203d 2831 302c 2037 2929 0d0a 2020 2020   =(10, 7))..    
-00000bb0: 5f2c 205f 2c20 6175 746f 7465 7874 7320  _, _, autotexts 
-00000bc0: 3d20 706c 742e 7069 6528 6461 7461 2c0d  = plt.pie(data,.
-00000bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000be0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00000bf0: 6162 656c 7320 3d20 736f 7274 6965 732c  abels = sorties,
-00000c00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c20: 6175 746f 7063 7420 3d20 6c61 6d62 6461  autopct = lambda
-00000c30: 2070 6374 3a20 6675 6e63 2870 6374 2c20   pct: func(pct, 
-00000c40: 6461 7461 292c 0d0a 2020 2020 2020 2020  data),..        
-00000c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c60: 2020 2020 2020 6578 706c 6f64 6520 3d20        explode = 
-00000c70: 6578 706c 6f64 652c 0d0a 2020 2020 2020  explode,..      
-00000c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c90: 2020 2020 2020 2020 7465 7874 7072 6f70          textprop
-00000ca0: 733d 7b27 666f 6e74 7369 7a65 273a 2031  s={'fontsize': 1
-00000cb0: 387d 290d 0a20 2020 2070 6c74 2e74 6974  8})..    plt.tit
-00000cc0: 6c65 2873 7472 2879 6561 7229 2c20 7061  le(str(year), pa
-00000cd0: 643d 3530 2c20 666f 6e74 7369 7a65 3d32  d=50, fontsize=2
-00000ce0: 3029 0d0a 2020 2020 0d0a 2020 2020 5f20  0)..    ..    _ 
-00000cf0: 3d20 706c 742e 7365 7470 2861 7574 6f74  = plt.setp(autot
-00000d00: 6578 7473 2c20 2a2a 7b27 636f 6c6f 7227  exts, **{'color'
-00000d10: 3a27 6b27 2c20 2777 6569 6768 7427 3a27  :'k', 'weight':'
-00000d20: 626f 6c64 272c 2027 666f 6e74 7369 7a65  bold', 'fontsize
-00000d30: 273a 3134 7d29 0d0a 2020 2020 0d0a 2020  ':14})..    ..  
-00000d40: 2020 706c 742e 7469 6768 745f 6c61 796f    plt.tight_layo
-00000d50: 7574 2829 0d0a 2020 2020 706c 742e 7368  ut()..    plt.sh
-00000d60: 6f77 2829 0d0a 2020 2020 0d0a 2020 2020  ow()..    ..    
-00000d70: 6669 675f 6669 6c65 203d 2027 534f 5254  fig_file = 'SORT
-00000d80: 4945 535f 5049 452e 706e 6727 0d0a 2020  IES_PIE.png'..  
-00000d90: 2020 706c 742e 7361 7665 6669 6728 6374    plt.savefig(ct
-00000da0: 675f 7061 7468 202f 2050 6174 6828 7374  g_path / Path(st
-00000db0: 7228 7965 6172 2929 202f 2050 6174 6828  r(year)) / Path(
-00000dc0: 2753 5441 5449 5354 4951 5545 5327 2920  'STATISTIQUES') 
-00000dd0: 2f20 5061 7468 2866 6967 5f66 696c 6529  / Path(fig_file)
-00000de0: 2c62 626f 785f 696e 6368 6573 3d27 7469  ,bbox_inches='ti
-00000df0: 6768 7427 2909 0d0a 0d0a 2020 2020 7265  ght').....    re
-00000e00: 7475 726e 2009 0d0a 090d 0a0d 0a64 6566  turn ........def
-00000e10: 2073 796e 7468 6573 655f 6164 6865 7265   synthese_adhere
-00000e20: 6e74 2879 6561 722c 6374 675f 7061 7468  nt(year,ctg_path
-00000e30: 293a 0d0a 0d0a 2020 2020 2320 5374 616e  ):....    # Stan
-00000e40: 6461 7264 206c 6962 7261 7279 2069 6d70  dard library imp
-00000e50: 6f72 7473 0d0a 2020 2020 6672 6f6d 2070  orts..    from p
-00000e60: 6174 686c 6962 2069 6d70 6f72 7420 5061  athlib import Pa
-00000e70: 7468 0d0a 2020 2020 0d0a 2020 2020 2320  th..    ..    # 
-00000e80: 5468 6972 6420 7061 7274 7920 696d 706f  Third party impo
-00000e90: 7274 730d 0a20 2020 2069 6d70 6f72 7420  rts..    import 
-00000ea0: 7061 6e64 6173 2061 7320 7064 0d0a 2020  pandas as pd..  
-00000eb0: 2020 0d0a 2020 2020 2320 496e 7465 726e    ..    # Intern
-00000ec0: 616c 2069 6d70 6f72 7473 0d0a 2020 2020  al imports..    
-00000ed0: 6672 6f6d 2043 5447 5f55 7469 6c73 2e43  from CTG_Utils.C
-00000ee0: 5447 5f46 756e 632e 4354 4743 6c61 7373  TG_Func.CTGClass
-00000ef0: 6573 2069 6d70 6f72 7420 4566 6665 6374  es import Effect
-00000f00: 6966 4374 670d 0a20 2020 200d 0a20 2020  ifCtg..    ..   
-00000f10: 2066 696c 655f 696e 203d 2063 7467 5f70   file_in = ctg_p
-00000f20: 6174 6820 2f20 5061 7468 2873 7472 2879  ath / Path(str(y
-00000f30: 6561 7229 2920 2f20 5061 7468 2827 5354  ear)) / Path('ST
-00000f40: 4154 4953 5449 5155 4553 2729 202f 2050  ATISTIQUES') / P
-00000f50: 6174 6828 2773 796e 7468 6573 652e 786c  ath('synthese.xl
-00000f60: 7378 2729 0d0a 2020 2020 6466 5f74 6f74  sx')..    df_tot
-00000f70: 616c 203d 2070 642e 7265 6164 5f65 7863  al = pd.read_exc
-00000f80: 656c 2866 696c 655f 696e 290d 0a20 2020  el(file_in)..   
-00000f90: 2064 665f 746f 7461 6c20 3d20 6466 5f74   df_total = df_t
-00000fa0: 6f74 616c 2e64 726f 706e 6128 7375 6273  otal.dropna(subs
-00000fb0: 6574 3d5b 2754 7970 6527 5d29 0d0a 2020  et=['Type'])..  
-00000fc0: 2020 6e62 7265 203d 207b 7d0d 0a20 2020    nbre = {}..   
-00000fd0: 200d 0a20 2020 2066 6f72 2069 645f 6c69   ..    for id_li
-00000fe0: 6365 6e63 652c 2064 6720 696e 2064 665f  cence, dg in df_
-00000ff0: 746f 7461 6c2e 6772 6f75 7062 7928 274e  total.groupby('N
-00001000: c2b0 204c 6963 656e 6369 c3a9 2729 3a0d  .. Licenci..'):.
-00001010: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00001020: 2020 206e 6272 655b 6964 5f6c 6963 656e     nbre[id_licen
-00001030: 6365 5d3d 5b64 675b 274e 6f6d 275d 2e75  ce]=[dg['Nom'].u
-00001040: 6e69 7175 6528 295b 305d 2c64 675b 2750  nique()[0],dg['P
-00001050: 72c3 a96e 6f6d 275d 2e75 6e69 7175 6528  r..nom'].unique(
-00001060: 295b 305d 5d0d 0a20 2020 200d 0a20 2020  )[0]]..    ..   
-00001070: 2020 2020 206e 625f 736f 7274 6965 5f64       nb_sortie_d
-00001080: 696d 616e 6368 6520 3d20 6c65 6e28 6467  imanche = len(dg
-00001090: 2e71 7565 7279 2822 5479 7065 2e73 7472  .query("Type.str
-000010a0: 2e63 6f6e 7461 696e 7328 2753 4f52 5449  .contains('SORTI
-000010b0: 4553 2044 5520 4449 4d41 4e43 4845 2729  ES DU DIMANCHE')
-000010c0: 2229 290d 0a20 2020 2020 2020 206e 6272  "))..        nbr
-000010d0: 655b 6964 5f6c 6963 656e 6365 5d20 3d20  e[id_licence] = 
-000010e0: 6e62 7265 5b69 645f 6c69 6365 6e63 655d  nbre[id_licence]
-000010f0: 202b 205b 6e62 5f73 6f72 7469 655f 6469   + [nb_sortie_di
-00001100: 6d61 6e63 6865 5d0d 0a20 2020 200d 0a20  manche]..    .. 
-00001110: 2020 2020 2020 206e 625f 736f 7274 6965         nb_sortie
-00001120: 5f73 616d 6564 6920 3d20 6c65 6e28 6467  _samedi = len(dg
-00001130: 2e71 7565 7279 2822 5479 7065 2e73 7472  .query("Type.str
-00001140: 2e63 6f6e 7461 696e 7328 2753 4f52 5449  .contains('SORTI
-00001150: 4553 2044 5520 5341 4d45 4449 2729 2229  ES DU SAMEDI')")
-00001160: 290d 0a20 2020 2020 2020 206e 6272 655b  )..        nbre[
-00001170: 6964 5f6c 6963 656e 6365 5d20 3d20 6e62  id_licence] = nb
-00001180: 7265 5b69 645f 6c69 6365 6e63 655d 202b  re[id_licence] +
-00001190: 205b 6e62 5f73 6f72 7469 655f 7361 6d65   [nb_sortie_same
-000011a0: 6469 5d0d 0a20 2020 200d 0a20 2020 2020  di]..    ..     
-000011b0: 2020 206e 625f 736f 7274 6965 5f6a 6575     nb_sortie_jeu
-000011c0: 6469 203d 206c 656e 2864 672e 7175 6572  di = len(dg.quer
-000011d0: 7928 2254 7970 652e 7374 722e 636f 6e74  y("Type.str.cont
-000011e0: 6169 6e73 2827 534f 5254 4945 5320 4455  ains('SORTIES DU
-000011f0: 204a 4555 4449 2729 2229 290d 0a20 2020   JEUDI')"))..   
-00001200: 2020 2020 206e 6272 655b 6964 5f6c 6963       nbre[id_lic
-00001210: 656e 6365 5d20 3d20 6e62 7265 5b69 645f  ence] = nbre[id_
-00001220: 6c69 6365 6e63 655d 202b 205b 6e62 5f73  licence] + [nb_s
-00001230: 6f72 7469 655f 6a65 7564 695d 0d0a 2020  ortie_jeudi]..  
-00001240: 2020 0d0a 2020 2020 2020 2020 6e62 5f72    ..        nb_r
-00001250: 616e 646f 203d 206c 656e 2864 672e 7175  ando = len(dg.qu
-00001260: 6572 7928 2254 7970 652e 7374 722e 636f  ery("Type.str.co
-00001270: 6e74 6169 6e73 2827 5241 4e44 4f4e 4e45  ntains('RANDONNE
-00001280: 4527 2922 2929 0d0a 2020 2020 2020 2020  E')"))..        
-00001290: 6e62 7265 5b69 645f 6c69 6365 6e63 655d  nbre[id_licence]
-000012a0: 203d 206e 6272 655b 6964 5f6c 6963 656e   = nbre[id_licen
-000012b0: 6365 5d20 2b20 5b6e 625f 7261 6e64 6f5d  ce] + [nb_rando]
-000012c0: 0d0a 2020 2020 0d0a 2020 2020 2020 2020  ..    ..        
-000012d0: 6e62 5f73 656a 6f75 725f 6a6f 7572 7320  nb_sejour_jours 
-000012e0: 3d20 7375 6d28 6467 2e71 7565 7279 2822  = sum(dg.query("
-000012f0: 5479 7065 2e73 7472 2e63 6f6e 7461 696e  Type.str.contain
-00001300: 7328 2753 454a 4f55 5227 2922 295b 276e  s('SEJOUR')")['n
-00001310: 6272 5f6a 6f75 7273 275d 2e74 6f6c 6973  br_jours'].tolis
-00001320: 7428 2929 0d0a 2020 2020 2020 2020 6e62  t())..        nb
-00001330: 7265 5b69 645f 6c69 6365 6e63 655d 203d  re[id_licence] =
-00001340: 206e 6272 655b 6964 5f6c 6963 656e 6365   nbre[id_licence
-00001350: 5d20 2b20 5b6e 625f 7365 6a6f 7572 5f6a  ] + [nb_sejour_j
-00001360: 6f75 7273 5d0d 0a0d 0a20 2020 2020 2020  ours]....       
-00001370: 206e 625f 7365 6a6f 7572 203d 206c 656e   nb_sejour = len
-00001380: 2864 672e 7175 6572 7928 2254 7970 652e  (dg.query("Type.
-00001390: 7374 722e 636f 6e74 6169 6e73 2827 5345  str.contains('SE
-000013a0: 4a4f 5552 2729 2229 5b27 7365 6a6f 7572  JOUR')")['sejour
-000013b0: 275d 2e75 6e69 7175 6528 2929 0d0a 2020  '].unique())..  
-000013c0: 2020 2020 2020 6e62 7265 5b69 645f 6c69        nbre[id_li
-000013d0: 6365 6e63 655d 203d 206e 6272 655b 6964  cence] = nbre[id
-000013e0: 5f6c 6963 656e 6365 5d20 2b20 5b6e 625f  _licence] + [nb_
-000013f0: 7365 6a6f 7572 5d0d 0a20 2020 200d 0a20  sejour]..    .. 
-00001400: 2020 2020 2020 206e 625f 6869 7665 7220         nb_hiver 
-00001410: 3d20 6c65 6e28 6467 2e71 7565 7279 2822  = len(dg.query("
-00001420: 5479 7065 2e73 7472 2e63 6f6e 7461 696e  Type.str.contain
-00001430: 7328 2753 4f52 5449 4553 2048 4956 4552  s('SORTIES HIVER
-00001440: 2729 2229 290d 0a20 2020 2020 2020 206e  ')"))..        n
-00001450: 6272 655b 6964 5f6c 6963 656e 6365 5d20  bre[id_licence] 
-00001460: 3d20 6e62 7265 5b69 645f 6c69 6365 6e63  = nbre[id_licenc
-00001470: 655d 202b 205b 6e62 5f68 6976 6572 5d0d  e] + [nb_hiver].
-00001480: 0a20 2020 200d 0a20 2020 2020 2020 206e  .    ..        n
-00001490: 6272 5f65 7665 6e65 6d65 6e74 7320 3d20  br_evenements = 
-000014a0: 5b6e 625f 736f 7274 6965 5f64 696d 616e  [nb_sortie_diman
-000014b0: 6368 6520 2b0d 0a20 2020 2020 2020 2020  che +..         
-000014c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014d0: 206e 625f 736f 7274 6965 5f73 616d 6564   nb_sortie_samed
-000014e0: 6920 2b20 0d0a 2020 2020 2020 2020 2020  i + ..          
-000014f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001500: 6e62 5f73 6f72 7469 655f 6a65 7564 6920  nb_sortie_jeudi 
-00001510: 2b0d 0a20 2020 2020 2020 2020 2020 2020  +..             
-00001520: 2020 2020 2020 2020 2020 2020 206e 625f               nb_
-00001530: 7261 6e64 6f20 2b0d 0a20 2020 2020 2020  rando +..       
-00001540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001550: 2020 206e 625f 7365 6a6f 7572 5f6a 6f75     nb_sejour_jou
-00001560: 7273 202b 0d0a 2020 2020 2020 2020 2020  rs +..          
-00001570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001580: 6e62 5f68 6976 6572 5d0d 0a20 2020 2020  nb_hiver]..     
-00001590: 2020 206e 6272 655b 6964 5f6c 6963 656e     nbre[id_licen
-000015a0: 6365 5d20 3d20 6e62 7265 5b69 645f 6c69  ce] = nbre[id_li
-000015b0: 6365 6e63 655d 202b 206e 6272 5f65 7665  cence] + nbr_eve
-000015c0: 6e65 6d65 6e74 730d 0a20 2020 200d 0a20  nements..    .. 
-000015d0: 2020 2064 6720 3d20 7064 2e44 6174 6146     dg = pd.DataF
-000015e0: 7261 6d65 2e66 726f 6d5f 6469 6374 286e  rame.from_dict(n
-000015f0: 6272 6529 2e54 0d0a 2020 2020 6467 2e63  bre).T..    dg.c
-00001600: 6f6c 756d 6e73 203d 205b 0d0a 2020 2020  olumns = [..    
-00001610: 2020 2020 2020 2020 2020 2020 2027 4e6f               'No
-00001620: 6d27 2c0d 0a20 2020 2020 2020 2020 2020  m',..           
-00001630: 2020 2020 2020 2750 72c3 a96e 6f6d 272c        'Pr..nom',
-00001640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001650: 2020 2027 534f 5254 4945 2044 5520 4449     'SORTIE DU DI
-00001660: 4d41 4e43 4845 2043 4c55 4227 2c0d 0a20  MANCHE CLUB',.. 
-00001670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001680: 2753 4f52 5449 4520 4455 2053 414d 4544  'SORTIE DU SAMED
-00001690: 4920 434c 5542 272c 0d0a 2020 2020 2020  I CLUB',..      
-000016a0: 2020 2020 2020 2020 2020 2027 534f 5254             'SORT
-000016b0: 4945 2044 5520 4a45 5544 4920 434c 5542  IE DU JEUDI CLUB
-000016c0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-000016d0: 2020 2020 2027 5241 4e44 4f4e 4e45 4527       'RANDONNEE'
-000016e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000016f0: 2020 2020 2753 454a 4f55 522d 4a4f 5552      'SEJOUR-JOUR
-00001700: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00001710: 2020 2020 2027 4e62 725f 5345 4a4f 5552       'Nbr_SEJOUR
-00001720: 5327 2c0d 0a20 2020 2020 2020 2020 2020  S',..           
-00001730: 2020 2020 2020 2753 4f52 5449 4520 4849        'SORTIE HI
-00001740: 5645 5227 2c0d 0a20 2020 2020 2020 2020  VER',..         
-00001750: 2020 2020 2020 2020 2754 4f54 414c 272c          'TOTAL',
-00001760: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001770: 2020 205d 0d0a 2020 2020 0d0a 2020 2020     ]..    ..    
-00001780: 6566 6665 6374 6966 203d 2045 6666 6563  effectif = Effec
-00001790: 7469 6643 7467 2879 6561 722c 6374 675f  tifCtg(year,ctg_
-000017a0: 7061 7468 290d 0a20 2020 2064 665f 6566  path)..    df_ef
-000017b0: 6665 6374 6966 203d 2065 6666 6563 7469  fectif = effecti
-000017c0: 662e 6566 6665 6374 6966 0d0a 2020 2020  f.effectif..    
-000017d0: 6466 5f65 6666 6563 7469 662e 696e 6465  df_effectif.inde
-000017e0: 7820 3d20 6466 5f65 6666 6563 7469 665b  x = df_effectif[
-000017f0: 274e c2b0 204c 6963 656e 6369 c3a9 275d  'N.. Licenci..']
-00001800: 0d0a 2020 2020 6f72 7068 616e 203d 2073  ..    orphan = s
-00001810: 6574 2864 665f 6566 6665 6374 6966 2e69  et(df_effectif.i
-00001820: 6e64 6578 2920 2d20 7365 7428 6467 2e69  ndex) - set(dg.i
-00001830: 6e64 6578 290d 0a20 2020 2064 665f 6f72  ndex)..    df_or
-00001840: 7068 616e 203d 2064 665f 6566 6665 6374  phan = df_effect
-00001850: 6966 2e6c 6f63 5b6c 6973 7428 6f72 7068  if.loc[list(orph
-00001860: 616e 295d 5b5b 274e 6f6d 272c 2750 72c3  an)][['Nom','Pr.
-00001870: a96e 6f6d 275d 5d0d 0a20 2020 2064 665f  .nom']]..    df_
-00001880: 6f72 7068 616e 5b5b 2753 4f52 5449 4520  orphan[['SORTIE 
-00001890: 4455 2044 494d 414e 4348 4520 434c 5542  DU DIMANCHE CLUB
-000018a0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-000018b0: 2020 2027 534f 5254 4945 2044 5520 5341     'SORTIE DU SA
-000018c0: 4d45 4449 2043 4c55 4227 2c0d 0a20 2020  MEDI CLUB',..   
-000018d0: 2020 2020 2020 2020 2020 2020 2753 4f52              'SOR
-000018e0: 5449 4520 4455 204a 4555 4449 2043 4c55  TIE DU JEUDI CLU
-000018f0: 4227 2c0d 0a20 2020 2020 2020 2020 2020  B',..           
-00001900: 2020 2020 2752 414e 444f 4e4e 4545 272c      'RANDONNEE',
-00001910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001920: 2027 5345 4a4f 5552 2d4a 4f55 5227 2c0d   'SEJOUR-JOUR',.
-00001930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001940: 274e 6272 5f53 454a 4f55 5253 272c 0d0a  'Nbr_SEJOURS',..
-00001950: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00001960: 534f 5254 4945 2048 4956 4552 272c 0d0a  SORTIE HIVER',..
-00001970: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00001980: 544f 5441 4c27 5d5d 203d 205b 302c 302c  TOTAL']] = [0,0,
-00001990: 302c 302c 302c 302c 302c 305d 0d0a 2020  0,0,0,0,0,0]..  
-000019a0: 2020 0d0a 2020 2020 6467 203d 2070 642e    ..    dg = pd.
-000019b0: 636f 6e63 6174 285b 6467 2c20 6466 5f6f  concat([dg, df_o
-000019c0: 7270 6861 6e5d 2c20 6178 6973 3d30 290d  rphan], axis=0).
-000019d0: 0a20 2020 200d 0a20 2020 2066 696c 655f  .    ..    file_
-000019e0: 6f75 7420 3d20 6374 675f 7061 7468 202f  out = ctg_path /
-000019f0: 2050 6174 6828 7374 7228 7965 6172 2929   Path(str(year))
-00001a00: 202f 2050 6174 6828 2753 5441 5449 5354   / Path('STATIST
-00001a10: 4951 5545 5327 2920 2f20 5061 7468 2827  IQUES') / Path('
-00001a20: 7379 6e74 6865 7365 5f61 6468 6572 656e  synthese_adheren
-00001a30: 742e 786c 7378 2729 0d0a 2020 2020 6467  t.xlsx')..    dg
-00001a40: 2e74 6f5f 6578 6365 6c28 6669 6c65 5f6f  .to_excel(file_o
-00001a50: 7574 290d 0a20 2020 200d 0a64 6566 2073  ut)..    ..def s
-00001a60: 796e 7468 6573 655f 7261 6e64 6f6e 6e65  ynthese_randonne
-00001a70: 6528 7965 6172 2c63 7467 5f70 6174 682c  e(year,ctg_path,
-00001a80: 7479 7065 5f73 656a 6f75 7229 3a0d 0a0d  type_sejour):...
-00001a90: 0a20 2020 2023 2053 7461 6e64 6172 6420  .    # Standard 
-00001aa0: 6c69 6272 6172 7920 696d 706f 7274 730d  library imports.
-00001ab0: 0a20 2020 2066 726f 6d20 7061 7468 6c69  .    from pathli
-00001ac0: 6220 696d 706f 7274 2050 6174 680d 0a20  b import Path.. 
-00001ad0: 2020 200d 0a20 2020 2023 2054 6869 7264     ..    # Third
-00001ae0: 2070 6172 7479 2069 6d70 6f72 7473 0d0a   party imports..
-00001af0: 2020 2020 696d 706f 7274 206d 6174 706c      import matpl
-00001b00: 6f74 6c69 622e 7079 706c 6f74 2061 7320  otlib.pyplot as 
-00001b10: 706c 740d 0a20 2020 2069 6d70 6f72 7420  plt..    import 
-00001b20: 7061 6e64 6173 2061 7320 7064 0d0a 2020  pandas as pd..  
-00001b30: 2020 0d0a 2020 2020 2320 496e 7465 726e    ..    # Intern
-00001b40: 616c 2069 6d70 6f72 7473 0d0a 2020 2020  al imports..    
-00001b50: 6672 6f6d 2043 5447 5f55 7469 6c73 2e43  from CTG_Utils.C
-00001b60: 5447 5f46 756e 632e 4354 475f 7574 696c  TG_Func.CTG_util
-00001b70: 6974 7920 696d 706f 7274 2067 6574 5f63  ity import get_c
-00001b80: 6f75 745f 746f 7461 6c0d 0a20 2020 200d  out_total..    .
-00001b90: 0a20 2020 2064 6566 2061 6464 6c61 6265  .    def addlabe
-00001ba0: 6c73 2878 2c79 2c6f 6666 7365 7429 3a0d  ls(x,y,offset):.
-00001bb0: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
-00001bc0: 6e20 7261 6e67 6528 6c65 6e28 7829 293a  n range(len(x)):
-00001bd0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00001be0: 2079 5b69 5d20 213d 2030 3a0d 0a20 2020   y[i] != 0:..   
-00001bf0: 2020 2020 2020 2020 2020 2020 2070 6c74               plt
-00001c00: 2e74 6578 7428 785b 695d 2c79 5b69 5d2b  .text(x[i],y[i]+
-00001c10: 6f66 6673 6574 2c72 6f75 6e64 2879 5b69  offset,round(y[i
-00001c20: 5d2c 3129 2c73 697a 653d 3130 290d 0a20  ],1),size=10).. 
-00001c30: 2020 2020 2020 200d 0a20 2020 200d 0a20         ..    .. 
-00001c40: 2020 2066 696c 655f 696e 203d 2050 6174     file_in = Pat
-00001c50: 6828 6374 675f 7061 7468 2920 2f20 5061  h(ctg_path) / Pa
-00001c60: 7468 2873 7472 2879 6561 7229 2920 2f20  th(str(year)) / 
-00001c70: 5061 7468 2827 5354 4154 4953 5449 5155  Path('STATISTIQU
-00001c80: 4553 2729 202f 2050 6174 6828 2773 796e  ES') / Path('syn
-00001c90: 7468 6573 652e 786c 7378 2729 0d0a 2020  these.xlsx')..  
-00001ca0: 2020 6466 5f74 6f74 616c 203d 2070 642e    df_total = pd.
-00001cb0: 7265 6164 5f65 7863 656c 2866 696c 655f  read_excel(file_
-00001cc0: 696e 290d 0a20 2020 2064 665f 746f 7461  in)..    df_tota
-00001cd0: 6c20 3d20 6466 5f74 6f74 616c 2e64 726f  l = df_total.dro
-00001ce0: 706e 6128 7375 6273 6574 3d5b 274e 6f6d  pna(subset=['Nom
-00001cf0: 275d 2920 0d0a 2020 2020 6467 203d 2064  ']) ..    dg = d
-00001d00: 665f 746f 7461 6c2e 7175 6572 7928 2754  f_total.query('T
-00001d10: 7970 653d 3d40 7479 7065 5f73 656a 6f75  ype==@type_sejou
-00001d20: 7227 292e 6772 6f75 7062 7928 2773 656a  r').groupby('sej
-00001d30: 6f75 7227 292e 6167 6728 2763 6f75 6e74  our').agg('count
-00001d40: 2729 5b27 4ec2 b020 4c69 6365 6e63 69c3  ')['N.. Licenci.
-00001d50: a927 5d0d 0a20 2020 0d0a 2020 2020 6669  .']..   ..    fi
-00001d60: 6c65 5f69 6e66 6f20 3d20 5061 7468 2863  le_info = Path(c
-00001d70: 7467 5f70 6174 6829 202f 2050 6174 6828  tg_path) / Path(
-00001d80: 7374 7228 7965 6172 2929 202f 2050 6174  str(year)) / Pat
-00001d90: 6828 2744 4154 4127 2920 2f20 5061 7468  h('DATA') / Path
-00001da0: 2827 696e 666f 5f72 616e 646f 732e 786c  ('info_randos.xl
-00001db0: 7378 2729 0d0a 2020 2020 636f 7574 5f74  sx')..    cout_t
-00001dc0: 6f74 616c 5f72 616e 646f 203d 2067 6574  otal_rando = get
-00001dd0: 5f63 6f75 745f 746f 7461 6c28 7965 6172  _cout_total(year
-00001de0: 2c74 7970 655f 7365 6a6f 7572 2e6c 6f77  ,type_sejour.low
-00001df0: 6572 2829 2c64 672c 6374 675f 7061 7468  er(),dg,ctg_path
-00001e00: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
-00001e10: 2066 6967 203d 2070 6c74 2e66 6967 7572   fig = plt.figur
-00001e20: 6528 290d 0a20 2020 2070 6c74 2e62 6172  e()..    plt.bar
-00001e30: 2872 616e 6765 286c 656e 2864 6729 292c  (range(len(dg)),
-00001e40: 6467 2e74 6f6c 6973 7428 2929 0d0a 2020  dg.tolist())..  
-00001e50: 2020 6164 646c 6162 656c 7328 6c69 7374    addlabels(list
-00001e60: 2872 616e 6765 286c 656e 2864 6729 2929  (range(len(dg)))
-00001e70: 2c64 672e 746f 6c69 7374 2829 2c30 2e32  ,dg.tolist(),0.2
-00001e80: 290d 0a20 2020 2070 6c74 2e78 7469 636b  )..    plt.xtick
-00001e90: 7328 7261 6e67 6528 6c65 6e28 6467 2929  s(range(len(dg))
-00001ea0: 2c20 6467 2e69 6e64 6578 2c20 726f 7461  , dg.index, rota
-00001eb0: 7469 6f6e 3d27 7665 7274 6963 616c 2729  tion='vertical')
-00001ec0: 0d0a 2020 2020 706c 742e 7469 636b 5f70  ..    plt.tick_p
-00001ed0: 6172 616d 7328 6178 6973 3d27 7827 2c20  arams(axis='x', 
-00001ee0: 726f 7461 7469 6f6e 3d39 302c 206c 6162  rotation=90, lab
-00001ef0: 656c 7369 7a65 3d31 3029 0d0a 2020 2020  elsize=10)..    
-00001f00: 706c 742e 7469 636b 5f70 6172 616d 7328  plt.tick_params(
-00001f10: 6178 6973 3d27 7927 2c6c 6162 656c 7369  axis='y',labelsi
-00001f20: 7a65 3d31 3029 0d0a 2020 2020 0d0a 2020  ze=10)..    ..  
-00001f30: 2020 6966 2074 7970 655f 7365 6a6f 7572    if type_sejour
-00001f40: 203d 3d20 2752 414e 444f 4e4e 4545 273a   == 'RANDONNEE':
-00001f50: 0d0a 2020 2020 2020 2020 5f20 3d20 706c  ..        _ = pl
-00001f60: 742e 7469 746c 6528 6627 2320 7261 6e64  t.title(f'# rand
-00001f70: 6f73 203a 207b 6c65 6e28 6467 297d 202c  os : {len(dg)} ,
-00001f80: 2023 2070 6172 7469 6369 7061 6e74 7320   # participants 
-00001f90: 3a20 7b73 756d 2864 6729 7d2c 2043 6fc3  : {sum(dg)}, Co.
-00001fa0: bb74 203a 207b 636f 7574 5f74 6f74 616c  .t : {cout_total
-00001fb0: 5f72 616e 646f 7d20 e282 ac27 290d 0a20  _rando} ...').. 
-00001fc0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00001fd0: 2020 5f20 3d20 706c 742e 7469 746c 6528    _ = plt.title(
-00001fe0: 6627 2320 7365 6a6f 7572 7320 3a20 7b6c  f'# sejours : {l
-00001ff0: 656e 2864 6729 7d20 2c20 2320 7061 7274  en(dg)} , # part
-00002000: 6963 6970 616e 7473 203a 207b 7375 6d28  icipants : {sum(
-00002010: 6467 297d 2c20 436f c3bb 7420 3a20 7b63  dg)}, Co..t : {c
-00002020: 6f75 745f 746f 7461 6c5f 7261 6e64 6f7d  out_total_rando}
-00002030: 20e2 82ac 2729 2020 2020 0d0a 2020 2020   ...')    ..    
-00002040: 706c 742e 7469 6768 745f 6c61 796f 7574  plt.tight_layout
-00002050: 2829 0d0a 2020 2020 706c 742e 7368 6f77  ()..    plt.show
-00002060: 2829 0d0a 2020 2020 0d0a 6465 6620 6e62  ()..    ..def nb
-00002070: 725f 7365 6a6f 7572 735f 6164 6865 7265  r_sejours_adhere
-00002080: 6e74 2879 6561 722c 2063 7467 5f70 6174  nt(year, ctg_pat
-00002090: 6829 3a0d 0a0d 0a20 2020 2023 2053 7461  h):....    # Sta
-000020a0: 6e64 6172 6420 6c69 6272 6172 7920 696d  ndard library im
-000020b0: 706f 7274 730d 0a20 2020 2066 726f 6d20  ports..    from 
-000020c0: 636f 6c6c 6563 7469 6f6e 7320 696d 706f  collections impo
-000020d0: 7274 2043 6f75 6e74 6572 0d0a 2020 2020  rt Counter..    
-000020e0: 6672 6f6d 2070 6174 686c 6962 2069 6d70  from pathlib imp
-000020f0: 6f72 7420 5061 7468 0d0a 2020 2020 0d0a  ort Path..    ..
-00002100: 2020 2020 2320 5468 6972 6420 7061 7274      # Third part
-00002110: 7920 696d 706f 7274 730d 0a20 2020 2069  y imports..    i
-00002120: 6d70 6f72 7420 6d61 7470 6c6f 746c 6962  mport matplotlib
-00002130: 2e70 7970 6c6f 7420 6173 2070 6c74 0d0a  .pyplot as plt..
-00002140: 2020 2020 696d 706f 7274 2070 616e 6461      import panda
-00002150: 7320 6173 2070 640d 0a20 2020 200d 0a20  s as pd..    .. 
-00002160: 2020 2070 6c74 2e73 7479 6c65 2e75 7365     plt.style.use
-00002170: 2827 6767 706c 6f74 2729 0d0a 2020 2020  ('ggplot')..    
-00002180: 0d0a 2020 2020 2320 6675 6e63 7469 6f6e  ..    # function
-00002190: 2074 6f20 6164 6420 7661 6c75 6520 6c61   to add value la
-000021a0: 6265 6c73 0d0a 2020 2020 6465 6620 6164  bels..    def ad
-000021b0: 646c 6162 656c 7328 782c 7929 3a0d 0a20  dlabels(x,y):.. 
-000021c0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-000021d0: 7261 6e67 6528 6c65 6e28 7829 293a 0d0a  range(len(x)):..
-000021e0: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
-000021f0: 7465 7874 2878 5b69 5d2d 302e 322c 795b  text(x[i]-0.2,y[
-00002200: 695d 2b31 2c79 5b69 5d2c 7369 7a65 3d6c  i]+1,y[i],size=l
-00002210: 6162 656c 5f73 697a 6529 0d0a 2020 2020  abel_size)..    
-00002220: 6c61 6265 6c5f 7369 7a65 203d 2031 350d  label_size = 15.
-00002230: 0a20 2020 2066 696c 655f 696e 203d 2063  .    file_in = c
-00002240: 7467 5f70 6174 6820 2f20 5061 7468 2873  tg_path / Path(s
-00002250: 7472 2879 6561 7229 2920 2f20 5061 7468  tr(year)) / Path
-00002260: 2827 5354 4154 4953 5449 5155 4553 2729  ('STATISTIQUES')
-00002270: 202f 2050 6174 6828 2773 796e 7468 6573   / Path('synthes
-00002280: 655f 6164 6865 7265 6e74 2e78 6c73 7827  e_adherent.xlsx'
-00002290: 290d 0a20 2020 2064 665f 746f 7461 6c20  )..    df_total 
-000022a0: 3d20 7064 2e72 6561 645f 6578 6365 6c28  = pd.read_excel(
-000022b0: 6669 6c65 5f69 6e29 0d0a 2020 2020 0d0a  file_in)..    ..
-000022c0: 2020 2020 6320 3d20 436f 756e 7465 7228      c = Counter(
-000022d0: 290d 0a20 2020 2063 203d 2043 6f75 6e74  )..    c = Count
-000022e0: 6572 2864 665f 746f 7461 6c5b 274e 6272  er(df_total['Nbr
-000022f0: 5f53 454a 4f55 5253 275d 2e74 6f6c 6973  _SEJOURS'].tolis
-00002300: 7428 2929 0d0a 2020 2020 6320 3d20 632e  t())..    c = c.
-00002310: 6d6f 7374 5f63 6f6d 6d6f 6e28 290d 0a0d  most_common()...
-00002320: 0a20 2020 2078 2c20 7920 3d20 7a69 7028  .    x, y = zip(
-00002330: 2a63 290d 0a20 2020 2078 203d 206c 6973  *c)..    x = lis
-00002340: 7428 7829 0d0a 2020 2020 7920 3d20 6c69  t(x)..    y = li
-00002350: 7374 2879 290d 0a20 2020 200d 0a20 2020  st(y)..    ..   
-00002360: 2066 6967 2c20 6178 203d 2070 6c74 2e73   fig, ax = plt.s
-00002370: 7562 706c 6f74 7328 6669 6773 697a 653d  ubplots(figsize=
-00002380: 2835 2c35 2929 0d0a 2020 2020 706c 742e  (5,5))..    plt.
-00002390: 6261 7228 5b73 7472 2878 5f73 2920 666f  bar([str(x_s) fo
-000023a0: 7220 785f 7320 696e 2078 5d2c 7929 0d0a  r x_s in x],y)..
-000023b0: 2020 2020 706c 742e 786c 6162 656c 2827      plt.xlabel('
-000023c0: 4e6f 6d62 7265 2064 6520 7061 7274 6963  Nombre de partic
-000023d0: 6970 6174 696f 6e20 c3a0 2064 6573 2073  ipation .. des s
-000023e0: c3a9 6a6f 7572 7327 290d 0a20 2020 2070  ..jours')..    p
-000023f0: 6c74 2e79 6c61 6265 6c28 274e 6f6d 6272  lt.ylabel('Nombr
-00002400: 6520 6465 206c 6963 656e 6369 6572 7327  e de licenciers'
-00002410: 290d 0a20 2020 2070 6c74 2e74 6963 6b5f  )..    plt.tick_
-00002420: 7061 7261 6d73 2861 7869 733d 2778 272c  params(axis='x',
-00002430: 206c 6162 656c 7369 7a65 3d6c 6162 656c   labelsize=label
-00002440: 5f73 697a 6529 0d0a 2020 2020 706c 742e  _size)..    plt.
-00002450: 7469 636b 5f70 6172 616d 7328 6178 6973  tick_params(axis
-00002460: 3d27 7927 2c20 6c61 6265 6c73 697a 653d  ='y', labelsize=
-00002470: 6c61 6265 6c5f 7369 7a65 290d 0a20 2020  label_size)..   
-00002480: 2070 6c74 2e74 6974 6c65 2873 7472 2879   plt.title(str(y
-00002490: 6561 7229 2c70 6164 3d32 302c 2066 6f6e  ear),pad=20, fon
-000024a0: 7473 697a 653d 3230 290d 0a20 2020 200d  tsize=20)..    .
-000024b0: 0a20 2020 2061 782e 7365 745f 786c 6162  .    ax.set_xlab
-000024c0: 656c 2827 4e20 73c3 a96a 6f75 7273 272c  el('N s..jours',
-000024d0: 2066 6f6e 7473 697a 6520 3d20 6c61 6265   fontsize = labe
-000024e0: 6c5f 7369 7a65 290d 0a20 2020 2061 782e  l_size)..    ax.
-000024f0: 7365 745f 796c 6162 656c 2827 4e6f 6d62  set_ylabel('Nomb
-00002500: 7265 2064 6520 4354 4720 6179 616e 7420  re de CTG ayant 
-00002510: 5c6e 2070 6172 7469 6369 70c3 a920 c3a0  \n particip.. ..
-00002520: 204e 2073 c3a9 6a6f 7572 7327 2c20 666f   N s..jours', fo
-00002530: 6e74 7369 7a65 203d 206c 6162 656c 5f73  ntsize = label_s
-00002540: 697a 6529 0d0a 2020 2020 0d0a 2020 2020  ize)..    ..    
-00002550: 782e 736f 7274 2829 0d0a 2020 2020 6164  x.sort()..    ad
-00002560: 646c 6162 656c 7328 782c 7929 0d0a 2020  dlabels(x,y)..  
-00002570: 2020 706c 742e 7469 6768 745f 6c61 796f    plt.tight_layo
-00002580: 7574 2829 0d0a 2020 2020 706c 742e 7368  ut()..    plt.sh
-00002590: 6f77 2829 0d0a 0d0a 2020 2020 6669 675f  ow()....    fig_
-000025a0: 6669 6c65 203d 2027 5345 4a4f 5552 535f  file = 'SEJOURS_
-000025b0: 5354 4154 5f50 4152 5449 4349 5041 5449  STAT_PARTICIPATI
-000025c0: 4f4e 2e70 6e67 270d 0a20 2020 2070 6c74  ON.png'..    plt
-000025d0: 2e73 6176 6566 6967 2863 7467 5f70 6174  .savefig(ctg_pat
-000025e0: 6820 2f20 5061 7468 2873 7472 2879 6561  h / Path(str(yea
-000025f0: 7229 2920 2f20 5061 7468 2827 5354 4154  r)) / Path('STAT
-00002600: 4953 5449 5155 4553 2729 202f 2050 6174  ISTIQUES') / Pat
-00002610: 6828 6669 675f 6669 6c65 292c 6262 6f78  h(fig_file),bbox
-00002620: 5f69 6e63 6865 733d 2774 6967 6874 2729  _inches='tight')
-00002630: 0d0a 2020 2020 0d0a 6465 6620 7265 6164  ..    ..def read
-00002640: 5f6d 656d 6f72 795f 736f 7274 6965 7328  _memory_sorties(
-00002650: 293a 0d0a 0d0a 2020 2020 2320 5374 616e  ):....    # Stan
-00002660: 6461 7264 206c 6962 7261 7279 2069 6d70  dard library imp
-00002670: 6f72 7473 0d0a 2020 2020 696d 706f 7274  orts..    import
-00002680: 206f 732e 7061 7468 0d0a 2020 2020 6672   os.path..    fr
-00002690: 6f6d 2070 6174 686c 6962 2069 6d70 6f72  om pathlib impor
-000026a0: 7420 5061 7468 0d0a 0d0a 2020 2020 2320  t Path....    # 
-000026b0: 3372 6420 7061 7274 7920 696d 706f 7274  3rd party import
-000026c0: 730d 0a20 2020 2069 6d70 6f72 7420 7961  s..    import ya
-000026d0: 6d6c 0d0a 2020 2020 0d0a 2020 2020 2320  ml..    ..    # 
-000026e0: 5265 6164 7320 7468 6520 6465 6661 756c  Reads the defaul
-000026f0: 7420 5056 6368 6172 6163 7465 7269 7a61  t PVcharacteriza
-00002700: 7469 6f6e 2e79 616d 6c20 636f 6e66 6967  tion.yaml config
-00002710: 2066 696c 650d 0a20 2020 2070 6174 685f   file..    path_
-00002720: 636f 6e66 6967 5f66 696c 6520 3d20 5061  config_file = Pa
-00002730: 7468 285f 5f66 696c 655f 5f29 2e70 6172  th(__file__).par
-00002740: 656e 742e 7061 7265 6e74 202f 2050 6174  ent.parent / Pat
-00002750: 6828 2743 5447 5f46 756e 6327 2920 2f20  h('CTG_Func') / 
-00002760: 5061 7468 2827 4354 475f 5265 6646 696c  Path('CTG_RefFil
-00002770: 6573 2729 202f 2050 6174 6828 276d 656d  es') / Path('mem
-00002780: 6f72 795f 736f 7274 6965 732e 796d 6c27  ory_sorties.yml'
-00002790: 290d 0a20 2020 2077 6974 6820 6f70 656e  )..    with open
-000027a0: 2870 6174 685f 636f 6e66 6967 5f66 696c  (path_config_fil
-000027b0: 6529 2061 7320 6669 6c65 3a0d 0a20 2020  e) as file:..   
-000027c0: 2020 2020 206d 656d 6f72 7920 3d20 7961       memory = ya
-000027d0: 6d6c 2e73 6166 655f 6c6f 6164 2866 696c  ml.safe_load(fil
-000027e0: 6529 0d0a 2020 2020 2020 2020 0d0a 2020  e)..        ..  
-000027f0: 2020 2020 200d 0a20 2020 2072 6574 7572       ..    retur
-00002800: 6e20 6d65 6d6f 7279 0d0a 2020 2020 0d0a  n memory..    ..
-00002810: 6465 6620 6576 6f6c 7574 696f 6e5f 736f  def evolution_so
-00002820: 7274 6965 7328 7479 7065 2c63 7467 5f70  rties(type,ctg_p
-00002830: 6174 6829 3a0d 0a0d 0a20 2020 2023 2053  ath):....    # S
-00002840: 7461 6e64 6172 6420 6c69 6272 6172 7920  tandard library 
-00002850: 696d 706f 7274 2020 2020 0d0a 2020 2020  import    ..    
-00002860: 696d 706f 7274 2064 6174 6574 696d 650d  import datetime.
-00002870: 0a20 2020 2066 726f 6d20 7061 7468 6c69  .    from pathli
-00002880: 6220 696d 706f 7274 2050 6174 680d 0a20  b import Path.. 
-00002890: 2020 2066 726f 6d20 636f 6c6c 6563 7469     from collecti
-000028a0: 6f6e 7320 696d 706f 7274 206e 616d 6564  ons import named
-000028b0: 7475 706c 650d 0a0d 0a20 2020 2023 2054  tuple....    # T
-000028c0: 6869 7264 2070 6172 7479 206c 6962 7261  hird party libra
-000028d0: 7279 2069 6d70 6f72 7420 2020 2020 0d0a  ry import     ..
-000028e0: 2020 2020 696d 706f 7274 206d 6174 706c      import matpl
-000028f0: 6f74 6c69 622e 7079 706c 6f74 2061 7320  otlib.pyplot as 
-00002900: 706c 740d 0a20 2020 2069 6d70 6f72 7420  plt..    import 
-00002910: 7061 6e64 6173 2061 7320 7064 0d0a 2020  pandas as pd..  
-00002920: 2020 2020 0d0a 2020 2020 2320 496e 7465      ..    # Inte
-00002930: 726e 616c 2069 6d70 6f72 740d 0a20 2020  rnal import..   
-00002940: 2069 6d70 6f72 7420 4354 475f 5574 696c   import CTG_Util
-00002950: 7320 6173 2063 7467 0d0a 2020 2020 6672  s as ctg..    fr
-00002960: 6f6d 2043 5447 5f55 7469 6c73 2e43 5447  om CTG_Utils.CTG
-00002970: 5f47 5549 2e47 5549 5f47 6c6f 6261 6c73  _GUI.GUI_Globals
-00002980: 2069 6d70 6f72 7420 4143 5449 5649 5445   import ACTIVITE
-00002990: 5f4c 4953 5420 0d0a 2020 2020 0d0a 2020  _LIST ..    ..  
-000029a0: 2020 6465 6620 6164 645f 6d65 6d6f 7279    def add_memory
-000029b0: 2873 7461 745f 6469 632c 7965 6172 7329  (stat_dic,years)
-000029c0: 3a0d 0a20 2020 2020 2020 206d 656d 6f72  :..        memor
-000029d0: 7920 3d20 7265 6164 5f6d 656d 6f72 795f  y = read_memory_
-000029e0: 736f 7274 6965 7328 290d 0a20 2020 200d  sorties()..    .
-000029f0: 0a20 2020 200d 0a20 2020 2020 2020 2066  .    ..        f
-00002a00: 6f72 2079 6561 722c 7620 696e 206d 656d  or year,v in mem
-00002a10: 6f72 795b 276d 656d 6f72 7927 5d2e 6974  ory['memory'].it
-00002a20: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
-00002a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a50: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00002a60: 2073 7461 745f 6469 635b 7374 7228 7965   stat_dic[str(ye
-00002a70: 6172 295d 203d 2073 7461 7479 6561 7228  ar)] = statyear(
-00002a80: 765b 2750 4152 5449 4349 5041 5449 4f4e  v['PARTICIPATION
-00002a90: 5f53 454a 4f55 5253 275d 2c20 2020 2020  _SEJOURS'],     
-00002aa0: 2020 2020 2020 2020 2020 2023 206e 6272             # nbr
-00002ab0: 5f73 656a 6f75 7273 0d0a 2020 2020 2020  _sejours..      
-00002ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ae0: 2020 2020 2030 2c20 2020 2020 2020 2020       0,         
-00002af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b00: 2023 206a 6f75 7273 5f73 656a 6f75 720d   # jours_sejour.
-00002b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b30: 2020 2020 2020 2020 2020 2020 765b 2753              v['S
-00002b40: 4f52 5449 4553 5f43 4c55 425f 4449 4d41  ORTIES_CLUB_DIMA
-00002b50: 4e43 4845 275d 2c20 2320 736f 7274 6965  NCHE'], # sortie
-00002b60: 5f64 696d 616e 6368 655f 636c 7562 0d0a  _dimanche_club..
-00002b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b90: 2020 2020 2020 2020 2020 2076 5b27 534f             v['SO
-00002ba0: 5254 4945 535f 434c 5542 5f53 414d 4544  RTIES_CLUB_SAMED
-00002bb0: 4927 5d2c 2020 2023 2073 6f72 7469 655f  I'],   # sortie_
-00002bc0: 7361 6d65 6469 5f63 6c75 620d 0a20 2020  samedi_club..   
-00002bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bf0: 2020 2020 2020 2020 765b 2753 4f52 5449          v['SORTI
-00002c00: 4553 5f48 4956 4552 275d 2c20 2020 2020  ES_HIVER'],     
-00002c10: 2020 2020 2320 736f 7274 6965 5f68 6976      # sortie_hiv
-00002c20: 6572 5f63 6c75 620d 0a20 2020 2020 2020  er_club..       
-00002c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c50: 2020 2020 765b 2753 4f52 5449 4553 5f43      v['SORTIES_C
-00002c60: 4c55 425f 4a45 5544 4927 5d2c 2020 2020  LUB_JEUDI'],    
-00002c70: 2320 736f 7274 6965 5f6a 6575 6469 5f63  # sortie_jeudi_c
-00002c80: 6c75 620d 0a20 2020 2020 2020 2020 2020  lub..           
-00002c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000000: 5f5f 616c 6c5f 5f20 3d5b 2765 766f 6c75  __all__ =['evolu
+00000010: 7469 6f6e 5f73 6f72 7469 6573 272c 0d0a  tion_sorties',..
+00000020: 2020 2020 2020 2020 2020 276e 6272 5f73            'nbr_s
+00000030: 656a 6f75 7273 5f61 6468 6572 656e 7427  ejours_adherent'
+00000040: 2c0d 0a20 2020 2020 2020 2020 2027 706c  ,..          'pl
+00000050: 6f74 5f70 6965 5f73 796e 7468 6573 6527  ot_pie_synthese'
+00000060: 2c0d 0a20 2020 2020 2020 2020 2027 7379  ,..          'sy
+00000070: 6e74 6865 7365 272c 0d0a 2020 2020 2020  nthese',..      
+00000080: 2020 2020 2773 796e 7468 6573 655f 6164      'synthese_ad
+00000090: 6865 7265 6e74 272c 0d0a 2020 2020 2020  herent',..      
+000000a0: 2020 2020 2773 796e 7468 6573 655f 7261      'synthese_ra
+000000b0: 6e64 6f6e 6e65 6527 2c0d 0a20 2020 2020  ndonnee',..     
+000000c0: 2020 2020 205d 0d0a 0d0a 2320 5374 616e       ]....# Stan
+000000d0: 6461 7264 206c 6962 7261 7279 2069 6d70  dard library imp
+000000e0: 6f72 7473 0d0a 696d 706f 7274 2064 6174  orts..import dat
+000000f0: 6574 696d 650d 0a69 6d70 6f72 7420 7061  etime..import pa
+00000100: 7468 6c69 620d 0a69 6d70 6f72 7420 6f73  thlib..import os
+00000110: 0d0a 696d 706f 7274 206f 732e 7061 7468  ..import os.path
+00000120: 0d0a 6672 6f6d 2063 6f6c 6c65 6374 696f  ..from collectio
+00000130: 6e73 2069 6d70 6f72 7420 436f 756e 7465  ns import Counte
+00000140: 720d 0a66 726f 6d20 636f 6c6c 6563 7469  r..from collecti
+00000150: 6f6e 7320 696d 706f 7274 206e 616d 6564  ons import named
+00000160: 7475 706c 650d 0a66 726f 6d20 7061 7468  tuple..from path
+00000170: 6c69 6220 696d 706f 7274 2050 6174 680d  lib import Path.
+00000180: 0a0d 0a23 2054 6869 7264 2070 6172 7479  ...# Third party
+00000190: 2069 6d70 6f72 7473 0d0a 696d 706f 7274   imports..import
+000001a0: 206d 6174 706c 6f74 6c69 622e 7079 706c   matplotlib.pypl
+000001b0: 6f74 2061 7320 706c 740d 0a69 6d70 6f72  ot as plt..impor
+000001c0: 7420 6e75 6d70 7920 6173 206e 700d 0a69  t numpy as np..i
+000001d0: 6d70 6f72 7420 7061 6e64 6173 2061 7320  mport pandas as 
+000001e0: 7064 0d0a 696d 706f 7274 2079 616d 6c0d  pd..import yaml.
+000001f0: 0a0d 0a23 2049 6e74 6572 6e61 6c20 696d  ...# Internal im
+00000200: 706f 7274 730d 0a66 726f 6d20 6374 6775  ports..from ctgu
+00000210: 7469 6c73 2e63 7467 6775 692e 6775 6967  tils.ctggui.guig
+00000220: 6c6f 6261 6c73 2069 6d70 6f72 7420 4143  lobals import AC
+00000230: 5449 5649 5445 5f4c 4953 540d 0a66 726f  TIVITE_LIST..fro
+00000240: 6d20 6374 6775 7469 6c73 2e63 7467 6675  m ctgutils.ctgfu
+00000250: 6e63 7473 2e63 7467 5f63 6c61 7373 6573  ncts.ctg_classes
+00000260: 2069 6d70 6f72 7420 4566 6665 6374 6966   import Effectif
+00000270: 4374 670d 0a66 726f 6d20 6374 6775 7469  Ctg..from ctguti
+00000280: 6c73 2e63 7467 6675 6e63 7473 2e63 7467  ls.ctgfuncts.ctg
+00000290: 5f74 6f6f 6c73 2069 6d70 6f72 7420 6765  _tools import ge
+000002a0: 745f 636f 7574 5f74 6f74 616c 0d0a 6672  t_cout_total..fr
+000002b0: 6f6d 2063 7467 7574 696c 732e 6374 6766  om ctgutils.ctgf
+000002c0: 756e 6374 732e 6374 675f 6566 6665 6374  uncts.ctg_effect
+000002d0: 6966 2069 6d70 6f72 7420 7265 6164 5f65  if import read_e
+000002e0: 6666 6563 7469 665f 636f 7272 6563 7465  ffectif_correcte
+000002f0: 640d 0a66 726f 6d20 6374 6775 7469 6c73  d..from ctgutils
+00000300: 2e63 7467 6675 6e63 7473 2e63 7467 5f74  .ctgfuncts.ctg_t
+00000310: 6f6f 6c73 2069 6d70 6f72 7420 6765 745f  ools import get_
+00000320: 7365 6a6f 7572 5f69 6e66 6f0d 0a0d 0a64  sejour_info....d
+00000330: 6566 2073 796e 7468 6573 6528 7965 6172  ef synthese(year
+00000340: 3a73 7472 2c63 7467 5f70 6174 683a 7061  :str,ctg_path:pa
+00000350: 7468 6c69 622e 5769 6e64 6f77 7350 6174  thlib.WindowsPat
+00000360: 6829 2d3e 4e6f 6e65 3a0d 0a0d 0a20 2020  h)->None:....   
+00000370: 2070 6174 685f 6469 725f 6c69 7374 203d   path_dir_list =
+00000380: 205b 6374 675f 7061 7468 202f 2050 6174   [ctg_path / Pat
+00000390: 6828 7965 6172 2920 2f20 5061 7468 2827  h(year) / Path('
+000003a0: 534f 5254 4945 5320 4455 2053 414d 4544  SORTIES DU SAMED
+000003b0: 4927 2920 2f20 5061 7468 2827 4558 4345  I') / Path('EXCE
+000003c0: 4c27 292c 0d0a 2020 2020 2020 2020 2020  L'),..          
+000003d0: 2020 2020 2020 2020 2020 2063 7467 5f70             ctg_p
+000003e0: 6174 6820 2f20 5061 7468 2879 6561 7229  ath / Path(year)
+000003f0: 202f 2050 6174 6828 2753 4f52 5449 4553   / Path('SORTIES
+00000400: 2044 5520 4449 4d41 4e43 4845 2729 202f   DU DIMANCHE') /
+00000410: 2050 6174 6828 2745 5843 454c 2729 2c0d   Path('EXCEL'),.
+00000420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000430: 2020 2020 2020 6374 675f 7061 7468 202f        ctg_path /
+00000440: 2050 6174 6828 7965 6172 2920 2f20 5061   Path(year) / Pa
+00000450: 7468 2827 534f 5254 4945 5320 4455 204a  th('SORTIES DU J
+00000460: 4555 4449 2729 202f 2050 6174 6828 2745  EUDI') / Path('E
+00000470: 5843 454c 2729 2c0d 0a20 2020 2020 2020  XCEL'),..       
+00000480: 2020 2020 2020 2020 2020 2020 2020 6374                ct
+00000490: 675f 7061 7468 202f 2050 6174 6828 7965  g_path / Path(ye
+000004a0: 6172 2920 2f20 5061 7468 2827 534f 5254  ar) / Path('SORT
+000004b0: 4945 5320 4849 5645 5227 2920 2f20 5061  IES HIVER') / Pa
+000004c0: 7468 2827 4558 4345 4c27 292c 0d0a 2020  th('EXCEL'),..  
+000004d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000004e0: 2020 2063 7467 5f70 6174 6820 2f20 5061     ctg_path / Pa
+000004f0: 7468 2879 6561 7229 202f 2050 6174 6828  th(year) / Path(
+00000500: 2753 4f52 5449 4553 2044 5520 4c55 4e44  'SORTIES DU LUND
+00000510: 4927 292f 2050 6174 6828 2745 5843 454c  I')/ Path('EXCEL
+00000520: 2729 2c0d 0a20 2020 2020 2020 2020 2020  '),..           
+00000530: 2020 2020 2020 2020 2020 6374 675f 7061            ctg_pa
+00000540: 7468 202f 2050 6174 6828 7965 6172 2920  th / Path(year) 
+00000550: 2f20 5061 7468 2827 5345 4a4f 5552 2729  / Path('SEJOUR')
+00000560: 202f 2050 6174 6828 2745 5843 454c 2729   / Path('EXCEL')
+00000570: 5d0d 0a0d 0a20 2020 206c 6973 745f 6466  ]....    list_df
+00000580: 203d 205b 5d0d 0a20 2020 2066 6f72 2070   = []..    for p
+00000590: 6174 685f 6469 7220 696e 2070 6174 685f  ath_dir in path_
+000005a0: 6469 725f 6c69 7374 3a0d 0a20 2020 2020  dir_list:..     
+000005b0: 2020 2069 6620 6f73 2e70 6174 682e 6973     if os.path.is
+000005c0: 6469 7228 7061 7468 5f64 6972 293a 0d0a  dir(path_dir):..
+000005d0: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+000005e0: 7320 3d20 5b78 2066 6f72 2078 2069 6e20  s = [x for x in 
+000005f0: 6f73 2e6c 6973 7464 6972 2870 6174 685f  os.listdir(path_
+00000600: 6469 7229 2069 6620 782e 656e 6473 7769  dir) if x.endswi
+00000610: 7468 2827 2e78 6c73 7827 2920 616e 6420  th('.xlsx') and 
+00000620: 227e 2422 206e 6f74 2069 6e20 785d 0d0a  "~$" not in x]..
+00000630: 2020 2020 2020 2020 2020 2020 6c69 7374              list
+00000640: 5f64 662e 6578 7465 6e64 285b 7064 2e72  _df.extend([pd.r
+00000650: 6561 645f 6578 6365 6c28 7061 7468 5f64  ead_excel(path_d
+00000660: 6972 202f 2050 6174 6828 6669 6c65 292c  ir / Path(file),
+00000670: 2065 6e67 696e 653d 276f 7065 6e70 7978   engine='openpyx
+00000680: 6c27 2920 666f 7220 6669 6c65 2069 6e20  l') for file in 
+00000690: 6669 6c65 735d 290d 0a0d 0a20 2020 2064  files])....    d
+000006a0: 665f 746f 7461 6c20 3d20 7064 2e63 6f6e  f_total = pd.con
+000006b0: 6361 7428 6c69 7374 5f64 662c 2069 676e  cat(list_df, ign
+000006c0: 6f72 655f 696e 6465 783d 5472 7565 290d  ore_index=True).
+000006d0: 0a0d 0a20 2020 2064 665f 6566 6665 6374  ...    df_effect
+000006e0: 6966 203d 2072 6561 645f 6566 6665 6374  if = read_effect
+000006f0: 6966 5f63 6f72 7265 6374 6564 2863 7467  if_corrected(ctg
+00000700: 5f70 6174 6829 0d0a 0d0a 2020 2020 6466  _path)....    df
+00000710: 5f74 6f74 616c 5b27 5072 6174 6971 7565  _total['Pratique
+00000720: 2056 4145 275d 2e66 696c 6c6e 6128 274e   VAE'].fillna('N
+00000730: 6f6e 272c 696e 706c 6163 653d 5472 7565  on',inplace=True
+00000740: 290d 0a0d 0a20 2020 2023 206e 6f6d 6272  )....    # nombr
+00000750: 6520 6d6f 7965 6e20 6465 2070 6172 7469  e moyen de parti
+00000760: 6369 7061 6e74 2070 6172 2061 6374 6976  cipant par activ
+00000770: 6974 c3a9 0d0a 2020 2020 666f 7220 7820  it....    for x 
+00000780: 696e 2064 665f 746f 7461 6c2e 6772 6f75  in df_total.grou
+00000790: 7062 7928 5b27 5479 7065 275d 293a 0d0a  pby(['Type']):..
+000007a0: 2020 2020 2020 2020 7072 696e 7428 785b          print(x[
+000007b0: 305d 2c6c 656e 2878 5b31 5d29 2c6c 656e  0],len(x[1]),len
+000007c0: 2873 6574 2878 5b31 5d5b 2773 656a 6f75  (set(x[1]['sejou
+000007d0: 7227 5d29 292c 6c65 6e28 785b 315d 292f  r'])),len(x[1])/
+000007e0: 6c65 6e28 7365 7428 785b 315d 5b27 7365  len(set(x[1]['se
+000007f0: 6a6f 7572 275d 2929 290d 0a0d 0a20 2020  jour'])))....   
+00000800: 2066 696c 6520 3d20 6374 675f 7061 7468   file = ctg_path
+00000810: 202f 2050 6174 6828 7965 6172 2920 2f20   / Path(year) / 
+00000820: 5061 7468 2827 5354 4154 4953 5449 5155  Path('STATISTIQU
+00000830: 4553 2729 202f 2050 6174 6828 2773 796e  ES') / Path('syn
+00000840: 7468 6573 652e 786c 7378 2729 0d0a 2020  these.xlsx')..  
+00000850: 2020 6466 5f74 6f74 616c 2e74 6f5f 6578    df_total.to_ex
+00000860: 6365 6c28 6669 6c65 290d 0a0d 0a64 6566  cel(file)....def
+00000870: 2070 6c6f 745f 7069 655f 7379 6e74 6865   plot_pie_synthe
+00000880: 7365 2879 6561 723a 7374 722c 6374 675f  se(year:str,ctg_
+00000890: 7061 7468 3a70 6174 686c 6962 2e57 696e  path:pathlib.Win
+000008a0: 646f 7773 5061 7468 292d 3e4e 6f6e 653a  dowsPath)->None:
+000008b0: 0d0a 0d0a 2020 2020 6465 6620 6675 6e63  ....    def func
+000008c0: 2870 6374 2c20 616c 6c76 616c 7565 7329  (pct, allvalues)
+000008d0: 3a0d 0a20 2020 2020 2020 2061 6273 6f6c  :..        absol
+000008e0: 7574 6520 3d20 726f 756e 6428 7063 7420  ute = round(pct 
+000008f0: 2f20 3130 302e 2a6e 702e 7375 6d28 616c  / 100.*np.sum(al
+00000900: 6c76 616c 7565 7329 2c30 290d 0a20 2020  lvalues),0)..   
+00000910: 2020 2020 2023 7265 7475 726e 2022 7b3a       #return "{:
+00000920: 2e31 667d 255c 6e28 7b3a 647d 2922 2e66  .1f}%\n({:d})".f
+00000930: 6f72 6d61 7428 7063 742c 2061 6273 6f6c  ormat(pct, absol
+00000940: 7574 6529 0d0a 2020 2020 2020 2020 7265  ute)..        re
+00000950: 7475 726e 2020 6622 7b69 6e74 2872 6f75  turn  f"{int(rou
+00000960: 6e64 2861 6273 6f6c 7574 652c 3129 297d  nd(absolute,1))}
+00000970: 5c6e 7b72 6f75 6e64 2870 6374 2c31 297d  \n{round(pct,1)}
+00000980: 2025 220d 0a0d 0a20 2020 2066 696c 655f   %"....    file_
+00000990: 696e 203d 2063 7467 5f70 6174 6820 2f20  in = ctg_path / 
+000009a0: 5061 7468 2879 6561 7229 202f 2050 6174  Path(year) / Pat
+000009b0: 6828 2753 5441 5449 5354 4951 5545 5327  h('STATISTIQUES'
+000009c0: 2920 2f20 5061 7468 2827 7379 6e74 6865  ) / Path('synthe
+000009d0: 7365 2e78 6c73 7827 290d 0a20 2020 2064  se.xlsx')..    d
+000009e0: 665f 746f 7461 6c20 3d20 7064 2e72 6561  f_total = pd.rea
+000009f0: 645f 6578 6365 6c28 6669 6c65 5f69 6e29  d_excel(file_in)
+00000a00: 0d0a 2020 2020 6466 5f74 6f74 616c 203d  ..    df_total =
+00000a10: 2064 665f 746f 7461 6c2e 6472 6f70 6e61   df_total.dropna
+00000a20: 2873 7562 7365 743d 5b27 5479 7065 275d  (subset=['Type']
+00000a30: 290d 0a20 2020 2064 665f 746f 7461 6c20  )..    df_total 
+00000a40: 3d20 6466 5f74 6f74 616c 2e64 726f 706e  = df_total.dropn
+00000a50: 6128 7375 6273 6574 3d5b 274e 6f6d 275d  a(subset=['Nom']
+00000a60: 290d 0a0d 0a20 2020 2064 6167 6720 3d20  )....    dagg = 
+00000a70: 6466 5f74 6f74 616c 2e67 726f 7570 6279  df_total.groupby
+00000a80: 2827 5479 7065 2729 5b27 6e62 725f 6a6f  ('Type')['nbr_jo
+00000a90: 7572 7327 5d2e 6167 6728 2773 756d 2729  urs'].agg('sum')
+00000aa0: 0d0a 0d0a 0d0a 0d0a 2020 2020 6578 706c  ........    expl
+00000ab0: 6f64 655f 6469 6320 3d20 7b27 5241 4e44  ode_dic = {'RAND
+00000ac0: 4f4e 4e45 4527 3a30 2e31 2c0d 0a20 2020  ONNEE':0.1,..   
+00000ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ae0: 2753 454a 4f55 5227 3a30 2e30 2c0d 0a20  'SEJOUR':0.0,.. 
+00000af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b00: 2020 2753 4f52 5449 4553 2044 5520 4449    'SORTIES DU DI
+00000b10: 4d41 4e43 4845 273a 302e 322c 0d0a 2020  MANCHE':0.2,..  
+00000b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b30: 2027 534f 5254 4945 5320 4455 204a 4555   'SORTIES DU JEU
+00000b40: 4449 273a 302e 322c 0d0a 2020 2020 2020  DI':0.2,..      
+00000b50: 2020 2020 2020 2020 2020 2020 2027 534f               'SO
+00000b60: 5254 4945 5320 4455 204c 554e 4449 273a  RTIES DU LUNDI':
+00000b70: 302e 322c 0d0a 2020 2020 2020 2020 2020  0.2,..          
+00000b80: 2020 2020 2020 2020 2027 534f 5254 4945           'SORTIE
+00000b90: 5320 4455 2053 414d 4544 4927 3a30 2e32  S DU SAMEDI':0.2
+00000ba0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000bb0: 2020 2020 2020 2753 4f52 5449 4553 2048        'SORTIES H
+00000bc0: 4956 4552 273a 302e 327d 0d0a 0d0a 2020  IVER':0.2}....  
+00000bd0: 2020 6461 7461 203d 205b 5d0d 0a20 2020    data = []..   
+00000be0: 2073 6f72 7469 6573 203d 205b 5d0d 0a20   sorties = [].. 
+00000bf0: 2020 2066 6f72 2074 7970 655f 7365 6a6f     for type_sejo
+00000c00: 7572 2c20 6e62 7220 696e 207a 6970 2864  ur, nbr in zip(d
+00000c10: 6167 672e 696e 6465 782c 6461 6767 2e74  agg.index,dagg.t
+00000c20: 6f6c 6973 7428 2929 3a0d 0a20 2020 2020  olist()):..     
+00000c30: 2020 2069 6620 6e62 7221 3d30 3a0d 0a20     if nbr!=0:.. 
+00000c40: 2020 2020 2020 2020 2020 2064 6174 612e             data.
+00000c50: 6170 7065 6e64 286e 6272 290d 0a20 2020  append(nbr)..   
+00000c60: 2020 2020 2020 2020 2073 6f72 7469 6573           sorties
+00000c70: 2e61 7070 656e 6428 7479 7065 5f73 656a  .append(type_sej
+00000c80: 6f75 7229 0d0a 0d0a 2020 2020 6578 706c  our)....    expl
+00000c90: 6f64 6520 3d20 5b65 7870 6c6f 6465 5f64  ode = [explode_d
+00000ca0: 6963 5b74 7970 5d20 666f 7220 7479 7020  ic[typ] for typ 
+00000cb0: 696e 2073 6f72 7469 6573 5d0d 0a0d 0a0d  in sorties].....
+00000cc0: 0a20 2020 2023 2043 7265 6174 696e 6720  .    # Creating 
+00000cd0: 706c 6f74 0d0a 2020 2020 6669 6720 3d20  plot..    fig = 
+00000ce0: 706c 742e 6669 6775 7265 2866 6967 7369  plt.figure(figsi
+00000cf0: 7a65 203d 2831 302c 2037 2929 0d0a 2020  ze =(10, 7))..  
+00000d00: 2020 5f2c 205f 2c20 6175 746f 7465 7874    _, _, autotext
+00000d10: 7320 3d20 706c 742e 7069 6528 6461 7461  s = plt.pie(data
+00000d20: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d40: 206c 6162 656c 7320 3d20 736f 7274 6965   labels = sortie
+00000d50: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
+00000d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d70: 2020 6175 746f 7063 7420 3d20 6c61 6d62    autopct = lamb
+00000d80: 6461 2070 6374 3a20 6675 6e63 2870 6374  da pct: func(pct
+00000d90: 2c20 6461 7461 292c 0d0a 2020 2020 2020  , data),..      
+00000da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000db0: 2020 2020 2020 2020 6578 706c 6f64 6520          explode 
+00000dc0: 3d20 6578 706c 6f64 652c 0d0a 2020 2020  = explode,..    
+00000dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000de0: 2020 2020 2020 2020 2020 7465 7874 7072            textpr
+00000df0: 6f70 733d 7b27 666f 6e74 7369 7a65 273a  ops={'fontsize':
+00000e00: 2031 387d 290d 0a20 2020 2070 6c74 2e74   18})..    plt.t
+00000e10: 6974 6c65 2879 6561 722c 2070 6164 3d35  itle(year, pad=5
+00000e20: 302c 2066 6f6e 7473 697a 653d 3230 290d  0, fontsize=20).
+00000e30: 0a0d 0a20 2020 205f 203d 2070 6c74 2e73  ...    _ = plt.s
+00000e40: 6574 7028 6175 746f 7465 7874 732c 202a  etp(autotexts, *
+00000e50: 2a7b 2763 6f6c 6f72 273a 276b 272c 2027  *{'color':'k', '
+00000e60: 7765 6967 6874 273a 2762 6f6c 6427 2c20  weight':'bold', 
+00000e70: 2766 6f6e 7473 697a 6527 3a31 347d 290d  'fontsize':14}).
+00000e80: 0a0d 0a20 2020 2070 6c74 2e74 6967 6874  ...    plt.tight
+00000e90: 5f6c 6179 6f75 7428 290d 0a20 2020 2070  _layout()..    p
+00000ea0: 6c74 2e73 686f 7728 290d 0a0d 0a20 2020  lt.show()....   
+00000eb0: 2066 6967 5f66 696c 6520 3d20 2753 4f52   fig_file = 'SOR
+00000ec0: 5449 4553 5f50 4945 2e70 6e67 270d 0a20  TIES_PIE.png'.. 
+00000ed0: 2020 2070 6c74 2e73 6176 6566 6967 2863     plt.savefig(c
+00000ee0: 7467 5f70 6174 6820 2f20 5061 7468 2879  tg_path / Path(y
+00000ef0: 6561 7229 202f 2050 6174 6828 2753 5441  ear) / Path('STA
+00000f00: 5449 5354 4951 5545 5327 2920 2f20 5061  TISTIQUES') / Pa
+00000f10: 7468 2866 6967 5f66 696c 6529 2c62 626f  th(fig_file),bbo
+00000f20: 785f 696e 6368 6573 3d27 7469 6768 7427  x_inches='tight'
+00000f30: 290d 0a0d 0a0d 0a0d 0a64 6566 2073 796e  )........def syn
+00000f40: 7468 6573 655f 6164 6865 7265 6e74 2879  these_adherent(y
+00000f50: 6561 723a 7374 722c 6374 675f 7061 7468  ear:str,ctg_path
+00000f60: 3a70 6174 686c 6962 2e57 696e 646f 7773  :pathlib.Windows
+00000f70: 5061 7468 293a 0d0a 0d0a 2020 2020 6669  Path):....    fi
+00000f80: 6c65 5f69 6e20 3d20 6374 675f 7061 7468  le_in = ctg_path
+00000f90: 202f 2050 6174 6828 7965 6172 2920 2f20   / Path(year) / 
+00000fa0: 5061 7468 2827 5354 4154 4953 5449 5155  Path('STATISTIQU
+00000fb0: 4553 2729 202f 2050 6174 6828 2773 796e  ES') / Path('syn
+00000fc0: 7468 6573 652e 786c 7378 2729 0d0a 2020  these.xlsx')..  
+00000fd0: 2020 6466 5f74 6f74 616c 203d 2070 642e    df_total = pd.
+00000fe0: 7265 6164 5f65 7863 656c 2866 696c 655f  read_excel(file_
+00000ff0: 696e 290d 0a20 2020 2064 665f 746f 7461  in)..    df_tota
+00001000: 6c20 3d20 6466 5f74 6f74 616c 2e64 726f  l = df_total.dro
+00001010: 706e 6128 7375 6273 6574 3d5b 2754 7970  pna(subset=['Typ
+00001020: 6527 5d29 0d0a 2020 2020 6e62 7265 203d  e'])..    nbre =
+00001030: 207b 7d0d 0a0d 0a20 2020 2066 6f72 2069   {}....    for i
+00001040: 645f 6c69 6365 6e63 652c 2064 6720 696e  d_licence, dg in
+00001050: 2064 665f 746f 7461 6c2e 6772 6f75 7062   df_total.groupb
+00001060: 7928 274e c2b0 204c 6963 656e 6369 c3a9  y('N.. Licenci..
+00001070: 2729 3a0d 0a0d 0a20 2020 2020 2020 206e  '):....        n
+00001080: 6272 655b 6964 5f6c 6963 656e 6365 5d3d  bre[id_licence]=
+00001090: 5b64 675b 274e 6f6d 275d 2e75 6e69 7175  [dg['Nom'].uniqu
+000010a0: 6528 295b 305d 2c64 675b 2750 72c3 a96e  e()[0],dg['Pr..n
+000010b0: 6f6d 275d 2e75 6e69 7175 6528 295b 305d  om'].unique()[0]
+000010c0: 5d0d 0a0d 0a20 2020 2020 2020 206e 625f  ]....        nb_
+000010d0: 736f 7274 6965 5f64 696d 616e 6368 6520  sortie_dimanche 
+000010e0: 3d20 6c65 6e28 6467 2e71 7565 7279 2822  = len(dg.query("
+000010f0: 5479 7065 2e73 7472 2e63 6f6e 7461 696e  Type.str.contain
+00001100: 7328 2753 4f52 5449 4553 2044 5520 4449  s('SORTIES DU DI
+00001110: 4d41 4e43 4845 2729 2229 290d 0a20 2020  MANCHE')"))..   
+00001120: 2020 2020 206e 6272 655b 6964 5f6c 6963       nbre[id_lic
+00001130: 656e 6365 5d20 3d20 6e62 7265 5b69 645f  ence] = nbre[id_
+00001140: 6c69 6365 6e63 655d 202b 205b 6e62 5f73  licence] + [nb_s
+00001150: 6f72 7469 655f 6469 6d61 6e63 6865 5d0d  ortie_dimanche].
+00001160: 0a0d 0a20 2020 2020 2020 206e 625f 736f  ...        nb_so
+00001170: 7274 6965 5f73 616d 6564 6920 3d20 6c65  rtie_samedi = le
+00001180: 6e28 6467 2e71 7565 7279 2822 5479 7065  n(dg.query("Type
+00001190: 2e73 7472 2e63 6f6e 7461 696e 7328 2753  .str.contains('S
+000011a0: 4f52 5449 4553 2044 5520 5341 4d45 4449  ORTIES DU SAMEDI
+000011b0: 2729 2229 290d 0a20 2020 2020 2020 206e  ')"))..        n
+000011c0: 6272 655b 6964 5f6c 6963 656e 6365 5d20  bre[id_licence] 
+000011d0: 3d20 6e62 7265 5b69 645f 6c69 6365 6e63  = nbre[id_licenc
+000011e0: 655d 202b 205b 6e62 5f73 6f72 7469 655f  e] + [nb_sortie_
+000011f0: 7361 6d65 6469 5d0d 0a0d 0a20 2020 2020  samedi]....     
+00001200: 2020 206e 625f 736f 7274 6965 5f6a 6575     nb_sortie_jeu
+00001210: 6469 203d 206c 656e 2864 672e 7175 6572  di = len(dg.quer
+00001220: 7928 2254 7970 652e 7374 722e 636f 6e74  y("Type.str.cont
+00001230: 6169 6e73 2827 534f 5254 4945 5320 4455  ains('SORTIES DU
+00001240: 204a 4555 4449 2729 2229 290d 0a20 2020   JEUDI')"))..   
+00001250: 2020 2020 206e 6272 655b 6964 5f6c 6963       nbre[id_lic
+00001260: 656e 6365 5d20 3d20 6e62 7265 5b69 645f  ence] = nbre[id_
+00001270: 6c69 6365 6e63 655d 202b 205b 6e62 5f73  licence] + [nb_s
+00001280: 6f72 7469 655f 6a65 7564 695d 0d0a 0d0a  ortie_jeudi]....
+00001290: 2020 2020 2020 2020 6e62 5f72 616e 646f          nb_rando
+000012a0: 203d 206c 656e 2864 672e 7175 6572 7928   = len(dg.query(
+000012b0: 2254 7970 652e 7374 722e 636f 6e74 6169  "Type.str.contai
+000012c0: 6e73 2827 5241 4e44 4f4e 4e45 4527 2922  ns('RANDONNEE')"
+000012d0: 2929 0d0a 2020 2020 2020 2020 6e62 7265  ))..        nbre
+000012e0: 5b69 645f 6c69 6365 6e63 655d 203d 206e  [id_licence] = n
+000012f0: 6272 655b 6964 5f6c 6963 656e 6365 5d20  bre[id_licence] 
+00001300: 2b20 5b6e 625f 7261 6e64 6f5d 0d0a 0d0a  + [nb_rando]....
+00001310: 2020 2020 2020 2020 6e62 5f73 656a 6f75          nb_sejou
+00001320: 725f 6a6f 7572 7320 3d20 7375 6d28 6467  r_jours = sum(dg
+00001330: 2e71 7565 7279 2822 5479 7065 2e73 7472  .query("Type.str
+00001340: 2e63 6f6e 7461 696e 7328 2753 454a 4f55  .contains('SEJOU
+00001350: 5227 2922 295b 276e 6272 5f6a 6f75 7273  R')")['nbr_jours
+00001360: 275d 2e74 6f6c 6973 7428 2929 0d0a 2020  '].tolist())..  
+00001370: 2020 2020 2020 6e62 7265 5b69 645f 6c69        nbre[id_li
+00001380: 6365 6e63 655d 203d 206e 6272 655b 6964  cence] = nbre[id
+00001390: 5f6c 6963 656e 6365 5d20 2b20 5b6e 625f  _licence] + [nb_
+000013a0: 7365 6a6f 7572 5f6a 6f75 7273 5d0d 0a0d  sejour_jours]...
+000013b0: 0a20 2020 2020 2020 206e 625f 7365 6a6f  .        nb_sejo
+000013c0: 7572 203d 206c 656e 2864 672e 7175 6572  ur = len(dg.quer
+000013d0: 7928 2254 7970 652e 7374 722e 636f 6e74  y("Type.str.cont
+000013e0: 6169 6e73 2827 5345 4a4f 5552 2729 2229  ains('SEJOUR')")
+000013f0: 5b27 7365 6a6f 7572 275d 2e75 6e69 7175  ['sejour'].uniqu
+00001400: 6528 2929 0d0a 2020 2020 2020 2020 6e62  e())..        nb
+00001410: 7265 5b69 645f 6c69 6365 6e63 655d 203d  re[id_licence] =
+00001420: 206e 6272 655b 6964 5f6c 6963 656e 6365   nbre[id_licence
+00001430: 5d20 2b20 5b6e 625f 7365 6a6f 7572 5d0d  ] + [nb_sejour].
+00001440: 0a0d 0a20 2020 2020 2020 206e 625f 6869  ...        nb_hi
+00001450: 7665 7220 3d20 6c65 6e28 6467 2e71 7565  ver = len(dg.que
+00001460: 7279 2822 5479 7065 2e73 7472 2e63 6f6e  ry("Type.str.con
+00001470: 7461 696e 7328 2753 4f52 5449 4553 2048  tains('SORTIES H
+00001480: 4956 4552 2729 2229 290d 0a20 2020 2020  IVER')"))..     
+00001490: 2020 206e 6272 655b 6964 5f6c 6963 656e     nbre[id_licen
+000014a0: 6365 5d20 3d20 6e62 7265 5b69 645f 6c69  ce] = nbre[id_li
+000014b0: 6365 6e63 655d 202b 205b 6e62 5f68 6976  cence] + [nb_hiv
+000014c0: 6572 5d0d 0a0d 0a20 2020 2020 2020 206e  er]....        n
+000014d0: 6272 5f65 7665 6e65 6d65 6e74 7320 3d20  br_evenements = 
+000014e0: 5b6e 625f 736f 7274 6965 5f64 696d 616e  [nb_sortie_diman
+000014f0: 6368 6520 2b0d 0a20 2020 2020 2020 2020  che +..         
+00001500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001510: 206e 625f 736f 7274 6965 5f73 616d 6564   nb_sortie_samed
+00001520: 6920 2b0d 0a20 2020 2020 2020 2020 2020  i +..           
+00001530: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00001540: 625f 736f 7274 6965 5f6a 6575 6469 202b  b_sortie_jeudi +
+00001550: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001560: 2020 2020 2020 2020 2020 2020 6e62 5f72              nb_r
+00001570: 616e 646f 202b 0d0a 2020 2020 2020 2020  ando +..        
+00001580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001590: 2020 6e62 5f73 656a 6f75 725f 6a6f 7572    nb_sejour_jour
+000015a0: 7320 2b0d 0a20 2020 2020 2020 2020 2020  s +..           
+000015b0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000015c0: 625f 6869 7665 725d 0d0a 2020 2020 2020  b_hiver]..      
+000015d0: 2020 6e62 7265 5b69 645f 6c69 6365 6e63    nbre[id_licenc
+000015e0: 655d 203d 206e 6272 655b 6964 5f6c 6963  e] = nbre[id_lic
+000015f0: 656e 6365 5d20 2b20 6e62 725f 6576 656e  ence] + nbr_even
+00001600: 656d 656e 7473 0d0a 0d0a 2020 2020 6467  ements....    dg
+00001610: 203d 2070 642e 4461 7461 4672 616d 652e   = pd.DataFrame.
+00001620: 6672 6f6d 5f64 6963 7428 6e62 7265 292e  from_dict(nbre).
+00001630: 540d 0a20 2020 2064 672e 636f 6c75 6d6e  T..    dg.column
+00001640: 7320 3d20 5b0d 0a20 2020 2020 2020 2020  s = [..         
+00001650: 2020 2020 2020 2020 274e 6f6d 272c 0d0a          'Nom',..
+00001660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001670: 2027 5072 c3a9 6e6f 6d27 2c0d 0a20 2020   'Pr..nom',..   
+00001680: 2020 2020 2020 2020 2020 2020 2020 2753                'S
+00001690: 4f52 5449 4520 4455 2044 494d 414e 4348  ORTIE DU DIMANCH
+000016a0: 4520 434c 5542 272c 0d0a 2020 2020 2020  E CLUB',..      
+000016b0: 2020 2020 2020 2020 2020 2027 534f 5254             'SORT
+000016c0: 4945 2044 5520 5341 4d45 4449 2043 4c55  IE DU SAMEDI CLU
+000016d0: 4227 2c0d 0a20 2020 2020 2020 2020 2020  B',..           
+000016e0: 2020 2020 2020 2753 4f52 5449 4520 4455        'SORTIE DU
+000016f0: 204a 4555 4449 2043 4c55 4227 2c0d 0a20   JEUDI CLUB',.. 
+00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001710: 2752 414e 444f 4e4e 4545 272c 0d0a 2020  'RANDONNEE',..  
+00001720: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00001730: 5345 4a4f 5552 2d4a 4f55 5227 2c0d 0a20  SEJOUR-JOUR',.. 
+00001740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001750: 274e 6272 5f53 454a 4f55 5253 272c 0d0a  'Nbr_SEJOURS',..
+00001760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001770: 2027 534f 5254 4945 2048 4956 4552 272c   'SORTIE HIVER',
+00001780: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001790: 2020 2027 544f 5441 4c27 2c0d 0a20 2020     'TOTAL',..   
+000017a0: 2020 2020 2020 2020 2020 2020 2020 5d0d                ].
+000017b0: 0a0d 0a20 2020 2065 6666 6563 7469 6620  ...    effectif 
+000017c0: 3d20 4566 6665 6374 6966 4374 6728 7965  = EffectifCtg(ye
+000017d0: 6172 2c63 7467 5f70 6174 6829 0d0a 2020  ar,ctg_path)..  
+000017e0: 2020 6466 5f65 6666 6563 7469 6620 3d20    df_effectif = 
+000017f0: 6566 6665 6374 6966 2e65 6666 6563 7469  effectif.effecti
+00001800: 660d 0a20 2020 2064 665f 6566 6665 6374  f..    df_effect
+00001810: 6966 2e69 6e64 6578 203d 2064 665f 6566  if.index = df_ef
+00001820: 6665 6374 6966 5b27 4ec2 b020 4c69 6365  fectif['N.. Lice
+00001830: 6e63 69c3 a927 5d0d 0a20 2020 206f 7270  nci..']..    orp
+00001840: 6861 6e20 3d20 7365 7428 6466 5f65 6666  han = set(df_eff
+00001850: 6563 7469 662e 696e 6465 7829 202d 2073  ectif.index) - s
+00001860: 6574 2864 672e 696e 6465 7829 0d0a 2020  et(dg.index)..  
+00001870: 2020 6466 5f6f 7270 6861 6e20 3d20 6466    df_orphan = df
+00001880: 5f65 6666 6563 7469 662e 6c6f 635b 6c69  _effectif.loc[li
+00001890: 7374 286f 7270 6861 6e29 5d5b 5b27 4e6f  st(orphan)][['No
+000018a0: 6d27 2c27 5072 c3a9 6e6f 6d27 5d5d 0d0a  m','Pr..nom']]..
+000018b0: 2020 2020 6466 5f6f 7270 6861 6e5b 5b27      df_orphan[['
+000018c0: 534f 5254 4945 2044 5520 4449 4d41 4e43  SORTIE DU DIMANC
+000018d0: 4845 2043 4c55 4227 2c0d 0a20 2020 2020  HE CLUB',..     
+000018e0: 2020 2020 2020 2020 2020 2753 4f52 5449            'SORTI
+000018f0: 4520 4455 2053 414d 4544 4920 434c 5542  E DU SAMEDI CLUB
+00001900: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00001910: 2020 2027 534f 5254 4945 2044 5520 4a45     'SORTIE DU JE
+00001920: 5544 4920 434c 5542 272c 0d0a 2020 2020  UDI CLUB',..    
+00001930: 2020 2020 2020 2020 2020 2027 5241 4e44             'RAND
+00001940: 4f4e 4e45 4527 2c0d 0a20 2020 2020 2020  ONNEE',..       
+00001950: 2020 2020 2020 2020 2753 454a 4f55 522d          'SEJOUR-
+00001960: 4a4f 5552 272c 0d0a 2020 2020 2020 2020  JOUR',..        
+00001970: 2020 2020 2020 2027 4e62 725f 5345 4a4f         'Nbr_SEJO
+00001980: 5552 5327 2c0d 0a20 2020 2020 2020 2020  URS',..         
+00001990: 2020 2020 2020 2753 4f52 5449 4520 4849        'SORTIE HI
+000019a0: 5645 5227 2c0d 0a20 2020 2020 2020 2020  VER',..         
+000019b0: 2020 2020 2020 2754 4f54 414c 275d 5d20        'TOTAL']] 
+000019c0: 3d20 5b30 2c30 2c30 2c30 2c30 2c30 2c30  = [0,0,0,0,0,0,0
+000019d0: 2c30 5d0d 0a0d 0a20 2020 2064 6720 3d20  ,0]....    dg = 
+000019e0: 7064 2e63 6f6e 6361 7428 5b64 672c 2064  pd.concat([dg, d
+000019f0: 665f 6f72 7068 616e 5d2c 2061 7869 733d  f_orphan], axis=
+00001a00: 3029 0d0a 0d0a 2020 2020 6669 6c65 5f6f  0)....    file_o
+00001a10: 7574 203d 2063 7467 5f70 6174 6820 2f20  ut = ctg_path / 
+00001a20: 5061 7468 2879 6561 7229 202f 2050 6174  Path(year) / Pat
+00001a30: 6828 2753 5441 5449 5354 4951 5545 5327  h('STATISTIQUES'
+00001a40: 2920 2f20 5061 7468 2827 7379 6e74 6865  ) / Path('synthe
+00001a50: 7365 5f61 6468 6572 656e 742e 786c 7378  se_adherent.xlsx
+00001a60: 2729 0d0a 2020 2020 6467 2e74 6f5f 6578  ')..    dg.to_ex
+00001a70: 6365 6c28 6669 6c65 5f6f 7574 290d 0a0d  cel(file_out)...
+00001a80: 0a64 6566 2073 796e 7468 6573 655f 7261  .def synthese_ra
+00001a90: 6e64 6f6e 6e65 6528 7965 6172 3a73 7472  ndonnee(year:str
+00001aa0: 2c63 7467 5f70 6174 683a 7061 7468 6c69  ,ctg_path:pathli
+00001ab0: 622e 5769 6e64 6f77 7350 6174 682c 7479  b.WindowsPath,ty
+00001ac0: 7065 5f73 656a 6f75 723a 7374 7229 3a0d  pe_sejour:str):.
+00001ad0: 0a0d 0a20 2020 2064 6566 2061 6464 6c61  ...    def addla
+00001ae0: 6265 6c73 2878 2c79 2c6f 6666 7365 7429  bels(x,y,offset)
+00001af0: 3a0d 0a20 2020 2020 2020 2066 6f72 2069  :..        for i
+00001b00: 2069 6e20 7261 6e67 6528 6c65 6e28 7829   in range(len(x)
+00001b10: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00001b20: 6966 2079 5b69 5d20 213d 2030 3a0d 0a20  if y[i] != 0:.. 
+00001b30: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00001b40: 6c74 2e74 6578 7428 785b 695d 2c79 5b69  lt.text(x[i],y[i
+00001b50: 5d2b 6f66 6673 6574 2c72 6f75 6e64 2879  ]+offset,round(y
+00001b60: 5b69 5d2c 3129 2c73 697a 653d 3130 290d  [i],1),size=10).
+00001b70: 0a0d 0a0d 0a20 2020 2066 696c 655f 696e  .....    file_in
+00001b80: 203d 2050 6174 6828 6374 675f 7061 7468   = Path(ctg_path
+00001b90: 2920 2f20 5061 7468 2879 6561 7229 202f  ) / Path(year) /
+00001ba0: 2050 6174 6828 2753 5441 5449 5354 4951   Path('STATISTIQ
+00001bb0: 5545 5327 2920 2f20 5061 7468 2827 7379  UES') / Path('sy
+00001bc0: 6e74 6865 7365 2e78 6c73 7827 290d 0a20  nthese.xlsx').. 
+00001bd0: 2020 2064 665f 746f 7461 6c20 3d20 7064     df_total = pd
+00001be0: 2e72 6561 645f 6578 6365 6c28 6669 6c65  .read_excel(file
+00001bf0: 5f69 6e29 0d0a 2020 2020 6466 5f74 6f74  _in)..    df_tot
+00001c00: 616c 203d 2064 665f 746f 7461 6c2e 6472  al = df_total.dr
+00001c10: 6f70 6e61 2873 7562 7365 743d 5b27 4e6f  opna(subset=['No
+00001c20: 6d27 5d29 0d0a 2020 2020 6467 203d 2064  m'])..    dg = d
+00001c30: 665f 746f 7461 6c2e 7175 6572 7928 2754  f_total.query('T
+00001c40: 7970 653d 3d40 7479 7065 5f73 656a 6f75  ype==@type_sejou
+00001c50: 7227 292e 6772 6f75 7062 7928 2773 656a  r').groupby('sej
+00001c60: 6f75 7227 292e 6167 6728 2763 6f75 6e74  our').agg('count
+00001c70: 2729 5b27 4ec2 b020 4c69 6365 6e63 69c3  ')['N.. Licenci.
+00001c80: a927 5d0d 0a0d 0a20 2020 2066 696c 655f  .']....    file_
+00001c90: 696e 666f 203d 2050 6174 6828 6374 675f  info = Path(ctg_
+00001ca0: 7061 7468 2920 2f20 5061 7468 2879 6561  path) / Path(yea
+00001cb0: 7229 202f 2050 6174 6828 2744 4154 4127  r) / Path('DATA'
+00001cc0: 2920 2f20 5061 7468 2827 696e 666f 5f72  ) / Path('info_r
+00001cd0: 616e 646f 732e 786c 7378 2729 0d0a 2020  andos.xlsx')..  
+00001ce0: 2020 636f 7574 5f74 6f74 616c 5f72 616e    cout_total_ran
+00001cf0: 646f 203d 2067 6574 5f63 6f75 745f 746f  do = get_cout_to
+00001d00: 7461 6c28 7965 6172 2c74 7970 655f 7365  tal(year,type_se
+00001d10: 6a6f 7572 2e6c 6f77 6572 2829 2c64 672c  jour.lower(),dg,
+00001d20: 6374 675f 7061 7468 290d 0a0d 0a20 2020  ctg_path)....   
+00001d30: 2066 6967 203d 2070 6c74 2e66 6967 7572   fig = plt.figur
+00001d40: 6528 290d 0a20 2020 2070 6c74 2e62 6172  e()..    plt.bar
+00001d50: 2872 616e 6765 286c 656e 2864 6729 292c  (range(len(dg)),
+00001d60: 6467 2e74 6f6c 6973 7428 2929 0d0a 2020  dg.tolist())..  
+00001d70: 2020 6164 646c 6162 656c 7328 6c69 7374    addlabels(list
+00001d80: 2872 616e 6765 286c 656e 2864 6729 2929  (range(len(dg)))
+00001d90: 2c64 672e 746f 6c69 7374 2829 2c30 2e32  ,dg.tolist(),0.2
+00001da0: 290d 0a20 2020 2070 6c74 2e78 7469 636b  )..    plt.xtick
+00001db0: 7328 7261 6e67 6528 6c65 6e28 6467 2929  s(range(len(dg))
+00001dc0: 2c20 6467 2e69 6e64 6578 2c20 726f 7461  , dg.index, rota
+00001dd0: 7469 6f6e 3d27 7665 7274 6963 616c 2729  tion='vertical')
+00001de0: 0d0a 2020 2020 706c 742e 7469 636b 5f70  ..    plt.tick_p
+00001df0: 6172 616d 7328 6178 6973 3d27 7827 2c20  arams(axis='x', 
+00001e00: 726f 7461 7469 6f6e 3d39 302c 206c 6162  rotation=90, lab
+00001e10: 656c 7369 7a65 3d31 3029 0d0a 2020 2020  elsize=10)..    
+00001e20: 706c 742e 7469 636b 5f70 6172 616d 7328  plt.tick_params(
+00001e30: 6178 6973 3d27 7927 2c6c 6162 656c 7369  axis='y',labelsi
+00001e40: 7a65 3d31 3029 0d0a 0d0a 2020 2020 6966  ze=10)....    if
+00001e50: 2074 7970 655f 7365 6a6f 7572 203d 3d20   type_sejour == 
+00001e60: 2752 414e 444f 4e4e 4545 273a 0d0a 2020  'RANDONNEE':..  
+00001e70: 2020 2020 2020 5f20 3d20 706c 742e 7469        _ = plt.ti
+00001e80: 746c 6528 6627 2320 7261 6e64 6f73 203a  tle(f'# randos :
+00001e90: 207b 6c65 6e28 6467 297d 202c 2023 2070   {len(dg)} , # p
+00001ea0: 6172 7469 6369 7061 6e74 7320 3a20 7b73  articipants : {s
+00001eb0: 756d 2864 6729 7d2c 2043 6fc3 bb74 203a  um(dg)}, Co..t :
+00001ec0: 207b 636f 7574 5f74 6f74 616c 5f72 616e   {cout_total_ran
+00001ed0: 646f 7d20 e282 ac27 290d 0a20 2020 2065  do} ...')..    e
+00001ee0: 6c73 653a 0d0a 2020 2020 2020 2020 5f20  lse:..        _ 
+00001ef0: 3d20 706c 742e 7469 746c 6528 6627 2320  = plt.title(f'# 
+00001f00: 7365 6a6f 7572 7320 3a20 7b6c 656e 2864  sejours : {len(d
+00001f10: 6729 7d20 2c20 2320 7061 7274 6963 6970  g)} , # particip
+00001f20: 616e 7473 203a 207b 7375 6d28 6467 297d  ants : {sum(dg)}
+00001f30: 2c20 436f c3bb 7420 3a20 7b63 6f75 745f  , Co..t : {cout_
+00001f40: 746f 7461 6c5f 7261 6e64 6f7d 20e2 82ac  total_rando} ...
+00001f50: 2729 0d0a 2020 2020 706c 742e 7469 6768  ')..    plt.tigh
+00001f60: 745f 6c61 796f 7574 2829 0d0a 2020 2020  t_layout()..    
+00001f70: 706c 742e 7368 6f77 2829 0d0a 0d0a 6465  plt.show()....de
+00001f80: 6620 6e62 725f 7365 6a6f 7572 735f 6164  f nbr_sejours_ad
+00001f90: 6865 7265 6e74 2879 6561 723a 7374 722c  herent(year:str,
+00001fa0: 2063 7467 5f70 6174 683a 7061 7468 6c69   ctg_path:pathli
+00001fb0: 622e 5769 6e64 6f77 7350 6174 6829 3a0d  b.WindowsPath):.
+00001fc0: 0a0d 0a20 2020 2070 6c74 2e73 7479 6c65  ...    plt.style
+00001fd0: 2e75 7365 2827 6767 706c 6f74 2729 0d0a  .use('ggplot')..
+00001fe0: 0d0a 2020 2020 2320 6675 6e63 7469 6f6e  ..    # function
+00001ff0: 2074 6f20 6164 6420 7661 6c75 6520 6c61   to add value la
+00002000: 6265 6c73 0d0a 2020 2020 6465 6620 6164  bels..    def ad
+00002010: 646c 6162 656c 7328 782c 7929 3a0d 0a20  dlabels(x,y):.. 
+00002020: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00002030: 7261 6e67 6528 6c65 6e28 7829 293a 0d0a  range(len(x)):..
+00002040: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
+00002050: 7465 7874 2878 5b69 5d2d 302e 322c 795b  text(x[i]-0.2,y[
+00002060: 695d 2b31 2c79 5b69 5d2c 7369 7a65 3d6c  i]+1,y[i],size=l
+00002070: 6162 656c 5f73 697a 6529 0d0a 2020 2020  abel_size)..    
+00002080: 6c61 6265 6c5f 7369 7a65 203d 2031 350d  label_size = 15.
+00002090: 0a20 2020 2066 696c 655f 696e 203d 2063  .    file_in = c
+000020a0: 7467 5f70 6174 6820 2f20 5061 7468 2879  tg_path / Path(y
+000020b0: 6561 7229 202f 2050 6174 6828 2753 5441  ear) / Path('STA
+000020c0: 5449 5354 4951 5545 5327 2920 2f20 5061  TISTIQUES') / Pa
+000020d0: 7468 2827 7379 6e74 6865 7365 5f61 6468  th('synthese_adh
+000020e0: 6572 656e 742e 786c 7378 2729 0d0a 2020  erent.xlsx')..  
+000020f0: 2020 6466 5f74 6f74 616c 203d 2070 642e    df_total = pd.
+00002100: 7265 6164 5f65 7863 656c 2866 696c 655f  read_excel(file_
+00002110: 696e 290d 0a0d 0a20 2020 2063 203d 2043  in)....    c = C
+00002120: 6f75 6e74 6572 2829 0d0a 2020 2020 6320  ounter()..    c 
+00002130: 3d20 436f 756e 7465 7228 6466 5f74 6f74  = Counter(df_tot
+00002140: 616c 5b27 4e62 725f 5345 4a4f 5552 5327  al['Nbr_SEJOURS'
+00002150: 5d2e 746f 6c69 7374 2829 290d 0a20 2020  ].tolist())..   
+00002160: 2063 203d 2063 2e6d 6f73 745f 636f 6d6d   c = c.most_comm
+00002170: 6f6e 2829 0d0a 0d0a 2020 2020 782c 2079  on()....    x, y
+00002180: 203d 207a 6970 282a 6329 0d0a 2020 2020   = zip(*c)..    
+00002190: 7820 3d20 6c69 7374 2878 290d 0a20 2020  x = list(x)..   
+000021a0: 2079 203d 206c 6973 7428 7929 0d0a 0d0a   y = list(y)....
+000021b0: 2020 2020 6669 672c 2061 7820 3d20 706c      fig, ax = pl
+000021c0: 742e 7375 6270 6c6f 7473 2866 6967 7369  t.subplots(figsi
+000021d0: 7a65 3d28 352c 3529 290d 0a20 2020 2070  ze=(5,5))..    p
+000021e0: 6c74 2e62 6172 285b 7374 7228 785f 7329  lt.bar([str(x_s)
+000021f0: 2066 6f72 2078 5f73 2069 6e20 785d 2c79   for x_s in x],y
+00002200: 290d 0a20 2020 2070 6c74 2e78 6c61 6265  )..    plt.xlabe
+00002210: 6c28 274e 6f6d 6272 6520 6465 2070 6172  l('Nombre de par
+00002220: 7469 6369 7061 7469 6f6e 20c3 a020 6465  ticipation .. de
+00002230: 7320 73c3 a96a 6f75 7273 2729 0d0a 2020  s s..jours')..  
+00002240: 2020 706c 742e 796c 6162 656c 2827 4e6f    plt.ylabel('No
+00002250: 6d62 7265 2064 6520 6c69 6365 6e63 6965  mbre de licencie
+00002260: 7273 2729 0d0a 2020 2020 706c 742e 7469  rs')..    plt.ti
+00002270: 636b 5f70 6172 616d 7328 6178 6973 3d27  ck_params(axis='
+00002280: 7827 2c20 6c61 6265 6c73 697a 653d 6c61  x', labelsize=la
+00002290: 6265 6c5f 7369 7a65 290d 0a20 2020 2070  bel_size)..    p
+000022a0: 6c74 2e74 6963 6b5f 7061 7261 6d73 2861  lt.tick_params(a
+000022b0: 7869 733d 2779 272c 206c 6162 656c 7369  xis='y', labelsi
+000022c0: 7a65 3d6c 6162 656c 5f73 697a 6529 0d0a  ze=label_size)..
+000022d0: 2020 2020 706c 742e 7469 746c 6528 7965      plt.title(ye
+000022e0: 6172 2c70 6164 3d32 302c 2066 6f6e 7473  ar,pad=20, fonts
+000022f0: 697a 653d 3230 290d 0a0d 0a20 2020 2061  ize=20)....    a
+00002300: 782e 7365 745f 786c 6162 656c 2827 4e20  x.set_xlabel('N 
+00002310: 73c3 a96a 6f75 7273 272c 2066 6f6e 7473  s..jours', fonts
+00002320: 697a 6520 3d20 6c61 6265 6c5f 7369 7a65  ize = label_size
+00002330: 290d 0a20 2020 2061 782e 7365 745f 796c  )..    ax.set_yl
+00002340: 6162 656c 2827 4e6f 6d62 7265 2064 6520  abel('Nombre de 
+00002350: 4354 4720 6179 616e 7420 5c6e 2070 6172  CTG ayant \n par
+00002360: 7469 6369 70c3 a920 c3a0 204e 2073 c3a9  ticip.. .. N s..
+00002370: 6a6f 7572 7327 2c20 666f 6e74 7369 7a65  jours', fontsize
+00002380: 203d 206c 6162 656c 5f73 697a 6529 0d0a   = label_size)..
+00002390: 0d0a 2020 2020 782e 736f 7274 2829 0d0a  ..    x.sort()..
+000023a0: 2020 2020 6164 646c 6162 656c 7328 782c      addlabels(x,
+000023b0: 7929 0d0a 2020 2020 706c 742e 7469 6768  y)..    plt.tigh
+000023c0: 745f 6c61 796f 7574 2829 0d0a 2020 2020  t_layout()..    
+000023d0: 706c 742e 7368 6f77 2829 0d0a 0d0a 2020  plt.show()....  
+000023e0: 2020 6669 675f 6669 6c65 203d 2027 5345    fig_file = 'SE
+000023f0: 4a4f 5552 535f 5354 4154 5f50 4152 5449  JOURS_STAT_PARTI
+00002400: 4349 5041 5449 4f4e 2e70 6e67 270d 0a20  CIPATION.png'.. 
+00002410: 2020 2070 6c74 2e73 6176 6566 6967 2863     plt.savefig(c
+00002420: 7467 5f70 6174 6820 2f20 5061 7468 2879  tg_path / Path(y
+00002430: 6561 7229 202f 2050 6174 6828 2753 5441  ear) / Path('STA
+00002440: 5449 5354 4951 5545 5327 2920 2f20 5061  TISTIQUES') / Pa
+00002450: 7468 2866 6967 5f66 696c 6529 2c62 626f  th(fig_file),bbo
+00002460: 785f 696e 6368 6573 3d27 7469 6768 7427  x_inches='tight'
+00002470: 290d 0a0d 0a64 6566 205f 7265 6164 5f6d  )....def _read_m
+00002480: 656d 6f72 795f 736f 7274 6965 7328 293a  emory_sorties():
+00002490: 0d0a 0d0a 2020 2020 2320 5265 6164 7320  ....    # Reads 
+000024a0: 7468 6520 6465 6661 756c 7420 5056 6368  the default PVch
+000024b0: 6172 6163 7465 7269 7a61 7469 6f6e 2e79  aracterization.y
+000024c0: 616d 6c20 636f 6e66 6967 2066 696c 650d  aml config file.
+000024d0: 0a20 2020 2070 6174 685f 636f 6e66 6967  .    path_config
+000024e0: 5f66 696c 6520 3d20 5061 7468 285f 5f66  _file = Path(__f
+000024f0: 696c 655f 5f29 2e70 6172 656e 742e 7061  ile__).parent.pa
+00002500: 7265 6e74 202f 2050 6174 6828 2763 7467  rent / Path('ctg
+00002510: 6675 6e63 7473 2729 202f 2050 6174 6828  functs') / Path(
+00002520: 2743 5447 5f52 6566 4669 6c65 7327 2920  'CTG_RefFiles') 
+00002530: 2f20 5061 7468 2827 6d65 6d6f 7279 5f73  / Path('memory_s
+00002540: 6f72 7469 6573 2e79 6d6c 2729 0d0a 2020  orties.yml')..  
+00002550: 2020 7769 7468 206f 7065 6e28 7061 7468    with open(path
+00002560: 5f63 6f6e 6669 675f 6669 6c65 2920 6173  _config_file) as
+00002570: 2066 696c 653a 0d0a 2020 2020 2020 2020   file:..        
+00002580: 6d65 6d6f 7279 203d 2079 616d 6c2e 7361  memory = yaml.sa
+00002590: 6665 5f6c 6f61 6428 6669 6c65 290d 0a0d  fe_load(file)...
+000025a0: 0a0d 0a20 2020 2072 6574 7572 6e20 6d65  ...    return me
+000025b0: 6d6f 7279 0d0a 0d0a 6465 6620 6576 6f6c  mory....def evol
+000025c0: 7574 696f 6e5f 736f 7274 6965 7328 7479  ution_sorties(ty
+000025d0: 7065 3a73 7472 2c63 7467 5f70 6174 683a  pe:str,ctg_path:
+000025e0: 7061 7468 6c69 622e 5769 6e64 6f77 7350  pathlib.WindowsP
+000025f0: 6174 6829 3a0d 0a0d 0a20 2020 2064 6566  ath):....    def
+00002600: 2061 6464 5f6d 656d 6f72 7928 7374 6174   add_memory(stat
+00002610: 5f64 6963 2c79 6561 7273 293a 0d0a 2020  _dic,years):..  
+00002620: 2020 2020 2020 6d65 6d6f 7279 203d 205f        memory = _
+00002630: 7265 6164 5f6d 656d 6f72 795f 736f 7274  read_memory_sort
+00002640: 6965 7328 290d 0a0d 0a0d 0a20 2020 2020  ies()......     
+00002650: 2020 2066 6f72 2079 6561 722c 7620 696e     for year,v in
+00002660: 206d 656d 6f72 795b 276d 656d 6f72 7927   memory['memory'
+00002670: 5d2e 6974 656d 7328 293a 0d0a 0d0a 2020  ].items():....  
+00002680: 2020 2020 2020 2020 2020 7374 6174 5f64            stat_d
+00002690: 6963 5b73 7472 2879 6561 7229 5d20 3d20  ic[str(year)] = 
+000026a0: 7374 6174 7965 6172 2876 5b27 5041 5254  statyear(v['PART
+000026b0: 4943 4950 4154 494f 4e5f 5345 4a4f 5552  ICIPATION_SEJOUR
+000026c0: 5327 5d2c 2020 2020 2020 2020 2020 2020  S'],            
+000026d0: 2020 2020 2320 6e62 725f 7365 6a6f 7572      # nbr_sejour
+000026e0: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+000026f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002700: 2020 2020 2020 2020 2020 2020 2020 302c                0,
+00002710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002720: 2020 2020 2020 2020 2020 2320 6a6f 7572            # jour
+00002730: 735f 7365 6a6f 7572 0d0a 2020 2020 2020  s_sejour..      
+00002740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002760: 2020 2020 2076 5b27 534f 5254 4945 535f       v['SORTIES_
+00002770: 434c 5542 5f44 494d 414e 4348 4527 5d2c  CLUB_DIMANCHE'],
+00002780: 2023 2073 6f72 7469 655f 6469 6d61 6e63   # sortie_dimanc
+00002790: 6865 5f63 6c75 620d 0a20 2020 2020 2020  he_club..       
+000027a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027c0: 2020 2020 765b 2753 4f52 5449 4553 5f43      v['SORTIES_C
+000027d0: 4c55 425f 5341 4d45 4449 275d 2c20 2020  LUB_SAMEDI'],   
+000027e0: 2320 736f 7274 6965 5f73 616d 6564 695f  # sortie_samedi_
+000027f0: 636c 7562 0d0a 2020 2020 2020 2020 2020  club..          
+00002800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002820: 2076 5b27 534f 5254 4945 535f 4849 5645   v['SORTIES_HIVE
+00002830: 5227 5d2c 2020 2020 2020 2020 2023 2073  R'],         # s
+00002840: 6f72 7469 655f 6869 7665 725f 636c 7562  ortie_hiver_club
+00002850: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002870: 2020 2020 2020 2020 2020 2020 2076 5b27               v['
+00002880: 534f 5254 4945 535f 434c 5542 5f4a 4555  SORTIES_CLUB_JEU
+00002890: 4449 275d 2c20 2020 2023 2073 6f72 7469  DI'],    # sorti
+000028a0: 655f 6a65 7564 695f 636c 7562 0d0a 2020  e_jeudi_club..  
+000028b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028d0: 2020 2020 2020 2020 2076 5b27 5241 4e44           v['RAND
+000028e0: 4f4e 4e45 4553 275d 2c20 2020 2020 2020  ONNEES'],       
+000028f0: 2020 2020 2023 2072 616e 646f 6e6e 6565       # randonnee
+00002900: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002920: 2020 2020 2020 2020 2020 2020 2076 5b27               v['
+00002930: 4e6f 6d62 7265 5f73 656a 6f75 7273 275d  Nombre_sejours']
+00002940: 2c20 2020 2020 2020 2023 206e 6272 5f73  ,        # nbr_s
+00002950: 656a 6f75 7273 0d0a 2020 2020 2020 2020  ejours..        
+00002960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002980: 2020 2030 2c29 2020 2020 2020 2020 2020     0,)          
+00002990: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000029a0: 206e 6272 5f6a 6f75 7273 5f73 656a 6f75   nbr_jours_sejou
+000029b0: 7273 0d0a 0d0a 2020 2020 2020 2020 2020  rs....          
+000029c0: 2020 7965 6172 732e 6170 7065 6e64 2873    years.append(s
+000029d0: 7472 2879 6561 7229 290d 0a0d 0a20 2020  tr(year))....   
+000029e0: 2064 6566 2066 696c 6c5f 7374 6174 5f79   def fill_stat_y
+000029f0: 6561 7228 7965 6172 3a73 7472 293a 0d0a  ear(year:str):..
+00002a00: 0d0a 2020 2020 2020 2020 7365 6a6f 7572  ..        sejour
+00002a10: 5f69 6e66 6f20 3d20 6765 745f 7365 6a6f  _info = get_sejo
+00002a20: 7572 5f69 6e66 6f28 6374 675f 7061 7468  ur_info(ctg_path
+00002a30: 2c79 6561 7229 0d0a 0d0a 0d0a 2020 2020  ,year)......    
+00002a40: 2020 2020 6669 6c65 5f69 6e20 3d20 6374      file_in = ct
+00002a50: 675f 7061 7468 202f 2050 6174 6828 7374  g_path / Path(st
+00002a60: 7228 7965 6172 2929 202f 2050 6174 6828  r(year)) / Path(
+00002a70: 2753 5441 5449 5354 4951 5545 5327 2920  'STATISTIQUES') 
+00002a80: 2f20 5061 7468 2827 7379 6e74 6865 7365  / Path('synthese
+00002a90: 5f61 6468 6572 656e 742e 786c 7378 2729  _adherent.xlsx')
+00002aa0: 0d0a 0d0a 2020 2020 2020 2020 6466 203d  ....        df =
+00002ab0: 2070 642e 7265 6164 5f65 7863 656c 2866   pd.read_excel(f
+00002ac0: 696c 655f 696e 290d 0a0d 0a20 2020 2020  ile_in)....     
+00002ad0: 2020 2073 7461 745f 7965 6172 203d 2073     stat_year = s
+00002ae0: 7461 7479 6561 7228 6466 5b27 4e62 725f  tatyear(df['Nbr_
+00002af0: 5345 4a4f 5552 5327 5d2e 7375 6d28 292c  SEJOURS'].sum(),
+00002b00: 2020 2020 2020 2020 2020 2020 2023 206e               # n
+00002b10: 6272 5f6a 6f75 7273 5f70 6172 7469 6369  br_jours_partici
+00002b20: 7061 7469 6f6e 5f73 656a 6f75 7273 0d0a  pation_sejours..
+00002b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b40: 2020 2020 2020 2020 2020 2020 2064 665b               df[
+00002b50: 2753 454a 4f55 522d 4a4f 5552 275d 2e73  'SEJOUR-JOUR'].s
+00002b60: 756d 2829 2c20 2020 2020 2020 2020 2020  um(),           
+00002b70: 2020 2320 6e62 725f 7061 7274 6963 6970    # nbr_particip
+00002b80: 6174 696f 6e73 5f73 656a 6f75 720d 0a20  ations_sejour.. 
+00002b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ba0: 2020 2020 2020 2020 2020 2020 6466 5b27              df['
+00002bb0: 534f 5254 4945 2044 5520 4449 4d41 4e43  SORTIE DU DIMANC
+00002bc0: 4845 2043 4c55 4227 5d2e 7375 6d28 292c  HE CLUB'].sum(),
+00002bd0: 2023 2073 6f72 7469 655f 6469 6d61 6e63   # sortie_dimanc
+00002be0: 6865 5f63 6c75 620d 0a20 2020 2020 2020  he_club..       
+00002bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c00: 2020 2020 2020 6466 5b27 534f 5254 4945        df['SORTIE
+00002c10: 2044 5520 5341 4d45 4449 2043 4c55 4227   DU SAMEDI CLUB'
+00002c20: 5d2e 7375 6d28 292c 2020 2023 2073 6f72  ].sum(),   # sor
+00002c30: 7469 655f 7361 6d65 6469 5f63 6c75 620d  tie_samedi_club.
+00002c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002c50: 2020 2020 2020 2020 2020 2020 2020 6466                df
+00002c60: 5b27 534f 5254 4945 2048 4956 4552 275d  ['SORTIE HIVER']
+00002c70: 2e73 756d 2829 2c20 2020 2020 2020 2020  .sum(),         
+00002c80: 2020 2023 2073 6f72 7469 655f 6869 7665     # sortie_hive
+00002c90: 725f 636c 7562 0d0a 2020 2020 2020 2020  r_club..        
 00002ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cb0: 765b 2752 414e 444f 4e4e 4545 5327 5d2c  v['RANDONNEES'],
-00002cc0: 2020 2020 2020 2020 2020 2020 2320 7261              # ra
-00002cd0: 6e64 6f6e 6e65 650d 0a20 2020 2020 2020  ndonnee..       
-00002ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cb0: 2020 2020 2064 665b 2753 4f52 5449 4520       df['SORTIE 
+00002cc0: 4455 204a 4555 4449 2043 4c55 4227 5d2e  DU JEUDI CLUB'].
+00002cd0: 7375 6d28 292c 2020 2020 2320 736f 7274  sum(),    # sort
+00002ce0: 6965 5f6a 6575 6469 5f63 6c75 620d 0a20  ie_jeudi_club.. 
 00002cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d00: 2020 2020 765b 274e 6f6d 6272 655f 7365      v['Nombre_se
-00002d10: 6a6f 7572 7327 5d2c 2020 2020 2020 2020  jours'],        
-00002d20: 2320 6e62 725f 7365 6a6f 7572 730d 0a20  # nbr_sejours.. 
-00002d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d00: 2020 2020 2020 2020 2020 2020 6466 5b27              df['
+00002d10: 5241 4e44 4f4e 4e45 4527 5d2e 7375 6d28  RANDONNEE'].sum(
+00002d20: 292c 2020 2020 2020 2020 2020 2020 2020  ),              
+00002d30: 2023 2072 616e 646f 6e6e 6565 0d0a 2020   # randonnee..  
 00002d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d50: 2020 2020 2020 2020 2020 302c 2920 2020            0,)   
-00002d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d70: 2020 2020 2020 2320 6e62 725f 6a6f 7572        # nbr_jour
-00002d80: 735f 7365 6a6f 7572 730d 0a20 2020 2020  s_sejours..     
+00002d50: 2020 2020 2020 2020 2020 2073 656a 6f75             sejou
+00002d60: 725f 696e 666f 2e6e 6272 5f73 656a 6f75  r_info.nbr_sejou
+00002d70: 7273 2c20 2020 2020 2020 2020 2020 2020  rs,             
+00002d80: 2320 6e62 725f 7365 6a6f 7572 730d 0a20  # nbr_sejours.. 
 00002d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002dc0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00002dd0: 2020 2020 2079 6561 7273 2e61 7070 656e       years.appen
-00002de0: 6428 7374 7228 7965 6172 2929 0d0a 2020  d(str(year))..  
-00002df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e00: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00002e10: 2020 2020 6465 6620 6669 6c6c 5f73 7461      def fill_sta
-00002e20: 745f 7965 6172 2879 6561 7229 3a0d 0a20  t_year(year):.. 
-00002e30: 2020 200d 0a20 2020 2020 2020 2023 2049     ..        # I
-00002e40: 6e74 6572 6e61 6c20 6c69 6272 6172 7920  nternal library 
-00002e50: 696d 706f 7274 730d 0a20 2020 2020 2020  imports..       
-00002e60: 2066 726f 6d20 4354 475f 5574 696c 732e   from CTG_Utils.
-00002e70: 4354 475f 4675 6e63 2e43 5447 5f75 7469  CTG_Func.CTG_uti
-00002e80: 6c69 7479 2069 6d70 6f72 7420 6765 745f  lity import get_
-00002e90: 7365 6a6f 7572 5f69 6e66 6f0d 0a20 2020  sejour_info..   
-00002ea0: 2020 2020 200d 0a20 2020 2020 2020 2073       ..        s
-00002eb0: 656a 6f75 725f 696e 666f 203d 2067 6574  ejour_info = get
-00002ec0: 5f73 656a 6f75 725f 696e 666f 2863 7467  _sejour_info(ctg
-00002ed0: 5f70 6174 682c 7965 6172 290d 0a20 2020  _path,year)..   
-00002ee0: 2020 2020 200d 0a20 2020 2020 2020 200d       ..        .
-00002ef0: 0a20 2020 2020 2020 2066 696c 655f 696e  .        file_in
-00002f00: 203d 2063 7467 5f70 6174 6820 2f20 5061   = ctg_path / Pa
-00002f10: 7468 2873 7472 2879 6561 7229 2920 2f20  th(str(year)) / 
-00002f20: 5061 7468 2827 5354 4154 4953 5449 5155  Path('STATISTIQU
-00002f30: 4553 2729 202f 2050 6174 6828 2773 796e  ES') / Path('syn
-00002f40: 7468 6573 655f 6164 6865 7265 6e74 2e78  these_adherent.x
-00002f50: 6c73 7827 290d 0a20 2020 2020 2020 200d  lsx')..        .
-00002f60: 0a20 2020 2020 2020 2064 6620 3d20 7064  .        df = pd
-00002f70: 2e72 6561 645f 6578 6365 6c28 6669 6c65  .read_excel(file
-00002f80: 5f69 6e29 0d0a 2020 2020 2020 2020 0d0a  _in)..        ..
-00002f90: 2020 2020 2020 2020 7374 6174 5f79 6561          stat_yea
-00002fa0: 7220 3d20 7374 6174 7965 6172 2864 665b  r = statyear(df[
-00002fb0: 274e 6272 5f53 454a 4f55 5253 275d 2e73  'Nbr_SEJOURS'].s
-00002fc0: 756d 2829 2c20 2020 2020 2020 2020 2020  um(),           
-00002fd0: 2020 2320 6e62 725f 6a6f 7572 735f 7061    # nbr_jours_pa
-00002fe0: 7274 6963 6970 6174 696f 6e5f 7365 6a6f  rticipation_sejo
-00002ff0: 7572 730d 0a20 2020 2020 2020 2020 2020  urs..           
-00003000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003010: 2020 6466 5b27 5345 4a4f 5552 2d4a 4f55    df['SEJOUR-JOU
-00003020: 5227 5d2e 7375 6d28 292c 2020 2020 2020  R'].sum(),      
-00003030: 2020 2020 2020 2023 206e 6272 5f70 6172         # nbr_par
-00003040: 7469 6369 7061 7469 6f6e 735f 7365 6a6f  ticipations_sejo
-00003050: 7572 0d0a 2020 2020 2020 2020 2020 2020  ur..            
-00003060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003070: 2064 665b 2753 4f52 5449 4520 4455 2044   df['SORTIE DU D
-00003080: 494d 414e 4348 4520 434c 5542 275d 2e73  IMANCHE CLUB'].s
-00003090: 756d 2829 2c20 2320 736f 7274 6965 5f64  um(), # sortie_d
-000030a0: 696d 616e 6368 655f 636c 7562 0d0a 2020  imanche_club..  
-000030b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030c0: 2020 2020 2020 2020 2020 2064 665b 2753             df['S
-000030d0: 4f52 5449 4520 4455 2053 414d 4544 4920  ORTIE DU SAMEDI 
-000030e0: 434c 5542 275d 2e73 756d 2829 2c20 2020  CLUB'].sum(),   
-000030f0: 2320 736f 7274 6965 5f73 616d 6564 695f  # sortie_samedi_
-00003100: 636c 7562 0d0a 2020 2020 2020 2020 2020  club..          
-00003110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003120: 2020 2064 665b 2753 4f52 5449 4520 4849     df['SORTIE HI
-00003130: 5645 5227 5d2e 7375 6d28 292c 2020 2020  VER'].sum(),    
-00003140: 2020 2020 2020 2020 2320 736f 7274 6965          # sortie
-00003150: 5f68 6976 6572 5f63 6c75 620d 0a20 2020  _hiver_club..   
-00003160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003170: 2020 2020 2020 2020 2020 6466 5b27 534f            df['SO
-00003180: 5254 4945 2044 5520 4a45 5544 4920 434c  RTIE DU JEUDI CL
-00003190: 5542 275d 2e73 756d 2829 2c20 2020 2023  UB'].sum(),    #
-000031a0: 2073 6f72 7469 655f 6a65 7564 695f 636c   sortie_jeudi_cl
-000031b0: 7562 0d0a 2020 2020 2020 2020 2020 2020  ub..            
-000031c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031d0: 2064 665b 2752 414e 444f 4e4e 4545 275d   df['RANDONNEE']
-000031e0: 2e73 756d 2829 2c20 2020 2020 2020 2020  .sum(),         
-000031f0: 2020 2020 2020 2320 7261 6e64 6f6e 6e65        # randonne
-00003200: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-00003210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003220: 7365 6a6f 7572 5f69 6e66 6f2e 6e62 725f  sejour_info.nbr_
-00003230: 7365 6a6f 7572 732c 2020 2020 2020 2020  sejours,        
-00003240: 2020 2020 2023 206e 6272 5f73 656a 6f75       # nbr_sejou
-00003250: 7273 200d 0a20 2020 2020 2020 2020 2020  rs ..           
-00003260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003270: 2020 7365 6a6f 7572 5f69 6e66 6f2e 6e62    sejour_info.nb
-00003280: 725f 6a6f 7572 7329 2020 2020 2020 2020  r_jours)        
-00003290: 2020 2020 2020 2023 206e 6272 5f6a 6f75         # nbr_jou
-000032a0: 7273 5f73 656a 6f75 7273 2020 2020 2020  rs_sejours      
-000032b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032c0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000032d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032e0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000032f0: 2072 6574 7572 6e20 7374 6174 5f79 6561   return stat_yea
-00003300: 720d 0a20 2020 200d 0a20 2020 2064 6566  r..    ..    def
-00003310: 2061 6464 6c61 6265 6c73 2878 2c79 2c6f   addlabels(x,y,o
-00003320: 6666 7365 7429 3a0d 0a20 2020 2020 2020  ffset):..       
-00003330: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00003340: 6c65 6e28 7829 293a 0d0a 2020 2020 2020  len(x)):..      
-00003350: 2020 2020 2020 706c 742e 7465 7874 2878        plt.text(x
-00003360: 5b69 5d2c 795b 695d 2b6f 6666 7365 742c  [i],y[i]+offset,
-00003370: 726f 756e 6428 795b 695d 2c31 292c 7369  round(y[i],1),si
-00003380: 7a65 3d31 3029 0d0a 2020 2020 2020 2020  ze=10)..        
-00003390: 2020 2020 0d0a 2020 2020 6465 6620 706c      ..    def pl
-000033a0: 6f74 5f73 7461 7428 7965 6172 732c 6e62  ot_stat(years,nb
-000033b0: 5f70 6172 7469 6369 7061 6e74 732c 7469  _participants,ti
-000033c0: 746c 652c 6c61 6265 6c5f 7929 3a0d 0a20  tle,label_y):.. 
-000033d0: 2020 2020 2020 2070 6c74 2e66 6967 7572         plt.figur
-000033e0: 6528 6669 6773 697a 653d 2838 2c20 3629  e(figsize=(8, 6)
-000033f0: 290d 0a20 2020 2020 2020 2063 6f6c 6f72  )..        color
-00003400: 7320 3d20 5b27 2366 6461 6134 3827 5d20  s = ['#fdaa48'] 
-00003410: 0d0a 2020 2020 2020 2020 7369 7a65 5f6c  ..        size_l
-00003420: 6162 656c 203d 2032 300d 0a20 2020 2020  abel = 20..     
-00003430: 2020 2070 6c74 2e62 6172 2879 6561 7273     plt.bar(years
-00003440: 2c6e 625f 7061 7274 6963 6970 616e 7473  ,nb_participants
-00003450: 2c63 6f6c 6f72 3d63 6f6c 6f72 7329 0d0a  ,color=colors)..
-00003460: 2020 2020 2020 2020 706c 742e 796c 6162          plt.ylab
-00003470: 656c 286c 6162 656c 5f79 2c73 697a 653d  el(label_y,size=
-00003480: 7369 7a65 5f6c 6162 656c 290d 0a20 2020  size_label)..   
-00003490: 2020 2020 2061 6464 6c61 6265 6c73 2879       addlabels(y
-000034a0: 6561 7273 2c6e 625f 7061 7274 6963 6970  ears,nb_particip
-000034b0: 616e 7473 2c31 290d 0a20 2020 2020 2020  ants,1)..       
-000034c0: 2070 6c74 2e78 7469 636b 7328 726f 7461   plt.xticks(rota
-000034d0: 7469 6f6e 3d39 3029 0d0a 2020 2020 2020  tion=90)..      
-000034e0: 2020 706c 742e 7469 636b 5f70 6172 616d    plt.tick_param
-000034f0: 7328 6178 6973 3d27 7827 2c20 6c61 6265  s(axis='x', labe
-00003500: 6c73 697a 653d 7369 7a65 5f6c 6162 656c  lsize=size_label
-00003510: 290d 0a20 2020 2020 2020 2070 6c74 2e74  )..        plt.t
-00003520: 6963 6b5f 7061 7261 6d73 2861 7869 733d  ick_params(axis=
-00003530: 2779 272c 206c 6162 656c 7369 7a65 3d73  'y', labelsize=s
-00003540: 697a 655f 6c61 6265 6c29 0d0a 2020 2020  ize_label)..    
-00003550: 2020 2020 706c 742e 7469 746c 6528 7469      plt.title(ti
-00003560: 746c 652c 666f 6e74 7369 7a65 3d31 3829  tle,fontsize=18)
-00003570: 0d0a 2020 2020 2020 2020 706c 742e 7469  ..        plt.ti
-00003580: 6768 745f 6c61 796f 7574 2829 0d0a 2020  ght_layout()..  
-00003590: 2020 2020 2020 706c 742e 7368 6f77 2829        plt.show()
-000035a0: 0d0a 2020 2020 0d0a 2020 2020 7374 6174  ..    ..    stat
-000035b0: 7965 6172 203d 206e 616d 6564 7475 706c  year = namedtupl
-000035c0: 6528 2761 6374 6976 6974 6527 2c20 4143  e('activite', AC
-000035d0: 5449 5649 5445 5f4c 4953 5429 0d0a 200d  TIVITE_LIST).. .
-000035e0: 0a20 2020 2070 6c74 2e73 7479 6c65 2e75  .    plt.style.u
-000035f0: 7365 2827 6767 706c 6f74 2729 0d0a 2020  se('ggplot')..  
-00003600: 2020 7965 6172 7320 3d20 5b5d 0d0a 2020    years = []..  
-00003610: 2020 7374 6174 5f64 6963 203d 207b 7d0d    stat_dic = {}.
-00003620: 0a20 2020 2061 6464 5f6d 656d 6f72 7928  .    add_memory(
-00003630: 7374 6174 5f64 6963 2c79 6561 7273 290d  stat_dic,years).
-00003640: 0a0d 0a20 2020 2074 6f64 6179 203d 2064  ...    today = d
-00003650: 6174 6574 696d 652e 6461 7465 7469 6d65  atetime.datetime
-00003660: 2e6e 6f77 2829 0d0a 2020 2020 7965 6172  .now()..    year
-00003670: 735f 6e65 7720 3d20 5b73 7472 2879 6561  s_new = [str(yea
-00003680: 7229 2066 6f72 2079 6561 7220 696e 2072  r) for year in r
-00003690: 616e 6765 2832 3032 322c 746f 6461 792e  ange(2022,today.
-000036a0: 7965 6172 2b31 295d 0d0a 2020 2020 666f  year+1)]..    fo
-000036b0: 7220 7965 6172 2069 6e20 7965 6172 735f  r year in years_
-000036c0: 6e65 773a 0d0a 2020 2020 2020 2020 7374  new:..        st
-000036d0: 6174 5f64 6963 5b79 6561 725d 203d 2066  at_dic[year] = f
-000036e0: 696c 6c5f 7374 6174 5f79 6561 7228 7965  ill_stat_year(ye
-000036f0: 6172 290d 0a20 2020 2020 2020 200d 0a20  ar)..        .. 
-00003700: 2020 2079 6561 7273 203d 2079 6561 7273     years = years
-00003710: 202b 2079 6561 7273 5f6e 6577 2020 200d   + years_new   .
-00003720: 0a20 2020 200d 0a20 2020 200d 0a20 2020  .    ..    ..   
-00003730: 2069 6620 7479 7065 203d 3d20 276e 6272   if type == 'nbr
-00003740: 5f6a 6f75 7273 5f70 6172 7469 6369 7061  _jours_participa
-00003750: 7469 6f6e 5f73 656a 6f75 7273 273a 0d0a  tion_sejours':..
-00003760: 2020 2020 2020 2020 706c 6f74 5f73 7461          plot_sta
-00003770: 7428 7965 6172 732c 0d0a 2020 2020 2020  t(years,..      
-00003780: 2020 2020 2020 2020 2020 2020 5b73 7461              [sta
-00003790: 745f 6469 635b 7965 6172 5d2e 6e62 725f  t_dic[year].nbr_
-000037a0: 6a6f 7572 735f 7061 7274 6963 6970 6174  jours_participat
-000037b0: 696f 6e5f 7365 6a6f 7572 7320 666f 7220  ion_sejours for 
-000037c0: 7965 6172 2069 6e20 7965 6172 735d 2c0d  year in years],.
-000037d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000037e0: 2020 2074 7970 652c 0d0a 2020 2020 2020     type,..      
-000037f0: 2020 2020 2020 2020 2020 2020 7479 7065              type
-00003800: 290d 0a20 2020 2065 6c69 6620 2074 7970  )..    elif  typ
-00003810: 6520 3d3d 2027 736f 7274 6965 5f64 696d  e == 'sortie_dim
-00003820: 616e 6368 655f 636c 7562 273a 0d0a 2020  anche_club':..  
-00003830: 2020 2020 2020 706c 6f74 5f73 7461 7428        plot_stat(
-00003840: 7965 6172 732c 0d0a 2020 2020 2020 2020  years,..        
-00003850: 2020 2020 2020 2020 2020 5b73 7461 745f            [stat_
-00003860: 6469 635b 7965 6172 5d2e 736f 7274 6965  dic[year].sortie
-00003870: 5f64 696d 616e 6368 655f 636c 7562 2066  _dimanche_club f
-00003880: 6f72 2079 6561 7220 696e 2079 6561 7273  or year in years
-00003890: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-000038a0: 2020 2020 2020 7479 7065 2c0d 0a20 2020        type,..   
-000038b0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000038c0: 2370 6172 7469 6369 7061 6e74 7327 290d  #participants').
-000038d0: 0a20 2020 2065 6c69 6620 2074 7970 6520  .    elif  type 
-000038e0: 3d3d 2027 736f 7274 6965 5f73 616d 6564  == 'sortie_samed
-000038f0: 695f 636c 7562 273a 0d0a 2020 2020 2020  i_club':..      
-00003900: 2020 706c 6f74 5f73 7461 7428 7965 6172    plot_stat(year
-00003910: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
-00003920: 2020 2020 2020 5b73 7461 745f 6469 635b        [stat_dic[
-00003930: 7965 6172 5d2e 736f 7274 6965 5f73 616d  year].sortie_sam
-00003940: 6564 695f 636c 7562 2066 6f72 2079 6561  edi_club for yea
-00003950: 7220 696e 2079 6561 7273 5d2c 0d0a 2020  r in years],..  
-00003960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003970: 7479 7065 2c0d 0a20 2020 2020 2020 2020  type,..         
-00003980: 2020 2020 2020 2020 2027 2370 6172 7469           '#parti
-00003990: 6369 7061 6e74 7327 290d 0a20 2020 2065  cipants')..    e
-000039a0: 6c69 6620 2074 7970 6520 3d3d 2027 736f  lif  type == 'so
-000039b0: 7274 6965 5f6a 6575 6469 5f63 6c75 6227  rtie_jeudi_club'
-000039c0: 3a0d 0a20 2020 2020 2020 2070 6c6f 745f  :..        plot_
-000039d0: 7374 6174 2879 6561 7273 2c0d 0a20 2020  stat(years,..   
-000039e0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-000039f0: 7374 6174 5f64 6963 5b79 6561 725d 2e73  stat_dic[year].s
-00003a00: 6f72 7469 655f 6a65 7564 695f 636c 7562  ortie_jeudi_club
-00003a10: 2066 6f72 2079 6561 7220 696e 2079 6561   for year in yea
-00003a20: 7273 5d2c 0d0a 2020 2020 2020 2020 2020  rs],..          
-00003a30: 2020 2020 2020 2020 7479 7065 2c0d 0a20          type,.. 
-00003a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a50: 2027 2370 6172 7469 6369 7061 6e74 7327   '#participants'
-00003a60: 2920 200d 0a20 2020 2065 6c69 6620 2074  )  ..    elif  t
-00003a70: 7970 6520 3d3d 2027 7261 6e64 6f6e 6e65  ype == 'randonne
-00003a80: 6527 3a0d 0a20 2020 2020 2020 2070 6c6f  e':..        plo
-00003a90: 745f 7374 6174 2879 6561 7273 2c0d 0a20  t_stat(years,.. 
-00003aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ab0: 205b 7374 6174 5f64 6963 5b79 6561 725d   [stat_dic[year]
-00003ac0: 2e72 616e 646f 6e6e 6565 2066 6f72 2079  .randonnee for y
-00003ad0: 6561 7220 696e 2079 6561 7273 5d2c 0d0a  ear in years],..
-00003ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003af0: 2020 7479 7065 2c0d 0a20 2020 2020 2020    type,..       
-00003b00: 2020 2020 2020 2020 2020 2027 2370 6172             '#par
-00003b10: 7469 6369 7061 6e74 7327 2920 200d 0a20  ticipants')  .. 
-00003b20: 2020 2065 6c69 6620 2074 7970 6520 3d3d     elif  type ==
-00003b30: 2027 6e62 725f 7061 7274 6963 6970 6174   'nbr_participat
-00003b40: 696f 6e73 5f73 656a 6f75 7273 273a 0d0a  ions_sejours':..
-00003b50: 2020 2020 2020 2020 706c 6f74 5f73 7461          plot_sta
-00003b60: 7428 7965 6172 732c 0d0a 2020 2020 2020  t(years,..      
-00003b70: 2020 2020 2020 2020 2020 2020 5b73 7461              [sta
-00003b80: 745f 6469 635b 7965 6172 5d2e 6e62 725f  t_dic[year].nbr_
-00003b90: 7061 7274 6963 6970 6174 696f 6e73 5f73  participations_s
-00003ba0: 656a 6f75 7273 2066 6f72 2079 6561 7220  ejours for year 
-00003bb0: 696e 2079 6561 7273 5d2c 0d0a 2020 2020  in years],..    
-00003bc0: 2020 2020 2020 2020 2020 2020 2020 274e                'N
-00003bd0: 6f6d 6272 6520 6465 2070 6172 7469 6369  ombre de partici
-00003be0: 7061 7469 6f6e 7320 6175 7820 73c3 a96a  pations aux s..j
-00003bf0: 6f75 7273 272c 0d0a 2020 2020 2020 2020  ours',..        
-00003c00: 2020 2020 2020 2020 2020 2723 2070 6172            '# par
-00003c10: 7469 6369 7061 7469 6f6e 7320 6175 7820  ticipations aux 
-00003c20: 73c3 a96a 6f75 7273 2729 200d 0a20 2020  s..jours') ..   
-00003c30: 2065 6c69 6620 2074 7970 6520 3d3d 2027   elif  type == '
-00003c40: 6e62 725f 7365 6a6f 7572 7327 3a0d 0a20  nbr_sejours':.. 
-00003c50: 2020 2020 2020 2070 6c6f 745f 7374 6174         plot_stat
-00003c60: 2879 6561 7273 2c0d 0a20 2020 2020 2020  (years,..       
-00003c70: 2020 2020 2020 2020 2020 205b 7374 6174             [stat
-00003c80: 5f64 6963 5b79 6561 725d 2e6e 6272 5f73  _dic[year].nbr_s
-00003c90: 656a 6f75 7273 2066 6f72 2079 6561 7220  ejours for year 
-00003ca0: 696e 2079 6561 7273 5d2c 0d0a 2020 2020  in years],..    
-00003cb0: 2020 2020 2020 2020 2020 2020 2020 274e                'N
-00003cc0: 6f6d 6272 6520 6465 2073 c3a9 6a6f 7572  ombre de s..jour
-00003cd0: 7327 2c0d 0a20 2020 2020 2020 2020 2020  s',..           
-00003ce0: 2020 2020 2020 2027 2320 73c3 a96a 6f75         '# s..jou
-00003cf0: 7273 2729 0d0a 2020 2020 656c 6966 2020  rs')..    elif  
-00003d00: 7479 7065 203d 3d20 276e 6272 5f6a 6f75  type == 'nbr_jou
-00003d10: 7273 5f73 656a 6f75 7273 273a 0d0a 2020  rs_sejours':..  
-00003d20: 2020 2020 2020 706c 6f74 5f73 7461 7428        plot_stat(
-00003d30: 7965 6172 732c 0d0a 2020 2020 2020 2020  years,..        
-00003d40: 2020 2020 2020 2020 2020 5b73 7461 745f            [stat_
-00003d50: 6469 635b 7965 6172 5d2e 6e62 725f 6a6f  dic[year].nbr_jo
-00003d60: 7572 735f 7365 6a6f 7572 7320 666f 7220  urs_sejours for 
-00003d70: 7965 6172 2069 6e20 7965 6172 735d 2c0d  year in years],.
-00003d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003d90: 2020 2027 4e6f 6d62 7265 2064 6520 6a6f     'Nombre de jo
-00003da0: 7572 7320 73c3 a96a 6f75 7273 272c 0d0a  urs s..jours',..
-00003db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003dc0: 2020 2723 206a 6f75 7273 2073 c3a9 6a6f    '# jours s..jo
-00003dd0: 7572 2729 2020 2020 2020 2020            ur')        
+00002da0: 2020 2020 2020 2020 2020 2020 7365 6a6f              sejo
+00002db0: 7572 5f69 6e66 6f2e 6e62 725f 6a6f 7572  ur_info.nbr_jour
+00002dc0: 7329 2020 2020 2020 2020 2020 2020 2020  s)              
+00002dd0: 2023 206e 6272 5f6a 6f75 7273 5f73 656a   # nbr_jours_sej
+00002de0: 6f75 7273 0d0a 0d0a 2020 2020 2020 2020  ours....        
+00002df0: 7265 7475 726e 2073 7461 745f 7965 6172  return stat_year
+00002e00: 0d0a 0d0a 2020 2020 6465 6620 6164 646c  ....    def addl
+00002e10: 6162 656c 7328 782c 792c 6f66 6673 6574  abels(x,y,offset
+00002e20: 293a 0d0a 2020 2020 2020 2020 666f 7220  ):..        for 
+00002e30: 6920 696e 2072 616e 6765 286c 656e 2878  i in range(len(x
+00002e40: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
+00002e50: 2070 6c74 2e74 6578 7428 785b 695d 2c79   plt.text(x[i],y
+00002e60: 5b69 5d2b 6f66 6673 6574 2c72 6f75 6e64  [i]+offset,round
+00002e70: 2879 5b69 5d2c 3129 2c73 697a 653d 3130  (y[i],1),size=10
+00002e80: 290d 0a0d 0a20 2020 2064 6566 2070 6c6f  )....    def plo
+00002e90: 745f 7374 6174 2879 6561 7273 2c6e 625f  t_stat(years,nb_
+00002ea0: 7061 7274 6963 6970 616e 7473 2c74 6974  participants,tit
+00002eb0: 6c65 2c6c 6162 656c 5f79 293a 0d0a 2020  le,label_y):..  
+00002ec0: 2020 2020 2020 706c 742e 6669 6775 7265        plt.figure
+00002ed0: 2866 6967 7369 7a65 3d28 382c 2036 2929  (figsize=(8, 6))
+00002ee0: 0d0a 2020 2020 2020 2020 636f 6c6f 7273  ..        colors
+00002ef0: 203d 205b 2723 6664 6161 3438 275d 0d0a   = ['#fdaa48']..
+00002f00: 2020 2020 2020 2020 7369 7a65 5f6c 6162          size_lab
+00002f10: 656c 203d 2032 300d 0a20 2020 2020 2020  el = 20..       
+00002f20: 2070 6c74 2e62 6172 2879 6561 7273 2c6e   plt.bar(years,n
+00002f30: 625f 7061 7274 6963 6970 616e 7473 2c63  b_participants,c
+00002f40: 6f6c 6f72 3d63 6f6c 6f72 7329 0d0a 2020  olor=colors)..  
+00002f50: 2020 2020 2020 706c 742e 796c 6162 656c        plt.ylabel
+00002f60: 286c 6162 656c 5f79 2c73 697a 653d 7369  (label_y,size=si
+00002f70: 7a65 5f6c 6162 656c 290d 0a20 2020 2020  ze_label)..     
+00002f80: 2020 2061 6464 6c61 6265 6c73 2879 6561     addlabels(yea
+00002f90: 7273 2c6e 625f 7061 7274 6963 6970 616e  rs,nb_participan
+00002fa0: 7473 2c31 290d 0a20 2020 2020 2020 2070  ts,1)..        p
+00002fb0: 6c74 2e78 7469 636b 7328 726f 7461 7469  lt.xticks(rotati
+00002fc0: 6f6e 3d39 3029 0d0a 2020 2020 2020 2020  on=90)..        
+00002fd0: 706c 742e 7469 636b 5f70 6172 616d 7328  plt.tick_params(
+00002fe0: 6178 6973 3d27 7827 2c20 6c61 6265 6c73  axis='x', labels
+00002ff0: 697a 653d 7369 7a65 5f6c 6162 656c 290d  ize=size_label).
+00003000: 0a20 2020 2020 2020 2070 6c74 2e74 6963  .        plt.tic
+00003010: 6b5f 7061 7261 6d73 2861 7869 733d 2779  k_params(axis='y
+00003020: 272c 206c 6162 656c 7369 7a65 3d73 697a  ', labelsize=siz
+00003030: 655f 6c61 6265 6c29 0d0a 2020 2020 2020  e_label)..      
+00003040: 2020 706c 742e 7469 746c 6528 7469 746c    plt.title(titl
+00003050: 652c 666f 6e74 7369 7a65 3d31 3829 0d0a  e,fontsize=18)..
+00003060: 2020 2020 2020 2020 706c 742e 7469 6768          plt.tigh
+00003070: 745f 6c61 796f 7574 2829 0d0a 2020 2020  t_layout()..    
+00003080: 2020 2020 706c 742e 7368 6f77 2829 0d0a      plt.show()..
+00003090: 0d0a 2020 2020 7374 6174 7965 6172 203d  ..    statyear =
+000030a0: 206e 616d 6564 7475 706c 6528 2761 6374   namedtuple('act
+000030b0: 6976 6974 6527 2c20 4143 5449 5649 5445  ivite', ACTIVITE
+000030c0: 5f4c 4953 5429 0d0a 0d0a 2020 2020 706c  _LIST)....    pl
+000030d0: 742e 7374 796c 652e 7573 6528 2767 6770  t.style.use('ggp
+000030e0: 6c6f 7427 290d 0a20 2020 2079 6561 7273  lot')..    years
+000030f0: 203d 205b 5d0d 0a20 2020 2073 7461 745f   = []..    stat_
+00003100: 6469 6320 3d20 7b7d 0d0a 2020 2020 6164  dic = {}..    ad
+00003110: 645f 6d65 6d6f 7279 2873 7461 745f 6469  d_memory(stat_di
+00003120: 632c 7965 6172 7329 0d0a 0d0a 2020 2020  c,years)....    
+00003130: 746f 6461 7920 3d20 6461 7465 7469 6d65  today = datetime
+00003140: 2e64 6174 6574 696d 652e 6e6f 7728 290d  .datetime.now().
+00003150: 0a20 2020 2079 6561 7273 5f6e 6577 203d  .    years_new =
+00003160: 205b 7374 7228 7965 6172 2920 666f 7220   [str(year) for 
+00003170: 7965 6172 2069 6e20 7261 6e67 6528 3230  year in range(20
+00003180: 3232 2c74 6f64 6179 2e79 6561 722b 3129  22,today.year+1)
+00003190: 5d0d 0a20 2020 2066 6f72 2079 6561 7220  ]..    for year 
+000031a0: 696e 2079 6561 7273 5f6e 6577 3a0d 0a20  in years_new:.. 
+000031b0: 2020 2020 2020 2073 7461 745f 6469 635b         stat_dic[
+000031c0: 7965 6172 5d20 3d20 6669 6c6c 5f73 7461  year] = fill_sta
+000031d0: 745f 7965 6172 2879 6561 7229 0d0a 0d0a  t_year(year)....
+000031e0: 2020 2020 7965 6172 7320 3d20 7965 6172      years = year
+000031f0: 7320 2b20 7965 6172 735f 6e65 770d 0a0d  s + years_new...
+00003200: 0a0d 0a20 2020 2069 6620 7479 7065 203d  ...    if type =
+00003210: 3d20 276e 6272 5f6a 6f75 7273 5f70 6172  = 'nbr_jours_par
+00003220: 7469 6369 7061 7469 6f6e 5f73 656a 6f75  ticipation_sejou
+00003230: 7273 273a 0d0a 2020 2020 2020 2020 706c  rs':..        pl
+00003240: 6f74 5f73 7461 7428 7965 6172 732c 0d0a  ot_stat(years,..
+00003250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003260: 2020 5b73 7461 745f 6469 635b 7965 6172    [stat_dic[year
+00003270: 5d2e 6e62 725f 6a6f 7572 735f 7061 7274  ].nbr_jours_part
+00003280: 6963 6970 6174 696f 6e5f 7365 6a6f 7572  icipation_sejour
+00003290: 7320 666f 7220 7965 6172 2069 6e20 7965  s for year in ye
+000032a0: 6172 735d 2c0d 0a20 2020 2020 2020 2020  ars],..         
+000032b0: 2020 2020 2020 2020 2074 7970 652c 0d0a           type,..
+000032c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032d0: 2020 7479 7065 290d 0a20 2020 2065 6c69    type)..    eli
+000032e0: 6620 2074 7970 6520 3d3d 2027 736f 7274  f  type == 'sort
+000032f0: 6965 5f64 696d 616e 6368 655f 636c 7562  ie_dimanche_club
+00003300: 273a 0d0a 2020 2020 2020 2020 706c 6f74  ':..        plot
+00003310: 5f73 7461 7428 7965 6172 732c 0d0a 2020  _stat(years,..  
+00003320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003330: 5b73 7461 745f 6469 635b 7965 6172 5d2e  [stat_dic[year].
+00003340: 736f 7274 6965 5f64 696d 616e 6368 655f  sortie_dimanche_
+00003350: 636c 7562 2066 6f72 2079 6561 7220 696e  club for year in
+00003360: 2079 6561 7273 5d2c 0d0a 2020 2020 2020   years],..      
+00003370: 2020 2020 2020 2020 2020 2020 7479 7065              type
+00003380: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00003390: 2020 2020 2027 2370 6172 7469 6369 7061       '#participa
+000033a0: 6e74 7327 290d 0a20 2020 2065 6c69 6620  nts')..    elif 
+000033b0: 2074 7970 6520 3d3d 2027 736f 7274 6965   type == 'sortie
+000033c0: 5f73 616d 6564 695f 636c 7562 273a 0d0a  _samedi_club':..
+000033d0: 2020 2020 2020 2020 706c 6f74 5f73 7461          plot_sta
+000033e0: 7428 7965 6172 732c 0d0a 2020 2020 2020  t(years,..      
+000033f0: 2020 2020 2020 2020 2020 2020 5b73 7461              [sta
+00003400: 745f 6469 635b 7965 6172 5d2e 736f 7274  t_dic[year].sort
+00003410: 6965 5f73 616d 6564 695f 636c 7562 2066  ie_samedi_club f
+00003420: 6f72 2079 6561 7220 696e 2079 6561 7273  or year in years
+00003430: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+00003440: 2020 2020 2020 7479 7065 2c0d 0a20 2020        type,..   
+00003450: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00003460: 2370 6172 7469 6369 7061 6e74 7327 290d  #participants').
+00003470: 0a20 2020 2065 6c69 6620 2074 7970 6520  .    elif  type 
+00003480: 3d3d 2027 736f 7274 6965 5f6a 6575 6469  == 'sortie_jeudi
+00003490: 5f63 6c75 6227 3a0d 0a20 2020 2020 2020  _club':..       
+000034a0: 2070 6c6f 745f 7374 6174 2879 6561 7273   plot_stat(years
+000034b0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000034c0: 2020 2020 205b 7374 6174 5f64 6963 5b79       [stat_dic[y
+000034d0: 6561 725d 2e73 6f72 7469 655f 6a65 7564  ear].sortie_jeud
+000034e0: 695f 636c 7562 2066 6f72 2079 6561 7220  i_club for year 
+000034f0: 696e 2079 6561 7273 5d2c 0d0a 2020 2020  in years],..    
+00003500: 2020 2020 2020 2020 2020 2020 2020 7479                ty
+00003510: 7065 2c0d 0a20 2020 2020 2020 2020 2020  pe,..           
+00003520: 2020 2020 2020 2027 2370 6172 7469 6369         '#partici
+00003530: 7061 6e74 7327 290d 0a20 2020 2065 6c69  pants')..    eli
+00003540: 6620 2074 7970 6520 3d3d 2027 7261 6e64  f  type == 'rand
+00003550: 6f6e 6e65 6527 3a0d 0a20 2020 2020 2020  onnee':..       
+00003560: 2070 6c6f 745f 7374 6174 2879 6561 7273   plot_stat(years
+00003570: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00003580: 2020 2020 205b 7374 6174 5f64 6963 5b79       [stat_dic[y
+00003590: 6561 725d 2e72 616e 646f 6e6e 6565 2066  ear].randonnee f
+000035a0: 6f72 2079 6561 7220 696e 2079 6561 7273  or year in years
+000035b0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+000035c0: 2020 2020 2020 7479 7065 2c0d 0a20 2020        type,..   
+000035d0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000035e0: 2370 6172 7469 6369 7061 6e74 7327 290d  #participants').
+000035f0: 0a20 2020 2065 6c69 6620 2074 7970 6520  .    elif  type 
+00003600: 3d3d 2027 6e62 725f 7061 7274 6963 6970  == 'nbr_particip
+00003610: 6174 696f 6e73 5f73 656a 6f75 7273 273a  ations_sejours':
+00003620: 0d0a 2020 2020 2020 2020 706c 6f74 5f73  ..        plot_s
+00003630: 7461 7428 7965 6172 732c 0d0a 2020 2020  tat(years,..    
+00003640: 2020 2020 2020 2020 2020 2020 2020 5b73                [s
+00003650: 7461 745f 6469 635b 7965 6172 5d2e 6e62  tat_dic[year].nb
+00003660: 725f 7061 7274 6963 6970 6174 696f 6e73  r_participations
+00003670: 5f73 656a 6f75 7273 2066 6f72 2079 6561  _sejours for yea
+00003680: 7220 696e 2079 6561 7273 5d2c 0d0a 2020  r in years],..  
+00003690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036a0: 274e 6f6d 6272 6520 6465 2070 6172 7469  'Nombre de parti
+000036b0: 6369 7061 7469 6f6e 7320 6175 7820 73c3  cipations aux s.
+000036c0: a96a 6f75 7273 272c 0d0a 2020 2020 2020  .jours',..      
+000036d0: 2020 2020 2020 2020 2020 2020 2723 2070              '# p
+000036e0: 6172 7469 6369 7061 7469 6f6e 7320 6175  articipations au
+000036f0: 7820 73c3 a96a 6f75 7273 2729 0d0a 2020  x s..jours')..  
+00003700: 2020 656c 6966 2020 7479 7065 203d 3d20    elif  type == 
+00003710: 276e 6272 5f73 656a 6f75 7273 273a 0d0a  'nbr_sejours':..
+00003720: 2020 2020 2020 2020 706c 6f74 5f73 7461          plot_sta
+00003730: 7428 7965 6172 732c 0d0a 2020 2020 2020  t(years,..      
+00003740: 2020 2020 2020 2020 2020 2020 5b73 7461              [sta
+00003750: 745f 6469 635b 7965 6172 5d2e 6e62 725f  t_dic[year].nbr_
+00003760: 7365 6a6f 7572 7320 666f 7220 7965 6172  sejours for year
+00003770: 2069 6e20 7965 6172 735d 2c0d 0a20 2020   in years],..   
+00003780: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00003790: 4e6f 6d62 7265 2064 6520 73c3 a96a 6f75  Nombre de s..jou
+000037a0: 7273 272c 0d0a 2020 2020 2020 2020 2020  rs',..          
+000037b0: 2020 2020 2020 2020 2723 2073 c3a9 6a6f          '# s..jo
+000037c0: 7572 7327 290d 0a20 2020 2065 6c69 6620  urs')..    elif 
+000037d0: 2074 7970 6520 3d3d 2027 6e62 725f 6a6f   type == 'nbr_jo
+000037e0: 7572 735f 7365 6a6f 7572 7327 3a0d 0a20  urs_sejours':.. 
+000037f0: 2020 2020 2020 2070 6c6f 745f 7374 6174         plot_stat
+00003800: 2879 6561 7273 2c0d 0a20 2020 2020 2020  (years,..       
+00003810: 2020 2020 2020 2020 2020 205b 7374 6174             [stat
+00003820: 5f64 6963 5b79 6561 725d 2e6e 6272 5f6a  _dic[year].nbr_j
+00003830: 6f75 7273 5f73 656a 6f75 7273 2066 6f72  ours_sejours for
+00003840: 2079 6561 7220 696e 2079 6561 7273 5d2c   year in years],
+00003850: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003860: 2020 2020 274e 6f6d 6272 6520 6465 206a      'Nombre de j
+00003870: 6f75 7273 2073 c3a9 6a6f 7572 7327 2c0d  ours s..jours',.
+00003880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003890: 2020 2027 2320 6a6f 7572 7320 73c3 a96a     '# jours s..j
+000038a0: 6f75 7227 29                             our')
```

### Comparing `CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/GUI_Globals.py` & `CTG_Utils-1.2.2/ctgutils/ctggui/guiglobals.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __all__ = ['ACTIVITE_LIST',
-           'ADD_SPACE_MM',           
+           'ADD_SPACE_MM',
            'BM_GUI_DISP',
            'CONTAINER_BUTTON_HEIGHT_PX',
            'FIRST_YEAR',
            'DIR_SORTIES_LIST',
            'FONT_NAME',
            'HELP_EVOLUTION_EFFECTIF',
            'HELP_MEMBER_ANALYSIS',
@@ -62,15 +62,15 @@
            'BUTT_MEMBER_ANALYSIS',
            'TEXT_COPYRIGHT',
            'TEXT_CORPUSES',
            'TEXT_EVOLUTION_EFFECTIF',
            'BUTT_EFFECTIF_ANALYSIS',
            'BUTT_EVOLUTION_EFFECTIF',
            'TEXT_INSTITUTE',
-           'TEXT_LAUNCH_PARSING', 
+           'TEXT_LAUNCH_PARSING',
            'TEXT_LAUNCH_SYNTHESE',
            'TEXT_MEMBER_ANALYSIS',
            'TEXT_PAUSE',
            'TEXT_RANDO',
            'BUTT_RANDO',
            'TEXT_SYNTHESE_SORTIES',
            'BUTT_SYNTHESE_SORTIES',
@@ -88,122 +88,120 @@
            'BUTT_TENDANCE_SORTIES',
            'TEXT_PRESENCE_EFFECTIF',
            'HELP_PRESENCE_EFFECTIF',
            'BUTT_PRESENCE_EFFECTIF',
            'TEXT_GEO_PI',
            'TEXT_GEO',
            'HELP_GEO',
-           'BUTT_GEO',           
+           'BUTT_GEO',
            'TEXT_NBR_SEJOURS',
            'HELP_NBR_SEJOURS',
            'BUTT_NBR_SEJOURS']
+# Standard library imports
+import math
 
+# 3rd party imports
+from screeninfo import get_monitors
 
 ################################## General globals ##################################
 
 # Setting BiblioMeter version value (internal)
 VERSION ='5.0.0'
 
 # Setting the first available year -1 for activity following
 FIRST_YEAR = 2021
 
 # Setting the title of the application main window (internal)
 APPLICATION_WINDOW_TITLE = f"CTG_Meter - Analyse des statistiques des effectifs et des sorties"
 
 ######################## Definition of display globals ###########################
 
-def _get_displays(in_to_mm): 
-    
+def _get_displays(in_to_mm):
+
     ''' The function `get_displays` allows to identify the set of displays
         available within the user hardware and to get their parameters.
-        If the width or the height of a display are not available in mm 
-        through the `get_monitors` method (as for Darwin platforms), 
+        If the width or the height of a display are not available in mm
+        through the `get_monitors` method (as for Darwin platforms),
         the user is asked to specify the displays diagonal size to compute them.
-        
+
     Returns:
         `list`: list of dicts with one dict per detected display,
-                each dict is keyed by 8 display parameters.   
+                each dict is keyed by 8 display parameters.
     '''
     # To Do: convert prints and inputs to gui displays and inputs
-    
-    # Standard library imports
-    import math
-    
-    # 3rd party imports
-    from screeninfo import get_monitors
-    
+
     displays = [{'x':m.x,'y':m.y,'width':m.width,
                  'height':m.height,'width_mm':m.width_mm,
                  'height_mm':m.height_mm,'name':m.name,
                  'is_primary':m.is_primary} for m in get_monitors()]
-    
+
     for disp in range(len(displays)):
         width_px = displays[disp]['width']
         height_px = displays[disp]['height']
-        diag_px = math.sqrt(int(width_px)**2 + int(height_px)**2)    
+        diag_px = math.sqrt(int(width_px)**2 + int(height_px)**2)
         width_mm = displays[disp]['width_mm']
         height_mm = displays[disp]['height_mm']
-        if width_mm is None or height_mm is None: 
+        if width_mm is None or height_mm is None:
             diag_in = float(input('Enter the diagonal size of the screen n°' + str(disp) + ' (inches)'))
             width_mm = round(int(width_px) * (diag_in/diag_px) * in_to_mm,1)
             height_mm = round(int(height_px) * (diag_in/diag_px) * in_to_mm,1)
             displays[disp]['width_mm'] = str(width_mm)
             displays[disp]['height_mm'] = str(height_mm)
         else:
             diag_in = math.sqrt(float(width_mm) ** 2 + float(height_mm) ** 2) / in_to_mm
         displays[disp]['ppi'] = round(diag_px/diag_in,2)
-        
+
     return displays
 
 # Conversion factor for inch to millimeter
-IN_TO_MM = 25.4 
+IN_TO_MM = 25.4
 
 DISPLAYS = _get_displays(IN_TO_MM)
 
 # Setting primary display
 BM_GUI_DISP = 0
 
-# Getting display resolution in pixels per inch 
+# Getting display resolution in pixels per inch
 PPI = DISPLAYS[BM_GUI_DISP]['ppi']
 
 # Setting display reference sizes in pixels and mm (internal)
 REF_SCREEN_WIDTH_PX       = 1920
 REF_SCREEN_HEIGHT_PX      = 1080
 REF_SCREEN_WIDTH_MM       = 467
 REF_SCREEN_HEIGHT_MM      = 267
 
 # Application window reference sizes in mm for the display reference sizes (internal)
 REF_WINDOW_WIDTH_MM       = 219
 REF_WINDOW_HEIGHT_MM      = 173
 
 
-#################################################################### 
-##########################  Pages globals ########################## 
-#################################################################### 
+####################################################################
+##########################  Pages globals ##########################
+####################################################################
 
 
 # Setting general globals for text edition
 FONT_NAME = "Helvetica"
 
 ########################## Reference coordinates for pages ##########################
 
-# Number of characters reference for editing the entered files-folder path 
+# Number of characters reference for editing the entered files-folder path
 REF_ENTRY_NB_CHAR          = 100     #100
 
 # Font size references for page label and button
 REF_SUB_TITLE_FONT_SIZE    = 15      #15
 REF_PAGE_TITLE_FONT_SIZE   = 30      #30
 REF_LAUNCH_FONT_SIZE       = 25      #25
 REF_BMF_FONT_SIZE          = 15      #15        #!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 REF_BUTTON_FONT_SIZE       = 12      #10
 REF_COPYRIGHT_FONT_SIZE    = 12      #10
 REF_VERSION_FONT_SIZE      = 12      #10
 
 # Y position reference in mm for page label
-REF_PAGE_TITLE_POS_Y_MM    = 20      #20 
+REF_PAGE_TITLE_POS_Y_MM    = 20      #20
 
 # Positions reference in mm for institute selection button
 REF_INST_POS_X_MM          = 5       #5
 REF_INST_POS_Y_MM          = 40      #45
 
 # Positions reference in mm for bmf label and button
 REF_BMF_POS_X_MM           = 5       #5
@@ -245,20 +243,20 @@
 REF_SORTIES_BUT_POS_X_MM   = 10      #10
 REF_SORTIES_BUT_POS_Y_MM   = 50      #26
 
 # Separation space in mm for check boxes
 REF_CHECK_BOXES_SEP_SPACE  = 25      #25
 
 # Setting label for each gui page
-PAGES_LABELS = {'PageEffectif': "Analyse des effectifs",
-                'PageSorties' : "Analyse des sorties",
-                'PageSynthese': "Synthèse des sorties et effectifs",
-                'PageTendance': "Analyse de l'évolution temporelle des pratiques ",
-                'PageTendance': "Analyse tendancielle",
-                'PageDivers'  : "Autres analyses",
+PAGES_LABELS = {'page_effectif': "Analyse des effectifs",
+                'pagesorties' : "Analyse des sorties",
+                'pagesynthese': "Synthèse des sorties et effectifs",
+                'pagetendance': "Analyse de l'évolution temporelle des pratiques ",
+                'pagetendance': "Analyse tendancielle",
+                'pagedivers'  : "Autres analyses",
                 'PageHelp'    : "Aide",
                }
 
 
 ########################## Cover Page (BiblioMeter launching Page) ##########################
 
 # Titre de la page
@@ -285,15 +283,15 @@
 # Copyright and contacts
 TEXT_COPYRIGHT              =   "Contributeurs et contacts :"
 TEXT_COPYRIGHT             +=  "\n- Amal Chabli"
 TEXT_COPYRIGHT             +=  "\n- François Bertin : francois.bertin7@wanadoo.fr"
 TEXT_COPYRIGHT             +=  "\n- Ludovic Desmeuzes"
 TEXT_VERSION                = f"\nVersion {VERSION}"
 
-##########################  Secondary pages ########################## 
+##########################  Secondary pages ##########################
 
 # Common to secondary pages
 TEXT_PAUSE           = "Mettre en pause"
 
 ###############  Parsing page
 
 # - Label ANNEE
@@ -366,15 +364,15 @@
 TEXT_PRESENCE_EFFECTIF    = "Analyse de la présence an club"
 HELP_PRESENCE_EFFECTIF    = " L'analyse de l'évolution de l'effectif est issue"
 HELP_PRESENCE_EFFECTIF   += " des archives disponnibles à partir de 2012."
 BUTT_PRESENCE_EFFECTIF    = "Lancer l'analyse de l'évolution des effectifs"
 TEXT_VAE_ANALYSIS         = "Analyse tendancielle depuis 2019 de la population de VAE"
 HELP_VAE_ANALYSIS         = " L'analyse de l'évolution de l'effectif est issue"
 HELP_VAE_ANALYSIS        += " des fichiers EXCEL https://ffcyclo.org/"
-BUTT_VAE_ANALYSIS         = "Lancer l'analyse de l'évolution des VAE"      
+BUTT_VAE_ANALYSIS         = "Lancer l'analyse de l'évolution des VAE"
 
 ### - Page analyse tendancielle
 TEXT_GEO_PI               = "Choix de l'année"
 TEXT_GEO                  = "Analyse de la répartition géographique des adhérents"
 HELP_GEO                  = " La synthèse est effectuée à partir des fichiers"
 HELP_GEO                 += " EXCEL extraits de https://cyclo38ffct.fr/"
 BUTT_GEO                  = "Lancer la construction du fichier html"
@@ -388,15 +386,15 @@
 DIR_SORTIES_LIST = ['SEJOUR',
                     'SORTIES DE DERNIERE MINUTE',
                     'SORTIES DU DIMANCHE',
                     'SORTIES DU JEUDI',
                     'SORTIES DU SAMEDI',
                     'SORTIES HIVER',
                     'SORTIES VTT']
-                    
+
 ACTIVITE_LIST =    ['nbr_participations_sejours',
                     'nbr_jours_participation_sejours',
                     'sortie_dimanche_club',
                     'sortie_samedi_club',
                     'sortie_hiver_club',
                     'sortie_jeudi_club',
                     'randonnee',
```

### Comparing `CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/PageEffectif.py` & `CTG_Utils-1.2.2/ctgutils/ctggui/page_effectif.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,263 +1,253 @@
 __all__ = ['create_effectif_analysis']
 
+# Standard library imports
+import os
+import shutil
+import tkinter as tk
+from tkinter import font as tkFont
+from tkinter import filedialog
+from tkinter import messagebox
+from pathlib import Path
+
+# 3rd party imports
+import pandas as pd
+
+# Local imports
+import ctgutils.ctggui.guiglobals as gg
+from ctgutils.ctggui.useful_functions import encadre_RL
+from ctgutils.ctggui.useful_functions import font_size
+from ctgutils.ctggui.useful_functions import mm_to_px
+from ctgutils.ctggui.useful_functions import place_after
+from ctgutils.ctggui.useful_functions import place_bellow
+from ctgutils.ctggui.useful_functions import last_available_years
+from ctgutils.ctgfuncts.ctg_classes import EffectifCtg
+from ctgutils.ctgfuncts.ctg_effectif import evolution_age_median
+from ctgutils.ctgfuncts.ctg_effectif import evolution_effectif
 
 def _launch_year_analysis(ctg_path, year_select):
     """
     """
 
-    # Standard library imports
-    from tkinter import messagebox
-    
-    
     info_title = "- Information -"
     info_text  = f"L'analyse des mots clefs a été effectuée pour l'année {year_select}."
     info_text += f"\nLes fichiers obtenus ont été créés dans le dossier :"
-    info_text += f"\n\n'{year_analysis_folder_path}' "       
-    messagebox.showinfo(info_title, info_text)        
-    
+    info_text += f"\n\n'{year_analysis_folder_path}' "
+    messagebox.showinfo(info_title, info_text)
 
 
-def _launch_effectif_year_analysis(ctg_path, 
+
+def _launch_effectif_year_analysis(ctg_path,
                         year_select):
     """
     """
-    
-    # Standard library imports
-    from tkinter import messagebox
-    
-    # Local imports
-    from CTG_Utils.CTG_Func.CTGClasses import EffectifCtg
-    
+
     effectif = EffectifCtg(year_select,ctg_path)
     effectif.stat()
     effectif.plot_histo()
-    
+
     #info_title = "- Information -"
     #info_text  = f"L'analyse des IFs a été effectuée pour l'année {year_select} "
     #info_text += f"avec les valeurs {analysis_if}. "
     #info_text += f"\n\nLes fichiers obtenus ont été créés dans le dossier :"
     #info_text += f"\n\n''."
     #info_text += f"\n\nLa base de donnée des indicateurs respective de l'Institut "
     #info_text += f"et de chaque département a été mise à jour "
-    #info_text += f"avec les résultats de cette analyse et se trouve dans le dossier :" 
+    #info_text += f"avec les résultats de cette analyse et se trouve dans le dossier :"
     #info_text += f"\n\n''."
-    #messagebox.showinfo(info_title, info_text)       
+    #messagebox.showinfo(info_title, info_text)
 
 def _launch_effectif_analysis(ctg_path):
-    from CTG_Utils.CTG_Func.CTG_effectif import evolution_effectif
 
-    evolution_effectif(ctg_path)  
+    evolution_effectif(ctg_path)
 
 def _launch_age_analysis(ctg_path):
-    from CTG_Utils.CTG_Func.CTG_effectif import evolution_age_median
 
-    evolution_age_median(ctg_path)    
+    evolution_age_median(ctg_path)
 
 def create_effectif_analysis(self, master, page_name, institute, ctg_path):
-    
+
     """
-    Description : function working as a bridge between the BiblioMeter 
+    Description : function working as a bridge between the BiblioMeter
     App and the functionalities needed for the use of the app
-    
-    Uses the following globals : 
+
+    Uses the following globals :
     - DIC_OUT_PARSING
     - FOLDER_NAMES
-    
-    Args: takes only self and ctg_path as arguments. 
+
+    Args: takes only self and ctg_path as arguments.
     self is the instense in which PageThree will be created
     ctg_path is a type Path, and is the path to where the folders
     organised in a very specific way are stored
-    
+
     Returns : nothing, it create the page in self
     """
-    
-    # Standard library imports
-    import os
-    import shutil
-    import tkinter as tk
-    from tkinter import font as tkFont
-    from tkinter import filedialog
-    from tkinter import messagebox
-    from pathlib import Path
-    
-    # 3rd party imports
-    import pandas as pd
-    
-    # Local imports
-    import CTG_Utils.CTG_GUI.GUI_Globals as gg
-    from CTG_Utils.CTG_GUI.Page_Classes import AppMain
-    from CTG_Utils.CTG_GUI.Useful_Functions import encadre_RL
-    from CTG_Utils.CTG_GUI.Useful_Functions import font_size
-    from CTG_Utils.CTG_GUI.Useful_Functions import mm_to_px
-    from CTG_Utils.CTG_GUI.Useful_Functions import place_after
-    from CTG_Utils.CTG_GUI.Useful_Functions import place_bellow
-    from CTG_Utils.CTG_GUI.Useful_Functions import last_available_years         
-   
-    # Internal functions    
-    def _launch_effectif_year_analysis_try():        
+
+    # Internal functions
+    def _launch_effectif_year_analysis_try():
         # Getting year selection
         year_select =  variable_years.get()
-        
-        _launch_effectif_year_analysis(ctg_path, 
+
+        _launch_effectif_year_analysis(ctg_path,
                             year_select)
         return
-    
-    
+
+    from ctgutils.ctggui.pageclasses import AppMain
+
     # Setting effective font sizes and positions (numbers are reference values)
     eff_etape_font_size      = font_size(gg.REF_ETAPE_FONT_SIZE,   AppMain.width_sf_min)           #14
     eff_launch_font_size     = font_size(gg.REF_ETAPE_FONT_SIZE-1, AppMain.width_sf_min)
     eff_help_font_size       = font_size(gg.REF_ETAPE_FONT_SIZE-2, AppMain.width_sf_min)
     eff_select_font_size     = font_size(gg.REF_ETAPE_FONT_SIZE, AppMain.width_sf_min)
-    eff_buttons_font_size    = font_size(gg.REF_ETAPE_FONT_SIZE-3, AppMain.width_sf_min)  
-    
+    eff_buttons_font_size    = font_size(gg.REF_ETAPE_FONT_SIZE-3, AppMain.width_sf_min)
+
     if_analysis_x_pos_px     = mm_to_px(10 * AppMain.width_sf_mm,  gg.PPI)
-    if_analysis_y_pos_px     = mm_to_px(40 * AppMain.height_sf_mm, gg.PPI)     
-    year_analysis_label_dx_px  = mm_to_px( 0 * AppMain.width_sf_mm,  gg.PPI)  
-    year_analysis_label_dy_px  = mm_to_px(15 * AppMain.height_sf_mm, gg.PPI)   
-    launch_dx_px             = mm_to_px( 0 * AppMain.width_sf_mm,  gg.PPI)    
-    launch_dy_px             = mm_to_px( 5 * AppMain.height_sf_mm, gg.PPI)   
+    if_analysis_y_pos_px     = mm_to_px(40 * AppMain.height_sf_mm, gg.PPI)
+    year_analysis_label_dx_px  = mm_to_px( 0 * AppMain.width_sf_mm,  gg.PPI)
+    year_analysis_label_dy_px  = mm_to_px(15 * AppMain.height_sf_mm, gg.PPI)
+    launch_dx_px             = mm_to_px( 0 * AppMain.width_sf_mm,  gg.PPI)
+    launch_dy_px             = mm_to_px( 5 * AppMain.height_sf_mm, gg.PPI)
 
-    year_button_x_pos        = mm_to_px(gg.REF_YEAR_BUT_POS_X_MM * AppMain.width_sf_mm,  gg.PPI)    #10  
-    year_button_y_pos        = mm_to_px(gg.REF_YEAR_BUT_POS_Y_MM * AppMain.height_sf_mm, gg.PPI)    #26     
+    year_button_x_pos        = mm_to_px(gg.REF_YEAR_BUT_POS_X_MM * AppMain.width_sf_mm,  gg.PPI)    #10
+    year_button_y_pos        = mm_to_px(gg.REF_YEAR_BUT_POS_Y_MM * AppMain.height_sf_mm, gg.PPI)    #26
     dy_year                  = -6
     ds_year                  = 5
-    
+
     # Setting common attributs
     etape_label_format = 'left'
-    etape_underline    = -1                              
-    
+    etape_underline    = -1
+
     ### Choix de l'année
     list_years = last_available_years(ctg_path,year_number=2000)[1:]
-    default_year = list_years[-1]  
+    default_year = list_years[-1]
     variable_years = tk.StringVar(self)
     variable_years.set(default_year)
-    
-        # Création de l'option button des années    
-    self.font_OptionButton_years = tkFont.Font(family = gg.FONT_NAME, 
+
+        # Création de l'option button des années
+    self.font_OptionButton_years = tkFont.Font(family = gg.FONT_NAME,
                                                size = eff_buttons_font_size)
-    self.OptionButton_years = tk.OptionMenu(self, 
-                                            variable_years, 
+    self.OptionButton_years = tk.OptionMenu(self,
+                                            variable_years,
                                             *list_years)
     self.OptionButton_years.config(font = self.font_OptionButton_years)
-    
+
         # Création du label
-    self.font_Label_years = tkFont.Font(family = gg.FONT_NAME, 
+    self.font_Label_years = tkFont.Font(family = gg.FONT_NAME,
                                         size = eff_select_font_size,
                                         weight = 'bold')
-    self.Label_years = tk.Label(self, 
-                                text = gg.TEXT_YEAR_PI, 
+    self.Label_years = tk.Label(self,
+                                text = gg.TEXT_YEAR_PI,
                                 font = self.font_Label_years)
     self.Label_years.place(x = year_button_x_pos, y = year_button_y_pos)
-    
-    place_after(self.Label_years, self.OptionButton_years, dy = dy_year)    
-    
+
+    place_after(self.Label_years, self.OptionButton_years, dy = dy_year)
+
     ################## Analyse des IFs
 
     ### Titre
-    if_analysis_font = tkFont.Font(family = gg.FONT_NAME, 
+    if_analysis_font = tkFont.Font(family = gg.FONT_NAME,
                                    size = eff_etape_font_size,
                                    weight = 'bold')
     if_analysis_label = tk.Label(self,
                                  text = gg.BUTT_EFFECTIF_ANALYSIS,
                                  justify = etape_label_format,
                                  font = if_analysis_font,
                                  underline = etape_underline)
-    
-    if_analysis_label.place(x = if_analysis_x_pos_px, 
+
+    if_analysis_label.place(x = if_analysis_x_pos_px,
                             y = if_analysis_y_pos_px)
-    
+
     ### Explication
-    help_label_font = tkFont.Font(family = gg.FONT_NAME, 
+    help_label_font = tkFont.Font(family = gg.FONT_NAME,
                                   size = eff_help_font_size)
-    help_label = tk.Label(self, 
-                          text = gg.HELP_EFFECTIF, 
-                          justify = "left", 
+    help_label = tk.Label(self,
+                          text = gg.HELP_EFFECTIF,
+                          justify = "left",
                           font = help_label_font)
-    place_bellow(if_analysis_label, 
-                 help_label)     
-                                         
+    place_bellow(if_analysis_label,
+                 help_label)
+
     ### Bouton pour lancer l'analyse des IFs
-    if_analysis_launch_font = tkFont.Font(family = gg.FONT_NAME, 
+    if_analysis_launch_font = tkFont.Font(family = gg.FONT_NAME,
                                           size = eff_launch_font_size)
     if_analysis_launch_button = tk.Button(self,
                                           text = gg.BUTT_EFFECTIF_ANALYSIS,
                                           font = if_analysis_launch_font,
                                           command = lambda: _launch_effectif_year_analysis_try())
-    place_bellow(help_label, 
-                 if_analysis_launch_button, 
-                 dx = launch_dx_px, 
+    place_bellow(help_label,
+                 if_analysis_launch_button,
+                 dx = launch_dx_px,
                  dy = launch_dy_px)
-    
+
     ################## Analyse de l'effectif
-    
-    ### Titre 
-    effectif_analysis_label_font = tkFont.Font(family = gg.FONT_NAME, 
+
+    ### Titre
+    effectif_analysis_label_font = tkFont.Font(family = gg.FONT_NAME,
                                         size = eff_etape_font_size,
                                         weight = 'bold')
-    effectif_analysis_label = tk.Label(self, 
-                               text = gg.TEXT_EVOLUTION_EFFECTIF, 
-                               justify = "left", 
+    effectif_analysis_label = tk.Label(self,
+                               text = gg.TEXT_EVOLUTION_EFFECTIF,
+                               justify = "left",
                                font = effectif_analysis_label_font)
-    place_bellow(if_analysis_launch_button, 
-                 effectif_analysis_label, 
-                 dx = year_analysis_label_dx_px, 
+    place_bellow(if_analysis_launch_button,
+                 effectif_analysis_label,
+                 dx = year_analysis_label_dx_px,
                  dy = year_analysis_label_dy_px)
-    
+
     ### Explication de l'étape
     help_label_font = tkFont.Font(family = gg.FONT_NAME,
                                size = eff_help_font_size)
-    help_label = tk.Label(self, 
-                          text = gg.HELP_EVOLUTION_EFFECTIF, 
-                          justify = "left", 
+    help_label = tk.Label(self,
+                          text = gg.HELP_EVOLUTION_EFFECTIF,
+                          justify = "left",
                           font = help_label_font)
-    place_bellow(effectif_analysis_label, 
-                 help_label) 
-    
+    place_bellow(effectif_analysis_label,
+                 help_label)
+
     ### Bouton pour lancer l'analyse de l'effectif
-    effectif_analysis_launch_font = tkFont.Font(family = gg.FONT_NAME, 
+    effectif_analysis_launch_font = tkFont.Font(family = gg.FONT_NAME,
                                                 size = eff_launch_font_size)
-    effectif_analysis_button = tk.Button(self, 
-                                         text = gg.BUTT_EVOLUTION_EFFECTIF, 
-                                         font = effectif_analysis_launch_font, 
-                                         command = lambda: _launch_effectif_analysis(ctg_path))  
-    place_bellow(help_label, 
-                 effectif_analysis_button, 
-                 dx = launch_dx_px, 
+    effectif_analysis_button = tk.Button(self,
+                                         text = gg.BUTT_EVOLUTION_EFFECTIF,
+                                         font = effectif_analysis_launch_font,
+                                         command = lambda: _launch_effectif_analysis(ctg_path))
+    place_bellow(help_label,
+                 effectif_analysis_button,
+                 dx = launch_dx_px,
                  dy = launch_dy_px)
-    
+
 ################## Analyse de l'évolution de la moyenne d'âge
-    
-    ### Titre 
-    age_analysis_label_font = tkFont.Font(family = gg.FONT_NAME, 
+
+    ### Titre
+    age_analysis_label_font = tkFont.Font(family = gg.FONT_NAME,
                                           size = eff_etape_font_size,
                                           weight = 'bold')
-    age_analysis_label = tk.Label(self, 
-                                  text = gg.TEXT_AGE_ANALYSIS, 
-                                  justify = "left", 
+    age_analysis_label = tk.Label(self,
+                                  text = gg.TEXT_AGE_ANALYSIS,
+                                  justify = "left",
                                   font = age_analysis_label_font)
-    place_bellow(effectif_analysis_button, 
-                 age_analysis_label, 
-                 dx = year_analysis_label_dx_px, 
+    place_bellow(effectif_analysis_button,
+                 age_analysis_label,
+                 dx = year_analysis_label_dx_px,
                  dy = year_analysis_label_dy_px)
-    
+
     ### Explication de l'étape
     help_label_font = tkFont.Font(family = gg.FONT_NAME,
                                size = eff_help_font_size)
-    help_label_age = tk.Label(self, 
-                              text = gg.HELP_AGE_ANALYSIS, 
-                              justify = "left", 
+    help_label_age = tk.Label(self,
+                              text = gg.HELP_AGE_ANALYSIS,
+                              justify = "left",
                               font = help_label_font)
-    place_bellow(age_analysis_label, 
-                 help_label_age) 
-    
+    place_bellow(age_analysis_label,
+                 help_label_age)
+
     ### Bouton pour lancer l'analyse des mots clefs
-    age_analysis_launch_font = tkFont.Font(family = gg.FONT_NAME, 
+    age_analysis_launch_font = tkFont.Font(family = gg.FONT_NAME,
                                          size = eff_launch_font_size)
-    age_analysis_button = tk.Button(self, 
-                                    text = gg.BUTT_AGE_ANALYSIS, 
-                                    font = age_analysis_launch_font, 
-                                    command = lambda: _launch_age_analysis(ctg_path))  
-    place_bellow(help_label_age, 
-                 age_analysis_button, 
-                 dx = launch_dx_px, 
+    age_analysis_button = tk.Button(self,
+                                    text = gg.BUTT_AGE_ANALYSIS,
+                                    font = age_analysis_launch_font,
+                                    command = lambda: _launch_age_analysis(ctg_path))
+    place_bellow(help_label_age,
+                 age_analysis_button,
+                 dx = launch_dx_px,
                  dy = launch_dy_px)
```

### Comparing `CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/PageSorties.py` & `CTG_Utils-1.2.2/ctgutils/ctggui/pagesorties.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,259 +1,249 @@
-__all__ = ['create_sorties_analysis']   
-    
-def _launch_sorties_analysis(ctg_path, 
+__all__ = ['create_sorties_analysis']
+
+# Standard library imports
+import os
+import shutil
+import tkinter as tk
+from tkinter import font as tkFont
+from tkinter import filedialog
+from tkinter import messagebox
+from pathlib import Path
+
+# 3rd party imports
+import pandas as pd
+
+# Local imports
+import ctgutils.ctggui.guiglobals as gg
+from ctgutils.ctgfuncts.ctg_plot import stat_sorties_club
+from ctgutils.ctgfuncts.ctg_synthese import synthese_randonnee
+from ctgutils.ctggui.useful_functions import encadre_RL
+from ctgutils.ctggui.useful_functions import font_size
+from ctgutils.ctggui.useful_functions import mm_to_px
+from ctgutils.ctggui.useful_functions import place_after
+from ctgutils.ctggui.useful_functions import place_bellow
+from ctgutils.ctggui.useful_functions import last_available_years
+from ctgutils.ctggui.useful_functions import get_available_sorties
+
+def _launch_sorties_analysis(ctg_path,
                              year,
                              type_sortie):
     """
     """
-    
-    # Standard library imports
-    from pathlib import Path
-    from tkinter import messagebox
-    
-    # Local imports
-    from CTG_Utils.CTG_Func.CTG_plot import stat_sorties_club
-    
+
+
+
     path_sorties =  ctg_path / Path(str(year)) / Path(type_sortie)
-    file_label =  ctg_path / Path(str(year)) / Path(r'DATA/info_randos.xlsx')    
+    file_label =  ctg_path / Path(str(year)) / Path(r'DATA/info_randos.xlsx')
     df_total = stat_sorties_club(path_sorties,ctg_path,None,file_label,year)
-    
-    
+
+
     #info_title = "- Information -"
     #info_text  = f"L'analyse des IFs a été effectuée pour l'année {year_select} "
     #info_text += f"avec les valeurs {analysis_if}. "
     #info_text += f"\n\nLes fichiers obtenus ont été créés dans le dossier :"
     #info_text += f"\n\n''."
     #info_text += f"\n\nLa base de donnée des indicateurs respective de l'Institut "
     #info_text += f"et de chaque département a été mise à jour "
-    #info_text += f"avec les résultats de cette analyse et se trouve dans le dossier :" 
+    #info_text += f"avec les résultats de cette analyse et se trouve dans le dossier :"
     #info_text += f"\n\n''."
-    #messagebox.showinfo(info_title, info_text) 
-    
-def _launch_rando_analysis(ctg_path, 
+    #messagebox.showinfo(info_title, info_text)
+
+def _launch_rando_analysis(ctg_path,
                            year,
                            type_sortie):
     """
     """
-    
-    # Standard library imports
-    from pathlib import Path
-    from tkinter import messagebox
-    
-    # Local imports
-    from CTG_Utils.CTG_Func.CTG_synthese import synthese_randonnee
-    
+
     if type_sortie == "SEJOUR":
         synthese_randonnee(year,ctg_path,'SEJOUR')
-    else:    
-        synthese_randonnee(year,ctg_path,'RANDONNEE')  
+    else:
+        synthese_randonnee(year,ctg_path,'RANDONNEE')
 
 def create_sorties_analysis(self, master, page_name, institute, ctg_path):
-    
+
     """
-    Description : function working as a bridge between the BiblioMeter 
+    Description : function working as a bridge between the BiblioMeter
     App and the functionalities needed for the use of the app
-    
-    Uses the following globals : 
+
+    Uses the following globals :
     - DIC_OUT_PARSING
     - FOLDER_NAMES
-    
-    Args: takes only self and ctg_path as arguments. 
+
+    Args: takes only self and ctg_path as arguments.
     self is the instense in which PageThree will be created
     ctg_path is a type Path, and is the path to where the folders
     organised in a very specific way are stored
-    
+
     Returns : nothing, it create the page in self
     """
-    
-    # Standard library imports
-    import os
-    import shutil
-    import tkinter as tk
-    from tkinter import font as tkFont
-    from tkinter import filedialog
-    from tkinter import messagebox
-    from pathlib import Path
-    
-    # 3rd party imports
-    import pandas as pd
-    
-    # Local imports
-    import CTG_Utils.CTG_GUI.GUI_Globals as gg
-    from CTG_Utils.CTG_GUI.Page_Classes import AppMain
-    from CTG_Utils.CTG_GUI.Useful_Functions import encadre_RL
-    from CTG_Utils.CTG_GUI.Useful_Functions import font_size
-    from CTG_Utils.CTG_GUI.Useful_Functions import mm_to_px
-    from CTG_Utils.CTG_GUI.Useful_Functions import place_after
-    from CTG_Utils.CTG_GUI.Useful_Functions import place_bellow
-    from CTG_Utils.CTG_GUI.Useful_Functions import last_available_years
-    from CTG_Utils.CTG_GUI.Useful_Functions import get_available_sorties    
-   
-    # Internal functions    
-    def _launch_sorties_analysis_try():        
+
+    # Internal functions
+    def _launch_sorties_analysis_try():
         # Getting year selection
         year_select = variable_years.get()
         type_sortie = variable_sortie.get()
-        _launch_sorties_analysis(ctg_path, 
+        _launch_sorties_analysis(ctg_path,
                                  year_select,
                                  type_sortie)
         return
-        
-    def _launch_rando_analysis_try():        
+
+    def _launch_rando_analysis_try():
         # Getting year selection
         year_select = variable_years.get()
         type_sortie = variable_sortie.get()
-        _launch_rando_analysis(ctg_path, 
+        _launch_rando_analysis(ctg_path,
                                year_select,
                                type_sortie)
-        return        
-    
-    
+        return
+
+    from ctgutils.ctggui.pageclasses import AppMain
+
     # Setting effective font sizes and positions (numbers are reference values)
     eff_etape_font_size      = font_size(gg.REF_ETAPE_FONT_SIZE,   AppMain.width_sf_min)           #14
     eff_launch_font_size     = font_size(gg.REF_ETAPE_FONT_SIZE-1, AppMain.width_sf_min)
     eff_help_font_size       = font_size(gg.REF_ETAPE_FONT_SIZE-2, AppMain.width_sf_min)
     eff_select_font_size     = font_size(gg.REF_ETAPE_FONT_SIZE, AppMain.width_sf_min)
-    eff_buttons_font_size    = font_size(gg.REF_ETAPE_FONT_SIZE-3, AppMain.width_sf_min)  
-    
+    eff_buttons_font_size    = font_size(gg.REF_ETAPE_FONT_SIZE-3, AppMain.width_sf_min)
+
     sorties_analysis_x_pos_px     = mm_to_px(10 * AppMain.width_sf_mm,  gg.PPI)
     sorties_analysis_y_pos_px     = mm_to_px(75 * AppMain.height_sf_mm, gg.PPI)
     rando_analysis_x_pos_px       = mm_to_px(10 * AppMain.width_sf_mm,  gg.PPI)
-    rando_analysis_y_pos_px       = mm_to_px(120 * AppMain.height_sf_mm, gg.PPI)    
-    launch_dx_px             = mm_to_px( 0 * AppMain.width_sf_mm,  gg.PPI)    
-    launch_dy_px             = mm_to_px( 5 * AppMain.height_sf_mm, gg.PPI)   
+    rando_analysis_y_pos_px       = mm_to_px(120 * AppMain.height_sf_mm, gg.PPI)
+    launch_dx_px             = mm_to_px( 0 * AppMain.width_sf_mm,  gg.PPI)
+    launch_dy_px             = mm_to_px( 5 * AppMain.height_sf_mm, gg.PPI)
 
-    year_button_x_pos        = mm_to_px(gg.REF_YEAR_BUT_POS_X_MM * AppMain.width_sf_mm,  gg.PPI)    #10  
+    year_button_x_pos        = mm_to_px(gg.REF_YEAR_BUT_POS_X_MM * AppMain.width_sf_mm,  gg.PPI)    #10
     year_button_y_pos        = mm_to_px(gg.REF_YEAR_BUT_POS_Y_MM * AppMain.height_sf_mm, gg.PPI)    #26
-    sorties_button_x_pos     = mm_to_px(gg.REF_SORTIES_BUT_POS_X_MM * AppMain.width_sf_mm,  gg.PPI)    #10  
-    sorties_button_y_pos     = mm_to_px(gg.REF_SORTIES_BUT_POS_Y_MM * AppMain.height_sf_mm, gg.PPI)    #26     
+    sorties_button_x_pos     = mm_to_px(gg.REF_SORTIES_BUT_POS_X_MM * AppMain.width_sf_mm,  gg.PPI)    #10
+    sorties_button_y_pos     = mm_to_px(gg.REF_SORTIES_BUT_POS_Y_MM * AppMain.height_sf_mm, gg.PPI)    #26
     dy_year                  = -6
     ds_year                  = 5
     dy_sorties               = -6
-    
+
     # Setting common attributs
     etape_label_format = 'left'
-    etape_underline    = -1                              
-    
+    etape_underline    = -1
+
     ### Choix de l'année
     list_years = last_available_years(ctg_path,year_number=2021)
-    default_year = list_years[-1]  
+    default_year = list_years[-1]
     variable_years = tk.StringVar(self)
     variable_years.set(default_year)
-    
-        # Création de l'option button des années    
-    self.font_OptionButton_years = tkFont.Font(family = gg.FONT_NAME, 
+
+        # Création de l'option button des années
+    self.font_OptionButton_years = tkFont.Font(family = gg.FONT_NAME,
                                                size = eff_buttons_font_size)
-    self.OptionButton_years = tk.OptionMenu(self, 
-                                            variable_years, 
+    self.OptionButton_years = tk.OptionMenu(self,
+                                            variable_years,
                                             *list_years)
     self.OptionButton_years.config(font = self.font_OptionButton_years)
-    
+
         # Création du label
-    self.font_Label_years = tkFont.Font(family = gg.FONT_NAME, 
+    self.font_Label_years = tkFont.Font(family = gg.FONT_NAME,
                                         size = eff_select_font_size,
                                         weight = 'bold')
-    self.Label_years = tk.Label(self, 
-                                text = gg.TEXT_YEAR_PI, 
+    self.Label_years = tk.Label(self,
+                                text = gg.TEXT_YEAR_PI,
                                 font = self.font_Label_years)
     self.Label_years.place(x = year_button_x_pos, y = year_button_y_pos)
-    
-    place_after(self.Label_years, self.OptionButton_years, dy = dy_year) 
+
+    place_after(self.Label_years, self.OptionButton_years, dy = dy_year)
 
     ### Choix de du type de sortie
     list_sorties = get_available_sorties(ctg_path,variable_years.get())
-    default_sortie = list_sorties[-1]  
+    default_sortie = list_sorties[-1]
     variable_sortie = tk.StringVar(self)
     variable_sortie.set(default_sortie)
-    
-        # Création de l'option button des sorties    
-    self.font_OptionButton_sorties = tkFont.Font(family = gg.FONT_NAME, 
+
+        # Création de l'option button des sorties
+    self.font_OptionButton_sorties = tkFont.Font(family = gg.FONT_NAME,
                                                  size = eff_buttons_font_size)
-    self.OptionButton_sorties = tk.OptionMenu(self, 
-                                              variable_sortie, 
+    self.OptionButton_sorties = tk.OptionMenu(self,
+                                              variable_sortie,
                                               *list_sorties)
     self.OptionButton_sorties.config(font = self.font_OptionButton_sorties)
-    
+
         # Création du label
-    self.font_Label_sorties = tkFont.Font(family = gg.FONT_NAME, 
+    self.font_Label_sorties = tkFont.Font(family = gg.FONT_NAME,
                                         size = eff_select_font_size,
                                         weight = 'bold')
-    self.Label_sorties = tk.Label(self, 
-                                  text = gg.TEXT_SORTIES_PI, 
+    self.Label_sorties = tk.Label(self,
+                                  text = gg.TEXT_SORTIES_PI,
                                   font = self.font_Label_sorties)
     self.Label_sorties.place(x = sorties_button_x_pos, y = sorties_button_y_pos)
-    
-    place_after(self.Label_sorties, self.OptionButton_sorties, dy = dy_sorties)    
-    
+
+    place_after(self.Label_sorties, self.OptionButton_sorties, dy = dy_sorties)
+
     ################## Analyse des sorties
 
     ### Titre
-    sorties_analysis_font = tkFont.Font(family = gg.FONT_NAME, 
+    sorties_analysis_font = tkFont.Font(family = gg.FONT_NAME,
                                         size = eff_etape_font_size,
                                         weight = 'bold')
     sorties_analysis_label = tk.Label(self,
                                       text = gg.TEXT_SORTIES,
                                       justify = etape_label_format,
                                       font = sorties_analysis_font,
                                       underline = etape_underline)
-    
-    sorties_analysis_label.place(x = sorties_analysis_x_pos_px, 
+
+    sorties_analysis_label.place(x = sorties_analysis_x_pos_px,
                                  y = sorties_analysis_y_pos_px)
-    
+
     ### Explication
-    help_label_font = tkFont.Font(family = gg.FONT_NAME, 
+    help_label_font = tkFont.Font(family = gg.FONT_NAME,
                                   size = eff_help_font_size)
-    help_label = tk.Label(self, 
-                          text = gg.HELP_SORTIES, 
-                          justify = "left", 
+    help_label = tk.Label(self,
+                          text = gg.HELP_SORTIES,
+                          justify = "left",
                           font = help_label_font)
-    place_bellow(sorties_analysis_label, 
-                 help_label)     
-                                         
+    place_bellow(sorties_analysis_label,
+                 help_label)
+
     ### Bouton pour lancer l'analyse des sorties
-    sorties_analysis_launch_font = tkFont.Font(family = gg.FONT_NAME, 
+    sorties_analysis_launch_font = tkFont.Font(family = gg.FONT_NAME,
                                           size = eff_launch_font_size)
     sorties_analysis_launch_button = tk.Button(self,
                                                text = gg.BUTT_SORTIES,
                                                font = sorties_analysis_launch_font,
                                                command = lambda: _launch_sorties_analysis_try())
-    place_bellow(help_label, 
-                 sorties_analysis_launch_button, 
-                 dx = launch_dx_px, 
+    place_bellow(help_label,
+                 sorties_analysis_launch_button,
+                 dx = launch_dx_px,
                  dy = launch_dy_px)
 
     ################## Analyse des randonnées
 
     ### Titre
-    rando_analysis_font = tkFont.Font(family = gg.FONT_NAME, 
+    rando_analysis_font = tkFont.Font(family = gg.FONT_NAME,
                                       size = eff_etape_font_size,
                                       weight = 'bold')
     rando_analysis_label = tk.Label(self,
                                     text = gg.TEXT_RANDO,
                                     justify = etape_label_format,
                                     font = rando_analysis_font,
                                     underline = etape_underline)
-    
-    rando_analysis_label.place(x = rando_analysis_x_pos_px, 
+
+    rando_analysis_label.place(x = rando_analysis_x_pos_px,
                                  y = rando_analysis_y_pos_px)
-    
+
     ### Explication
-    help_label_font = tkFont.Font(family = gg.FONT_NAME, 
+    help_label_font = tkFont.Font(family = gg.FONT_NAME,
                                   size = eff_help_font_size)
-    help_label_rando = tk.Label(self, 
-                                text = gg.HELP_RANDO, 
-                                justify = "left", 
+    help_label_rando = tk.Label(self,
+                                text = gg.HELP_RANDO,
+                                justify = "left",
                                 font = help_label_font)
-    place_bellow(rando_analysis_label, 
-                 help_label_rando)     
-                                         
+    place_bellow(rando_analysis_label,
+                 help_label_rando)
+
     ### Bouton pour lancer l'analyse des sorties
-    rando_analysis_launch_font = tkFont.Font(family = gg.FONT_NAME, 
+    rando_analysis_launch_font = tkFont.Font(family = gg.FONT_NAME,
                                              size = eff_launch_font_size)
     rando_analysis_launch_button = tk.Button(self,
                                              text = gg.BUTT_RANDO,
                                              font = sorties_analysis_launch_font,
                                              command = lambda: _launch_rando_analysis_try())
-    place_bellow(help_label_rando, 
-                 rando_analysis_launch_button, 
-                 dx = launch_dx_px, 
-                 dy = launch_dy_px)  
+    place_bellow(help_label_rando,
+                 rando_analysis_launch_button,
+                 dx = launch_dx_px,
+                 dy = launch_dy_px)
```

### Comparing `CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/PageSynthese.py` & `CTG_Utils-1.2.2/ctgutils/ctggui/pagetendance.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,228 +1,231 @@
-__all__ = ['create_effectif_analysis']   
+__all__ = ['create_tendance_analysis']
+
+# Standard library imports
+import os
+import shutil
+import tkinter as tk
+from tkinter import font as tkFont
+from tkinter import filedialog
+from tkinter import messagebox
+from pathlib import Path
+
+# 3rd party imports
+import pandas as pd
+
+# Internal imports
+import ctgutils.ctggui.guiglobals as gg
+from ctgutils.ctgfuncts.ctg_effectif import statistique_vae
+from ctgutils.ctgfuncts.ctg_effectif import builds_excel_presence_au_club
+from ctgutils.ctgfuncts.ctg_effectif import anciennete_au_club
+from ctgutils.ctggui.useful_functions import encadre_RL
+from ctgutils.ctggui.useful_functions import font_size
+from ctgutils.ctggui.useful_functions import mm_to_px
+from ctgutils.ctggui.useful_functions import place_after
+from ctgutils.ctggui.useful_functions import place_bellow
+from ctgutils.ctggui.useful_functions import last_available_years
+from ctgutils.ctgfuncts.ctg_synthese import evolution_sorties
+
+def create_tendance_analysis(self, master, page_name, institute, ctg_path):
 
-def create_synthese_analysis(self, master, page_name, institute, ctg_path):
-    
     """
-    Description : function working as a bridge between the BiblioMeter 
+    Description : function working as a bridge between the BiblioMeter
     App and the functionalities needed for the use of the app
-    
-    Uses the following globals : 
+
+    Uses the following globals :
     - DIC_OUT_PARSING
     - FOLDER_NAMES
-    
-    Args: takes only self and ctg_path as arguments. 
+
+    Args: takes only self and ctg_path as arguments.
     self is the instense in which PageThree will be created
     ctg_path is a type Path, and is the path to where the folders
     organised in a very specific way are stored
-    
+
     Returns : nothing, it create the page in self
     """
-    
-    # Standard library imports
-    import os
-    import shutil
-    import tkinter as tk
-    from tkinter import font as tkFont
-    from tkinter import filedialog
-    from tkinter import messagebox
-    from pathlib import Path
-    
-    # 3rd party imports
-    import pandas as pd
-    
-    # Local imports
-    import CTG_Utils.CTG_GUI.GUI_Globals as gg
-    from CTG_Utils.CTG_GUI.Page_Classes import AppMain
-    from CTG_Utils.CTG_GUI.Useful_Functions import encadre_RL
-    from CTG_Utils.CTG_GUI.Useful_Functions import font_size
-    from CTG_Utils.CTG_GUI.Useful_Functions import mm_to_px
-    from CTG_Utils.CTG_GUI.Useful_Functions import place_after
-    from CTG_Utils.CTG_GUI.Useful_Functions import place_bellow
-    from CTG_Utils.CTG_GUI.Useful_Functions import last_available_years         
-   
-    # Internal functions    
-    def _launch_synthese_analysis():
-        # Internal imports
-        from CTG_Utils.CTG_Func.CTG_synthese import synthese
-        from CTG_Utils.CTG_Func.CTG_synthese import plot_pie_synthese
-    
+
+    # Internal functions
+    def _launch_evolution_sorties(ctg_path):
+
         # Getting year selection
-        year_select =  variable_years.get()
-        
-        synthese(year_select,ctg_path)
-        plot_pie_synthese(year_select,ctg_path)
-        
-    def _launch_member_analysis(ctg_path):
-        # Internal imports
-        from CTG_Utils.CTG_Func.CTG_synthese import synthese_adherent
-    
+        activite =  variable_activite.get()
+
+        evolution_sorties (activite,ctg_path)
+
+    def _launch_member_history_analysis(ctg_path):
+
         # Getting year selection
-        year_select =  variable_years.get()
-        
-        synthese_adherent(year_select,ctg_path)
+
+        out_path = builds_excel_presence_au_club(ctg_path)
+
         info_title = "- Information -"
-        info_text  = f"L'analyse de la participation aux sorties par membre a été effectuée pour l'année {year_select} "
-        info_text += f"\n\nLe fichier EXCEL obtenu : 'synthese_adherent.xlsx' a été créé dans le dossier :"
-        info_text += f"\n\n{ctg_path}\{str(year_select)}\STATISTIQUES."
-  
-        messagebox.showinfo(info_title, info_text) 
-    
-    
+        info_text  = f"L'analyse de la présence au club par membre a été effectuée  "
+        info_text += f"\n\nLe fichier EXCEL obtenu synthese_adherent.xlsx a été créé dans le dossier :"
+        info_text += f"\n\n{out_path}."
+
+        messagebox.showinfo(info_title, info_text)
+
+        anciennete_au_club(ctg_path)
+
+    def _launch_vae_analysis(ctg_path):
+        statistique_vae(ctg_path)
+
+    from ctgutils.ctggui.pageclasses import AppMain
+
     # Setting effective font sizes and positions (numbers are reference values)
     eff_etape_font_size      = font_size(gg.REF_ETAPE_FONT_SIZE,   AppMain.width_sf_min)           #14
     eff_launch_font_size     = font_size(gg.REF_ETAPE_FONT_SIZE-1, AppMain.width_sf_min)
     eff_help_font_size       = font_size(gg.REF_ETAPE_FONT_SIZE-2, AppMain.width_sf_min)
     eff_select_font_size     = font_size(gg.REF_ETAPE_FONT_SIZE, AppMain.width_sf_min)
-    eff_buttons_font_size    = font_size(gg.REF_ETAPE_FONT_SIZE-3, AppMain.width_sf_min)  
-    
+    eff_buttons_font_size    = font_size(gg.REF_ETAPE_FONT_SIZE-3, AppMain.width_sf_min)
+
     synthese_analysis_x_pos_px     = mm_to_px(10 * AppMain.width_sf_mm,  gg.PPI)
-    synthese_analysis_y_pos_px     = mm_to_px(40 * AppMain.height_sf_mm, gg.PPI)     
-    year_analysis_label_dx_px  = mm_to_px( 0 * AppMain.width_sf_mm,  gg.PPI)  
-    year_analysis_label_dy_px  = mm_to_px(15 * AppMain.height_sf_mm, gg.PPI)   
-    launch_dx_px             = mm_to_px( 0 * AppMain.width_sf_mm,  gg.PPI)    
-    launch_dy_px             = mm_to_px( 5 * AppMain.height_sf_mm, gg.PPI)   
+    synthese_analysis_y_pos_px     = mm_to_px(40 * AppMain.height_sf_mm, gg.PPI)
+    year_analysis_label_dx_px  = mm_to_px( 0 * AppMain.width_sf_mm,  gg.PPI)
+    year_analysis_label_dy_px  = mm_to_px(15 * AppMain.height_sf_mm, gg.PPI)
+    launch_dx_px             = mm_to_px( 0 * AppMain.width_sf_mm,  gg.PPI)
+    launch_dy_px             = mm_to_px( 5 * AppMain.height_sf_mm, gg.PPI)
 
-    year_button_x_pos        = mm_to_px(gg.REF_YEAR_BUT_POS_X_MM * AppMain.width_sf_mm,  gg.PPI)    #10  
-    year_button_y_pos        = mm_to_px(gg.REF_YEAR_BUT_POS_Y_MM * AppMain.height_sf_mm, gg.PPI)    #26     
+    year_button_x_pos        = mm_to_px(gg.REF_YEAR_BUT_POS_X_MM * AppMain.width_sf_mm,  gg.PPI)    #10
+    year_button_y_pos        = mm_to_px(gg.REF_YEAR_BUT_POS_Y_MM * AppMain.height_sf_mm, gg.PPI)    #26
     dy_year                  = -6
     ds_year                  = 5
-    
+
     # Setting common attributs
     etape_label_format = 'left'
-    etape_underline    = -1                              
-    
+    etape_underline    = -1
+
     ### Choix de l'année
-    list_years = last_available_years(ctg_path,year_number=2020)[1:]
-    default_year = list_years[-1]  
-    variable_years = tk.StringVar(self)
-    variable_years.set(default_year)
-    
-        # Création de l'option button des années    
-    self.font_OptionButton_years = tkFont.Font(family = gg.FONT_NAME, 
+    list_activites = gg.ACTIVITE_LIST
+    default_activite = list_activites[-1]
+    variable_activite = tk.StringVar(self)
+    variable_activite.set(default_activite)
+
+        # Création de l'option button des années
+    self.font_OptionButton_years = tkFont.Font(family = gg.FONT_NAME,
                                                size = eff_buttons_font_size)
-    self.OptionButton_years = tk.OptionMenu(self, 
-                                            variable_years, 
-                                            *list_years)
+    self.OptionButton_years = tk.OptionMenu(self,
+                                            variable_activite,
+                                            *list_activites)
     self.OptionButton_years.config(font = self.font_OptionButton_years)
-    
+
         # Création du label
-    self.font_Label_years = tkFont.Font(family = gg.FONT_NAME, 
+    self.font_Label_years = tkFont.Font(family = gg.FONT_NAME,
                                         size = eff_select_font_size,
                                         weight = 'bold')
-    self.Label_years = tk.Label(self, 
-                                text = gg.TEXT_YEAR_PI, 
+    self.Label_years = tk.Label(self,
+                                text = gg.TEXT_ACTIVITE_PI,
                                 font = self.font_Label_years)
     self.Label_years.place(x = year_button_x_pos, y = year_button_y_pos)
-    
-    place_after(self.Label_years, self.OptionButton_years, dy = dy_year)    
-    
-    ################## Synthèse des activité
+
+    place_after(self.Label_years, self.OptionButton_years, dy = dy_year)
+
+    ################## Synthèse des activités
 
     ### Titre
-    synthese_analysis_font = tkFont.Font(family = gg.FONT_NAME, 
+    synthese_analysis_font = tkFont.Font(family = gg.FONT_NAME,
                                          size = eff_etape_font_size,
                                          weight = 'bold')
     synthese_analysis_label = tk.Label(self,
-                                       text = gg.TEXT_SYNTHESE_SORTIES,
+                                       text = gg.TEXT_TENDANCE_SORTIES,
                                        justify = etape_label_format,
                                        font = synthese_analysis_font,
                                        underline = etape_underline)
-    
-    synthese_analysis_label.place(x = synthese_analysis_x_pos_px, 
+
+    synthese_analysis_label.place(x = synthese_analysis_x_pos_px,
                                   y = synthese_analysis_y_pos_px)
-    
+
     ### Explication
-    help_label_font = tkFont.Font(family = gg.FONT_NAME, 
+    help_label_font = tkFont.Font(family = gg.FONT_NAME,
                                   size = eff_help_font_size)
-    help_label = tk.Label(self, 
-                          text = gg.HELP_SYNTHESE_SORTIES, 
-                          justify = "left", 
+    help_label = tk.Label(self,
+                          text = gg.HELP_TENDANCE_SORTIES,
+                          justify = "left",
                           font = help_label_font)
-    place_bellow(synthese_analysis_label, 
-                 help_label)     
-                                         
-    ### Bouton pour lancer l'analyse des IFs
-    synthese_analysis_launch_font = tkFont.Font(family = gg.FONT_NAME, 
+    place_bellow(synthese_analysis_label,
+                 help_label)
+
+    ### Bouton pour lancer l'analyse tendancielle des activités
+    synthese_analysis_launch_font = tkFont.Font(family = gg.FONT_NAME,
                                                 size = eff_launch_font_size)
     synthese_analysis_launch_button = tk.Button(self,
-                                                text = gg.BUTT_SYNTHESE_SORTIES,
+                                                text = gg.BUTT_TENDANCE_SORTIES,
                                                 font = synthese_analysis_launch_font,
-                                                command = lambda: _launch_synthese_analysis())
-    place_bellow(help_label, 
-                 synthese_analysis_launch_button, 
-                 dx = launch_dx_px, 
+                                                command = lambda: _launch_evolution_sorties(ctg_path))
+    place_bellow(help_label,
+                 synthese_analysis_launch_button,
+                 dx = launch_dx_px,
                  dy = launch_dy_px)
-    
-    ################## Analyse des mots clefs
-    
-    ### Titre 
-    member_analysis_label_font = tkFont.Font(family = gg.FONT_NAME, 
+
+    ################## Analyse de de la présence des membres au club
+
+    ### Titre
+    member_analysis_label_font = tkFont.Font(family = gg.FONT_NAME,
                                              size = eff_etape_font_size,
                                              weight = 'bold')
-    member_analysis_label = tk.Label(self, 
-                                     text = gg.TEXT_MEMBER_ANALYSIS, 
-                                     justify = "left", 
+    member_analysis_label = tk.Label(self,
+                                     text = gg.TEXT_PRESENCE_EFFECTIF,
+                                     justify = "left",
                                      font = member_analysis_label_font)
-    place_bellow(synthese_analysis_launch_button, 
-                 member_analysis_label, 
-                 dx = year_analysis_label_dx_px, 
+    place_bellow(synthese_analysis_launch_button,
+                 member_analysis_label,
+                 dx = year_analysis_label_dx_px,
                  dy = year_analysis_label_dy_px)
-    
+
     ### Explication de l'étape
     help_label_font = tkFont.Font(family = gg.FONT_NAME,
                                   size = eff_help_font_size)
-    help_label = tk.Label(self, 
-                          text = gg.HELP_MEMBER_ANALYSIS, 
-                          justify = "left", 
+    help_label = tk.Label(self,
+                          text = gg.HELP_PRESENCE_EFFECTIF,
+                          justify = "left",
                           font = help_label_font)
-    place_bellow(member_analysis_label, 
-                 help_label) 
-    
+    place_bellow(member_analysis_label,
+                 help_label)
+
     ### Bouton pour lancer l'analyse des mots clefs
-    member_analysis_launch_font = tkFont.Font(family = gg.FONT_NAME, 
+    member_analysis_launch_font = tkFont.Font(family = gg.FONT_NAME,
                                                 size = eff_launch_font_size)
-    member_analysis_button = tk.Button(self, 
-                                         text = gg.BUTT_MEMBER_ANALYSIS, 
-                                         font = member_analysis_launch_font, 
-                                         command = lambda: _launch_member_analysis(ctg_path))  
-    place_bellow(help_label, 
-                 member_analysis_button, 
-                 dx = launch_dx_px, 
+    member_analysis_button = tk.Button(self,
+                                         text = gg.BUTT_PRESENCE_EFFECTIF,
+                                         font = member_analysis_launch_font,
+                                         command = lambda: _launch_member_history_analysis(ctg_path))
+    place_bellow(help_label,
+                 member_analysis_button,
+                 dx = launch_dx_px,
                  dy = launch_dy_px)
-    
-################## Analyse de l'évolution de la moyenne d'âge
-    
-    ### Titre 
-    #age_analysis_label_font = tkFont.Font(family = gg.FONT_NAME, 
-    #                                      size = eff_etape_font_size,
-    #                                      weight = 'bold')
-    #age_analysis_label = tk.Label(self, 
-    #                              text = gg.TEXT_AGE_ANALYSIS, 
-    #                              justify = "left", 
-    #                              font = age_analysis_label_font)
-    #place_bellow(member_analysis_button, 
-    #             age_analysis_label, 
-    #             dx = year_analysis_label_dx_px, 
-    #             dy = year_analysis_label_dy_px)
-    #
-    #### Explication de l'étape
-    #help_label_font = tkFont.Font(family = gg.FONT_NAME,
-    #                           size = eff_help_font_size)
-    #help_label_age = tk.Label(self, 
-    #                          text = gg.HELP_AGE_ANALYSIS, 
-    #                          justify = "left", 
-    #                          font = help_label_font)
-    #place_bellow(age_analysis_label, 
-    #             help_label_age) 
-    #
-    #### Bouton pour lancer l'analyse des mots clefs
-    #age_analysis_launch_font = tkFont.Font(family = gg.FONT_NAME, 
-    #                                     size = eff_launch_font_size)
-    #age_analysis_button = tk.Button(self, 
-    #                                text = gg.BUTT_AGE_ANALYSIS, 
-    #                                font = age_analysis_launch_font, 
-    #                                command = lambda: _launch_age_analysis(ctg_path))  
-    #place_bellow(help_label_age, 
-    #             age_analysis_button, 
-    #             dx = launch_dx_px, 
-    #             dy = launch_dy_px)
+
+################## Analyse de l'évolution de la population VAE
+
+    ## Titre
+    vae_analysis_label_font = tkFont.Font(family = gg.FONT_NAME,
+                                          size = eff_etape_font_size,
+                                          weight = 'bold')
+    vae_analysis_label = tk.Label(self,
+                                  text = gg.TEXT_VAE_ANALYSIS,
+                                  justify = "left",
+                                  font = vae_analysis_label_font)
+    place_bellow(member_analysis_button,
+                 vae_analysis_label,
+                 dx = year_analysis_label_dx_px,
+                 dy = year_analysis_label_dy_px)
+
+    ### Explication de l'étape
+    help_label_font = tkFont.Font(family = gg.FONT_NAME,
+                                  size = eff_help_font_size)
+    help_label_vae = tk.Label(self,
+                              text = gg.HELP_VAE_ANALYSIS,
+                              justify = "left",
+                              font = help_label_font)
+    place_bellow(vae_analysis_label,
+                 help_label_vae)
+
+    ### Bouton pour lancer l'analyse evolution VAE
+    vae_analysis_launch_font = tkFont.Font(family = gg.FONT_NAME,
+                                           size = eff_launch_font_size)
+    vae_analysis_button = tk.Button(self,
+                                    text = gg.BUTT_VAE_ANALYSIS,
+                                    font = vae_analysis_launch_font,
+                                    command = lambda: _launch_vae_analysis(ctg_path))
+    place_bellow(help_label_vae,
+                 vae_analysis_button,
+                 dx = launch_dx_px,
+                 dy = launch_dy_px)
```

### Comparing `CTG_Utils-1.2.1/CTG_Utils/CTG_GUI/Useful_Functions.py` & `CTG_Utils-1.2.2/ctgutils/ctggui/useful_functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,110 +1,123 @@
-__all__ = ['encadre_RL', 
-           'encadre_UD', 
+__all__ = ['encadre_RL',
+           'encadre_UD',
            'font_size',
            'get_available_sorties',
            'last_available_years',
            'mm_to_px',
-           'place_after', 
-           'place_bellow', 
+           'place_after',
+           'place_bellow',
            'place_bellow_LabelEntry',
            'str_size_mm',
            'show_frame',
            'create_archi',
            'window_properties'
           ]
 
-def show_frame(self, page_name):        
+# Standard library imports
+import datetime
+import itertools
+import os
+import re
+from calendar import monthrange
+from pathlib import Path
+from tkinter import messagebox
+
+# Standard library imports
+import math
+
+# Local imports
+import ctgutils.ctggui.guiglobals as gg
+from ctgutils.ctggui.guiglobals import IN_TO_MM
+from ctgutils.ctggui.guiglobals import DIR_SORTIES_LIST
+
+
+def show_frame(self, page_name):
     '''Show a frame for the given page name'''
     frame = self.frames[page_name]
     frame.tkraise()
-    
+
 
 def last_available_years(ctg_path, year_number=2021):
-    
+
     '''
     Returns a list of the available five last available years where corpuses are stored
     '''
-        
-    # Standard library imports
-    import os
-    import re
-    from tkinter import messagebox
-    
+
     # Récupérer les corpus disponibles TO DO : consolider le choix des années
     try:
         list_dir = os.listdir(ctg_path)
         years_full_list = list()
         for year in list_dir:
             if re.findall(r'^\d{4}$',year):
                 years_full_list.append(year)
         if year_number is not None:
             years_list = [year for year in years_full_list if int(year)>year_number]
     except FileNotFoundError:
         warning_title = "!!! ATTENTION : Dossier de travail inaccessible !!!"
         warning_text  = f"L'accès au dossier {ctg_path} est impossible."
-        warning_text += f"\nChoisissez un autre dossier de travail."                       
+        warning_text += f"\nChoisissez un autre dossier de travail."
         messagebox.showwarning(warning_title, warning_text)
         years_list = []
     return years_list
 
 def place_after(gauche, droite, dx = 5, dy = 0):
     gauche_info = gauche.place_info()
     x = int(gauche_info['x']) + gauche.winfo_reqwidth() + dx
     y = int(gauche_info['y']) + dy
     droite.place(x = x, y = y)
-    
+
 def place_bellow(haut, bas, dx = 0, dy = 5):
     haut_info = haut.place_info()
     x = int(haut_info['x']) + dx
     y = int(haut_info['y']) + haut.winfo_reqheight() + dy
     bas.place(x = x, y = y)
-    
+
 def encadre_RL(fond, gauche, droite, color = "red", dn = 10, de = 10, ds = 10, dw = 10):
-    
+
     gauche_info = gauche.place_info()
     droite_info = droite.place_info()
 
     x1 = int(gauche_info['x']) - dw
     y1 = int(gauche_info['y']) - dn
-    
+
     x2 = int(gauche_info['x']) + gauche.winfo_reqwidth() + droite.winfo_reqwidth() + de
     y2 = int(droite_info['y']) + max(gauche.winfo_reqheight(), droite.winfo_reqheight()) + ds
 
     rectangle = fond.create_rectangle(x1, y1, x2, y2, outline = color, width = 2)
     fond.place(x = 0, y = 0)
-    
+
 def encadre_UD(fond, haut, bas, color = "red", dn = 10, de = 10, ds = 10, dw = 10):
-    
+
     haut_info = haut.place_info()
     bas_info = bas.place_info()
 
     x1 = int(haut_info['x']) - dw
     y1 = int(haut_info['y']) - dn
-    
+
     x2 = int(bas_info['x']) + max(haut.winfo_reqwidth(), bas.winfo_reqwidth()) + de
     y2 = int(bas_info['y']) + haut.winfo_reqheight() + bas.winfo_reqheight() + ds
 
     rectangle = fond.create_rectangle(x1, y1, x2, y2, outline = color, width = 2)
     fond.place(x = 0, y = 0)
-    
+
 def place_bellow_LabelEntry(haut, label_entry, dx = 0, dy = 5):
-    
+
     haut_info = haut.place_info()
     x = int(haut_info['x']) + dx
     y = int(haut_info['y']) + haut.winfo_reqheight() + dy
     label_entry.place(x = x, y = y)
-    
+
 
 def font_size(size, scale_factor):
     '''Set the fontsize based on scale_factor.
-    If the fontsize is less than minimum_size, 
+    If the fontsize is less than minimum_size,
     it is set to the minimum size.'''
-    
-    fontsize = int(size * scale_factor)    
+
+    fontsize = int(size * scale_factor)
     if fontsize < 8:
         fontsize = 8
     return fontsize
 
 
 def str_size_mm(text, font, ppi):
     '''The function `_str_size_mm` computes the sizes in mm of a string.
@@ -114,167 +127,141 @@
         font (tk.font): the font of the text.
         ppi (int): pixels per inch of the display.
 
     Returns:
         `(tuple)`: width in mm `(float)`, height in mm `(float)`.
 
     Note:
-        The use of this function requires a tkinter window availability 
+        The use of this function requires a tkinter window availability
         since it is based on a tkinter font definition.
 
     '''
 
-    # Local imports
-    from CTG_Utils.CTG_GUI.GUI_Globals import IN_TO_MM
-       
     (w_px,h_px) = (font.measure(text),font.metrics("linespace"))
     w_mm = w_px * IN_TO_MM / ppi
     h_mm = h_px * IN_TO_MM / ppi
 
-    return (w_mm,h_mm )
+    return (w_mm,h_mm)
 
 
 def mm_to_px(size_mm, ppi, fact = 1.0):
     '''The `mm_to_px' function converts a value in mm to a value in pixels
     using the ppi of the used display and a factor fact.
-    
+
     Args:
         size_mm (float): value in mm to be converted.
         ppi ( float): pixels per inch of the display.
         fact (float): factor (default= 1).
-        
+
     Returns:
         `(int)`: upper integer value of the conversion to pixels
-        
+
     '''
-    
-    # Standard library imports 
-    import math
-    
-    # Local imports
-    from CTG_Utils.CTG_GUI.GUI_Globals import IN_TO_MM
 
     size_px = math.ceil((size_mm * fact / IN_TO_MM) * ppi)
-    
+
     return size_px
 
 
 def window_properties(screen_width_px, screen_height_px):
-    # Local imports
-    import CTG_Utils.CTG_GUI.GUI_Globals as gg
-    from CTG_Utils.CTG_GUI.Useful_Functions import mm_to_px
-    
+
     # Getting number of pixels per inch screen resolution from imported global DISPLAYS
     ppi = gg.DISPLAYS[gg.BM_GUI_DISP]["ppi"]
-    
+
     # Setting screen effective sizes in mm from imported global DISPLAYS
     screen_width_mm  = gg.DISPLAYS[gg.BM_GUI_DISP]["width_mm"]
     screen_height_mm = gg.DISPLAYS[gg.BM_GUI_DISP]["height_mm"]
-    
+
     # Setting screen reference sizes in pixels and mm from globals internal to module "Coordinates.py"
     ref_width_px  = gg.REF_SCREEN_WIDTH_PX
     ref_height_px = gg.REF_SCREEN_HEIGHT_PX
     ref_width_mm  = gg.REF_SCREEN_WIDTH_MM
     ref_height_mm = gg.REF_SCREEN_HEIGHT_MM
-    
+
     # Setting secondary window reference sizes in mm from globals internal to module "Coordinates.py"
     ref_window_width_mm  = gg.REF_WINDOW_WIDTH_MM
     ref_window_height_mm = gg.REF_WINDOW_HEIGHT_MM
-    
+
     # Computing ratii of effective screen sizes to screen reference sizes in pixels
     scale_factor_width_px  = screen_width_px / ref_width_px
     scale_factor_height_px = screen_height_px / ref_height_px
-        
-    # Computing ratii of effective screen sizes to screen reference sizes in mm   
+
+    # Computing ratii of effective screen sizes to screen reference sizes in mm
     scale_factor_width_mm  = screen_width_mm / ref_width_mm
     scale_factor_height_mm = screen_height_mm / ref_height_mm
-    
+
     # Computing secondary window sizes in pixels depending on scale factors
-    win_width_px  = mm_to_px(ref_window_width_mm * scale_factor_width_mm, ppi)    
+    win_width_px  = mm_to_px(ref_window_width_mm * scale_factor_width_mm, ppi)
     win_height_px = mm_to_px(ref_window_height_mm * scale_factor_height_mm, ppi)
-    
-    sizes_tuple = (win_width_px, win_height_px, 
-                   scale_factor_width_px, scale_factor_height_px, 
+
+    sizes_tuple = (win_width_px, win_height_px,
+                   scale_factor_width_px, scale_factor_height_px,
                    scale_factor_width_mm, scale_factor_height_mm)
-    
+
     return sizes_tuple
 
 def create_folder(root_path, folder, verbose = False):
-    # Standard library imports
-    import os
-    from pathlib import Path
-    
+
     folder_path = root_path / Path(folder)
-    if not os.path.exists(folder_path): 
+    if not os.path.exists(folder_path):
         os.makedirs(folder_path)
         message = f"{folder_path} created"
     else:
         message = f"{folder_path} already exists"
     if verbose : print(message)
     return folder_path
-    
+
 def create_archi(ctg_path, year_folder, verbose = False):
     '''The `create_archi` function creates a corpus folder with the required architecture.
     It uses the global "ARCHI_YEAR" for the names of the sub_folders.
-    
+
     Args:
         ctg_path (path): The full path of the working folder.
         year_folder (str): The name of the folder of the corpus.
-        
+
     Returns:
         (str): The message giving the folder creation status.
-    
+
     '''
-   
-    # Internal import imports
-    from pathlib import Path
-    
+
     dir_list = ['DATA','SEJOUR', 'SORTIES DE DERNIERE MINUTE','SORTIES DU DIMANCHE', 'SORTIES DU JEUDI',
                 'SORTIES DU SAMEDI','SORTIES HIVER', 'SORTIES VTT', 'STATISTIQUES']
-                
+
     new_year_folder_path = create_folder(ctg_path, year_folder, verbose = verbose)
     for dir in dir_list:
         _ = create_folder(new_year_folder_path, dir, verbose = verbose)
-    
+
     dir_list_sorties = ['SEJOUR', 'SORTIES DE DERNIERE MINUTE','SORTIES DU DIMANCHE', 'SORTIES DU JEUDI',
                 'SORTIES DU SAMEDI','SORTIES HIVER', 'SORTIES VTT']
-                
+
     for dir in dir_list_sorties:
         _ = create_folder(Path(ctg_path) / Path(year_folder) / Path(dir), 'CSV', verbose = verbose)
         _ = create_folder(Path(ctg_path) / Path(year_folder) / Path(dir), 'EXCEL', verbose = verbose)
-    
+
     jours_sortie_club(year_folder,ctg_path)
     message = f"Architecture created for {year_folder} folder"
     return message
 
 def jours_sortie_club(year,ctg_path):
 
-    import itertools
-    from calendar import monthrange
-    import datetime
-    import os
-    from pathlib import Path
-
-    import CTG_Utils.CTG_Func as ctg
-
     days_dict = {0: 'dimanche',
                  1: 'Lundi',
                  2: 'mardi',
                  3: 'mercredi',
                  4: 'jeudi',
                  5: 'vendredi',
                  6: 'samedi'}
     inv_days_dict = dict(zip(days_dict.values(),days_dict.keys()))
     month_dict = dict(zip(itertools.islice(itertools.cycle(l:=range(1,13)),2,2+len(l)),l))
 
     root = Path(ctg_path) / Path(str(year))
 
     for day in ['dimanche','samedi','jeudi']:
         path = ctg_path / Path(str(year)) / Path('SORTIES DU '+day.upper()) / Path('CSV')
-            
+
         r = []
         rw = []
         for m in range(1,13):
             m_save=m
             y = int(year)%100
             c = int(int(year)/100)
             m = month_dict[m]
@@ -283,31 +270,24 @@
             for d in range (1,nb_days+1):
                 if (d + int(2.6*m - 0.2) - 2*c + y + int(c/4) + int(y/4))%7 == inv_days_dict[day]:
                     r.append(f'{str(m_save).zfill(2)}_{str(d).zfill(2)} sortie du {day}.csv')
                     try:
                         num_week = datetime.date(year,m_save, d).isocalendar().week
                     except:
                         num_week = None
-                    
+
                     if num_week is not None:
                         rw.append((f'{str(m_save).zfill(2)}_{str(d).zfill(2)} sortie du {day}.csv' ,
                                         num_week))
-                    
+
                     file_name = f'{year}_{str(m_save).zfill(2)}_{str(d).zfill(2)} sortie du {day}.csv'
                     with open(os.path.join(path,file_name), 'w') as fp:
                         fp.write(f'{str(year)} SORTIES DU {day.upper()}')
- 
+
 def get_available_sorties(ctg_path,year):
-    
-    # Standard library imports
-    import os
-    from pathlib import Path
-
-    # Internal imports
-    from CTG_Utils.CTG_GUI.GUI_Globals import DIR_SORTIES_LIST
-    
-    year_path = ctg_path / Path(str(year)) 
+
+    year_path = ctg_path / Path(str(year))
     dir_year_list = os.listdir(year_path)
 
     available_sorties_list = list(set(DIR_SORTIES_LIST).intersection(dir_year_list))
-    
-    return available_sorties_list 
+
+    return available_sorties_list
```

### Comparing `CTG_Utils-1.2.1/CTG_Utils.egg-info/PKG-INFO` & `CTG_Utils-1.2.2/CTG_Utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTG-Utils
-Version: 1.2.1
+Version: 1.2.2
 Summary: A toolbox for ctg statistics analysis
 Home-page: https://github.com/Bertin-fap/CTG_Utils 
 Author: f. bertin
 Author-email: francois.bertin7@wanadoo.fr
 License: MIT
 Keywords: ffvelo,ctg
 Platform: UNKNOWN
```

### Comparing `CTG_Utils-1.2.1/LICENSE` & `CTG_Utils-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.2.1/PKG-INFO` & `CTG_Utils-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTG_Utils
-Version: 1.2.1
+Version: 1.2.2
 Summary: A toolbox for ctg statistics analysis
 Home-page: https://github.com/Bertin-fap/CTG_Utils 
 Author: f. bertin
 Author-email: francois.bertin7@wanadoo.fr
 License: MIT
 Keywords: ffvelo,ctg
 Platform: UNKNOWN
```

### Comparing `CTG_Utils-1.2.1/setup.py` & `CTG_Utils-1.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = f.read()
 
 install_requires = open(path.join(this_directory, 'requirements.txt'), encoding='utf-8').read().strip().split('\n') 
 
 # This setup is suitable for "python setup.py develop".
 
 setup(name='CTG_Utils',
-      version='1.2.1',
+      version='1.2.2',
       description='A toolbox for ctg statistics analysis',
       long_description=long_description,
       long_description_content_type='text/markdown',
       include_package_data = True,
       license = 'MIT',
       classifiers = [
         'Development Status :: 4 - Beta',
@@ -28,9 +28,9 @@
         'Intended Audience :: Science/Research'
         ],
       keywords = 'ffvelo,ctg',
       install_requires = install_requires,
       author= 'f. bertin',
       author_email= 'francois.bertin7@wanadoo.fr',
       url= 'https://github.com/Bertin-fap/CTG_Utils ',
-      packages=['CTG_Utils\CTG_Func','CTG_Utils\CTG_GUI'],
+      packages=['ctgutils\ctgFuncts','ctgutils\ctggui'],
       )
```

