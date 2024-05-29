# Comparing `tmp/cosmosis-3.6.tar.gz` & `tmp/cosmosis-3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmosis-3.6.tar", last modified: Mon May 27 11:19:08 2024, max compression
+gzip compressed data, was "cosmosis-3.7.tar", last modified: Wed May 29 12:48:22 2024, max compression
```

## Comparing `cosmosis-3.6.tar` & `cosmosis-3.7.tar`

### file list

```diff
@@ -1,292 +1,292 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.974270 cosmosis-3.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-27 11:19:03.000000 cosmosis-3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-27 11:19:03.000000 cosmosis-3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-27 11:19:08.974270 cosmosis-3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-27 11:19:03.000000 cosmosis-3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.930270 cosmosis-3.6/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-05-27 11:19:03.000000 cosmosis-3.6/bin/cosmosis
--rwxr-xr-x   0 runner    (1001) docker     (127)      122 2024-05-27 11:19:03.000000 cosmosis-3.6/bin/cosmosis-campaign
--rwxr-xr-x   0 runner    (1001) docker     (127)      792 2024-05-27 11:19:03.000000 cosmosis-3.6/bin/cosmosis-configure
--rwxr-xr-x   0 runner    (1001) docker     (127)     1434 2024-05-27 11:19:03.000000 cosmosis-3.6/bin/cosmosis-extract
--rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-05-27 11:19:03.000000 cosmosis-3.6/bin/cosmosis-postprocess
--rwxr-xr-x   0 runner    (1001) docker     (127)     1527 2024-05-27 11:19:03.000000 cosmosis-3.6/bin/cosmosis-sample-fisher
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.934270 cosmosis-3.6/cosmosis/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26386 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/campaign.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.934270 cosmosis-3.6/cosmosis/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/config/compilers.mk
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/config/subdirs.mk
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.938270 cosmosis-3.6/cosmosis/datablock/
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51706 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/c_datablock.cc
--rw-r--r--   0 runner    (1001) docker     (127)    22811 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/c_datablock.h
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/clamp.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/cosmosis_constants.fh
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/cosmosis_constants.h
--rw-r--r--   0 runner    (1001) docker     (127)    34029 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/cosmosis_modules.F90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.942270 cosmosis-3.6/cosmosis/datablock/cosmosis_py/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/cosmosis_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52767 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/cosmosis_py/block.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/cosmosis_py/dbt_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/cosmosis_py/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/cosmosis_py/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/cosmosis_py/section_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/cosmosis_section_names.F90
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/cosmosis_types.F90
--rw-r--r--   0 runner    (1001) docker     (127)    28871 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/cosmosis_wrappers.F90
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/datablock.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11180 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/datablock.hh
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/datablock_logging.cc
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/datablock_logging.h
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/datablock_status.h
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/datablock_types.h
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/entry.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/entry.hh
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/exceptions.hh
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/generate_sections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/handler.c
--rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/ndarray.hh
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/section.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/section.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/section_names.h
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/section_names.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14009 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/gaussian_likelihood.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22952 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.942270 cosmosis-3.6/cosmosis/output/
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/output/astropy_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/output/cosmomc_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/output/fits_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/output/in_memory_output.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/output/null_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/output/output_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/output/text_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/output/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.942270 cosmosis-3.6/cosmosis/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7748 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/plotting/chain_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/plotting/grid_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/plotting/kde.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      404 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/plotting/plot_demo_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/plotting/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/plotting/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5502 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.946270 cosmosis-3.6/cosmosis/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16175 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/cosmology_theory_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/density.py
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/latex.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/lazy_pylab.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    50319 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/postprocess_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/reruns.py
--rw-r--r--   0 runner    (1001) docker     (127)    33609 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.950270 cosmosis-3.6/cosmosis/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/attribution.py
--rw-r--r--   0 runner    (1001) docker     (127)    14033 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/declare.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.950270 cosmosis-3.6/cosmosis/runtime/julia_modules/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/julia_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/julia_modules/julia.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/memmon.py
--rw-r--r--   0 runner    (1001) docker     (127)    17170 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/mpi_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    12277 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    58652 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    21210 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/prior.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/process_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.950270 cosmosis-3.6/cosmosis/samplers/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.950270 cosmosis-3.6/cosmosis/samplers/abc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/abc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7126 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/abc/abc_sampler.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6698 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/abc/abc_sampler_mpi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.950270 cosmosis-3.6/cosmosis/samplers/apriori/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/apriori/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2766 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/apriori/apriori_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.950270 cosmosis-3.6/cosmosis/samplers/dynesty/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/dynesty/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3707 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/dynesty/dynesty_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.950270 cosmosis-3.6/cosmosis/samplers/emcee/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/emcee/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7516 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/emcee/emcee_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.950270 cosmosis-3.6/cosmosis/samplers/fisher/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/fisher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/fisher/fisher.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6642 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/fisher/fisher_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.950270 cosmosis-3.6/cosmosis/samplers/grid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/grid/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4745 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/grid/grid_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.950270 cosmosis-3.6/cosmosis/samplers/gridmax/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/gridmax/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4370 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/gridmax/gridmax_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/hints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.954270 cosmosis-3.6/cosmosis/samplers/importance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/importance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/importance/importance_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.954270 cosmosis-3.6/cosmosis/samplers/kombine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/kombine/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4932 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/kombine/kombine_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.954270 cosmosis-3.6/cosmosis/samplers/list/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/list/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5094 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/list/list_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.954270 cosmosis-3.6/cosmosis/samplers/maxlike/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/maxlike/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4666 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/maxlike/maxlike_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.954270 cosmosis-3.6/cosmosis/samplers/metropolis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/metropolis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9773 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/metropolis/metropolis.py
--rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/metropolis/metropolis_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.954270 cosmosis-3.6/cosmosis/samplers/metropolis/proposal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/metropolis/proposal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/metropolis/proposal/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.954270 cosmosis-3.6/cosmosis/samplers/minuit/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/minuit/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/minuit/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7323 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/minuit/minuit_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/minuit/minuit_wrapper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.954270 cosmosis-3.6/cosmosis/samplers/multinest/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9039 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/multinest_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.958270 cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    19512 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/README
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/cwrapper.f90
--rw-r--r--   0 runner    (1001) docker     (127)    42915 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90
--rw-r--r--   0 runner    (1001) docker     (127)   107766 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/nested.f90
--rw-r--r--   0 runner    (1001) docker     (127)    22010 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/posterior.f90
--rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/priors.f90
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/utils.f90
--rw-r--r--   0 runner    (1001) docker     (127)    28039 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/utils1.f90
--rw-r--r--   0 runner    (1001) docker     (127)    86938 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.958270 cosmosis-3.6/cosmosis/samplers/nautilus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/nautilus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/nautilus/nautilus_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.958270 cosmosis-3.6/cosmosis/samplers/pmaxlike/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/pmaxlike/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4151 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.958270 cosmosis-3.6/cosmosis/samplers/pmc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/pmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/pmc/pmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/pmc/pmc_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.958270 cosmosis-3.6/cosmosis/samplers/poco/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/poco/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3703 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/poco/poco_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.958270 cosmosis-3.6/cosmosis/samplers/polychord/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12986 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.966270 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     8599 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/README
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/abort.F90
--rw-r--r--   0 runner    (1001) docker     (127)    18110 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/array_utils.f90
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/c_interface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/calculate.f90
--rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90
--rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/clustering.f90
--rw-r--r--   0 runner    (1001) docker     (127)    13421 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/feedback.f90
--rw-r--r--   0 runner    (1001) docker     (127)    26147 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/generate.F90
--rw-r--r--   0 runner    (1001) docker     (127)    19077 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/ini.f90
--rw-r--r--   0 runner    (1001) docker     (127)    20999 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/interfaces.F90
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/interfaces.h
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/interfaces.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    24257 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90
--rw-r--r--   0 runner    (1001) docker     (127)    20674 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/params.f90
--rw-r--r--   0 runner    (1001) docker     (127)    19675 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/priors.f90
--rw-r--r--   0 runner    (1001) docker     (127)    18291 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/random_utils.F90
--rw-r--r--   0 runner    (1001) docker     (127)    44750 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/read_write.f90
--rw-r--r--   0 runner    (1001) docker     (127)    47427 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/run_time_info.f90
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/settings.f90
--rw-r--r--   0 runner    (1001) docker     (127)    29353 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/utils.F90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.966270 cosmosis-3.6/cosmosis/samplers/pymc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/pymc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/pymc/pymc_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.966270 cosmosis-3.6/cosmosis/samplers/snake/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/snake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/snake/snake.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2017 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/snake/snake_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.966270 cosmosis-3.6/cosmosis/samplers/star/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/star/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4468 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/star/star_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.966270 cosmosis-3.6/cosmosis/samplers/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3221 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/test/test_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.966270 cosmosis-3.6/cosmosis/samplers/zeus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/zeus/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11554 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/zeus/zeus_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.970270 cosmosis-3.6/cosmosis/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/bad-campaign.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/campaign.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/example-priors.ini
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/example-values.ini
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/example.ini
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/example_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/example_module2.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/example_module3.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/example_module4.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/included.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.974270 cosmosis-3.6/cosmosis/test/libtest/
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/c_datablock_complex_array_test.c
--rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/c_datablock_double_array_test.c
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/c_datablock_int_array_test.c
--rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c
--rw-r--r--   0 runner    (1001) docker     (127)    11722 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/c_datablock_test.c
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/cosmosis_test.F90
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/cosmosis_tests.supp
--rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/datablock_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/entry_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/ndarray_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/section_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)    28088 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/test_c_datablock_scalars.h
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/test_c_datablock_scalars.template
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/test_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/test_campaign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/test_chaining.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8666 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/test_polychord.py
--rw-r--r--   0 runner    (1001) docker     (127)     6358 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/test_samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/test_text_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.974270 cosmosis-3.6/cosmosis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-27 11:19:08.000000 cosmosis-3.6/cosmosis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9278 2024-05-27 11:19:08.000000 cosmosis-3.6/cosmosis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 11:19:08.000000 cosmosis-3.6/cosmosis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-27 11:19:08.000000 cosmosis-3.6/cosmosis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-27 11:19:08.000000 cosmosis-3.6/cosmosis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-27 11:19:03.000000 cosmosis-3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 11:19:08.974270 cosmosis-3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-27 11:19:03.000000 cosmosis-3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.751531 cosmosis-3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-29 12:48:20.000000 cosmosis-3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-29 12:48:20.000000 cosmosis-3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-29 12:48:22.751531 cosmosis-3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-29 12:48:20.000000 cosmosis-3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.715531 cosmosis-3.7/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-05-29 12:48:20.000000 cosmosis-3.7/bin/cosmosis
+-rwxr-xr-x   0 runner    (1001) docker     (127)      122 2024-05-29 12:48:20.000000 cosmosis-3.7/bin/cosmosis-campaign
+-rwxr-xr-x   0 runner    (1001) docker     (127)      792 2024-05-29 12:48:20.000000 cosmosis-3.7/bin/cosmosis-configure
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1434 2024-05-29 12:48:20.000000 cosmosis-3.7/bin/cosmosis-extract
+-rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-05-29 12:48:20.000000 cosmosis-3.7/bin/cosmosis-postprocess
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1527 2024-05-29 12:48:20.000000 cosmosis-3.7/bin/cosmosis-sample-fisher
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.715531 cosmosis-3.7/cosmosis/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26386 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/campaign.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.715531 cosmosis-3.7/cosmosis/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/config/compilers.mk
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/config/subdirs.mk
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.719531 cosmosis-3.7/cosmosis/datablock/
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51706 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/c_datablock.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    22811 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/c_datablock.h
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/clamp.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/cosmosis_constants.fh
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/cosmosis_constants.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34029 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/cosmosis_modules.F90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.723531 cosmosis-3.7/cosmosis/datablock/cosmosis_py/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/cosmosis_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52767 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/cosmosis_py/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/cosmosis_py/dbt_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/cosmosis_py/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/cosmosis_py/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/cosmosis_py/section_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/cosmosis_section_names.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/cosmosis_types.F90
+-rw-r--r--   0 runner    (1001) docker     (127)    28871 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/cosmosis_wrappers.F90
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/datablock.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11180 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/datablock.hh
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/datablock_logging.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/datablock_logging.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/datablock_status.h
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/datablock_types.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/entry.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/entry.hh
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/exceptions.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/generate_sections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/handler.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/ndarray.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/section.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/section.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/section_names.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/datablock/section_names.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14009 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/gaussian_likelihood.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22955 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.723531 cosmosis-3.7/cosmosis/output/
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/output/astropy_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/output/cosmomc_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/output/fits_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/output/in_memory_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/output/null_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/output/output_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/output/text_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/output/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.723531 cosmosis-3.7/cosmosis/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7748 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/plotting/chain_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/plotting/grid_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/plotting/kde.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      404 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/plotting/plot_demo_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/plotting/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/plotting/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5502 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.727531 cosmosis-3.7/cosmosis/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/postprocessing/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16175 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/postprocessing/cosmology_theory_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/postprocessing/density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/postprocessing/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/postprocessing/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/postprocessing/latex.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/postprocessing/lazy_pylab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/postprocessing/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/postprocessing/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50319 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/postprocessing/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/postprocessing/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/postprocessing/postprocess_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/postprocessing/reruns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33609 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/postprocessing/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/postprocessing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.727531 cosmosis-3.7/cosmosis/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/runtime/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/runtime/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14033 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/runtime/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/runtime/declare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/runtime/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.731531 cosmosis-3.7/cosmosis/runtime/julia_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/runtime/julia_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/runtime/julia_modules/julia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/runtime/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/runtime/memmon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17170 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/runtime/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/runtime/mpi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12277 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/runtime/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58652 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/runtime/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21210 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/runtime/prior.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/runtime/process_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/runtime/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.731531 cosmosis-3.7/cosmosis/samplers/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.731531 cosmosis-3.7/cosmosis/samplers/abc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/abc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7126 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/abc/abc_sampler.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6698 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/abc/abc_sampler_mpi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.731531 cosmosis-3.7/cosmosis/samplers/apriori/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/apriori/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2766 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/apriori/apriori_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.731531 cosmosis-3.7/cosmosis/samplers/dynesty/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/dynesty/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3707 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/dynesty/dynesty_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.731531 cosmosis-3.7/cosmosis/samplers/emcee/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/emcee/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7516 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/emcee/emcee_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.731531 cosmosis-3.7/cosmosis/samplers/fisher/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/fisher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/fisher/fisher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6642 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/fisher/fisher_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.731531 cosmosis-3.7/cosmosis/samplers/grid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/grid/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4745 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/grid/grid_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.731531 cosmosis-3.7/cosmosis/samplers/gridmax/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/gridmax/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4370 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/gridmax/gridmax_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/hints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.731531 cosmosis-3.7/cosmosis/samplers/importance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/importance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/importance/importance_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.731531 cosmosis-3.7/cosmosis/samplers/kombine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/kombine/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4932 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/kombine/kombine_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.731531 cosmosis-3.7/cosmosis/samplers/list/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/list/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5555 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/list/list_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.735531 cosmosis-3.7/cosmosis/samplers/maxlike/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/maxlike/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4666 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/maxlike/maxlike_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.735531 cosmosis-3.7/cosmosis/samplers/metropolis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/metropolis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9773 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/metropolis/metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/metropolis/metropolis_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.735531 cosmosis-3.7/cosmosis/samplers/metropolis/proposal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/metropolis/proposal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/metropolis/proposal/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.735531 cosmosis-3.7/cosmosis/samplers/minuit/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/minuit/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/minuit/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7376 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/minuit/minuit_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/minuit/minuit_wrapper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.735531 cosmosis-3.7/cosmosis/samplers/multinest/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/multinest/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/multinest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9039 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/multinest/multinest_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.739531 cosmosis-3.7/cosmosis/samplers/multinest/multinest_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/multinest/multinest_src/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/multinest/multinest_src/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    19512 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/multinest/multinest_src/README
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/multinest/multinest_src/cwrapper.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    42915 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90
+-rw-r--r--   0 runner    (1001) docker     (127)   107766 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/multinest/multinest_src/nested.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    22010 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/multinest/multinest_src/posterior.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/multinest/multinest_src/priors.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/multinest/multinest_src/utils.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    28039 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/multinest/multinest_src/utils1.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    86938 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.739531 cosmosis-3.7/cosmosis/samplers/nautilus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/nautilus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/nautilus/nautilus_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.739531 cosmosis-3.7/cosmosis/samplers/pmaxlike/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/pmaxlike/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4151 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.739531 cosmosis-3.7/cosmosis/samplers/pmc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/pmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/pmc/pmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/pmc/pmc_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.739531 cosmosis-3.7/cosmosis/samplers/poco/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/poco/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3703 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/poco/poco_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.739531 cosmosis-3.7/cosmosis/samplers/polychord/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12986 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.743531 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     8599 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/README
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/abort.F90
+-rw-r--r--   0 runner    (1001) docker     (127)    18110 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/array_utils.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/c_interface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/calculate.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/clustering.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    13421 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/feedback.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    26147 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/generate.F90
+-rw-r--r--   0 runner    (1001) docker     (127)    19077 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/ini.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    20999 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/interfaces.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/interfaces.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/interfaces.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    24257 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90
+-rw-r--r--   0 runner    (1001) docker     (127)    20674 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/params.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    19675 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/priors.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    18291 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/random_utils.F90
+-rw-r--r--   0 runner    (1001) docker     (127)    44750 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/read_write.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    47427 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/run_time_info.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/settings.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    29353 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/utils.F90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.743531 cosmosis-3.7/cosmosis/samplers/pymc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/pymc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/pymc/pymc_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9344 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.743531 cosmosis-3.7/cosmosis/samplers/snake/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/snake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/snake/snake.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2017 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/snake/snake_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.743531 cosmosis-3.7/cosmosis/samplers/star/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/star/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4468 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/star/star_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.743531 cosmosis-3.7/cosmosis/samplers/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3221 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/test/test_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.747531 cosmosis-3.7/cosmosis/samplers/zeus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/zeus/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11554 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/samplers/zeus/zeus_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.747531 cosmosis-3.7/cosmosis/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/bad-campaign.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/campaign.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/example-priors.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/example-values.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/example.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/example_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/example_module2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/example_module3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/example_module4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/included.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.751531 cosmosis-3.7/cosmosis/test/libtest/
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/libtest/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/libtest/c_datablock_complex_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/libtest/c_datablock_double_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/libtest/c_datablock_int_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11722 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/libtest/c_datablock_test.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/libtest/cosmosis_test.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/libtest/cosmosis_tests.supp
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/libtest/datablock_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/libtest/entry_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/libtest/ndarray_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/libtest/section_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    28088 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/libtest/test_c_datablock_scalars.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/libtest/test_c_datablock_scalars.template
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/test_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/test_chaining.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8666 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/test_polychord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/test_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/test_text_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-29 12:48:20.000000 cosmosis-3.7/cosmosis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:48:22.751531 cosmosis-3.7/cosmosis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-29 12:48:22.000000 cosmosis-3.7/cosmosis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9278 2024-05-29 12:48:22.000000 cosmosis-3.7/cosmosis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:48:22.000000 cosmosis-3.7/cosmosis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-29 12:48:22.000000 cosmosis-3.7/cosmosis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 12:48:22.000000 cosmosis-3.7/cosmosis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-29 12:48:20.000000 cosmosis-3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 12:48:22.751531 cosmosis-3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-29 12:48:20.000000 cosmosis-3.7/setup.py
```

### Comparing `cosmosis-3.6/LICENSE` & `cosmosis-3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/MANIFEST.in` & `cosmosis-3.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/PKG-INFO` & `cosmosis-3.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmosis
-Version: 3.6
+Version: 3.7
 Summary: The CosmoSIS parameter estimation library.
 Home-page: https://github.com/joezuntz/cosmosis
 Author: Joe Zuntz
 Author-email: joezuntz@googlemail.com
 License-File: LICENSE
 Requires-Dist: pyyaml
 Requires-Dist: emcee
@@ -14,11 +14,11 @@
 Requires-Dist: pybind11
 Requires-Dist: pyyaml
 Requires-Dist: scipy
 Requires-Dist: threadpoolctl
 Requires-Dist: emcee
 Requires-Dist: dynesty
 Requires-Dist: zeus-mcmc
-Requires-Dist: nautilus-sampler==0.6.*
+Requires-Dist: nautilus-sampler>=1.0.1
 Requires-Dist: dulwich
 Requires-Dist: scikit-learn
 Requires-Dist: future
```

### Comparing `cosmosis-3.6/bin/cosmosis-configure` & `cosmosis-3.7/bin/cosmosis-configure`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/bin/cosmosis-extract` & `cosmosis-3.7/bin/cosmosis-extract`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/bin/cosmosis-sample-fisher` & `cosmosis-3.7/bin/cosmosis-sample-fisher`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/__init__.py` & `cosmosis-3.7/cosmosis/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,7 +5,8 @@
 from .samplers import Sampler
 from . import samplers
 from .version import __version__
 from .datablock import option_section, DataBlock
 from .gaussian_likelihood import GaussianLikelihood, \
                                  SingleValueGaussianLikelihood, \
                                  WindowedGaussianLikelihood
+from .output import TextColumnOutput, InMemoryOutput, NullOutput, AstropyOutput, CosmoMCOutput, FitsOutput
```

### Comparing `cosmosis-3.6/cosmosis/campaign.py` & `cosmosis-3.7/cosmosis/campaign.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/config/compilers.mk` & `cosmosis-3.7/cosmosis/config/compilers.mk`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/configure.py` & `cosmosis-3.7/cosmosis/configure.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/constants.py` & `cosmosis-3.7/cosmosis/constants.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/Makefile` & `cosmosis-3.7/cosmosis/datablock/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/c_datablock.cc` & `cosmosis-3.7/cosmosis/datablock/c_datablock.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/c_datablock.h` & `cosmosis-3.7/cosmosis/datablock/c_datablock.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/clamp.hh` & `cosmosis-3.7/cosmosis/datablock/clamp.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/cosmosis_constants.fh` & `cosmosis-3.7/cosmosis/datablock/cosmosis_constants.fh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/cosmosis_constants.h` & `cosmosis-3.7/cosmosis/datablock/cosmosis_constants.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/cosmosis_modules.F90` & `cosmosis-3.7/cosmosis/datablock/cosmosis_modules.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/cosmosis_py/block.py` & `cosmosis-3.7/cosmosis/datablock/cosmosis_py/block.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/cosmosis_py/errors.py` & `cosmosis-3.7/cosmosis/datablock/cosmosis_py/errors.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/cosmosis_py/lib.py` & `cosmosis-3.7/cosmosis/datablock/cosmosis_py/lib.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/cosmosis_py/section_names.py` & `cosmosis-3.7/cosmosis/datablock/cosmosis_py/section_names.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/cosmosis_section_names.F90` & `cosmosis-3.7/cosmosis/datablock/cosmosis_section_names.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/cosmosis_wrappers.F90` & `cosmosis-3.7/cosmosis/datablock/cosmosis_wrappers.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/datablock.cc` & `cosmosis-3.7/cosmosis/datablock/datablock.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/datablock.hh` & `cosmosis-3.7/cosmosis/datablock/datablock.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/datablock_logging.cc` & `cosmosis-3.7/cosmosis/datablock/datablock_logging.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/datablock_logging.h` & `cosmosis-3.7/cosmosis/datablock/datablock_logging.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/datablock_status.h` & `cosmosis-3.7/cosmosis/datablock/datablock_status.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/entry.cc` & `cosmosis-3.7/cosmosis/datablock/entry.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/entry.hh` & `cosmosis-3.7/cosmosis/datablock/entry.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/generate_sections.py` & `cosmosis-3.7/cosmosis/datablock/generate_sections.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/handler.c` & `cosmosis-3.7/cosmosis/datablock/handler.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/ndarray.hh` & `cosmosis-3.7/cosmosis/datablock/ndarray.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/section.cc` & `cosmosis-3.7/cosmosis/datablock/section.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/section.hh` & `cosmosis-3.7/cosmosis/datablock/section.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/section_names.h` & `cosmosis-3.7/cosmosis/datablock/section_names.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/datablock/section_names.txt` & `cosmosis-3.7/cosmosis/datablock/section_names.txt`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/gaussian_likelihood.py` & `cosmosis-3.7/cosmosis/gaussian_likelihood.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/main.py` & `cosmosis-3.7/cosmosis/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -426,15 +426,15 @@
             run_count_ok_total = pool.comm.allreduce(pipeline.run_count_ok)
         
         if is_root and sampler_name != 'test':
             logs.overview(f"Total posterior evaluations = {run_count_total} across all processes")
             logs.overview(f"Successful posterior evaluations = {run_count_ok_total} across all processes")
             if output:
                 output.final("evaluations", run_count_total)
-                output.final("successes", run_count_total)
+                output.final("successes", run_count_ok_total)
                 output.final("complete", "1")
 
 
         if output:
             output.close()
 
     if cleanup_pipeline:
```

### Comparing `cosmosis-3.6/cosmosis/output/__init__.py` & `cosmosis-3.7/cosmosis/output/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/output/astropy_output.py` & `cosmosis-3.7/cosmosis/output/astropy_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/output/cosmomc_output.py` & `cosmosis-3.7/cosmosis/output/cosmomc_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/output/fits_output.py` & `cosmosis-3.7/cosmosis/output/fits_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/output/in_memory_output.py` & `cosmosis-3.7/cosmosis/output/in_memory_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/output/null_output.py` & `cosmosis-3.7/cosmosis/output/null_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/output/output_base.py` & `cosmosis-3.7/cosmosis/output/output_base.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/output/text_output.py` & `cosmosis-3.7/cosmosis/output/text_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/output/utils.py` & `cosmosis-3.7/cosmosis/output/utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/plotting/chain_plots.py` & `cosmosis-3.7/cosmosis/plotting/chain_plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/plotting/grid_plots.py` & `cosmosis-3.7/cosmosis/plotting/grid_plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/plotting/kde.py` & `cosmosis-3.7/cosmosis/plotting/kde.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/plotting/plotter.py` & `cosmosis-3.7/cosmosis/plotting/plotter.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/postprocess.py` & `cosmosis-3.7/cosmosis/postprocess.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/postprocessing/__init__.py` & `cosmosis-3.7/cosmosis/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/postprocessing/cosmology_theory_plots.py` & `cosmosis-3.7/cosmosis/postprocessing/cosmology_theory_plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/postprocessing/density.py` & `cosmosis-3.7/cosmosis/postprocessing/density.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/postprocessing/elements.py` & `cosmosis-3.7/cosmosis/postprocessing/elements.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/postprocessing/inputs.py` & `cosmosis-3.7/cosmosis/postprocessing/inputs.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/postprocessing/latex.ini` & `cosmosis-3.7/cosmosis/postprocessing/latex.ini`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/postprocessing/lazy_pylab.py` & `cosmosis-3.7/cosmosis/postprocessing/lazy_pylab.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/postprocessing/main.py` & `cosmosis-3.7/cosmosis/postprocessing/main.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/postprocessing/outputs.py` & `cosmosis-3.7/cosmosis/postprocessing/outputs.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/postprocessing/plots.py` & `cosmosis-3.7/cosmosis/postprocessing/plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/postprocessing/postprocess.py` & `cosmosis-3.7/cosmosis/postprocessing/postprocess.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/postprocessing/postprocess_base.py` & `cosmosis-3.7/cosmosis/postprocessing/postprocess_base.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/postprocessing/reruns.py` & `cosmosis-3.7/cosmosis/postprocessing/reruns.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/postprocessing/statistics.py` & `cosmosis-3.7/cosmosis/postprocessing/statistics.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/postprocessing/utils.py` & `cosmosis-3.7/cosmosis/postprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/runtime/analytics.py` & `cosmosis-3.7/cosmosis/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/runtime/attribution.py` & `cosmosis-3.7/cosmosis/runtime/attribution.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/runtime/config.py` & `cosmosis-3.7/cosmosis/runtime/config.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/runtime/declare.py` & `cosmosis-3.7/cosmosis/runtime/declare.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/runtime/julia_modules/julia.py` & `cosmosis-3.7/cosmosis/runtime/julia_modules/julia.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/runtime/logs.py` & `cosmosis-3.7/cosmosis/runtime/logs.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/runtime/memmon.py` & `cosmosis-3.7/cosmosis/runtime/memmon.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/runtime/module.py` & `cosmosis-3.7/cosmosis/runtime/module.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/runtime/mpi_pool.py` & `cosmosis-3.7/cosmosis/runtime/mpi_pool.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/runtime/parameter.py` & `cosmosis-3.7/cosmosis/runtime/parameter.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/runtime/pipeline.py` & `cosmosis-3.7/cosmosis/runtime/pipeline.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/runtime/prior.py` & `cosmosis-3.7/cosmosis/runtime/prior.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/runtime/process_pool.py` & `cosmosis-3.7/cosmosis/runtime/process_pool.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/__init__.py` & `cosmosis-3.7/cosmosis/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/abc/abc_sampler.py` & `cosmosis-3.7/cosmosis/samplers/abc/abc_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/abc/abc_sampler_mpi.py` & `cosmosis-3.7/cosmosis/samplers/abc/abc_sampler_mpi.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/apriori/apriori_sampler.py` & `cosmosis-3.7/cosmosis/samplers/apriori/apriori_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/dynesty/dynesty_sampler.py` & `cosmosis-3.7/cosmosis/samplers/dynesty/dynesty_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/emcee/emcee_sampler.py` & `cosmosis-3.7/cosmosis/samplers/emcee/emcee_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/fisher/fisher.py` & `cosmosis-3.7/cosmosis/samplers/fisher/fisher.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/fisher/fisher_sampler.py` & `cosmosis-3.7/cosmosis/samplers/fisher/fisher_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/grid/grid_sampler.py` & `cosmosis-3.7/cosmosis/samplers/grid/grid_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/gridmax/gridmax_sampler.py` & `cosmosis-3.7/cosmosis/samplers/gridmax/gridmax_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/hints.py` & `cosmosis-3.7/cosmosis/samplers/hints.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/importance/importance_sampler.py` & `cosmosis-3.7/cosmosis/samplers/importance/importance_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/kombine/kombine_sampler.py` & `cosmosis-3.7/cosmosis/samplers/kombine/kombine_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/list/list_sampler.py` & `cosmosis-3.7/cosmosis/samplers/list/list_sampler.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,21 @@
     def config(self):
         global list_sampler
         list_sampler = self
 
         self.converged = False
         self.filename = self.read_ini("filename", str)
         self.save_name = self.read_ini("save", str, "")
-        self.burn = self.read_ini("burn", int, 0)
+        # The burn parameter can be an int or a float
+        # so we read it as a string and then convert it
+        burn = self.read_ini("burn", str, "0")
+        try:
+            self.burn = int(burn)
+        except ValueError:
+            self.burn = float(burn)
         self.thin = self.read_ini("thin", int, 1)
         limits = self.read_ini("limits", bool, False)
         self.chunk_size = self.read_ini("chunk_size", int, 100)
 
         #overwrite the parameter limits
         if not limits:
             if self.output is not None:
@@ -53,14 +59,20 @@
 
     def execute(self):
 
         #Load in the filename that was requested
         file_options = {"filename":self.filename}
         column_names, samples, _, _, _ = TextColumnOutput.load_from_options(file_options)
         samples = samples[0]
+        if (self.burn != 0) or (self.thin != 1):
+            if isinstance(self.burn, float):
+                burn = int(self.burn*len(samples))
+            else:
+                burn = self.burn
+            samples = samples[burn::self.thin]
         # find where in the parameter vector of the pipeline
         # each of the table parameters can be found
         replaced_params = []
         for i,column_name in enumerate(column_names):
             # ignore additional columns like e.g. "like", "weight"
             try:
                 section,name = column_name.split('--')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cosmosis-3.6/cosmosis/samplers/maxlike/maxlike_sampler.py` & `cosmosis-3.7/cosmosis/samplers/maxlike/maxlike_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/metropolis/metropolis.py` & `cosmosis-3.7/cosmosis/samplers/metropolis/metropolis.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/metropolis/metropolis_sampler.py` & `cosmosis-3.7/cosmosis/samplers/metropolis/metropolis_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py` & `cosmosis-3.7/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/metropolis/proposal/standard.py` & `cosmosis-3.7/cosmosis/samplers/metropolis/proposal/standard.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/minuit/Makefile` & `cosmosis-3.7/cosmosis/samplers/minuit/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/minuit/minuit_sampler.py` & `cosmosis-3.7/cosmosis/samplers/minuit/minuit_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,23 +24,24 @@
     ]
 
 libname=os.path.join(os.path.split(__file__)[0],"minuit_wrapper.so")
 
 class MinuitSampler(ParallelSampler):
     needs_output = True
     needs_parallel_output = False
+    libminuit_name = libname
     libminuit = None
     sampler_outputs = [("prior", float), ("post", float)]
 
     def config(self):
         self.converged = False
         if MinuitSampler.libminuit is None:
-            if not os.path.exists(libname):
+            if not os.path.exists(self.libminuit_name):
                 raise ValueError("The CosmoSIS minuit2 wrapper was not compiled.  If you installed CosmoSIS manually you need the library minuit2 to use this sampler. See the wiki for more details.")
-            MinuitSampler.libminuit = ct.cdll.LoadLibrary(libname)
+            MinuitSampler.libminuit = ct.cdll.LoadLibrary(self.libminuit_name)
         self.maxiter = self.read_ini("maxiter", int, 1000)
         self.save_dir = self.read_ini("save_dir", str, "")
         self.save_cov = self.read_ini("save_cov", str, "")
         self.output_ini = self.read_ini("output_ini", str, "")
         self.verbose = self.read_ini("verbose", bool, False)
         self.iterations = 0
```

### Comparing `cosmosis-3.6/cosmosis/samplers/minuit/minuit_wrapper.cpp` & `cosmosis-3.7/cosmosis/samplers/minuit/minuit_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/multinest/multinest_sampler.py` & `cosmosis-3.7/cosmosis/samplers/multinest/multinest_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/LICENCE` & `cosmosis-3.7/cosmosis/samplers/multinest/multinest_src/LICENCE`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/Makefile` & `cosmosis-3.7/cosmosis/samplers/multinest/multinest_src/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/README` & `cosmosis-3.7/cosmosis/samplers/multinest/multinest_src/README`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/cwrapper.f90` & `cosmosis-3.7/cosmosis/samplers/multinest/multinest_src/cwrapper.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90` & `cosmosis-3.7/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/nested.f90` & `cosmosis-3.7/cosmosis/samplers/multinest/multinest_src/nested.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/posterior.f90` & `cosmosis-3.7/cosmosis/samplers/multinest/multinest_src/posterior.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/priors.f90` & `cosmosis-3.7/cosmosis/samplers/multinest/multinest_src/priors.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/utils.f90` & `cosmosis-3.7/cosmosis/samplers/multinest/multinest_src/utils.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/utils1.f90` & `cosmosis-3.7/cosmosis/samplers/multinest/multinest_src/utils1.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90` & `cosmosis-3.7/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/nautilus/nautilus_sampler.py` & `cosmosis-3.7/cosmosis/samplers/nautilus/nautilus_sampler.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,14 +45,17 @@
             self.seed = self.read_ini("seed", int, -1)
             if self.seed < 0:
                 self.seed = None
             self.resume_ = self.read_ini("resume", bool, False)
             self.f_live = self.read_ini("f_live", float, 0.01)
             self.n_shell = self.read_ini("n_shell", int, self.n_batch)
             self.n_eff = self.read_ini("n_eff", float, 10000.0)
+            self.n_like_max = self.read_ini("n_like_max", int, -1)
+            if self.n_like_max < 0:
+                self.n_like_max = np.inf
             self.discard_exploration = self.read_ini(
                 "discard_exploration", bool, False)
             self.verbose = self.read_ini("verbose", bool, False)
 
         self.converged = False
 
     def execute(self):
@@ -88,26 +91,27 @@
             pool=self.pool,
             blobs_dtype=float
         )
 
         sampler.run(f_live=self.f_live,
                     n_shell=self.n_shell,
                     n_eff=self.n_eff,
+                    n_like_max=self.n_like_max,
                     discard_exploration=self.discard_exploration,
                     verbose=self.verbose)
 
         for sample, logwt, logl, blob in zip(*sampler.posterior(return_blobs=True)):
             blob = np.atleast_1d(blob)
             prior = blob[0]
             extra = blob[1:]
             logp = logl + prior
             self.output.parameters(sample, extra, logwt, prior, logp)
 
-        self.output.final(
-            "efficiency", sampler.effective_sample_size() / sampler.n_like)
-        self.output.final("neff", sampler.effective_sample_size())
+        self.output.final("efficiency", sampler.n_eff / sampler.n_like)
+        self.output.final("neff", sampler.n_eff)
         self.output.final("nsample", len(sampler.posterior()[0]))
-        self.output.final("log_z", sampler.evidence())
+        self.output.final("log_z", sampler.log_z)
+        self.output.final("log_z_error", 1.0 / np.sqrt(sampler.n_eff))
         self.converged = True
 
     def is_converged(self):
         return self.converged
```

### Comparing `cosmosis-3.6/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py` & `cosmosis-3.7/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/pmc/pmc.py` & `cosmosis-3.7/cosmosis/samplers/pmc/pmc.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/pmc/pmc_sampler.py` & `cosmosis-3.7/cosmosis/samplers/pmc/pmc_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/poco/poco_sampler.py` & `cosmosis-3.7/cosmosis/samplers/poco/poco_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_sampler.py` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/LICENCE` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/LICENCE`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/Makefile` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/README` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/README`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/abort.F90` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/abort.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/array_utils.f90` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/array_utils.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/c_interface.cpp` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/c_interface.cpp`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/calculate.f90` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/calculate.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/clustering.f90` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/clustering.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/feedback.f90` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/feedback.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/generate.F90` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/generate.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/ini.f90` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/ini.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/interfaces.F90` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/interfaces.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/interfaces.h` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/interfaces.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/interfaces.hpp` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/interfaces.hpp`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/params.f90` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/params.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/priors.f90` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/priors.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/random_utils.F90` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/random_utils.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/read_write.f90` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/read_write.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/run_time_info.f90` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/run_time_info.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/settings.f90` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/settings.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/utils.F90` & `cosmosis-3.7/cosmosis/samplers/polychord/polychord_src/utils.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/pymc/pymc_sampler.py` & `cosmosis-3.7/cosmosis/samplers/pymc/pymc_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/sampler.py` & `cosmosis-3.7/cosmosis/samplers/sampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
             return None
         with open(filename, 'rb') as f:
             return pickle.load(f)
 
     @classmethod
     def get_sampler(cls, name):
         try:
-            cls.registry[name.lower()]
+            return cls.registry[name.lower()]
         except KeyError:
             raise KeyError(f"Unknown sampler {name}")
 
 
     def resume(self):
         raise NotImplementedError("The sampler {} does not support resuming".format(self.name))
```

### Comparing `cosmosis-3.6/cosmosis/samplers/snake/snake.py` & `cosmosis-3.7/cosmosis/samplers/snake/snake.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/snake/snake_sampler.py` & `cosmosis-3.7/cosmosis/samplers/snake/snake_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/star/star_sampler.py` & `cosmosis-3.7/cosmosis/samplers/star/star_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/test/test_sampler.py` & `cosmosis-3.7/cosmosis/samplers/test/test_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/samplers/zeus/zeus_sampler.py` & `cosmosis-3.7/cosmosis/samplers/zeus/zeus_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/campaign.yml` & `cosmosis-3.7/cosmosis/test/campaign.yml`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/example_module2.py` & `cosmosis-3.7/cosmosis/test/example_module2.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/libtest/Makefile` & `cosmosis-3.7/cosmosis/test/libtest/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/libtest/c_datablock_complex_array_test.c` & `cosmosis-3.7/cosmosis/test/libtest/c_datablock_complex_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/libtest/c_datablock_double_array_test.c` & `cosmosis-3.7/cosmosis/test/libtest/c_datablock_double_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/libtest/c_datablock_int_array_test.c` & `cosmosis-3.7/cosmosis/test/libtest/c_datablock_int_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c` & `cosmosis-3.7/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c` & `cosmosis-3.7/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c` & `cosmosis-3.7/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/libtest/c_datablock_test.c` & `cosmosis-3.7/cosmosis/test/libtest/c_datablock_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/libtest/cosmosis_test.F90` & `cosmosis-3.7/cosmosis/test/libtest/cosmosis_test.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/libtest/datablock_test.cc` & `cosmosis-3.7/cosmosis/test/libtest/datablock_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/libtest/entry_test.cc` & `cosmosis-3.7/cosmosis/test/libtest/entry_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/libtest/ndarray_test.cc` & `cosmosis-3.7/cosmosis/test/libtest/ndarray_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/libtest/section_test.cc` & `cosmosis-3.7/cosmosis/test/libtest/section_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/libtest/test_c_datablock_scalars.h` & `cosmosis-3.7/cosmosis/test/libtest/test_c_datablock_scalars.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/libtest/test_c_datablock_scalars.template` & `cosmosis-3.7/cosmosis/test/libtest/test_c_datablock_scalars.template`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/test_block.py` & `cosmosis-3.7/cosmosis/test/test_block.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/test_campaign.py` & `cosmosis-3.7/cosmosis/test/test_campaign.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/test_chaining.py` & `cosmosis-3.7/cosmosis/test/test_chaining.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/test_gaussian.py` & `cosmosis-3.7/cosmosis/test/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/test_lib.py` & `cosmosis-3.7/cosmosis/test/test_lib.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/test_modules.py` & `cosmosis-3.7/cosmosis/test/test_modules.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/test_parameters.py` & `cosmosis-3.7/cosmosis/test/test_parameters.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/test_pipeline.py` & `cosmosis-3.7/cosmosis/test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/test_polychord.py` & `cosmosis-3.7/cosmosis/test/test_polychord.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/test_samplers.py` & `cosmosis-3.7/cosmosis/test/test_samplers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-from cosmosis.runtime.config import Inifile
-from cosmosis.samplers.sampler import Sampler
-import cosmosis.samplers.minuit.minuit_sampler
-from cosmosis.runtime.pipeline import LikelihoodPipeline
-from cosmosis.output.in_memory_output import InMemoryOutput
+from cosmosis import Inifile, Sampler, LikelihoodPipeline, InMemoryOutput, TextColumnOutput
 from cosmosis.postprocessing import postprocessor_for_sampler
 import tempfile
 import os
 import sys
 import pytest
 import numpy as np
 from astropy.table import Table
 
-minuit_compiled = os.path.exists(cosmosis.samplers.minuit.minuit_sampler.libname)
+
+minuit_compiled = os.path.exists(Sampler.get_sampler("minuit").libminuit_name)
 
 def run(name, check_prior, check_extra=True, can_postprocess=True, do_truth=False, no_extra=False, pp_extra=True, pp_2d=True, **options):
 
     sampler_class = Sampler.registry[name]
 
     values = tempfile.NamedTemporaryFile('w')
     values.write(
@@ -171,14 +168,45 @@
 
 def test_star():
         run('star', False, pp_extra=False, pp_2d=False)
 
 def test_test():
     run('test', False, can_postprocess=False)
 
+def test_list_sampler():
+    # test that the burn and thin parameters work
+    # make a mock output file with some samples
+    with tempfile.TemporaryDirectory() as dirname:
+
+        input_chain_filename = os.path.join(dirname, "input_chain.txt")
+        input_chain = TextColumnOutput(input_chain_filename)
+        input_chain.add_column('parameters--p1', float)
+        input_chain.add_column('parameters--p2', float)
+        nrow = 100
+        data = np.random.normal(size=(nrow, 2)).clip(-2.99, 2.99)
+        for i in range(nrow):
+            input_chain.parameters(data[i, 0], data[i, 1])
+        input_chain.close()
+
+        burn = 0.2
+        thin = 2
+
+        data = data[20::thin]
+
+        output = run("list", True, can_postprocess=False, filename=input_chain_filename, burn=burn, thin=thin)
+        p1 = output['parameters--p1']
+        p2 = output['parameters--p2']
+        p3 = p1 + p2
+        expected_like = -(p1**2 + p2**2)/2.
+        assert p1.size == 40
+        assert np.allclose(p1, data[:, 0])
+        assert np.allclose(p2, data[:, 1])
+        assert np.allclose(output['PARAMETERS--P3'], p3)
+        assert np.allclose(output["post"] - output["prior"], expected_like)
+
 @pytest.mark.skipif(sys.version_info < (3,7), reason="pocomc requires python3.6+")
 def test_poco():
     try:
         import pocomc
     except ImportError:
         pytest.skip("pocomc not installed")
     run('poco', True, check_extra=False, n_particles=100)
```

### Comparing `cosmosis-3.6/cosmosis/test/test_text_output.py` & `cosmosis-3.7/cosmosis/test/test_text_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/test/test_utils.py` & `cosmosis-3.7/cosmosis/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis/utils.py` & `cosmosis-3.7/cosmosis/utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/cosmosis.egg-info/PKG-INFO` & `cosmosis-3.7/cosmosis.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmosis
-Version: 3.6
+Version: 3.7
 Summary: The CosmoSIS parameter estimation library.
 Home-page: https://github.com/joezuntz/cosmosis
 Author: Joe Zuntz
 Author-email: joezuntz@googlemail.com
 License-File: LICENSE
 Requires-Dist: pyyaml
 Requires-Dist: emcee
@@ -14,11 +14,11 @@
 Requires-Dist: pybind11
 Requires-Dist: pyyaml
 Requires-Dist: scipy
 Requires-Dist: threadpoolctl
 Requires-Dist: emcee
 Requires-Dist: dynesty
 Requires-Dist: zeus-mcmc
-Requires-Dist: nautilus-sampler==0.6.*
+Requires-Dist: nautilus-sampler>=1.0.1
 Requires-Dist: dulwich
 Requires-Dist: scikit-learn
 Requires-Dist: future
```

### Comparing `cosmosis-3.6/cosmosis.egg-info/SOURCES.txt` & `cosmosis-3.7/cosmosis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cosmosis-3.6/setup.py` & `cosmosis-3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
     "pybind11",
     "pyyaml",
     "scipy",
     "threadpoolctl",
     "emcee",
     "dynesty",
     "zeus-mcmc",
-    "nautilus-sampler==0.6.*",
+    "nautilus-sampler>=1.0.1",
     "dulwich",
     "scikit-learn",
     "future",
 
 ]
 
 all_package_files = (datablock_libs + sampler_libs
```

