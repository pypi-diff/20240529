# Comparing `tmp/matchmaps-0.6.3.tar.gz` & `tmp/matchmaps-0.6.4.tar.gz`

## Comparing `matchmaps-0.6.3.tar` & `matchmaps-0.6.4.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 matchmaps-0.6.3/.github_changelog_generator
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 matchmaps-0.6.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 matchmaps-0.6.3/setup.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 matchmaps-0.6.3/tox.ini
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 matchmaps-0.6.3/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 matchmaps-0.6.3/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 matchmaps-0.6.3/.github/dependabot.yml
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 matchmaps-0.6.3/.github/workflows/build_docs.yml
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 matchmaps-0.6.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 matchmaps-0.6.3/.github/workflows/cron.yml
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 matchmaps-0.6.3/.github/workflows/test_docs.yml
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 matchmaps-0.6.3/docs/Makefile
--rw-r--r--   0        0        0    10422 2020-02-02 00:00:00.000000 matchmaps-0.6.3/docs/about.md
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 matchmaps-0.6.3/docs/cli.md
--rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 matchmaps-0.6.3/docs/conf.py
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 matchmaps-0.6.3/docs/index.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 matchmaps-0.6.3/docs/make.bat
--rw-r--r--   0        0        0    10904 2020-02-02 00:00:00.000000 matchmaps-0.6.3/docs/quickstart.md
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 matchmaps-0.6.3/docs/visualization.md
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 matchmaps-0.6.3/docs/_static/custom.css
--rw-r--r--   0        0        0   217883 2020-02-02 00:00:00.000000 matchmaps-0.6.3/docs/images/isdifferencemap.png
--rw-r--r--   0        0        0   116988 2020-02-02 00:00:00.000000 matchmaps-0.6.3/docs/images/openmap.png
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 matchmaps-0.6.3/docs/images/rs-favicon_32x32.png
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 matchmaps-0.6.3/src/matchmaps/__init__.py
--rw-r--r--   0        0        0    17174 2020-02-02 00:00:00.000000 matchmaps-0.6.3/src/matchmaps/_compute_mr_diff.py
--rw-r--r--   0        0        0    11587 2020-02-02 00:00:00.000000 matchmaps-0.6.3/src/matchmaps/_compute_ncs_diff.py
--rwxr-xr-x   0        0        0    16618 2020-02-02 00:00:00.000000 matchmaps-0.6.3/src/matchmaps/_compute_realspace_diff.py
--rw-r--r--   0        0        0    32935 2020-02-02 00:00:00.000000 matchmaps-0.6.3/src/matchmaps/_utils.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 matchmaps-0.6.3/src/matchmaps/_version_util.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 matchmaps-0.6.3/tests/test_matchmaps.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 matchmaps-0.6.3/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 matchmaps-0.6.3/LICENSE
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 matchmaps-0.6.3/README.md
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 matchmaps-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 matchmaps-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 matchmaps-0.6.4/.github_changelog_generator
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 matchmaps-0.6.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 matchmaps-0.6.4/setup.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 matchmaps-0.6.4/tox.ini
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 matchmaps-0.6.4/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 matchmaps-0.6.4/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 matchmaps-0.6.4/.github/dependabot.yml
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 matchmaps-0.6.4/.github/workflows/build_docs.yml
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 matchmaps-0.6.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 matchmaps-0.6.4/.github/workflows/cron.yml
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 matchmaps-0.6.4/.github/workflows/test_docs.yml
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 matchmaps-0.6.4/docs/Makefile
+-rw-r--r--   0        0        0    10453 2020-02-02 00:00:00.000000 matchmaps-0.6.4/docs/about.md
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 matchmaps-0.6.4/docs/cli.md
+-rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 matchmaps-0.6.4/docs/conf.py
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 matchmaps-0.6.4/docs/index.md
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 matchmaps-0.6.4/docs/make.bat
+-rw-r--r--   0        0        0     8819 2020-02-02 00:00:00.000000 matchmaps-0.6.4/docs/quickstart.md
+-rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 matchmaps-0.6.4/docs/troubleshooting.md
+-rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 matchmaps-0.6.4/docs/visualization.md
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 matchmaps-0.6.4/docs/_static/custom.css
+-rw-r--r--   0        0        0   217883 2020-02-02 00:00:00.000000 matchmaps-0.6.4/docs/images/isdifferencemap.png
+-rw-r--r--   0        0        0   116988 2020-02-02 00:00:00.000000 matchmaps-0.6.4/docs/images/openmap.png
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 matchmaps-0.6.4/docs/images/rs-favicon_32x32.png
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 matchmaps-0.6.4/src/matchmaps/__init__.py
+-rw-r--r--   0        0        0    17174 2020-02-02 00:00:00.000000 matchmaps-0.6.4/src/matchmaps/_compute_mr_diff.py
+-rw-r--r--   0        0        0    11587 2020-02-02 00:00:00.000000 matchmaps-0.6.4/src/matchmaps/_compute_ncs_diff.py
+-rwxr-xr-x   0        0        0    16618 2020-02-02 00:00:00.000000 matchmaps-0.6.4/src/matchmaps/_compute_realspace_diff.py
+-rw-r--r--   0        0        0    32935 2020-02-02 00:00:00.000000 matchmaps-0.6.4/src/matchmaps/_utils.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 matchmaps-0.6.4/src/matchmaps/_version_util.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 matchmaps-0.6.4/tests/test_matchmaps.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 matchmaps-0.6.4/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 matchmaps-0.6.4/LICENSE
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 matchmaps-0.6.4/README.md
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 matchmaps-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 matchmaps-0.6.4/PKG-INFO
```

### Comparing `matchmaps-0.6.3/.pre-commit-config.yaml` & `matchmaps-0.6.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.3/setup.py` & `matchmaps-0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.3/tox.ini` & `matchmaps-0.6.4/tox.ini`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.3/.github/workflows/build_docs.yml` & `matchmaps-0.6.4/.github/workflows/build_docs.yml`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.3/.github/workflows/ci.yml` & `matchmaps-0.6.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.3/.github/workflows/cron.yml` & `matchmaps-0.6.4/.github/workflows/cron.yml`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.3/.github/workflows/test_docs.yml` & `matchmaps-0.6.4/.github/workflows/test_docs.yml`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.3/docs/Makefile` & `matchmaps-0.6.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.3/docs/about.md` & `matchmaps-0.6.4/docs/about.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # About the `matchmaps` algorithm
 
-If you want to learn more about the idea behind `matchmaps`, along with some examples, please check out our new pre-print!  
+If you want to learn more about the idea behind `matchmaps`, along with some examples, please check out paper in the Journal of Applied Crystallography!  
 
-> [MatchMaps: Non-isomorphous difference maps for X-ray crystallography](https://www.biorxiv.org/content/10.1101/2023.09.01.555333v2) 
+> [MatchMaps: non-isomorphous difference maps for X-ray crystallography](https://journals.iucr.org/j/issues/2024/03/00/ei5112/index.html) 
 
-If what you're looking for is a user's guide, you can find that [here](quickstart.md). But if you're looking for more details about how `matchmaps` works, read on!
+If you're looking for a user guide, you can find that [here](quickstart.md). But if you're looking for more details about how `matchmaps` works, read on!
 
 ## Abstract
-Conformational change mediates the biological functions of macromolecules. Crystal-lographic measurements can map these changes with extraordinary sensitivity as a function of mutations, ligands, and time. The isomorphous difference map remains the gold standard for detecting structural differences between datasets. Isomorphous difference maps combine the phases of a chosen reference state with the observed changes in structure factor amplitudes to yield a map of changes in electron density. Such maps are much more sensitive to conformational change than structure refinement is, and are unbiased in the sense that observed differences do not depend on refinement of the perturbed state. However, even minute changes in unit cell properties can render isomorphous difference maps useless. This is unnecessary. Here we describe a generalized procedure for calculating observed difference maps that retains the high sensitivity to conformational change and avoids structure refinement of the perturbed state. We have implemented this procedure in an open-source python package, MatchMaps, that can be run in any software environment supporting PHENIX and CCP4. Through examples, we show that MatchMaps “rescues” observed difference electron density maps for poorly-isomorphous crystals, corrects artifacts in nominally isomorphous difference maps, and extends to detecting differences across copies within the asymmetric unit, or across altogether different crystal forms.
+
+Conformational change mediates the biological functions of macromolecules. Crystallographic measurements can map these changes with extraordinary sensitivity as a function of mutations, ligands, and time. A popular method for detecting structural differences between crystallographic datasets is the isomorphous difference map. Isomorphous difference maps combine the phases of a chosen reference state with the observed changes in structure factor amplitudes to yield a map of changes in electron density. Such maps are much more sensitive to conformational change than structure refinement is, and are unbiased in the sense that observed differences do not depend on refinement of the perturbed state. However, even modest changes in unit cell properties can render isomorphous difference maps useless. This is unnecessary. Here we describe a generalized procedure for calculating observed difference maps that retains the high sensitivity to conformational change and avoids structure refinement of the perturbed state. We have implemented this procedure in an open-source python package, MatchMaps, that can be run in any software environment supporting PHENIX and CCP4. Through examples, we show that MatchMaps "rescues" observed difference electron density maps for poorly-isomorphous crystals, corrects artifacts in nominally isomorphous difference maps, and extends to detecting differences across copies within the asymmetric unit, or across altogether different crystal forms.
 
 ## Algorithm overview
 
   1. Place both sets of structure factor amplitudes on a common scale using CCP4’s `SCALEIT` utility and truncate the data to the same resolution range.
   2. Generate phases for each dataset via the `phenix.refine` program. For both datasets, the OFF starting model is used, and only rigid-body refinement is permitted to prevent the introduction of model bias.
   3. Fourier-transform each set of complex structure factors into a real-space electron density map using the python packages `reciprocalspaceship` and `gemmi`.
   4. Compute the translation and rotation necessary to overlay the two rigid-body refined models. Apply this translation-rotation to the ON real-space map such that it overlays with the OFF map. These computations are carried out using `gemmi`.
```

### Comparing `matchmaps-0.6.3/docs/conf.py` & `matchmaps-0.6.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.3/docs/index.md` & `matchmaps-0.6.4/docs/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,12 +20,14 @@
 
 ```{eval-rst}
 .. toctree::
    :maxdepth: 1
    :hidden:
 
    Quickstart guide <quickstart>
-   Command-line options <cli>
+   Troubleshooting and advanced usage <troubleshooting>
    Visualizing results <visualization>
    About the algorithm <about>
+   Full command-line API <cli>
+
 
 ```
```

### Comparing `matchmaps-0.6.3/docs/make.bat` & `matchmaps-0.6.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.3/docs/quickstart.md` & `matchmaps-0.6.4/docs/quickstart.md`

 * *Files 12% similar despite different names*

```diff
@@ -26,23 +26,23 @@
 Though `matchmaps` is a python package, it relies on two pieces of external software that are not (yet!) `pip`-installable. If they do become `pip`-installable in the future, I will excitedly update this package and save you the trouble. For the time being, you will need to install:
 
  - [ccp4](https://www.ccp4.ac.uk/download/#os=mac)
  - [phenix](https://phenix-online.org/documentation/install-setup-run.html)
 
 ```{eval-rst}
 .. note::
-    Please note that phenix 1.21 is **not** supported at this time. I hope to update `matchmaps` to support this in the near future. In the meantime, make sure you're using phenix 1.20 or earlier, and everything should work fine. 
+    Please note that phenix 1.21 is **not** supported at this time. I hope to update `matchmaps` to support this in the near future. In the meantime, make sure you're using phenix 1.20 or earlier, and everything should work fine. As of `matchmaps 0.6.3`, an error should be thrown if you're using phenix 1.21 reminding you to downgrade.
 ```
 When actually using `matchmaps` in the command-line, you'll need to have both ccp4 and phenix active. Doing that will look something like:
 ```bash
 source /path/to/phenix/phenix_env.sh
 /path/to/ccp4/start
 ```
 
-At this point, you should be good to go! Please [file an issue on github](https://github.com/dennisbrookner/matchmaps/issues) is this is not working.
+At this point, you should be good to go! Please [file an issue on github](https://github.com/rs-station/matchmaps/issues) is this is not working.
 
 ## Input files
 
 To run `matchmaps`, you will need:
  - one `.pdb` (or `.cif`) file containing a refined structural model corresponding to your "off" data.
  - two `.mtz` (or `.cif`) files corresponding to your "on" and "off" data respectively.
 
@@ -112,32 +112,20 @@
 ```
 
 ### Running `matchmaps` from a script
 After your `matchmaps` run completes successfully, it will write out a file (called `run_matchmaps.sh` unless you specify a different name to the `--script` flag) which can be run to reproduce exactly the same command. Note that, to ensure the compatibility of input/output paths, this script is written to your ***current working directory***.
 
 If you'd then like to run `matchmaps` again with slightly different parameters, you can use this script as a starting point. No need to remember exactly which parameters you used the first time!
 
-## Other useful options
-
- - `--on-as-stationary`: The `matchmaps` algorithm always involves an alignment in real-space of the "on" and "off" maps. By default, the "off" map is stationary, and the "on" map is moved. This is typically desired, such that everything lines up with your "off" structural model. However, say that your structures are "apo" and "bound", and you would like to line up your maps with a "bound" structure (which you never have to supply to `matchmaps`!). In this case, you could use the `--on-as-stationary` flag.
- - `--dmin`: The input `mtz` files are truncated to equal resolution by default. If you would like, the `mtz`s may be truncated even more stringently.
- - `--unmasked-radius`: How far away from the protein model do you expect to see difference signal? Use this flag to change the behavior of the `_unmasked` difference map output to show more or less signal far from the protein. Defaults to 5 A. See [below](#important-map-outputs) for more details.
- - `--no-bss`: If included, skip the bulk solvent scaling step of phenix.refine. Like `--unmasked-radius`, this option may be useful in situtations where you expect signal far away from your protein model. For example, bulk solvent scaling may "flatten" or otherwise alter signal for an unmodeled bound ligand.
- - `--spacing`: This flag defines the approximate size of the voxels in your real-space maps. The default (0.5 A) is fine for most purposes. For making figures in PyMOL, you might want finer spacing (0.25 A or so); this comes at a cost of much larger file size. If your computer/coot is being really slow, you could consider increasing the spacing.
- - `--verbose`: Use this option to print out to the terminal all of the log output from CCP4 and phenix. This is disabled by default because it's very annoying, but it can be useful for debugging purposes.
- - `--rbr-selections`: When doing rigid-body refinement, refine as multiple explicitly defined rigid bodies rather than a single rigid body containing everything. This flag is admittedly a little finnicky; please [file an issue](https://github.com/rs-station/matchmaps/issues)  if you have any trouble.
-
 Note that most of the command-line options have short and long versions, e.g. `-i` vs. `--input-dir`. For clarity, the long names have been used exclusively on this page. The [full documentation](cli.md) lits all short and long options.
 
 ## Output files
 
 Below is a quick tour of the output files that `matchmaps` will produce and what you might want to do with them.
 
-### Important `.map` outputs
-
 Let's assume that your input files are called `off.mtz` and `on.mtz`. The following files created by `matchmaps` may be of interest:
 
  - `on_minus_off.map`: This is your difference map! It should contain positive and negative signal in the vicinity (>= 2 Angstroms) of your protein model.
  - `on_minus_off_unmasked.map`: The same as the previous difference map, but before the 2 A solvent mask was applied. This file can be useful if you're expecting signal (perhaps a bound ligand) far away from your protein model. By default, this map contains signal up to 5 A away from the protein model; this radius can be changed with the `--unmasked-radius` flag for `matchmaps` and `matchmaps.mr` utilites. 
  - `on.map` / `off.map`: The real-space maps which are subtracted to produce the above difference maps. It is a good idea to open these files and inspect them. They should be generally aligned in space. Any interesting signal you expect to see in a difference map may also be apparent by inspecting these maps. Remember that both of these maps were computed using the "off" model, so structural features of the "off" data are likely to be more prominent.
  - `on_before.map` / `off_before.map`: The real-space maps, prior to alignment. These maps may be useful a) if you're curious how much alignment was necessary, or b) to troubleshoot where in the pipeline something went wrong.
```

### Comparing `matchmaps-0.6.3/docs/visualization.md` & `matchmaps-0.6.4/docs/visualization.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 ![Is difference map](images/isdifferencemap.png)
 
 Happy difference mapping! From here, working with a `.map` file should be no different than typical work in Coot with an `.mtz` file.
 
 ### Periodic boundary conditions in Coot
 
-`matchmaps` always produces outputs in spacegroup P1, and thus will sometimes produces outputs in P1 and with an orthorhombic unit cell. Unfortunately, Coot assumes that P1 orthorhombic `.map` files are cryo-EM maps, and thus does not render periodic boundary conditions! This is an issue, because often we wish to visualize parts of the protein model which lie outside of the unit cell. As a workaround, any P1 orthorhombic maps produced by `matchmaps` will artifically set `alpha=90.006`. This difference is imperceptible, but is enough to convince Coot that the map is crystallographic in origin. In all likelihood, a user of `matchmaps` will not need to deal with this issue directly. However, it is good to keep in mind in case you are ever working with a `matchmaps` output for another purpose downstream, or if a related bug arises. Of course, if your maps in Coot are ever abruptly ending at the edge of the unit cells, please [file an issue on GitHub](https://github.com/rs-station/matchmaps/issues).
+`matchmaps` always produces outputs in spacegroup P1, and thus sometimes produces outputs in P1 and with an orthorhombic unit cell. Unfortunately, Coot assumes that P1 orthorhombic `.map` files are cryo-EM maps, and thus does not render periodic boundary conditions! This is an issue, because often we wish to visualize parts of the protein model which lie outside of the unit cell. As a workaround, any P1 orthorhombic maps produced by `matchmaps` will artifically set `alpha=90.006`. This difference is imperceptible, but is enough to convince Coot that the map is crystallographic in origin. In all likelihood, a user of `matchmaps` will not need to deal with this issue directly. However, it is good to keep in mind in case you are ever working with a `matchmaps` output for another purpose downstream, or if a related bug arises. Of course, if your maps in Coot are ever abruptly ending at the edge of the unit cells, please [file an issue on GitHub](https://github.com/rs-station/matchmaps/issues).
 
 ## Working with `.map` files in PyMOL
 
 PyMOL is, for many crystallographers, the preferred software for producing figures. Unfortunately, PyMOL's default behaviors around `.map` inputs can be counterintuitive and hard to work with. I will attempt here to briefly outline the key issues that you might encounter.
 
 Loading a map into PyMOL is easy:
 ```
```

### Comparing `matchmaps-0.6.3/docs/images/isdifferencemap.png` & `matchmaps-0.6.4/docs/images/isdifferencemap.png`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.3/docs/images/openmap.png` & `matchmaps-0.6.4/docs/images/openmap.png`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.3/docs/images/rs-favicon_32x32.png` & `matchmaps-0.6.4/docs/images/rs-favicon_32x32.png`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.3/src/matchmaps/_compute_mr_diff.py` & `matchmaps-0.6.4/src/matchmaps/_compute_mr_diff.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.3/src/matchmaps/_compute_ncs_diff.py` & `matchmaps-0.6.4/src/matchmaps/_compute_ncs_diff.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.3/src/matchmaps/_compute_realspace_diff.py` & `matchmaps-0.6.4/src/matchmaps/_compute_realspace_diff.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.3/src/matchmaps/_utils.py` & `matchmaps-0.6.4/src/matchmaps/_utils.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.3/.gitignore` & `matchmaps-0.6.4/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -113,8 +113,11 @@
 .cruft.json
 
 # weird thing
 .notconda/*
 
 # logo in illustrator
 docs/images/logo.ai
-docs/images/logo2.ai
+docs/images/logo2.ai
+
+# PyCharm files
+.idea/*
```

### Comparing `matchmaps-0.6.3/LICENSE` & `matchmaps-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.3/pyproject.toml` & `matchmaps-0.6.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,25 +5,24 @@
 
 # https://peps.python.org/pep-0621/
 [project]
 name = "matchmaps"
 # versioning through releases
 description = "Make unbiased difference maps even for non-isomorphous inputs"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = { text = "BSD 3-Clause License" }
 authors = [
     { email = "debrookner@gmail.com", name = "Dennis Brookner" },
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Typing :: Typed",
 ]
 dynamic = ["version"]
```

### Comparing `matchmaps-0.6.3/PKG-INFO` & `matchmaps-0.6.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.3
 Name: matchmaps
-Version: 0.6.3
+Version: 0.6.4
 Summary: Make unbiased difference maps even for non-isomorphous inputs
 Project-URL: homepage, https://rs-station.github.io/matchmaps/
 Project-URL: repository, https://github.com/rs-station/matchmaps
 Author-email: Dennis Brookner <debrookner@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Requires-Dist: gemmi
 Requires-Dist: numpy
 Requires-Dist: reciprocalspaceship>=1.0.1
 Requires-Dist: rs-booster>=0.1.2
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
@@ -40,14 +39,14 @@
 Provides-Extra: test
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest>=6.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 # matchmaps
 
-[![License](https://img.shields.io/pypi/l/matchmaps.svg?color=green)](https://github.com/dennisbrookner/matchmaps/raw/main/LICENSE)
+[![License](https://img.shields.io/pypi/l/matchmaps.svg?color=green)](https://github.com/rs-station/matchmaps/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/matchmaps.svg?color=green)](https://pypi.org/project/matchmaps)
 [![Python Version](https://img.shields.io/pypi/pyversions/matchmaps.svg?color=green)](https://python.org)
-[![CI](https://github.com/dennisbrookner/matchmaps/actions/workflows/ci.yml/badge.svg)](https://github.com/dennisbrookner/matchmaps/actions/workflows/ci.yml)
-[![codecov](https://codecov.io/gh/dennisbrookner/matchmaps/branch/main/graph/badge.svg)](https://codecov.io/gh/dennisbrookner/matchmaps)
+[![CI](https://github.com/rs-station/matchmaps/actions/workflows/ci.yml/badge.svg)](https://github.com/rs-station/matchmaps/actions/workflows/ci.yml)
+[![codecov](https://codecov.io/gh/rs-station/matchmaps/branch/main/graph/badge.svg)](https://codecov.io/gh/rs-station/matchmaps)
 
-Make unbiased difference maps even for non-isomorphous inputs
+Make unbiased difference maps even for non-isomorphous inputs. Check out the [package documentation](https://rs-station.github.io/matchmaps/)
```

