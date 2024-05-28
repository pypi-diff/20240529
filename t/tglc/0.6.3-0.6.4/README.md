# Comparing `tmp/tglc-0.6.3.tar.gz` & `tmp/tglc-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tglc-0.6.3.tar", last modified: Thu Apr 25 03:59:06 2024, max compression
+gzip compressed data, was "tglc-0.6.4.tar", last modified: Tue May 28 23:42:40 2024, max compression
```

## Comparing `tglc-0.6.3.tar` & `tglc-0.6.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 tehan     (1000) tehan     (1000)        0 2024-04-25 03:59:06.940890 tglc-0.6.3/
--rw-rw-r--   0 tehan     (1000) tehan     (1000)     1063 2022-09-16 07:04:15.000000 tglc-0.6.3/LICENSE
--rw-rw-r--   0 tehan     (1000) tehan     (1000)       35 2022-09-16 07:04:15.000000 tglc-0.6.3/MANIFEST.in
--rw-rw-r--   0 tehan     (1000) tehan     (1000)     5779 2024-04-25 03:59:06.940890 tglc-0.6.3/PKG-INFO
--rw-rw-r--   0 tehan     (1000) tehan     (1000)     4890 2024-04-25 03:59:03.000000 tglc-0.6.3/README.rst
--rw-rw-r--   0 tehan     (1000) tehan     (1000)       38 2024-04-25 03:59:06.940890 tglc-0.6.3/setup.cfg
--rw-rw-r--   0 tehan     (1000) tehan     (1000)      925 2024-04-25 03:57:37.000000 tglc-0.6.3/setup.py
-drwxrwxr-x   0 tehan     (1000) tehan     (1000)        0 2024-04-25 03:59:06.940890 tglc-0.6.3/tglc/
--rw-rw-r--   0 tehan     (1000) tehan     (1000)      115 2024-04-25 03:57:37.000000 tglc-0.6.3/tglc/__init__.py
-drwxrwxr-x   0 tehan     (1000) tehan     (1000)        0 2024-04-25 03:59:06.940890 tglc-0.6.3/tglc/background_mask/
--rw-rw-r--   0 tehan     (1000) tehan     (1000)        0 2022-09-16 07:04:15.000000 tglc-0.6.3/tglc/background_mask/__init__.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)   267840 2022-09-16 07:04:15.000000 tglc-0.6.3/tglc/background_mask/median_mask.fits
--rw-rw-r--   0 tehan     (1000) tehan     (1000)    22712 2024-02-26 08:55:20.000000 tglc-0.6.3/tglc/effective_psf.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)    15649 2024-04-25 03:57:17.000000 tglc-0.6.3/tglc/ffi.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)    11963 2024-04-25 03:57:17.000000 tglc-0.6.3/tglc/ffi_cut.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)   136246 2024-04-25 00:29:36.000000 tglc-0.6.3/tglc/lc_plot.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)     4331 2023-03-18 21:06:07.000000 tglc-0.6.3/tglc/mast.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)    27838 2024-04-25 00:51:21.000000 tglc-0.6.3/tglc/quick_lc.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)     4123 2024-04-25 00:29:12.000000 tglc-0.6.3/tglc/run.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)     3171 2024-04-25 00:29:12.000000 tglc-0.6.3/tglc/source_output.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)    20692 2024-04-25 00:29:12.000000 tglc-0.6.3/tglc/target_lightcurve.py
-drwxrwxr-x   0 tehan     (1000) tehan     (1000)        0 2024-04-25 03:59:06.940890 tglc-0.6.3/tglc.egg-info/
--rw-rw-r--   0 tehan     (1000) tehan     (1000)     5779 2024-04-25 03:59:06.000000 tglc-0.6.3/tglc.egg-info/PKG-INFO
--rw-rw-r--   0 tehan     (1000) tehan     (1000)      422 2024-04-25 03:59:06.000000 tglc-0.6.3/tglc.egg-info/SOURCES.txt
--rw-rw-r--   0 tehan     (1000) tehan     (1000)        1 2024-04-25 03:59:06.000000 tglc-0.6.3/tglc.egg-info/dependency_links.txt
--rw-rw-r--   0 tehan     (1000) tehan     (1000)       96 2024-04-25 03:59:06.000000 tglc-0.6.3/tglc.egg-info/requires.txt
--rw-rw-r--   0 tehan     (1000) tehan     (1000)        5 2024-04-25 03:59:06.000000 tglc-0.6.3/tglc.egg-info/top_level.txt
+drwxrwxr-x   0 tehan     (1000) tehan     (1000)        0 2024-05-28 23:42:40.288577 tglc-0.6.4/
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)     1063 2022-09-16 07:04:15.000000 tglc-0.6.4/LICENSE
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)       35 2024-04-25 04:05:59.000000 tglc-0.6.4/MANIFEST.in
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)     5313 2024-05-28 23:42:40.288577 tglc-0.6.4/PKG-INFO
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)     4890 2024-05-28 23:42:29.000000 tglc-0.6.4/README.rst
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)       38 2024-05-28 23:42:40.288577 tglc-0.6.4/setup.cfg
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)      925 2024-05-28 23:32:35.000000 tglc-0.6.4/setup.py
+drwxrwxr-x   0 tehan     (1000) tehan     (1000)        0 2024-05-28 23:42:40.288577 tglc-0.6.4/tglc/
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)      115 2024-05-28 23:32:35.000000 tglc-0.6.4/tglc/__init__.py
+drwxrwxr-x   0 tehan     (1000) tehan     (1000)        0 2024-05-28 23:42:40.288577 tglc-0.6.4/tglc/background_mask/
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)        0 2024-04-25 04:05:59.000000 tglc-0.6.4/tglc/background_mask/__init__.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)   267840 2024-04-25 04:05:59.000000 tglc-0.6.4/tglc/background_mask/median_mask.fits
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)    22712 2024-05-03 21:42:24.000000 tglc-0.6.4/tglc/effective_psf.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)    15656 2024-05-07 21:02:06.000000 tglc-0.6.4/tglc/ffi.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)    11969 2024-05-07 21:02:06.000000 tglc-0.6.4/tglc/ffi_cut.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)   136246 2024-05-03 21:42:24.000000 tglc-0.6.4/tglc/lc_plot.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)     4331 2024-05-03 21:42:24.000000 tglc-0.6.4/tglc/mast.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)    27132 2024-05-28 23:30:57.000000 tglc-0.6.4/tglc/quick_lc.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)     4123 2024-05-03 21:42:24.000000 tglc-0.6.4/tglc/run.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)     3171 2024-05-03 21:42:24.000000 tglc-0.6.4/tglc/source_output.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)    20692 2024-05-07 21:02:06.000000 tglc-0.6.4/tglc/target_lightcurve.py
+drwxrwxr-x   0 tehan     (1000) tehan     (1000)        0 2024-05-28 23:42:40.288577 tglc-0.6.4/tglc.egg-info/
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)     5313 2024-05-28 23:42:40.000000 tglc-0.6.4/tglc.egg-info/PKG-INFO
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)      422 2024-05-28 23:42:40.000000 tglc-0.6.4/tglc.egg-info/SOURCES.txt
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)        1 2024-05-28 23:42:40.000000 tglc-0.6.4/tglc.egg-info/dependency_links.txt
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)       96 2024-05-28 23:42:40.000000 tglc-0.6.4/tglc.egg-info/requires.txt
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)        5 2024-05-28 23:42:40.000000 tglc-0.6.4/tglc.egg-info/top_level.txt
```

### Comparing `tglc-0.6.3/LICENSE` & `tglc-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tglc-0.6.3/PKG-INFO` & `tglc-0.6.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,69 @@
 Metadata-Version: 2.1
 Name: tglc
-Version: 0.6.3
+Version: 0.6.4
 Summary: TESS-Gaia Light Curve
 Home-page: https://github.com/TeHanHunter/TESS_Gaia_Light_Curve
 Author: Te Han
 Author-email: tehanhunter@gmail.com
-License: UNKNOWN
-Description: ==================================
-        Introduction
-        ==================================
-        
-        TESS-Gaia Light Curve (`TGLC <https://archive.stsci.edu/hlsp/tglc>`_) is a dataset of TESS full-frame image light curves publicly available via the MAST portal. It is fitted with effective PSF and decontaminated with Gaia DR3 and achieved percent-level photometric precision down to 16th TESS magnitude! It unlocks astrophysics to a vast number of dim stars below 12th TESS magnitude. A package called tglc is pip-installable for customized light curve fits.
-        
-        ==================================
-        Usage
-        ==================================
-        There are four fluxes in each FITS file: aperture flux, PSF flux, calibrated aperture flux, and calibrated PSF flux.
-        If you are uncertain which to use:
-        
-        * Calibrated psf flux is better in **deblending** targets. Use this if you need to deblend a target near a variable source. The best deblending can be achieved with tglc package by setting a non-zero prior. It also gives the more accurate **transit depth** in most cases, especially when fitting with an optimized prior.
-        * Calibrated aperture flux usually has slightly **higher SNR**. The transit depth (or variation amplitude), however, can be imperfect since the normalization depends on the PSF fitting which is imperfect. This imperfection can be minimized by using a bigger aperture than the default aperture (3*3). One need to use the tglc package and set tglc_lc(save_aper=True) to access the 5*5 aperture. In the presence of a bright but "constant" contamination (several magnitudes brighter), the calibrated aperture flux is better in removing the constant contamination. 
-        * The aperture flux and PSF flux are not detrended or normalized. Use this if you are doing stellar variability science with long baseline. Or, if the detrending is not optimal (default detrending has a window length of 1 day; see Known Problems below), start with the aperture flux or PSF flux and detrend carefully!
-        * **If you are uncertain, start with calibrated aperture flux!**
-        
-        The `tutorial <tutorial/TGLC_tutorial.ipynb>`_ shows the syntaxes and differences among these light curves in several examples.
-        
-        ==================================
-        Data Access
-        ==================================
-        There are three data access methods:
-        
-        * MAST Portal: Easiest for acquiring light curves for a few stars. However, new sectors are updated relatively slowly. 
-        * MAST bulk download: Best for downloading light curves for all stars (<16 TESS magnitude) in a sectors. 
-        * tglc package: Capable of producing similar quality light curves for any sector and any star with custom options. 
-        
-        MAST Portal/bulk download
-        ----------------------------
-        The easiest usage requires no package installation. Simply follow the `TGLC HLSP page <https://archive.stsci.edu/hlsp/tglc>`_ to download light curves from MAST or use `MAST Portal <https://mast.stsci.edu/portal/Mashup/Clients/Mast/Portal.html>`_. Light curves are being fitted sector by sector and will be available on MAST gradually. MAST hosts all Gaia DR3 stars down to 16th magnitude. Each .fits file includes PSF and aperture light curves and their calibrated versions.
-        
-        MAST available sectors: `sector worklist <https://docs.google.com/spreadsheets/d/1FhHElWb1wmx9asWiZecAJ2umN0-P_aXn55OBVB34_rg/edit?usp=sharing>`_
-        
-        
-        tglc package
-        ----------------------------
-        Users can also fit light curves using the package tglc. Using tglc, one can specify a region, sector(s), and customized aperture shape if needed. It can also allow all field stars to float by assigning Gaussian priors, which can help decontaminate variable field stars. tglc is currently only available for linux. Run::
-        
-          pip install tglc
-          
-        for the latest tglc release. After installation, follow the `tutorial <tutorial/TGLC_tutorial.ipynb>`_ to fit light curves. If there is a problem, please leave a comment in the Issues section to help us improve. Thank you!
-        
-        
-        ==================================
-        Known Problems
-        ==================================
-        There are several imperfections we noticed in the MAST TGLC light curves and tglc package:
-        
-        * If the star is very dim (~< 15 Tmag) near a variable source, it can make the aperture and/or PSF light curve negative for some cadences. The detrending algorithm could malfunction and result in bad cal_aper_flux and/or cal_psf_flux. This is now fixed for tglc package, but this problem remains for the primary mission light curves published on MAST. Please detrend again if necessary. The extended mission light curves on MAST will not be affected. This is a very rare scenario, but could be important.
-        
-        ==================================
-        Reference
-        ==================================
-        If you find the TGLC light curves or the tglc package useful in your research, please cite `our paper <https://iopscience.iop.org/article/10.3847/1538-3881/acaaa7>`_ published on the Astronomical Journal. 
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+==================================
+Introduction
+==================================
+
+TESS-Gaia Light Curve (`TGLC <https://archive.stsci.edu/hlsp/tglc>`_) is a dataset of TESS full-frame image light curves publicly available via the MAST portal. It is fitted with effective PSF and decontaminated with Gaia DR3 and achieved percent-level photometric precision down to 16th TESS magnitude! It unlocks astrophysics to a vast number of dim stars below 12th TESS magnitude. A package called tglc is pip-installable for customized light curve fits.
+
+==================================
+Usage
+==================================
+There are four fluxes in each FITS file: aperture flux, PSF flux, calibrated aperture flux, and calibrated PSF flux.
+If you are uncertain which to use:
+
+* Calibrated psf flux is better in **deblending** targets. Use this if you need to deblend a target near a variable source. The best deblending can be achieved with tglc package by setting a non-zero prior. It also gives the more accurate **transit depth** in most cases, especially when fitting with an optimized prior.
+* Calibrated aperture flux usually has slightly **higher SNR**. The transit depth (or variation amplitude), however, can be imperfect since the normalization depends on the PSF fitting which is imperfect. This imperfection can be minimized by using a bigger aperture than the default aperture (3*3). One need to use the tglc package and set tglc_lc(save_aper=True) to access the 5*5 aperture. In the presence of a bright but "constant" contamination (several magnitudes brighter), the calibrated aperture flux is better in removing the constant contamination. 
+* The aperture flux and PSF flux are not detrended or normalized. Use this if you are doing stellar variability science with long baseline. Or, if the detrending is not optimal (default detrending has a window length of 1 day; see Known Problems below), start with the aperture flux or PSF flux and detrend carefully!
+* **If you are uncertain, start with calibrated aperture flux!**
+
+The `tutorial <tutorial/TGLC_tutorial.ipynb>`_ shows the syntaxes and differences among these light curves in several examples.
+
+==================================
+Data Access
+==================================
+There are three data access methods:
+
+* MAST Portal: Easiest for acquiring light curves for a few stars. However, new sectors are updated relatively slowly. 
+* MAST bulk download: Best for downloading light curves for all stars (<16 TESS magnitude) in a sectors. 
+* tglc package: Capable of producing similar quality light curves for any sector and any star with custom options. 
+
+MAST Portal/bulk download
+----------------------------
+The easiest usage requires no package installation. Simply follow the `TGLC HLSP page <https://archive.stsci.edu/hlsp/tglc>`_ to download light curves from MAST or use `MAST Portal <https://mast.stsci.edu/portal/Mashup/Clients/Mast/Portal.html>`_. Light curves are being fitted sector by sector and will be available on MAST gradually. MAST hosts all Gaia DR3 stars down to 16th magnitude. Each .fits file includes PSF and aperture light curves and their calibrated versions.
+
+MAST available sectors: `sector worklist <https://docs.google.com/spreadsheets/d/1FhHElWb1wmx9asWiZecAJ2umN0-P_aXn55OBVB34_rg/edit?usp=sharing>`_
+
+
+tglc package
+----------------------------
+Users can also fit light curves using the package tglc. Using tglc, one can specify a region, sector(s), and customized aperture shape if needed. It can also allow all field stars to float by assigning Gaussian priors, which can help decontaminate variable field stars. tglc is currently only available for linux. Run::
+
+  pip install tglc
+  
+for the latest tglc release. After installation, follow the `tutorial <tutorial/TGLC_tutorial.ipynb>`_ to fit light curves. If there is a problem, please leave a comment in the Issues section to help us improve. Thank you!
+
+
+==================================
+Known Problems
+==================================
+There are several imperfections we noticed in the MAST TGLC light curves and tglc package:
+
+* If the star is very dim (~< 15 Tmag) near a variable source, it can make the aperture and/or PSF light curve negative for some cadences. The detrending algorithm could malfunction and result in bad cal_aper_flux and/or cal_psf_flux. This is now fixed for tglc package, but this problem remains for the primary mission light curves published on MAST. Please detrend again if necessary. The extended mission light curves on MAST will not be affected. This is a very rare scenario, but could be important.
+
+==================================
+Reference
+==================================
+If you find the TGLC light curves or the tglc package useful in your research, please cite `our paper <https://iopscience.iop.org/article/10.3847/1538-3881/acaaa7>`_ published on the Astronomical Journal.
```

### Comparing `tglc-0.6.3/README.rst` & `tglc-0.6.4/README.rst`

 * *Files identical despite different names*

### Comparing `tglc-0.6.3/setup.py` & `tglc-0.6.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 sys.path.insert(0, "tglc")
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="tglc",
-    version='0.6.3',
+    version='0.6.4',
     author="Te Han",
     author_email="tehanhunter@gmail.com",
     description="TESS-Gaia Light Curve",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/TeHanHunter/TESS_Gaia_Light_Curve",
     classifiers=[
```

### Comparing `tglc-0.6.3/tglc/background_mask/median_mask.fits` & `tglc-0.6.4/tglc/background_mask/median_mask.fits`

 * *Files identical despite different names*

### Comparing `tglc-0.6.3/tglc/effective_psf.py` & `tglc-0.6.4/tglc/effective_psf.py`

 * *Files identical despite different names*

### Comparing `tglc-0.6.3/tglc/ffi.py` & `tglc-0.6.4/tglc/ffi.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
 
     def search_gaia(self, x, y, co1, co2):
         coord = self.wcs.pixel_to_world([x + co1 + 44], [y + co2])[0].to_string()
         radius = u.Quantity((self.size / 2 + 4) * 21 * 0.707 / 3600, u.deg)
         attempt = 0
         while attempt < 5:
             try:
-                catalogdata = Gaia.cone_search_async(coord, radius,
+                catalogdata = Gaia.cone_search_async(coord, radius=radius,
                                              columns=['DESIGNATION', 'phot_g_mean_mag', 'phot_bp_mean_mag',
                                                       'phot_rp_mean_mag', 'ra', 'dec', 'pmra', 'pmdec']).get_results()
                 return catalogdata
             except:
                 attempt += 1
                 time.sleep(10)
                 print(f'Trying Gaia search again. Coord = {coord}, radius = {radius}')
```

### Comparing `tglc-0.6.3/tglc/ffi_cut.py` & `tglc-0.6.4/tglc/ffi_cut.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         if len(target) == 0:
             target = Catalogs.query_object(self.name, radius=5 * 21 * 0.707 / 3600, catalog="Gaia", version=2)
         ra = target[0]['ra']
         dec = target[0]['dec']
         coord = SkyCoord(ra=ra, dec=dec, unit=(u.degree, u.degree), frame='icrs')
         radius = u.Quantity((self.size + 6) * 21 * 0.707 / 3600, u.deg)
         print(f'Target Gaia: {target[0]["designation"]}')
-        catalogdata = Gaia.cone_search_async(coord, radius,
+        catalogdata = Gaia.cone_search_async(coord, radius=radius,
                                              columns=['DESIGNATION', 'phot_g_mean_mag', 'phot_bp_mean_mag',
                                                       'phot_rp_mean_mag', 'ra', 'dec', 'pmra', 'pmdec']).get_results()
         print(f'Found {len(catalogdata)} Gaia DR3 objects.')
         catalogdata_tic = tic_advanced_search_position_rows(ra=ra, dec=dec, radius=(self.size + 2) * 21 * 0.707 / 3600, limit_mag=limit_mag)
         print(f'Found {len(catalogdata_tic)} TIC objects.')
         self.tic = convert_gaia_id(catalogdata_tic)
         sector_table = Tesscut.get_sectors(coordinates=coord)
@@ -90,15 +90,14 @@
             sector_list.append(hdulist[i][0].header['SECTOR'])
         self.sector_list = sector_list
         if sector is None:
             self.select_sector(sector=sector_table['sector'][0])
         else:
             self.select_sector(sector=sector)
 
-
     def select_sector(self, sector=1):
         """
         select sector to use if target is in multi-sectors
         :param sector: int, required
         TESS sector number
         """
         if self.sector == sector:
```

### Comparing `tglc-0.6.3/tglc/lc_plot.py` & `tglc-0.6.4/tglc/lc_plot.py`

 * *Files identical despite different names*

### Comparing `tglc-0.6.3/tglc/mast.py` & `tglc-0.6.4/tglc/mast.py`

 * *Files identical despite different names*

### Comparing `tglc-0.6.3/tglc/quick_lc.py` & `tglc-0.6.4/tglc/quick_lc.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,19 +26,19 @@
 @controller.wrap(limits=1, user_api='blas')
 def tglc_lc(target='TIC 264468702', local_directory='', size=90, save_aper=True, limit_mag=16, get_all_lc=False,
             first_sector_only=False, last_sector_only=False, sector=None, prior=None, transient=None):
     '''
     Generate light curve for a single target.
 
     :param target: target identifier
-    :type target: str, required
+    :kind target: str, required
     :param local_directory: output directory
-    :type local_directory: str, required
+    :kind local_directory: str, required
     :param size: size of the FFI cut, default size is 90. Recommend large number for better quality. Cannot exceed 100.
-    :type size: int, optional
+    :kind size: int, optional
     '''
     os.makedirs(local_directory + f'logs/', exist_ok=True)
     os.makedirs(local_directory + f'lc/', exist_ok=True)
     os.makedirs(local_directory + f'epsf/', exist_ok=True)
     os.makedirs(local_directory + f'source/', exist_ok=True)
     if first_sector_only:
         sector = 'first'
@@ -157,47 +157,47 @@
                  tics=None, local_directory=None):
     for i in range(server, 27, 2):
         with Pool(16) as p:
             p.map(partial(search_stars, sector=i, tics=tics, local_directory=local_directory), range(16))
     return
 
 
-def plot_lc(local_directory=None, type='cal_aper_flux', xlow=None, xhigh=None, ylow=None, yhigh=None):
+def plot_lc(local_directory=None, kind='cal_aper_flux', xlow=None, xhigh=None, ylow=None, yhigh=None):
     files = glob(f'{local_directory}lc/*.fits')
     os.makedirs(f'{local_directory}plots/', exist_ok=True)
     for i in range(len(files)):
         with fits.open(files[i], mode='denywrite') as hdul:
             q = [a and b for a, b in zip(list(hdul[1].data['TESS_flags'] == 0), list(hdul[1].data['TGLC_flags'] == 0))]
             plt.figure(constrained_layout=False, figsize=(8, 4))
-            plt.plot(hdul[1].data['time'], hdul[1].data[type], '.', c='silver', label=type)
-            plt.plot(hdul[1].data['time'][q], hdul[1].data[type][q], '.k', label=f'{type}_flagged')
+            plt.plot(hdul[1].data['time'], hdul[1].data[kind], '.', c='silver', label=kind)
+            plt.plot(hdul[1].data['time'][q], hdul[1].data[kind][q], '.k', label=f'{kind}_flagged')
             plt.xlim(xlow, xhigh)
             plt.ylim(ylow, yhigh)
-            plt.title(f'TIC_{hdul[0].header["TICID"]}_sector_{hdul[0].header["SECTOR"]:04d}_{type}')
+            plt.title(f'TIC_{hdul[0].header["TICID"]}_sector_{hdul[0].header["SECTOR"]:04d}_{kind}')
             plt.legend()
             # plt.show()
             plt.savefig(
-                f'{local_directory}plots/TIC_{hdul[0].header["TICID"]}_sector_{hdul[0].header["SECTOR"]:04d}_{type}.png',
+                f'{local_directory}plots/TIC_{hdul[0].header["TICID"]}_sector_{hdul[0].header["SECTOR"]:04d}_{kind}.png',
                 dpi=300)
             plt.close()
 
 
-def plot_aperture(local_directory=None, type='cal_aper_flux'):
+def plot_aperture(local_directory=None, kind='cal_aper_flux'):
     files = glob(f'{local_directory}*.fits')
     os.makedirs(f'{local_directory}plots/', exist_ok=True)
     portion = [0.9361215204370542, 0.9320709087810205]
     data = np.empty((3, 0))
 
     for i in range(len(files)):
         with fits.open(files[i], mode='denywrite') as hdul:
             print(files[i], portion[i])
             q = [a and b for a, b in zip(list(hdul[1].data['TESS_flags'] == 0), list(hdul[1].data['TGLC_flags'] == 0))]
             plt.figure(constrained_layout=False, figsize=(8, 4))
-            plt.plot(hdul[1].data['time'] % 3.79262026, hdul[1].data[type], '.', c='silver', label=type)
-            plt.plot(hdul[1].data['time'][q] % 3.79262026, hdul[1].data[type][q], '.k', label=f'{type}_flagged')
+            plt.plot(hdul[1].data['time'] % 3.79262026, hdul[1].data[kind], '.', c='silver', label=kind)
+            plt.plot(hdul[1].data['time'][q] % 3.79262026, hdul[1].data[kind][q], '.k', label=f'{kind}_flagged')
             aperture_bar = 709.5512462444653 * portion[i]
             aper_lc = np.nansum(hdul[0].data, axis=(1, 2))
             local_bg = np.nanmedian(aper_lc) - aperture_bar
             aper_lc = (aper_lc - local_bg) / portion[i]
             cal_aper_lc = aper_lc / np.nanmedian(aper_lc)
             cal_aper_lc[np.where(cal_aper_lc > 100)] = np.nan
             _, trend = flatten(hdul[1].data['time'], cal_aper_lc - np.nanmin(cal_aper_lc) + 1000,
@@ -222,74 +222,74 @@
                               flux[not_nan],
                               np.array([f_err] * len(time[not_nan]))
                               ])
             data = np.append(data, data_, axis=1)
     np.savetxt(f'{local_directory}TESS_TOI-5344_5_5_aper.csv', data, delimiter=',')
 
 
-def plot_pf_lc(local_directory=None, period=None, mid_transit_tbjd=None, type='cal_aper_flux'):
+def plot_pf_lc(local_directory=None, period=None, mid_transit_tbjd=None, kind='cal_aper_flux'):
     files = glob(f'{local_directory}*.fits')
     os.makedirs(f'{local_directory}plots/', exist_ok=True)
     fig = plt.figure(figsize=(13, 5))
     t_all = np.array([])
     f_all = np.array([])
     f_err_all = np.array([])
     for j in range(len(files)):
         not_plotted_num = 0
         with fits.open(files[j], mode='denywrite') as hdul:
             q = [a and b for a, b in
                  zip(list(hdul[1].data['TESS_flags'] == 0), list(hdul[1].data['TGLC_flags'] == 0))]
-            # q = [a and b for a, b in zip(q, list(hdul[1].data[type] > 0.85))]
+            # q = [a and b for a, b in zip(q, list(hdul[1].data[kind] > 0.85))]
             # if hdul[0].header['sector'] == 15:
             #     q = [a and b for a, b in zip(q, list(hdul[1].data['time'] < 1736))]
             if len(hdul[1].data['cal_aper_flux']) == len(hdul[1].data['time']):
                 if hdul[0].header["SECTOR"] <= 26:
                     t = hdul[1].data['time'][q]
-                    f = hdul[1].data[type][q]
+                    f = hdul[1].data[kind][q]
                 elif hdul[0].header["SECTOR"] <= 55:
                     t = np.mean(hdul[1].data['time'][q][:len(hdul[1].data['time'][q]) // 3 * 3].reshape(-1, 3), axis=1)
                     f = np.mean(
-                        hdul[1].data[type][q][:len(hdul[1].data[type][q]) // 3 * 3].reshape(-1, 3), axis=1)
+                        hdul[1].data[kind][q][:len(hdul[1].data[kind][q]) // 3 * 3].reshape(-1, 3), axis=1)
                 else:
                     t = np.mean(hdul[1].data['time'][q][:len(hdul[1].data['time'][q]) // 9 * 9].reshape(-1, 9), axis=1)
                     f = np.mean(
-                        hdul[1].data[type][q][:len(hdul[1].data[type][q]) // 9 * 9].reshape(-1, 9), axis=1)
+                        hdul[1].data[kind][q][:len(hdul[1].data[kind][q]) // 9 * 9].reshape(-1, 9), axis=1)
                 t_all = np.append(t_all, t)
                 f_all = np.append(f_all, f)
                 f_err_all = np.append(f_err_all, np.array([hdul[1].header['CAPE_ERR']] * len(t)))
 
-                # plt.plot(hdul[1].data['time'] % period / period, hdul[1].data[type], '.', c='silver', ms=3)
-                plt.errorbar(t % period / period, f, hdul[1].header['CAPE_ERR'], c='silver', ls='', elinewidth=1.5,
+                # plt.plot(hdul[1].data['time'] % period / period, hdul[1].data[kind], '.', c='silver', ms=3)
+                plt.errorbar(t % period / period, f, hdul[1].header['CAPE_ERR'], c='silver', ls='', elinewidth=0.1,
                              marker='.', ms=3, zorder=2)
                 # time_out, meas_out, meas_err_out = timebin(time=t % period, meas=f,
                 #                                            meas_err=np.array([hdul[1].header['CAPE_ERR']] * len(t)),
                 #                                            binsize=600 / 86400)
                 # plt.errorbar(np.array(time_out) / period, meas_out, meas_err_out, c=f'C{j}', ls='', elinewidth=1.5,
                 #              marker='.', ms=8, zorder=3, label=f'Sector {hdul[0].header["sector"]}')
             else:
                 not_plotted_num += 1
-            title = f'TIC_{hdul[0].header["TICID"]} with {len(files) - not_plotted_num} sector(s) of data, {type}'
+            title = f'TIC_{hdul[0].header["TICID"]} with {len(files) - not_plotted_num} sector(s) of data, {kind}'
     # PDCSAP_files = glob('/home/tehan/Documents/GEMS/TIC 172370679/PDCSAP/*.txt')
     # for i in range(len(files)):
     #     PDCSAP = ascii.read(PDCSAP_files[i])
     #     t = np.mean(PDCSAP['col1'][:len(PDCSAP['col1']) // 15 * 15].reshape(-1, 15), axis=1)
     #     f = np.mean(PDCSAP['col2'][:len(PDCSAP['col2']) // 15 * 15].reshape(-1, 15), axis=1)
     #     ferr = np.mean(PDCSAP['col3'][:len(PDCSAP['col3']) // 15 * 15].reshape(-1, 15), axis=1)
     #     plt.errorbar((t - 2457000) % period / period, f, ferr, c='C0', ls='', elinewidth=0, marker='.', ms=2, zorder=1)
     time_out, meas_out, meas_err_out = timebin(time=t_all % period, meas=f_all,
                                                meas_err=f_err_all,
                                                binsize=300 / 86400)
     plt.errorbar(np.array(time_out) / period, meas_out, meas_err_out, c=f'r', ls='', elinewidth=1.5,
                  marker='.', ms=8, zorder=3, label=f'All sectors')
 
-    plt.ylim(0.87, 1.05)
+    plt.ylim(0.998, 1.001)
     # plt.xlim(0.3, 0.43)
     plt.legend()
     plt.title(title)
-    plt.xlim(mid_transit_tbjd % period - 0.1 * period, mid_transit_tbjd % period + 0.1 * period)
+    # plt.xlim(mid_transit_tbjd % period - 0.1 * period, mid_transit_tbjd % period + 0.1 * period)
     # plt.ylim(0.9, 1.1)
     # plt.hlines(y=0.92, xmin=0, xmax=1, ls='dotted', colors='k')
     # plt.hlines(y=0.93, xmin=0, xmax=1, ls='dotted', colors='k')
     plt.vlines(x=(mid_transit_tbjd % period), ymin=0, ymax=2, ls='dotted', colors='grey')
     plt.xlabel('Phase')
     plt.ylabel('Normalized flux')
     plt.savefig(f'{local_directory}/plots/{title}.png', dpi=300)
@@ -351,15 +351,15 @@
                               x_gaia - source.gaia[f'sector_{sector}_x'][nearby_stars[l]],
                               y_gaia - source.gaia[f'sector_{sector}_y'][nearby_stars[l]],
                               width=0.02, color='r', edgecolor=None, head_width=0.1)
                     try:
                         ax0.text(source.gaia[f'sector_{sector}_x'][nearby_stars[l]] - 0.1,
                                  source.gaia[f'sector_{sector}_y'][nearby_stars[l]] + 0.3,
                                  f'TIC {int(source.tic["TIC"][index])}', rotation=90)
-                    except TypeError:
+                    except kindError:
                         ax0.text(source.gaia[f'sector_{sector}_x'][nearby_stars[l]] - 0.1,
                                  source.gaia[f'sector_{sector}_y'][nearby_stars[l]] + 0.2,
                                  f'{source.gaia[f"DESIGNATION"][nearby_stars[l]]}', rotation=90)
                 ax0.scatter(star_x, star_y, s=300, c='r', marker='*', label='target star')
 
                 # ax0.legend()
                 ax0.set_xlim(round(star_x) - 5.5, round(star_x) + 5.5)
@@ -447,36 +447,25 @@
         for i in range(len(tics)):
             target = f'TIC {tics[i]}'
             local_directory = f'{directory}{target}/'
             os.makedirs(local_directory, exist_ok=True)
             tglc_lc(target=target, local_directory=local_directory, size=90, save_aper=True, limit_mag=16,
                     get_all_lc=False, first_sector_only=False, last_sector_only=False, sector=None, prior=prior,
                     transient=None)
-            plot_lc(local_directory=f'{directory}TIC {tics[i]}/', type='cal_aper_flux')
+            plot_lc(local_directory=f'{directory}TIC {tics[i]}/', kind='cal_aper_flux')
     if method == 'search':
         star_spliter(server=server, tics=tics, local_directory=directory)
 
 
 if __name__ == '__main__':
     tics = [16005254]
-    directory = f'/home/tehan/Documents/tglc/'
-    # directory = f'/home/tehan/data/cosmos/GEMS/'
+    directory = f'/home/tehan/data/'
     os.makedirs(directory, exist_ok=True)
-    # get_tglc_lc(tics=tics, method='query', server=1, directory=directory)
-    plot_lc(local_directory=f'/home/tehan/Documents/tglc/TIC 16005254/', type='cal_aper_flux', ylow=0.9, yhigh=1.1)
-    plot_contamination(local_directory=f'{directory}TIC {tics[0]}/', gaia_dr3=5751990597042725632)
+    get_tglc_lc(tics=tics, method='query', server=1, directory=directory)
+    # plot_lc(local_directory=f'{directory}TIC {tics[0]}/', kind='cal_aper_flux')
+    # plot_lc(local_directory=f'/home/tehan/Documents/tglc/TIC 16005254/', kind='cal_aper_flux', ylow=0.9, yhigh=1.1)
+    # plot_contamination(local_directory=f'{directory}TIC {tics[0]}/', gaia_dr3=5751990597042725632)
     # plot_epsf(local_directory=f'{directory}TIC {tics[0]}/')
     # plot_pf_lc(local_directory=f'{directory}TIC {tics[0]}/lc/', period=0.71912603, mid_transit_tbjd=2790.58344,
-    #            type='cal_psf_flux')
-    # plot_pf_lc(local_directory=f'{directory}TIC {tics[0]}/lc/', period=0.71912603, mid_transit_tbjd=2790.58344,
-    #            type='cal_aper_flux')
-
-    # target = f'266.489125, -33.8428'
-    # directory = f'/home/tehan/data/cosmos/michelle/'
-    # local_directory = f'{directory}{target}/'
-    # os.makedirs(local_directory, exist_ok=True)
-    # tglc_lc(target=target, local_directory=local_directory, size=50, save_aper=True, limit_mag=17,
-    #         get_all_lc=False, first_sector_only=False, last_sector_only=False, sector=39, prior=None,
-    #         transient=['266.489125, -33.8428', 266.489125, -33.8428])
-    # plot_lc(local_directory=f'{local_directory}', type='cal_aper_flux')
-    # plot_lc(local_directory=f'{local_directory}', yhigh=150, type='aperture_flux')
-    # plot_contamination(local_directory=f'{local_directory}', gaia_dr3=4041831235071242624)
+    #            kind='cal_psf_flux')
+    # plot_pf_lc(local_directory=f'{directory}TIC {tics[0]}/lc/', period=0.23818244, mid_transit_tbjd=1738.71248,
+    #            kind='cal_aper_flux')
```

### Comparing `tglc-0.6.3/tglc/run.py` & `tglc-0.6.4/tglc/run.py`

 * *Files identical despite different names*

### Comparing `tglc-0.6.3/tglc/source_output.py` & `tglc-0.6.4/tglc/source_output.py`

 * *Files identical despite different names*

### Comparing `tglc-0.6.3/tglc/target_lightcurve.py` & `tglc-0.6.4/tglc/target_lightcurve.py`

 * *Files identical despite different names*

### Comparing `tglc-0.6.3/tglc.egg-info/PKG-INFO` & `tglc-0.6.4/tglc.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,69 @@
 Metadata-Version: 2.1
 Name: tglc
-Version: 0.6.3
+Version: 0.6.4
 Summary: TESS-Gaia Light Curve
 Home-page: https://github.com/TeHanHunter/TESS_Gaia_Light_Curve
 Author: Te Han
 Author-email: tehanhunter@gmail.com
-License: UNKNOWN
-Description: ==================================
-        Introduction
-        ==================================
-        
-        TESS-Gaia Light Curve (`TGLC <https://archive.stsci.edu/hlsp/tglc>`_) is a dataset of TESS full-frame image light curves publicly available via the MAST portal. It is fitted with effective PSF and decontaminated with Gaia DR3 and achieved percent-level photometric precision down to 16th TESS magnitude! It unlocks astrophysics to a vast number of dim stars below 12th TESS magnitude. A package called tglc is pip-installable for customized light curve fits.
-        
-        ==================================
-        Usage
-        ==================================
-        There are four fluxes in each FITS file: aperture flux, PSF flux, calibrated aperture flux, and calibrated PSF flux.
-        If you are uncertain which to use:
-        
-        * Calibrated psf flux is better in **deblending** targets. Use this if you need to deblend a target near a variable source. The best deblending can be achieved with tglc package by setting a non-zero prior. It also gives the more accurate **transit depth** in most cases, especially when fitting with an optimized prior.
-        * Calibrated aperture flux usually has slightly **higher SNR**. The transit depth (or variation amplitude), however, can be imperfect since the normalization depends on the PSF fitting which is imperfect. This imperfection can be minimized by using a bigger aperture than the default aperture (3*3). One need to use the tglc package and set tglc_lc(save_aper=True) to access the 5*5 aperture. In the presence of a bright but "constant" contamination (several magnitudes brighter), the calibrated aperture flux is better in removing the constant contamination. 
-        * The aperture flux and PSF flux are not detrended or normalized. Use this if you are doing stellar variability science with long baseline. Or, if the detrending is not optimal (default detrending has a window length of 1 day; see Known Problems below), start with the aperture flux or PSF flux and detrend carefully!
-        * **If you are uncertain, start with calibrated aperture flux!**
-        
-        The `tutorial <tutorial/TGLC_tutorial.ipynb>`_ shows the syntaxes and differences among these light curves in several examples.
-        
-        ==================================
-        Data Access
-        ==================================
-        There are three data access methods:
-        
-        * MAST Portal: Easiest for acquiring light curves for a few stars. However, new sectors are updated relatively slowly. 
-        * MAST bulk download: Best for downloading light curves for all stars (<16 TESS magnitude) in a sectors. 
-        * tglc package: Capable of producing similar quality light curves for any sector and any star with custom options. 
-        
-        MAST Portal/bulk download
-        ----------------------------
-        The easiest usage requires no package installation. Simply follow the `TGLC HLSP page <https://archive.stsci.edu/hlsp/tglc>`_ to download light curves from MAST or use `MAST Portal <https://mast.stsci.edu/portal/Mashup/Clients/Mast/Portal.html>`_. Light curves are being fitted sector by sector and will be available on MAST gradually. MAST hosts all Gaia DR3 stars down to 16th magnitude. Each .fits file includes PSF and aperture light curves and their calibrated versions.
-        
-        MAST available sectors: `sector worklist <https://docs.google.com/spreadsheets/d/1FhHElWb1wmx9asWiZecAJ2umN0-P_aXn55OBVB34_rg/edit?usp=sharing>`_
-        
-        
-        tglc package
-        ----------------------------
-        Users can also fit light curves using the package tglc. Using tglc, one can specify a region, sector(s), and customized aperture shape if needed. It can also allow all field stars to float by assigning Gaussian priors, which can help decontaminate variable field stars. tglc is currently only available for linux. Run::
-        
-          pip install tglc
-          
-        for the latest tglc release. After installation, follow the `tutorial <tutorial/TGLC_tutorial.ipynb>`_ to fit light curves. If there is a problem, please leave a comment in the Issues section to help us improve. Thank you!
-        
-        
-        ==================================
-        Known Problems
-        ==================================
-        There are several imperfections we noticed in the MAST TGLC light curves and tglc package:
-        
-        * If the star is very dim (~< 15 Tmag) near a variable source, it can make the aperture and/or PSF light curve negative for some cadences. The detrending algorithm could malfunction and result in bad cal_aper_flux and/or cal_psf_flux. This is now fixed for tglc package, but this problem remains for the primary mission light curves published on MAST. Please detrend again if necessary. The extended mission light curves on MAST will not be affected. This is a very rare scenario, but could be important.
-        
-        ==================================
-        Reference
-        ==================================
-        If you find the TGLC light curves or the tglc package useful in your research, please cite `our paper <https://iopscience.iop.org/article/10.3847/1538-3881/acaaa7>`_ published on the Astronomical Journal. 
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+==================================
+Introduction
+==================================
+
+TESS-Gaia Light Curve (`TGLC <https://archive.stsci.edu/hlsp/tglc>`_) is a dataset of TESS full-frame image light curves publicly available via the MAST portal. It is fitted with effective PSF and decontaminated with Gaia DR3 and achieved percent-level photometric precision down to 16th TESS magnitude! It unlocks astrophysics to a vast number of dim stars below 12th TESS magnitude. A package called tglc is pip-installable for customized light curve fits.
+
+==================================
+Usage
+==================================
+There are four fluxes in each FITS file: aperture flux, PSF flux, calibrated aperture flux, and calibrated PSF flux.
+If you are uncertain which to use:
+
+* Calibrated psf flux is better in **deblending** targets. Use this if you need to deblend a target near a variable source. The best deblending can be achieved with tglc package by setting a non-zero prior. It also gives the more accurate **transit depth** in most cases, especially when fitting with an optimized prior.
+* Calibrated aperture flux usually has slightly **higher SNR**. The transit depth (or variation amplitude), however, can be imperfect since the normalization depends on the PSF fitting which is imperfect. This imperfection can be minimized by using a bigger aperture than the default aperture (3*3). One need to use the tglc package and set tglc_lc(save_aper=True) to access the 5*5 aperture. In the presence of a bright but "constant" contamination (several magnitudes brighter), the calibrated aperture flux is better in removing the constant contamination. 
+* The aperture flux and PSF flux are not detrended or normalized. Use this if you are doing stellar variability science with long baseline. Or, if the detrending is not optimal (default detrending has a window length of 1 day; see Known Problems below), start with the aperture flux or PSF flux and detrend carefully!
+* **If you are uncertain, start with calibrated aperture flux!**
+
+The `tutorial <tutorial/TGLC_tutorial.ipynb>`_ shows the syntaxes and differences among these light curves in several examples.
+
+==================================
+Data Access
+==================================
+There are three data access methods:
+
+* MAST Portal: Easiest for acquiring light curves for a few stars. However, new sectors are updated relatively slowly. 
+* MAST bulk download: Best for downloading light curves for all stars (<16 TESS magnitude) in a sectors. 
+* tglc package: Capable of producing similar quality light curves for any sector and any star with custom options. 
+
+MAST Portal/bulk download
+----------------------------
+The easiest usage requires no package installation. Simply follow the `TGLC HLSP page <https://archive.stsci.edu/hlsp/tglc>`_ to download light curves from MAST or use `MAST Portal <https://mast.stsci.edu/portal/Mashup/Clients/Mast/Portal.html>`_. Light curves are being fitted sector by sector and will be available on MAST gradually. MAST hosts all Gaia DR3 stars down to 16th magnitude. Each .fits file includes PSF and aperture light curves and their calibrated versions.
+
+MAST available sectors: `sector worklist <https://docs.google.com/spreadsheets/d/1FhHElWb1wmx9asWiZecAJ2umN0-P_aXn55OBVB34_rg/edit?usp=sharing>`_
+
+
+tglc package
+----------------------------
+Users can also fit light curves using the package tglc. Using tglc, one can specify a region, sector(s), and customized aperture shape if needed. It can also allow all field stars to float by assigning Gaussian priors, which can help decontaminate variable field stars. tglc is currently only available for linux. Run::
+
+  pip install tglc
+  
+for the latest tglc release. After installation, follow the `tutorial <tutorial/TGLC_tutorial.ipynb>`_ to fit light curves. If there is a problem, please leave a comment in the Issues section to help us improve. Thank you!
+
+
+==================================
+Known Problems
+==================================
+There are several imperfections we noticed in the MAST TGLC light curves and tglc package:
+
+* If the star is very dim (~< 15 Tmag) near a variable source, it can make the aperture and/or PSF light curve negative for some cadences. The detrending algorithm could malfunction and result in bad cal_aper_flux and/or cal_psf_flux. This is now fixed for tglc package, but this problem remains for the primary mission light curves published on MAST. Please detrend again if necessary. The extended mission light curves on MAST will not be affected. This is a very rare scenario, but could be important.
+
+==================================
+Reference
+==================================
+If you find the TGLC light curves or the tglc package useful in your research, please cite `our paper <https://iopscience.iop.org/article/10.3847/1538-3881/acaaa7>`_ published on the Astronomical Journal.
```

