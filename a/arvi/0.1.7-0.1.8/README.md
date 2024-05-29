# Comparing `tmp/arvi-0.1.7.tar.gz` & `tmp/arvi-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arvi-0.1.7.tar", last modified: Mon Feb  5 13:16:01 2024, max compression
+gzip compressed data, was "arvi-0.1.8.tar", last modified: Tue Feb  6 16:16:43 2024, max compression
```

## Comparing `arvi-0.1.7.tar` & `arvi-0.1.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 13:16:01.496234 arvi-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 13:16:01.488234 arvi-0.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 13:16:01.492234 arvi-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-02-05 13:15:44.000000 arvi-0.1.7/.github/workflows/docs-gh-pages.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-02-05 13:15:44.000000 arvi-0.1.7/.github/workflows/install.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-02-05 13:15:44.000000 arvi-0.1.7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-02-05 13:15:44.000000 arvi-0.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-02-05 13:15:44.000000 arvi-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-02-05 13:16:01.496234 arvi-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-02-05 13:15:44.000000 arvi-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 13:16:01.492234 arvi-0.1.7/arvi/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-02-05 13:15:44.000000 arvi-0.1.7/arvi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-02-05 13:15:44.000000 arvi-0.1.7/arvi/binning.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-05 13:15:44.000000 arvi-0.1.7/arvi/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9390 2024-02-05 13:15:44.000000 arvi-0.1.7/arvi/dace_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 13:16:01.496234 arvi-0.1.7/arvi/data/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-02-05 13:15:44.000000 arvi-0.1.7/arvi/data/info.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-02-05 13:15:44.000000 arvi-0.1.7/arvi/data/obs_affected_ADC_issues.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-02-05 13:15:44.000000 arvi-0.1.7/arvi/data/obs_affected_blue_cryostat_issues.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-02-05 13:15:44.000000 arvi-0.1.7/arvi/instrument_specific.py
--rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-02-05 13:15:44.000000 arvi-0.1.7/arvi/lbl_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-02-05 13:15:44.000000 arvi-0.1.7/arvi/nasaexo_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    11167 2024-02-05 13:15:44.000000 arvi-0.1.7/arvi/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-02-05 13:15:44.000000 arvi-0.1.7/arvi/programs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-02-05 13:15:44.000000 arvi-0.1.7/arvi/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-05 13:15:44.000000 arvi-0.1.7/arvi/setup_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-02-05 13:15:44.000000 arvi-0.1.7/arvi/simbad_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-02-05 13:15:44.000000 arvi-0.1.7/arvi/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    40962 2024-02-05 13:15:44.000000 arvi-0.1.7/arvi/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-05 13:15:44.000000 arvi-0.1.7/arvi/translations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-02-05 13:15:44.000000 arvi-0.1.7/arvi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 13:16:01.496234 arvi-0.1.7/arvi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-02-05 13:16:01.000000 arvi-0.1.7/arvi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-02-05 13:16:01.000000 arvi-0.1.7/arvi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 13:16:01.000000 arvi-0.1.7/arvi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-05 13:16:01.000000 arvi-0.1.7/arvi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-05 13:16:01.000000 arvi-0.1.7/arvi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 13:16:01.496234 arvi-0.1.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-02-05 13:15:44.000000 arvi-0.1.7/docs/API.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 13:15:44.000000 arvi-0.1.7/docs/detailed.md
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-02-05 13:15:44.000000 arvi-0.1.7/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 13:16:01.496234 arvi-0.1.7/docs/logo/
--rw-r--r--   0 runner    (1001) docker     (127)    13121 2024-02-05 13:15:44.000000 arvi-0.1.7/docs/logo/detective.png
--rw-r--r--   0 runner    (1001) docker     (127)    53569 2024-02-05 13:15:44.000000 arvi-0.1.7/docs/logo/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-02-05 13:15:44.000000 arvi-0.1.7/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-02-05 13:15:44.000000 arvi-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 13:16:01.496234 arvi-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-05 13:15:44.000000 arvi-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 13:16:01.496234 arvi-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-02-05 13:15:44.000000 arvi-0.1.7/tests/test_import_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:16:43.789605 arvi-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:16:43.781605 arvi-0.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:16:43.785605 arvi-0.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-02-06 16:16:30.000000 arvi-0.1.8/.github/workflows/docs-gh-pages.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-02-06 16:16:30.000000 arvi-0.1.8/.github/workflows/install.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-02-06 16:16:30.000000 arvi-0.1.8/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-02-06 16:16:30.000000 arvi-0.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-02-06 16:16:30.000000 arvi-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-02-06 16:16:43.789605 arvi-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-02-06 16:16:30.000000 arvi-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:16:43.785605 arvi-0.1.8/arvi/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-02-06 16:16:30.000000 arvi-0.1.8/arvi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-02-06 16:16:30.000000 arvi-0.1.8/arvi/binning.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-06 16:16:30.000000 arvi-0.1.8/arvi/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9390 2024-02-06 16:16:30.000000 arvi-0.1.8/arvi/dace_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:16:43.789605 arvi-0.1.8/arvi/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-02-06 16:16:30.000000 arvi-0.1.8/arvi/data/info.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-02-06 16:16:30.000000 arvi-0.1.8/arvi/data/obs_affected_ADC_issues.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-02-06 16:16:30.000000 arvi-0.1.8/arvi/data/obs_affected_blue_cryostat_issues.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-02-06 16:16:30.000000 arvi-0.1.8/arvi/instrument_specific.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-02-06 16:16:30.000000 arvi-0.1.8/arvi/lbl_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-02-06 16:16:30.000000 arvi-0.1.8/arvi/nasaexo_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11405 2024-02-06 16:16:30.000000 arvi-0.1.8/arvi/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-02-06 16:16:30.000000 arvi-0.1.8/arvi/programs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-02-06 16:16:30.000000 arvi-0.1.8/arvi/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-06 16:16:30.000000 arvi-0.1.8/arvi/setup_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-02-06 16:16:30.000000 arvi-0.1.8/arvi/simbad_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-02-06 16:16:30.000000 arvi-0.1.8/arvi/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41213 2024-02-06 16:16:30.000000 arvi-0.1.8/arvi/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-06 16:16:30.000000 arvi-0.1.8/arvi/translations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-02-06 16:16:30.000000 arvi-0.1.8/arvi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:16:43.789605 arvi-0.1.8/arvi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-02-06 16:16:43.000000 arvi-0.1.8/arvi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-02-06 16:16:43.000000 arvi-0.1.8/arvi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 16:16:43.000000 arvi-0.1.8/arvi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-06 16:16:43.000000 arvi-0.1.8/arvi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-06 16:16:43.000000 arvi-0.1.8/arvi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:16:43.789605 arvi-0.1.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-02-06 16:16:30.000000 arvi-0.1.8/docs/API.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 16:16:30.000000 arvi-0.1.8/docs/detailed.md
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-02-06 16:16:30.000000 arvi-0.1.8/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:16:43.789605 arvi-0.1.8/docs/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)    13121 2024-02-06 16:16:30.000000 arvi-0.1.8/docs/logo/detective.png
+-rw-r--r--   0 runner    (1001) docker     (127)    53569 2024-02-06 16:16:30.000000 arvi-0.1.8/docs/logo/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-02-06 16:16:30.000000 arvi-0.1.8/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-02-06 16:16:30.000000 arvi-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 16:16:43.789605 arvi-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-06 16:16:30.000000 arvi-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:16:43.789605 arvi-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-02-06 16:16:30.000000 arvi-0.1.8/tests/test_import_object.py
```

### Comparing `arvi-0.1.7/.github/workflows/docs-gh-pages.yml` & `arvi-0.1.8/.github/workflows/docs-gh-pages.yml`

 * *Files identical despite different names*

### Comparing `arvi-0.1.7/.github/workflows/install.yml` & `arvi-0.1.8/.github/workflows/install.yml`

 * *Files identical despite different names*

### Comparing `arvi-0.1.7/.github/workflows/python-publish.yml` & `arvi-0.1.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `arvi-0.1.7/.gitignore` & `arvi-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `arvi-0.1.7/LICENSE` & `arvi-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `arvi-0.1.7/PKG-INFO` & `arvi-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arvi
-Version: 0.1.7
+Version: 0.1.8
 Summary: The Automated RV Inspector
 Author-email: João Faria <joao.faria@unige.ch>
 License: MIT
 Project-URL: Repository, https://github.com/j-faria/arvi
 Keywords: RV,exoplanets
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `arvi-0.1.7/README.md` & `arvi-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `arvi-0.1.7/arvi/binning.py` & `arvi-0.1.8/arvi/binning.py`

 * *Files identical despite different names*

### Comparing `arvi-0.1.7/arvi/dace_wrapper.py` & `arvi-0.1.8/arvi/dace_wrapper.py`

 * *Files identical despite different names*

### Comparing `arvi-0.1.7/arvi/data/obs_affected_ADC_issues.dat` & `arvi-0.1.8/arvi/data/obs_affected_ADC_issues.dat`

 * *Files identical despite different names*

### Comparing `arvi-0.1.7/arvi/data/obs_affected_blue_cryostat_issues.dat` & `arvi-0.1.8/arvi/data/obs_affected_blue_cryostat_issues.dat`

 * *Files identical despite different names*

### Comparing `arvi-0.1.7/arvi/instrument_specific.py` & `arvi-0.1.8/arvi/instrument_specific.py`

 * *Files identical despite different names*

### Comparing `arvi-0.1.7/arvi/lbl_wrapper.py` & `arvi-0.1.8/arvi/lbl_wrapper.py`

 * *Files identical despite different names*

### Comparing `arvi-0.1.7/arvi/plots.py` & `arvi-0.1.8/arvi/plots.py`

 * *Files 12% similar despite different names*

```diff
@@ -277,15 +277,19 @@
                 logger.info(f'calculating periodogram for instrument {instrument}')
     else:
         t = self.time[self.mask]
         y = self.vrad[self.mask]
         e = self.svrad[self.mask]
 
     self._gls = gls = LombScargle(t, y, e)
-    freq, power = gls.autopower(maximum_frequency=1.0, samples_per_peak=10)
+    maximum_frequency = kwargs.pop('maximum_frequency', 1.0)
+    minimum_frequency = kwargs.pop('minimum_frequency', None)
+    freq, power = gls.autopower(maximum_frequency=maximum_frequency,
+                                minimum_frequency=minimum_frequency,
+                                samples_per_peak=10)
     ax.semilogx(1/freq, power, picker=picker, label=label, **kwargs)
 
     if fap:
         ax.axhline(gls.false_alarm_level(0.01),
                    color='k', alpha=0.2, zorder=-1)
 
     ax.set(xlabel='Period [days]', ylabel='Normalized power', ylim=(0, None))
```

### Comparing `arvi-0.1.7/arvi/programs.py` & `arvi-0.1.8/arvi/programs.py`

 * *Files identical despite different names*

### Comparing `arvi-0.1.7/arvi/reports.py` & `arvi-0.1.8/arvi/reports.py`

 * *Files identical despite different names*

### Comparing `arvi-0.1.7/arvi/simbad_wrapper.py` & `arvi-0.1.8/arvi/simbad_wrapper.py`

 * *Files identical despite different names*

### Comparing `arvi-0.1.7/arvi/stats.py` & `arvi-0.1.8/arvi/stats.py`

 * *Files identical despite different names*

### Comparing `arvi-0.1.7/arvi/timeseries.py` & `arvi-0.1.8/arvi/timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -804,14 +804,18 @@
 
         for inst in snew.instruments:
             s = getattr(snew, inst)
 
             # only one observation?
             if s.N == 1:
                 continue
+        
+            # are all observations masked?
+            if s.mtime.size == 0:
+                continue
 
             tb, vb, svb = binRV(s.mtime, s.mvrad, s.msvrad)
             s.vrad = vb
             s.svrad = svb
 
             bad_quantities = []
 
@@ -831,22 +835,24 @@
 
                 if np.isnan(Q).all():
                     yb = np.full_like(tb, np.nan)
                     setattr(s, q, yb)
 
                 elif q + '_err' in s._quantities:
                     Qerr = getattr(s, q + '_err')
-                    if (Qerr == 0.0).all():
+                    if (Qerr == 0.0).all(): # if all errors are NaN, don't use them
                         _, yb = binRV(s.mtime, Q[s.mask], stat='mean', tstat='mean')
                     else:
-                        _, yb, eb = binRV(s.mtime, Q[s.mask], Qerr[s.mask],
-                                          remove_nans=False)
+                        if (Qerr <= 0.0).any(): # if any error is <= 0, set it to NaN
+                            Qerr[Qerr <= 0.0] = np.nan
+
+                        _, yb, eb = binRV(s.mtime, Q[s.mask], Qerr[s.mask], remove_nans=False)
                         setattr(s, q + '_err', eb)
-                    setattr(s, q, yb)
 
+                    setattr(s, q, yb)
 
                 elif not q.endswith('_err'):
                     with warnings.catch_warnings():
                         warnings.filterwarnings('ignore', category=RuntimeWarning)
                         try:
                             _, yb = binRV(s.mtime, Q[s.mask], 
                                         stat=np.nanmean, tstat=np.nanmean)
```

### Comparing `arvi-0.1.7/arvi/utils.py` & `arvi-0.1.8/arvi/utils.py`

 * *Files identical despite different names*

### Comparing `arvi-0.1.7/arvi.egg-info/PKG-INFO` & `arvi-0.1.8/arvi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arvi
-Version: 0.1.7
+Version: 0.1.8
 Summary: The Automated RV Inspector
 Author-email: João Faria <joao.faria@unige.ch>
 License: MIT
 Project-URL: Repository, https://github.com/j-faria/arvi
 Keywords: RV,exoplanets
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `arvi-0.1.7/arvi.egg-info/SOURCES.txt` & `arvi-0.1.8/arvi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arvi-0.1.7/docs/API.md` & `arvi-0.1.8/docs/API.md`

 * *Files identical despite different names*

### Comparing `arvi-0.1.7/docs/index.md` & `arvi-0.1.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `arvi-0.1.7/docs/logo/detective.png` & `arvi-0.1.8/docs/logo/detective.png`

 * *Files identical despite different names*

### Comparing `arvi-0.1.7/docs/logo/logo.png` & `arvi-0.1.8/docs/logo/logo.png`

 * *Files identical despite different names*

### Comparing `arvi-0.1.7/mkdocs.yml` & `arvi-0.1.8/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `arvi-0.1.7/pyproject.toml` & `arvi-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "arvi"
 authors = [
     {name = "João Faria", email = "joao.faria@unige.ch"},
 ]
 description = "The Automated RV Inspector"
-version = "0.1.7"
+version = "0.1.8"
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.8"
 keywords = ["RV", "exoplanets"]
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
```

