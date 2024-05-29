# Comparing `tmp/geoschem-gcpy-1.4.2.tar.gz` & `tmp/geoschem_gcpy-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoschem-gcpy-1.4.2.tar", last modified: Fri Jan 26 17:18:27 2024, max compression
+gzip compressed data, was "geoschem_gcpy-1.5.0.tar", last modified: Wed May 29 18:05:15 2024, max compression
```

## Comparing `geoschem-gcpy-1.4.2.tar` & `geoschem_gcpy-1.5.0.tar`

### file list

```diff
@@ -1,141 +1,162 @@
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2024-01-26 17:18:27.976673 geoschem-gcpy-1.4.2/
--rw-r--r--   0 bob       (1000) bob       (1000)     5521 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/AUTHORS.txt
--rw-r--r--   0 bob       (1000) bob       (1000)    22055 2024-01-26 16:24:05.000000 geoschem-gcpy-1.4.2/CHANGELOG.md
--rw-r--r--   0 bob       (1000) bob       (1000)     3397 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/CONTRIBUTING.md
--rw-r--r--   0 bob       (1000) bob       (1000)    14200 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/LICENSE.txt
--rw-r--r--   0 bob       (1000) bob       (1000)      335 2023-02-13 19:44:12.000000 geoschem-gcpy-1.4.2/MANIFEST.in
--rw-r--r--   0 bob       (1000) bob       (1000)     1817 2024-01-26 17:18:27.976673 geoschem-gcpy-1.4.2/PKG-INFO
--rw-r--r--   0 bob       (1000) bob       (1000)     3665 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/README.md
--rw-r--r--   0 bob       (1000) bob       (1000)     2084 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/SUPPORT.md
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2024-01-26 17:18:27.956673 geoschem-gcpy-1.4.2/docs/
--rw-r--r--   0 bob       (1000) bob       (1000)      638 2023-02-13 19:44:12.000000 geoschem-gcpy-1.4.2/docs/Makefile
--rw-r--r--   0 bob       (1000) bob       (1000)      799 2023-02-13 19:44:12.000000 geoschem-gcpy-1.4.2/docs/make.bat
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2024-01-26 17:18:27.966673 geoschem-gcpy-1.4.2/docs/source/
--rw-r--r--   0 bob       (1000) bob       (1000)     3126 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/docs/source/About-GCPy.rst
--rw-r--r--   0 bob       (1000) bob       (1000)    61739 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/docs/source/Benchmarking.rst
--rw-r--r--   0 bob       (1000) bob       (1000)    13370 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/docs/source/Getting-Started-with-GCPy.rst
--rw-r--r--   0 bob       (1000) bob       (1000)     7830 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/docs/source/Guide-to-Useful-Capabilities.rst
--rw-r--r--   0 bob       (1000) bob       (1000)    28586 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/docs/source/Plotting.rst
--rw-r--r--   0 bob       (1000) bob       (1000)    22110 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/docs/source/Regridding.rst
--rw-r--r--   0 bob       (1000) bob       (1000)     2310 2024-01-26 16:24:05.000000 geoschem-gcpy-1.4.2/docs/source/Release_guide.rst
--rw-r--r--   0 bob       (1000) bob       (1000)     4450 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/docs/source/Single_panel.rst
--rw-r--r--   0 bob       (1000) bob       (1000)     4308 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/docs/source/Six_panel.rst
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2024-01-26 17:18:27.956673 geoschem-gcpy-1.4.2/docs/source/_static/
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2024-01-26 17:18:27.966673 geoschem-gcpy-1.4.2/docs/source/_static/images/
--rw-r--r--   0 bob       (1000) bob       (1000)    45959 2023-02-13 19:44:12.000000 geoschem-gcpy-1.4.2/docs/source/_static/images/GEOS-Chem_Logo_Light_Background.png
--rw-r--r--   0 bob       (1000) bob       (1000)    59949 2023-02-13 19:44:12.000000 geoschem-gcpy-1.4.2/docs/source/_static/images/budget_table.png
--rw-r--r--   0 bob       (1000) bob       (1000)    15763 2023-02-13 19:44:12.000000 geoschem-gcpy-1.4.2/docs/source/_static/images/emissions_totals.png
--rw-r--r--   0 bob       (1000) bob       (1000)    34087 2023-02-13 19:44:12.000000 geoschem-gcpy-1.4.2/docs/source/_static/images/inventory_totals.png
--rw-r--r--   0 bob       (1000) bob       (1000)    45337 2023-02-13 19:44:12.000000 geoschem-gcpy-1.4.2/docs/source/_static/images/mass_table.png
--rw-r--r--   0 bob       (1000) bob       (1000)    51460 2023-02-13 19:44:12.000000 geoschem-gcpy-1.4.2/docs/source/_static/images/single_panel_single_level.png
--rw-r--r--   0 bob       (1000) bob       (1000)    21547 2023-02-13 19:44:12.000000 geoschem-gcpy-1.4.2/docs/source/_static/images/single_panel_zonal_mean.png
--rw-r--r--   0 bob       (1000) bob       (1000)   677269 2023-02-13 19:44:12.000000 geoschem-gcpy-1.4.2/docs/source/_static/images/six_panel_single_level.png
--rw-r--r--   0 bob       (1000) bob       (1000)   162738 2023-02-13 19:44:12.000000 geoschem-gcpy-1.4.2/docs/source/_static/images/six_panel_zonal_mean.png
--rw-r--r--   0 bob       (1000) bob       (1000)     3744 2023-02-13 19:44:12.000000 geoschem-gcpy-1.4.2/docs/source/editing_these_docs.rst
--rw-r--r--   0 bob       (1000) bob       (1000)     1242 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/docs/source/index.rst
--rw-r--r--   0 bob       (1000) bob       (1000)    12451 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/docs/source/plot_timeseries.rst
--rw-r--r--   0 bob       (1000) bob       (1000)     2780 2024-01-26 16:24:05.000000 geoschem-gcpy-1.4.2/environment.yml
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2024-01-26 17:18:27.966673 geoschem-gcpy-1.4.2/gcpy/
--rw-r--r--   0 bob       (1000) bob       (1000)      608 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/__init__.py
--rw-r--r--   0 bob       (1000) bob       (1000)       23 2024-01-26 17:18:27.000000 geoschem-gcpy-1.4.2/gcpy/_version.py
--rw-r--r--   0 bob       (1000) bob       (1000)      390 2023-02-13 19:44:12.000000 geoschem-gcpy-1.4.2/gcpy/aod_species.yml
--rw-r--r--   0 bob       (1000) bob       (1000)     1028 2023-02-13 19:44:12.000000 geoschem-gcpy-1.4.2/gcpy/append_grid_corners.py
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2024-01-26 17:18:27.966673 geoschem-gcpy-1.4.2/gcpy/benchmark/
--rw-r--r--   0 bob       (1000) bob       (1000)      722 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/benchmark/README.md
--rw-r--r--   0 bob       (1000) bob       (1000)       80 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/benchmark/__init__.py
--rwxr-xr-x   0 bob       (1000) bob       (1000)     1205 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/benchmark/benchmark_slurm.sh
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2024-01-26 17:18:27.966673 geoschem-gcpy-1.4.2/gcpy/benchmark/cloud/
--rw-r--r--   0 bob       (1000) bob       (1000)      408 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/benchmark/cloud/README.md
--rw-r--r--   0 bob       (1000) bob       (1000)     4090 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/benchmark/cloud/template.1hr_benchmark.yml
--rw-r--r--   0 bob       (1000) bob       (1000)     4087 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/benchmark/cloud/template.1mo_benchmark.yml
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2024-01-26 17:18:27.966673 geoschem-gcpy-1.4.2/gcpy/benchmark/config/
--rw-r--r--   0 bob       (1000) bob       (1000)     3956 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/benchmark/config/1mo_benchmark.yml
--rw-r--r--   0 bob       (1000) bob       (1000)     3981 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/benchmark/config/1yr_ch4_benchmark.yml
--rw-r--r--   0 bob       (1000) bob       (1000)     4108 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/benchmark/config/1yr_fullchem_benchmark.yml
--rw-r--r--   0 bob       (1000) bob       (1000)     3809 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/benchmark/config/1yr_tt_benchmark.yml
--rw-r--r--   0 bob       (1000) bob       (1000)      799 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/benchmark/config/README.md
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2024-01-26 17:18:27.976673 geoschem-gcpy-1.4.2/gcpy/benchmark/modules/
--rw-r--r--   0 bob       (1000) bob       (1000)     2025 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/benchmark/modules/GC_72_vertical_levels.csv
--rw-r--r--   0 bob       (1000) bob       (1000)      547 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/benchmark/modules/README.md
--rw-r--r--   0 bob       (1000) bob       (1000)       27 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/benchmark/modules/__init__.py
--rw-r--r--   0 bob       (1000) bob       (1000)    32399 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/benchmark/modules/benchmark_models_vs_obs.py
--rw-r--r--   0 bob       (1000) bob       (1000)    83846 2024-01-26 16:24:05.000000 geoschem-gcpy-1.4.2/gcpy/benchmark/modules/run_1yr_fullchem_benchmark.py
--rw-r--r--   0 bob       (1000) bob       (1000)    51190 2024-01-26 16:24:05.000000 geoschem-gcpy-1.4.2/gcpy/benchmark/modules/run_1yr_tt_benchmark.py
--rwxr-xr-x   0 bob       (1000) bob       (1000)    64285 2024-01-26 16:24:05.000000 geoschem-gcpy-1.4.2/gcpy/benchmark/run_benchmark.py
--rw-r--r--   0 bob       (1000) bob       (1000)     3550 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/benchmark_categories.yml
--rw-r--r--   0 bob       (1000) bob       (1000)   201912 2024-01-26 16:24:05.000000 geoschem-gcpy-1.4.2/gcpy/benchmark_funcs.py
--rw-r--r--   0 bob       (1000) bob       (1000)    12809 2023-02-13 19:44:12.000000 geoschem-gcpy-1.4.2/gcpy/bpch_to_nc_names.yml
--rw-r--r--   0 bob       (1000) bob       (1000)    24006 2023-02-13 19:44:12.000000 geoschem-gcpy-1.4.2/gcpy/budget_ox.py
--rw-r--r--   0 bob       (1000) bob       (1000)    31014 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/budget_tt.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1702 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/constants.py
--rw-r--r--   0 bob       (1000) bob       (1000)    23271 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/cstools.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1960 2023-02-13 19:44:12.000000 geoschem-gcpy-1.4.2/gcpy/date_time.py
--rw-r--r--   0 bob       (1000) bob       (1000)      487 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/emission_inventories.yml
--rw-r--r--   0 bob       (1000) bob       (1000)      884 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/emission_species.yml
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2024-01-26 17:18:27.976673 geoschem-gcpy-1.4.2/gcpy/examples/
--rw-r--r--   0 bob       (1000) bob       (1000)      102 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/README.txt
--rw-r--r--   0 bob       (1000) bob       (1000)      275 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/__init__.py
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2024-01-26 17:18:27.976673 geoschem-gcpy-1.4.2/gcpy/examples/bpch_to_nc/
--rw-r--r--   0 bob       (1000) bob       (1000)       93 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/bpch_to_nc/__init__.py
--rwxr-xr-x   0 bob       (1000) bob       (1000)     6621 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/bpch_to_nc/bpch2nc.py
--rwxr-xr-x   0 bob       (1000) bob       (1000)     4882 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/bpch_to_nc/bpch_tagco_prodloss_to_nc.py
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2024-01-26 17:18:27.976673 geoschem-gcpy-1.4.2/gcpy/examples/diagnostics/
--rw-r--r--   0 bob       (1000) bob       (1000)      865 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/diagnostics/README.md
--rw-r--r--   0 bob       (1000) bob       (1000)       58 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/diagnostics/__init__.py
--rw-r--r--   0 bob       (1000) bob       (1000)   628862 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/diagnostics/compare_diagnostics.ipynb
--rwxr-xr-x   0 bob       (1000) bob       (1000)    11775 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/diagnostics/compare_diags.py
--rw-r--r--   0 bob       (1000) bob       (1000)      890 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/diagnostics/compare_diags.yml
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2024-01-26 17:18:27.976673 geoschem-gcpy-1.4.2/gcpy/examples/dry_run/
--rw-r--r--   0 bob       (1000) bob       (1000)       85 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/dry_run/__init__.py
--rwxr-xr-x   0 bob       (1000) bob       (1000)    23073 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/dry_run/download_data.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1685 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/dry_run/download_data.yml
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2024-01-26 17:18:27.976673 geoschem-gcpy-1.4.2/gcpy/examples/plotting/
--rw-r--r--   0 bob       (1000) bob       (1000)      124 2024-01-26 16:24:05.000000 geoschem-gcpy-1.4.2/gcpy/examples/plotting/__init__.py
--rwxr-xr-x   0 bob       (1000) bob       (1000)     1359 2024-01-26 16:24:05.000000 geoschem-gcpy-1.4.2/gcpy/examples/plotting/create_test_plot.py
--rwxr-xr-x   0 bob       (1000) bob       (1000)     5703 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/plotting/plot_comparisons.py
--rwxr-xr-x   0 bob       (1000) bob       (1000)     5660 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/plotting/plot_single_panel.py
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2024-01-26 17:18:27.976673 geoschem-gcpy-1.4.2/gcpy/examples/timeseries/
--rw-r--r--   0 bob       (1000) bob       (1000)       99 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/timeseries/README.txt
--rw-r--r--   0 bob       (1000) bob       (1000)       93 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/timeseries/__init__.py
--rwxr-xr-x   0 bob       (1000) bob       (1000)     2738 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/timeseries/mda8_o3_timeseries.py
--rwxr-xr-x   0 bob       (1000) bob       (1000)    11364 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/timeseries/plot_timeseries.py
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2024-01-26 17:18:27.976673 geoschem-gcpy-1.4.2/gcpy/examples/working_with_files/
--rw-r--r--   0 bob       (1000) bob       (1000)      190 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/working_with_files/__init__.py
--rwxr-xr-x   0 bob       (1000) bob       (1000)     2349 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/working_with_files/add_blank_var_to_restart_file.py
--rwxr-xr-x   0 bob       (1000) bob       (1000)     5268 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/working_with_files/concatenate_files.py
--rwxr-xr-x   0 bob       (1000) bob       (1000)     2837 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/working_with_files/insert_field_into_restart_file.py
--rwxr-xr-x   0 bob       (1000) bob       (1000)     3378 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/working_with_files/regrid_restart_ll_to_cs.py
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2024-01-26 17:18:27.976673 geoschem-gcpy-1.4.2/gcpy/examples/xarray_examples/
--rw-r--r--   0 bob       (1000) bob       (1000)       72 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/xarray_examples/__init__.py
--rw-r--r--   0 bob       (1000) bob       (1000)   887334 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/examples/xarray_examples/xarray_overview.ipynb
--rw-r--r--   0 bob       (1000) bob       (1000)    49693 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/file_regrid.py
--rw-r--r--   0 bob       (1000) bob       (1000)    54559 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/grid.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1778 2023-02-13 19:44:12.000000 geoschem-gcpy-1.4.2/gcpy/grid_stretching_transforms.py
--rw-r--r--   0 bob       (1000) bob       (1000)     2926 2023-02-13 19:44:12.000000 geoschem-gcpy-1.4.2/gcpy/lumped_species.yml
--rw-r--r--   0 bob       (1000) bob       (1000)     7937 2023-02-13 19:44:12.000000 geoschem-gcpy-1.4.2/gcpy/mean_oh_from_logs.py
--rw-r--r--   0 bob       (1000) bob       (1000)    14128 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/oh_metrics.py
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2024-01-26 17:18:27.976673 geoschem-gcpy-1.4.2/gcpy/plot/
--rw-r--r--   0 bob       (1000) bob       (1000)      169 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/plot/__init__.py
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2024-01-26 17:18:27.976673 geoschem-gcpy-1.4.2/gcpy/plot/colormaps/
--rw-r--r--   0 bob       (1000) bob       (1000)     2607 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/plot/colormaps/WhGrYlRd.txt
--rw-r--r--   0 bob       (1000) bob       (1000)    47231 2024-01-26 16:24:05.000000 geoschem-gcpy-1.4.2/gcpy/plot/compare_single_level.py
--rw-r--r--   0 bob       (1000) bob       (1000)    42923 2024-01-26 16:24:05.000000 geoschem-gcpy-1.4.2/gcpy/plot/compare_zonal_mean.py
--rw-r--r--   0 bob       (1000) bob       (1000)     4530 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/plot/core.py
--rw-r--r--   0 bob       (1000) bob       (1000)      798 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/plot/gcpy_plot_style
--rw-r--r--   0 bob       (1000) bob       (1000)    22706 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/plot/single_panel.py
--rw-r--r--   0 bob       (1000) bob       (1000)    28282 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/plot/six_plot.py
--rw-r--r--   0 bob       (1000) bob       (1000)     7685 2023-02-13 19:44:12.000000 geoschem-gcpy-1.4.2/gcpy/raveller_1D.py
--rw-r--r--   0 bob       (1000) bob       (1000)    40679 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/regrid.py
--rw-r--r--   0 bob       (1000) bob       (1000)    20101 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/regrid_restart_file.py
--rw-r--r--   0 bob       (1000) bob       (1000)    96622 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/species_database.yml
--rw-r--r--   0 bob       (1000) bob       (1000)    10815 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/ste_flux.py
--rw-r--r--   0 bob       (1000) bob       (1000)    11970 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/units.py
--rw-r--r--   0 bob       (1000) bob       (1000)    78943 2024-01-26 16:03:22.000000 geoschem-gcpy-1.4.2/gcpy/util.py
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2024-01-26 17:18:27.976673 geoschem-gcpy-1.4.2/geoschem_gcpy.egg-info/
--rw-r--r--   0 bob       (1000) bob       (1000)     1817 2024-01-26 17:18:27.000000 geoschem-gcpy-1.4.2/geoschem_gcpy.egg-info/PKG-INFO
--rw-r--r--   0 bob       (1000) bob       (1000)     3883 2024-01-26 17:18:27.000000 geoschem-gcpy-1.4.2/geoschem_gcpy.egg-info/SOURCES.txt
--rw-r--r--   0 bob       (1000) bob       (1000)        1 2024-01-26 17:18:27.000000 geoschem-gcpy-1.4.2/geoschem_gcpy.egg-info/dependency_links.txt
--rw-r--r--   0 bob       (1000) bob       (1000)      572 2024-01-26 17:18:27.000000 geoschem-gcpy-1.4.2/geoschem_gcpy.egg-info/requires.txt
--rw-r--r--   0 bob       (1000) bob       (1000)        5 2024-01-26 17:18:27.000000 geoschem-gcpy-1.4.2/geoschem_gcpy.egg-info/top_level.txt
--rw-r--r--   0 bob       (1000) bob       (1000)       38 2024-01-26 17:18:27.976673 geoschem-gcpy-1.4.2/setup.cfg
--rw-r--r--   0 bob       (1000) bob       (1000)     3815 2024-01-26 16:24:05.000000 geoschem-gcpy-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:15.469491 geoschem_gcpy-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    27901 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14200 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-29 18:05:15.469491 geoschem_gcpy-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/SUPPORT.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:15.441491 geoschem_gcpy-1.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:15.445491 geoschem_gcpy-1.5.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/About-GCPy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    78458 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/Benchmarking.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/Compare-Diags.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15075 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/Getting-Started-with-GCPy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7705 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/Guide-to-Useful-Capabilities.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/Hemco-Formatting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/Known-Bugs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/Matplotlib-Backend.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/ObsPack.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    28633 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/Plotting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    22105 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/Regridding.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/Release-Guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/Single-Panel.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/Six-Panel.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/Test-Plot.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:15.437491 geoschem_gcpy-1.5.0/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:15.449491 geoschem_gcpy-1.5.0/docs/source/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    45959 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/_static/images/GEOS-Chem_Logo_Light_Background.png
+-rw-r--r--   0 runner    (1001) docker     (127)    59949 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/_static/images/budget_table.png
+-rw-r--r--   0 runner    (1001) docker     (127)   127845 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/_static/images/create_test_plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15763 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/_static/images/emissions_totals.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34087 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/_static/images/inventory_totals.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45337 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/_static/images/mass_table.png
+-rw-r--r--   0 runner    (1001) docker     (127)    81135 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/_static/images/single_panel_single_level.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25537 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/_static/images/single_panel_zonal_mean.png
+-rw-r--r--   0 runner    (1001) docker     (127)   275021 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/_static/images/six_panel_single_level.png
+-rw-r--r--   0 runner    (1001) docker     (127)    91508 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/_static/images/six_panel_zonal_mean.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/editing_these_docs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:15.449491 geoschem_gcpy-1.5.0/gcpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 18:05:15.000000 geoschem_gcpy-1.5.0/gcpy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/append_grid_corners.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:15.453491 geoschem_gcpy-1.5.0/gcpy/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1213 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/benchmark_slurm.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:15.453491 geoschem_gcpy-1.5.0/gcpy/benchmark/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/cloud/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/cloud/template.1hr_benchmark.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/cloud/template.1mo_benchmark.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:15.453491 geoschem_gcpy-1.5.0/gcpy/benchmark/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/config/1mo_benchmark.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/config/1yr_ch4_benchmark.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/config/1yr_fullchem_benchmark.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/config/1yr_tt_benchmark.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/config/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:15.457491 geoschem_gcpy-1.5.0/gcpy/benchmark/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/modules/GC_72_vertical_levels.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/modules/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/modules/aod_species.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/modules/benchmark_categories.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/modules/benchmark_drydep.py
+-rw-r--r--   0 runner    (1001) docker     (127)   196329 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/modules/benchmark_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18657 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/modules/benchmark_mass_cons_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27034 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/modules/benchmark_models_vs_obs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16593 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/modules/benchmark_models_vs_sondes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8983 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/modules/benchmark_scrape_gcclassic_timers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11431 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/modules/benchmark_scrape_gchp_timers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20633 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/modules/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24157 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/modules/budget_ox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/modules/budget_tt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/modules/emission_inventories.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/modules/emission_species.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/modules/lumped_species.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    14128 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/modules/oh_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93135 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/modules/run_1yr_fullchem_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55652 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/modules/run_1yr_tt_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96622 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/modules/species_database.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    10833 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/modules/ste_flux.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    67367 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/benchmark/run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12809 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/bpch_to_nc_names.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:15.457491 geoschem_gcpy-1.5.0/gcpy/community/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/community/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/community/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6083 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/community/create_obspack_coords_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16065 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/community/format_hemco_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23703 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/cstools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/date_time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:15.457491 geoschem_gcpy-1.5.0/gcpy/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:15.457491 geoschem_gcpy-1.5.0/gcpy/examples/bpch_to_nc/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/bpch_to_nc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6621 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/bpch_to_nc/bpch2nc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4882 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/bpch_to_nc/bpch_tagco_prodloss_to_nc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:15.461491 geoschem_gcpy-1.5.0/gcpy/examples/diagnostics/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/diagnostics/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/diagnostics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   628862 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/diagnostics/compare_diagnostics.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11796 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/diagnostics/compare_diags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/diagnostics/compare_diags.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:15.461491 geoschem_gcpy-1.5.0/gcpy/examples/dry_run/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/dry_run/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23073 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/dry_run/download_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/dry_run/download_data.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:15.461491 geoschem_gcpy-1.5.0/gcpy/examples/hemco/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/hemco/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/hemco/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4898 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/hemco/format_hemco_demo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3152 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/hemco/make_mask_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:15.461491 geoschem_gcpy-1.5.0/gcpy/examples/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/plotting/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1359 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/plotting/create_test_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5703 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/plotting/plot_comparisons.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5660 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/plotting/plot_single_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:15.461491 geoschem_gcpy-1.5.0/gcpy/examples/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/timeseries/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/timeseries/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11364 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/timeseries/plot_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:15.465491 geoschem_gcpy-1.5.0/gcpy/examples/working_with_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/working_with_files/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2349 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/working_with_files/add_blank_var_to_restart_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5268 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/working_with_files/concatenate_files.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2837 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/working_with_files/insert_field_into_restart_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3378 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/working_with_files/regrid_restart_ll_to_cs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:15.465491 geoschem_gcpy-1.5.0/gcpy/examples/xarray_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/xarray_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   887334 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/examples/xarray_examples/xarray_overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    50107 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/file_regrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58944 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/grid_stretching_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:15.465491 geoschem_gcpy-1.5.0/gcpy/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/plot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:15.465491 geoschem_gcpy-1.5.0/gcpy/plot/colormaps/
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/plot/colormaps/WhGrYlRd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    47231 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/plot/compare_single_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42923 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/plot/compare_zonal_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/plot/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/plot/gcpy_plot_style
+-rw-r--r--   0 runner    (1001) docker     (127)    22706 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/plot/single_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28282 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/plot/six_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/raveller_1D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40695 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/regrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20101 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/regrid_restart_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72404 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/gcpy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:05:15.469491 geoschem_gcpy-1.5.0/geoschem_gcpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-29 18:05:15.000000 geoschem_gcpy-1.5.0/geoschem_gcpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-29 18:05:15.000000 geoschem_gcpy-1.5.0/geoschem_gcpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:05:15.000000 geoschem_gcpy-1.5.0/geoschem_gcpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-29 18:05:15.000000 geoschem_gcpy-1.5.0/geoschem_gcpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-29 18:05:15.000000 geoschem_gcpy-1.5.0/geoschem_gcpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 18:05:15.469491 geoschem_gcpy-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-05-29 18:05:11.000000 geoschem_gcpy-1.5.0/setup.py
```

### Comparing `geoschem-gcpy-1.4.2/AUTHORS.txt` & `geoschem_gcpy-1.5.0/AUTHORS.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-List of Developers for GEOS-Chem, HEMCO, and Related Software,
-including GCPy (11 Jul 2023)
+List of Developers for GEOS-Chem, HEMCO, and Related Software
+(23 May 2024)
 ===============================================================================
 
 ADAMS, Peter
 ALEXANDER, Becky
 ALVARADO, Matthew
 AMOS, Helen
 ANGOT, Helene
@@ -19,14 +19,15 @@
 BINDLE, Liam
 BOERSMA, Folkert
 BOJJAGANI, Sreekanth
 BONILLA, Eimy
 BOVY, Benoit
 BOWMAN, Kevin
 BOYS, Brian
+BRANFORD, Simon
 BRATTICH, Erika
 BREIDER, Tom
 BREWER, Jared
 BROWNE, Ellie
 BROWN-STEINER, Benjamin
 BUKOSA, Beata
 BUTENHOFF, Christopher
@@ -286,14 +287,15 @@
 SUNDERLAND, Elsie
 SUNTHARALINGAM, Parvada
 SURL, Luke
 SUTHERLAND, Bethany
 SUTO, Kimito
 SZELAG, Monika
 TAI, Amos
+TANG, Yidan
 TANIMOTO, Hiroshi
 TANNAHILL, John
 TAO, Shu
 THACKRAY, Colin
 THOMPSON, Matt
 THONAT, Thibaud
 TIAN, Rong
@@ -308,14 +310,15 @@
 TZOMPA-SOSA, Zitely
 UNGER, Nadine
 VAL MARTIN, Maria
 VAN DONKELAAR, Aaron 
 VAROTSOS, Kostas
 VINKEN, Geert
 VITT, Francis
+VOHRA, Karn
 WAGSTROM, Kristina
 WALKER, Thomas
 WANG, James
 WANG, Jun
 WANG, Qiaoqiao
 WANG, Xuan
 WANG, Xiaoli
@@ -355,12 +358,13 @@
 ZHANG, Dandan
 ZHANG, Hongliang
 ZHANG, Jiawei
 ZHANG, Li
 ZHANG, Lin
 ZHANG, Qiang
 ZHANG, Yanxu
+ZHU, Haihui
 ZHU, Lei
 ZHU, Liye
 ZHUANG, Jiawei
 ZHUANG, Quanlai
 ZOOGMAN, Peter
```

### Comparing `geoschem-gcpy-1.4.2/CHANGELOG.md` & `geoschem_gcpy-1.5.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,98 @@
 # GCPy Changelog
 
 All notable changes to GCPy will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.5.0] - 2024-05-29
+### Added
+- Script `gcpy/benchmark/modules/benchmark_utils.py`, with common benchmark utility functions
+- Script `gcpy/benchmark/modules/benchmark_drydep.py`, with code to create drydep velocity plots
+- YAML tag `plot_drydep` in `gcpy/benchmark/config/*.yml` files
+- Badge for `build-gcpy-environment` GitHub Action in `README.md`
+- Badges in `docs/source/index.rst`
+- GitHub action to push GCPy releases to PyPi
+- Script `./release/changeVersionNumbers.sh`, used to update version numbers in various files before release
+- Mamba/Conda enviroment file `docs/environment_files/read_the_docs_environment.yml`, for building ReadTheDocs documentation
+- Environment files `docs/environment_files/gcpy_requirements.txt` and `docs/environment_files/read_the_docs_requirements.txt`
+- New benchmark script `gcpy/benchmark/modules/benchmark_models_vs_sondes.py`
+- Added fixed level budget diagnostic to budget operations table
+- Function `rename_speciesconc_to_speciesconcvv` in `gcpy/benchmark/modules/benchmark_utils.py`
+- Function `copy_file_to_dir` in `gcpy/util.py`.  This is a wrapper for `shutil.copyfile`.
+- GitHub Action config file `.github/workflows/stale.yml`, which replaces StaleBot
+- Added `gcpy/community/format_hemco_data.py` from @hannahnesser
+- Added `gcpy/examples/hemco/format_hemco_demo.py` from @hannahnesser
+- Added HCl to `gcpy/benchmark/modules/emission_species.yml` and GTChlorine to `gcpy/benchmark/modules/emission_inventories.yml` for GEOS-Chem 14.4.0
+- Example script `gcpy/examples/working_with_files/make_mask_file.py`
+- Convenience function `replace_whitespace` in `gcpy/util.py`
+- Benchmark script `gcpy/benchmark/modules/benchmark_scrape_gcclassic_timers.py`
+- Benchmark script `gcpy/benchmark/modules/benchmark_scrape_gchp_timers.py`
+- 1-year benchmark scripts now produce GCC vs GCC and GCHP vs GCHP timing tables
+- Functions `gcc_vs_gcc_dirs`, `gchp_vs_gcc_dirs`, `gchp_vs_gchp_dirs`, and `get_log_filepaths` in `gcpy/benchmark/modules/benchmark_utils.py`
+- Script `gcpy/benchmark/modules/benchmark_mass_cons_table.py`, with code to create mass conservation tables
+- Expanded statistics output in benchmark mass conservation tables
+- Function `get_datetimes_from_filenames` in `gcpy/benchmark/modules/benchmark_utils.py`
+- Function `replace_whitespace` in `gcpy/util.py`
+
+### Changed
+- Bump pip from 23.2.1 to 23.3 (dependabot suggested this)
+- Bump pypdf from 3.16.1 to 3.17.0 (dependabot suggested this)
+- YAML tag `operations_budget` is now `ops_budget_table` in `gcpy/benchmark/config/1yr_tt_benchmark.yml`
+- Now require `matplotlib=3.8.0` in `docs/environment_files/environment.yml` (with other pegged versions)
+- Now run the `stale` GitHub action at 00:00 UTC on the 1st of each month
+- Renamed `docs/environment_files/environment.yml` to `gcpy_environment.yml`
+- `environment.yml` links to `docs/environment_files/gcpy_environment.yml`
+- `requirements.txt` links to `docs/environment_files/requirements.txt`
+- Python packages for RTD documenation builds from `docs/environment_files/environment.yml`
+- Script `benchmark_model_vs_obs.py` now uses grid inquiry functions from `grid.py` to return data nearest to a (lat,lon) location
+- Moved routine `get_geoschem_level_metadata` to `gcpy/benchmark/modules/benchmark_utils.py`
+- Refactored `get_vert_grid.py` (in `gcpy/grid.py`) to accept the `p_sfc` argument; Also never-nested the if-block logic.
+- `benchmark_slurm.sh` script now saves output to a log file with the same base name as the YAML config file
+- `benchmark_models_vs_obs.py` now reads the observational data paths and metadata from  `1yr_fullchem_benchmark.yml`
+- Moved benchmark code from `gcpy/` to `gcpy/benchmark/modules/`
+- Benchmark functions now call `rename_speciesconc_to_speciesconcvv`
+- Create radionuclide, STE flux, and mass conservation tables for Ref and Dev versions in TransportTracers benchmarks
+- Use new function `copy_file_to_dir` to copy the benchmark script and configuration file to the benchmark results folders
+- Updated GitHub stalebot config file `stale.yml` with new issue/PR labels that should not go stale
+- Updated benchmark driver scripts and config files to print GCClassic & GCHP timing information
+- Updated documentation for GCPy 1.5.0 release
+- Converted Github issue templates to issue forms using YAML definition files
+
+### Fixed
+- CS inquiry functions in `gcpy/cstools.py` now work properly for `xr.Dataset` and `xr.DataArray` objects
+- Prevent an import error by using `seaborn-v0_8-darkgrid` in`gcpy/benchmark/modules/benchmark_models_vs_obs.py`
+- `gcpy/file_regrid.py` now creates GCHP files with `DELP_DRY` instead of `DELPDRY`
+- Fixed bugs in GCHP vs GCHP sections of 1-yr benchmark run scripts to allow comparison of GCHP runs with different grid resolutions
+- Fixed silent bug in transport tracer benchmark GCC vs GCHP mass
+  tables preventi ng them from being generated
+- Import error in `gcpy/examples/diagnostics/compare_diags.py`
+- Added missing `n_cores` to `gcpy/examples/diagnostics/compare_diags.yml`
+- Added missing `plot_drydep` option to `gcpy/gcpy/benchmark/config/1yr_ch4_benchmark.yml`
+- Add `docs/requirements.txt` symbolic link to `docs/environment_files/read_the_docs_requirements.txt` for RTD builds 
+- `gcpy/file_regrid.py` now tests if `lon_bnds`, `lat_bnds` are in the dataset before trying to drop them
+
+### Removed
+- Example script `gcpy/examples/plotting/mda8_o3_timeseries.py`
+- Removed `Pylint` GitHub action
+- Environment file `docs/environment_files/environment.yml`
+- Environment file `docs/environment_files/requirements.txt`
+- Removed `awscli` from the GCPy environment; version 2 is no longer available on conda-forge or PyPi
+- GitHub config files `.github/stale.yml` and `.github/no-response.yml`
+- Routine `make_benchmark_mass_conservation_table` in `benchmark_funcs.py`; this is now obsolete
+
 ## [1.4.2] - 2024-01-26
 ### Added
 - Example script `create_test_plot.py`, which can be used to check that GCPy has been installed properly
 - GitHub action `build-gcpy-environment` which tests installation of the mamba environment specified in in `docs/environment_files/environment.yml`
 - YAML file`docs/environment_files/testing.yml` for building an environment without pegged package versions (for testing)
 - GitHub action `build-test-environment` to test the environment specified in `testing.yml`
 
 ### Changed
-- `build-gcpy-environment` GitHub action now runs with several Python versions 
+- `build-gcpy-environment` GitHub action now runs with several Python versions
 
 ### Fixed
 - Prevent overwriting of the `results` variable when parallel plotting is deactivated (`n_cores: 1`)
 
 ## [1.4.1] - 2023-12-08
 ### Fixed
 - Now use the proper default value for the `--weightsdir` argument to `gcpy/file_regrid.py`
```

### Comparing `geoschem-gcpy-1.4.2/CONTRIBUTING.md` & `geoschem_gcpy-1.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/LICENSE.txt` & `geoschem_gcpy-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/PKG-INFO` & `geoschem_gcpy-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoschem-gcpy
-Version: 1.4.2
+Version: 1.5.0
 Home-page: https://github.com/geoschem/gcpy
 Author: GEOS-Chem Support Team
 Author-email: geos-chem-support@g.harvard.edu
 Maintainer: GEOS-Chem Support Team
 Maintainer-email: geos-chem-support@g.harvard.edu
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,21 +25,21 @@
 Requires-Dist: joblib==1.3.2
 Requires-Dist: jupyter==1.0.0
 Requires-Dist: matplotlib==3.8.0
 Requires-Dist: netcdf4==1.6.0
 Requires-Dist: netcdf-fortran==4.5.4
 Requires-Dist: numpy==1.26.0
 Requires-Dist: pandas==2.1.1
-Requires-Dist: pip==23.2.1
+Requires-Dist: pip==23.3
 Requires-Dist: pylint==2.17.5
 Requires-Dist: pyproj==3.6.1
 Requires-Dist: python==3.9.18
-Requires-Dist: pypdf==3.16.1
+Requires-Dist: pypdf==3.17.0
 Requires-Dist: recommonmark==0.7.1
-Requires-Dist: requests==2.31.0
+Requires-Dist: requests==2.32.0
 Requires-Dist: scipy==1.11.2
 Requires-Dist: sparselt==0.1.3
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: tk==8.6.12
 Requires-Dist: xarray==2023.8.0
 Requires-Dist: esmf==8.1.1
 Requires-Dist: esmpy==8.1.1
```

### Comparing `geoschem-gcpy-1.4.2/README.md` & `geoschem_gcpy-1.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # GCPy: Python toolkit for GEOS-Chem
 
 <p>
   <a href="https://github.com/geoschem/gcpy/releases"><img src="https://img.shields.io/github/v/release/geoschem/gcpy?include_prereleases&label=Latest%20Pre-Release"></a>
   <a href="https://github.com/geoschem/gcpy/releases"><img src="https://img.shields.io/github/v/release/geoschem/gcpy?label=Latest%20Stable%20Release"></a>
-  <a href="https://github.com/geoschem/gcpy/releases/"><img src="https://img.shields.io/github/release-date/geoschem/gcpy"></a>
-  <br />
   <a href="https://doi.org/10.5281/zenodo.3689589"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.3689589.svg" alt="DOI"></a>
+ <br />
   <a href="https://github.com/geoschem/gcpy/blob/main/LICENSE.txt"><img src="https://img.shields.io/badge/License-MIT-blue.svg"></a>
+  <a href="https://github.com/geoschem/gcpy/releases/"><img src="https://img.shields.io/github/release-date/geoschem/gcpy"></a>
   <a href="https://gcpy.readthedocs.io/en/latest/"><img src="https://img.shields.io/readthedocs/gcpy?label=ReadTheDocs"></a>
+  <a href="https://github.com/geoschem/gcpy/actions/workflows/build-gcpy-environment.yml"><img src="https://github.com/geoschem/gcpy/actions/workflows/build-gcpy-environment.yml/badge.svg"></a>
 </p>
 
-
 **GCPy** is a Python-based toolkit containing useful functions for working specifically with the GEOS-Chem model of atmospheric chemistry and composition.
 
 **GCPy** aims to build on the well-established scientific Python technical stack, leveraging tools like **cartopy**, **numpy**, and **xarray** to simplify the task of working with GEOS-Chem model output and performing atmospheric chemistry analyses.
 
 
 ## What GCPy was intended to do:
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
 # GCPy: Python toolkit for GEOS-Chem
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_g_e_o_s_c_h_e_m_/
 _g_c_p_y_?_i_n_c_l_u_d_e___p_r_e_r_e_l_e_a_s_e_s_&_l_a_b_e_l_=_L_a_t_e_s_t_%_2_0_P_r_e_-_R_e_l_e_a_s_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_g_e_o_s_c_h_e_m_/_g_c_p_y_?_l_a_b_e_l_=_L_a_t_e_s_t_%_2_0_S_t_a_b_l_e_%_2_0_R_e_l_e_a_s_e_]_[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_r_e_l_e_a_s_e_-_d_a_t_e_/_g_e_o_s_c_h_e_m_/_g_c_p_y_]
-_[_D_O_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_r_e_a_d_t_h_e_d_o_c_s_/_g_c_p_y_?_l_a_b_e_l_=_R_e_a_d_T_h_e_D_o_c_s_]
+_g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_g_e_o_s_c_h_e_m_/_g_c_p_y_?_l_a_b_e_l_=_L_a_t_e_s_t_%_2_0_S_t_a_b_l_e_%_2_0_R_e_l_e_a_s_e_]_[_D_O_I_]
+_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_g_i_t_h_u_b_/_r_e_l_e_a_s_e_-_d_a_t_e_/_g_e_o_s_c_h_e_m_/_g_c_p_y_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_r_e_a_d_t_h_e_d_o_c_s_/
+_g_c_p_y_?_l_a_b_e_l_=_R_e_a_d_T_h_e_D_o_c_s_]_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_g_e_o_s_c_h_e_m_/_g_c_p_y_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/
+_b_u_i_l_d_-_g_c_p_y_-_e_n_v_i_r_o_n_m_e_n_t_._y_m_l_/_b_a_d_g_e_._s_v_g_]
 **GCPy** is a Python-based toolkit containing useful functions for working
 specifically with the GEOS-Chem model of atmospheric chemistry and composition.
 **GCPy** aims to build on the well-established scientific Python technical
 stack, leveraging tools like **cartopy**, **numpy**, and **xarray** to simplify
 the task of working with GEOS-Chem model output and performing atmospheric
 chemistry analyses. ## What GCPy was intended to do: 1. Produce plots and
 tables from [GEOS-Chem](https://geos-chem.readthedocs.io) output using simple
```

### Comparing `geoschem-gcpy-1.4.2/SUPPORT.md` & `geoschem_gcpy-1.5.0/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/docs/Makefile` & `geoschem_gcpy-1.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/docs/make.bat` & `geoschem_gcpy-1.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/docs/source/About-GCPy.rst` & `geoschem_gcpy-1.5.0/docs/source/About-GCPy.rst`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/docs/source/Benchmarking.rst` & `geoschem_gcpy-1.5.0/docs/source/Benchmarking.rst`

 * *Files 13% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 
 .. _bmk:
 
 ############
 Benchmarking
 ############
 
-The GEOS-Chem Support Team uses GCPy to produce comparison plots and
-summary tables from GEOS-Chem benchmark simulations.  In this chapter
-we will describe this capability of GCPy.
+The `GEOS-Chem Support Team
+<https://geoschem.github.io/support-team>`_ uses GCPy to produce
+comparison plots and summary tables from GEOS-Chem benchmark
+simulations.  In this chapter we will describe this capability of
+GCPy.
 
 .. _bmk-scripts:
 
 ======================================
 Location of benchmark plotting scripts
 ======================================
 
@@ -96,15 +98,25 @@
       #   obs_data_dir: Path to observational data (for models vs obs plots)
       #
       paths:
         main_dir: /path/to/benchmark/main/dir    # EDIT AS NEEDED
         results_dir: /path/to/BenchmarkResults   # EDIT AS NEEDED
         weights_dir: /n/holyscratch01/external_repos/GEOS-CHEM/gcgrid/data/ExtData/GCHP/RegriddingWeights
         spcdb_dir: default
-        obs_data_dir: /path/to/observational/data
+      #
+      # Observational data dirs are on Harvard Cannon, edit if necessary
+      #
+      obs_data:
+        ebas_o3:
+          data_dir: /n/jacob_lab/Lab/obs_data_for_bmk/ebas_sfc_o3_2019
+          data_label: "O3 (EBAS, 2019)"
+        sondes:
+          data_dir: /n/jacob_lab/Lab/obs_data_for_bmk/sondes_2010-2019
+          data_file: allozonesondes_2010-2019.csv
+          site_file: allozonesondes_site_elev.csv
 
    |br|
 
 #. Edit the :literal:`data` section to specify the directories (and
    labels) for the Ref and Dev versions for GEOS-Chem Classic and GCHP.
 
    .. code-block:: yaml
@@ -122,39 +134,48 @@
       data:
         ref:
           gcc:
             version: GCC_ref
             dir: GCC_ref
             outputs_subdir: OutputDir
             restarts_subdir: Restarts
-            bmk_start: "2019-01-01T00:00:00"
-            bmk_end: "2020-01-01T00:00:00"
+            logs_subdir: .
+            logs_template: "GC.log"
+            bmk_start: "2019-07-01T00:00:00"
+            bmk_end: "2019-08-01T00:00:00"
           gchp:
-            version: GCC_dev
-            dir: GCC_dev
+            version: GCHP_ref
+            dir: GCHP_ref
             outputs_subdir: OutputDir
             restarts_subdir: Restarts
-            bmk_start: "2019-01-01T00:00:00"
-            bmk_end: "2020-01-01T00:00:00"
+            logs_subdir: .
+            logs_template: "gchp.%Y%m%d_0000z.log"
+            bmk_start: "2019-07-01T00:00:00"
+            bmk_end: "2019-08-01T00:00:00"
             is_pre_14.0: False
             resolution: c24
         dev:
           gcc:
             version: GCC_dev
             dir: GCC_dev
             outputs_subdir: OutputDir
             restarts_subdir: Restarts
-            bmk_start: "2019-01-01T00:00:00"
-            bmk_end: "2020-01-01T00:00:00"
+            logs_subdir: .
+            logs_template: "GC.log"
+            bmk_start: "2019-07-01T00:00:00"
+            bmk_end: "2019-08-01T00:00:00"
           gchp:
-            version: GCC_dev
-            dir: GCC_dev
+            version: GCHP_dev
+            dir: GCHP_dev
+            outputs_subdir: OutputDir
             restarts_subdir: Restarts
-            bmk_start: "2019-01-01T00:00:00"
-            bmk_end: "2020-01-01T00:00:00"
+            logs_subdir: Logs
+            logs_template: "gchp.%Y%m%d_0000z.log"
+            bmk_start: "2019-07-01T00:00:00"
+            bmk_end: "2019-08-01T00:00:00"
             is_pre_14.0: False
             resolution: c24
 
    |br|
 
 #. Edit the :literal:`comparisons` section to specify the types of
    comparisons you would like to perform.
@@ -177,38 +198,41 @@
           run: True
           dir: GCHP_version_comparison
           tables_subdir: Tables
         gchp_vs_gcc_diff_of_diffs:
           run: True
           dir: GCHP_GCC_diff_of_diffs
 
+   |br|
+
 #. Edit the :literal:`outputs` section to select the plots and tables
    that you would like to generate.
 
    .. code-block:: yaml
 
       #
       # outputs: Specifies the plots and tables to generate
       #
       outputs:
-         plot_conc: True
-         plot_emis: True
-         emis_table: True
-         plot_jvalues: True
-         plot_aod: True
-         mass_table: True
-         ops_budget_table: False
-         aer_budget_table: True
-         Ox_budget_table: True
-         ste_table: True # GCC only
-         OH_metrics: True
-         plot_models_vs_obs: True
-         plot_options:
-           by_spc_cat: True
-           by_hco_cat: True
+        plot_conc: True
+        plot_emis: True
+        emis_table: True
+        plot_jvalues: True
+        plot_aod: True
+        plot_drydep: False  # Need to save out DryDep collection for 1-mo
+        mass_table: True
+        mass_accum_table: False
+        ops_budget_table: False
+        OH_metrics: True
+        ste_table: True # GCC only
+        timing_table: True
+        summary_table: True
+        plot_options:
+          by_spc_cat: True
+          by_hco_cat: True
 
    |br|
 
 #. Edit the :literal:`n_cores` setting if you wish to change the
    number of computational cores to use.  If not, leave
    :literal:`n_cores` set to :literal:`-1`, which will use as many
    cores as possible.
@@ -281,15 +305,15 @@
          # Specify a YAML file with benchmark options
          # Uncomment the file that you wish:
          #config="1mo_benchmark.yml"
          config="1yr_fullchem_benchmark.yml"
          #config="1yr_tt_benchmark.yml"
 
          # Call the run_benchmark script to make the plots
-         python -m gcpy.benchmark.run_benchmark "${config}" > benchmark.log 2>&1
+         python -m gcpy.benchmark.run_benchmark "${config}" > "${config/.yml/.log}" 2>&1
 
          # Turn off python environment
          mamba deactivate
 
          exit 0
 
       Lastly, start the SLURM batch execution with this command:
@@ -319,30 +343,44 @@
 .. note::
 
    We are working towards moving all benchmark-related source code to
    the :file:`gcpy/benchmark/` directory tree.  For the time being,
    the :file:`benchmark_funcs.py` script is located in the
    :file:`/path/to/GCPy/gcpy/` directory.
 
-.. table:: **Functions creating comparison plots from benchmark
-           simulation output**
+.. table:: **Functions creating six-panel comparison plots**
+   :align: center
 
-   +-----------------------------------------------+----------------------------------------------+
-   | Function                                      | Type of 6-panel comparison plot created      |
-   +===============================================+==============================================+
-   | ``make_benchmark_aod_plots()``                | Comparison plots for aerosol optical depth   |
-   +-----------------------------------------------+----------------------------------------------+
-   | ``make_benchmark_conc_plots()``               | Species concentration                        |
-   +-----------------------------------------------+----------------------------------------------+
-   | ``make_benchmark_emis_plots()``               | Emissions (by species and catgegory)         |
-   +-----------------------------------------------+----------------------------------------------+
-   | ``make_benchmark_jvalue_plots()``             | Comparison plots for J-values (photolysis)   |
-   +-----------------------------------------------+----------------------------------------------+
-   | ``make_benchmark_wetdep_plots()``             | Comparison plots for species wet deposition  |
-   +-----------------------------------------------+----------------------------------------------+
+   +-------------------------------+----------------------------------------+
+   | Function                      | Plot that it creates                   |
+   +===============================+========================================+
+   | :ref:`bmk-funcs-plot-aod`     | Aerosol optical depth                  |
+   +-------------------------------+----------------------------------------+
+   | :ref:`bmk-funcs-plot-conc`    | Species concentrations                 |
+   +-------------------------------+----------------------------------------+
+   | :ref:`bmk-funcs-plot-dryd`    | Dry deposition velocities              |
+   +-------------------------------+----------------------------------------+
+   | :ref:`bmk-funcs-plot-emis`    | Emissions (by species and catgegory)   |
+   +-------------------------------+----------------------------------------+
+   | :ref:`bmk-funcs-plot-jvalue`  | J-values (photolysis)                  |
+   +-------------------------------+----------------------------------------+
+   | :ref:`bmk-funcs-plot-wetdep`  | Wet deposition of soluble species      |
+   +-------------------------------+----------------------------------------+
+
+.. table:: **Functions creating model vs. observation plots**
+   :align: center
+
+   +-----------------------------+----------------------------------------------+
+   | Function                    | Plot that it creates                         |
+   +=============================+==============================================+
+   | :ref:`bmk-funcs-plot-mvo`   | Modeled ozone vs. surface observations       |
+   +-----------------------------+----------------------------------------------+
+   | :ref:`bmk-funcs-plot-mvs`   | Vertical profiles of modeled ozone vs.       |
+   |                             | ozonesondes                                  |
+   +-----------------------------+----------------------------------------------+
 
 The functions listed above create comparison plots of most GEOS-Chem
 output variables divided into specific categories, e.g. species
 categories such as :literal:`Aerosols` or :literal:`Bromine` for the
 :literal:`SpeciesConcVV` diagnostic. In eachcategory, these function
 create single level PDFs for the surface and 500hPa and zonal
 mean PDFs for the entire atmosphere and only the stratosphere (defined
@@ -361,14 +399,16 @@
 dataset will be considered to be NaN and will be plotted as such.
 
 .. _bmk-funcs-plot-aod:
 
 make_benchmark_aod_plots
 ------------------------
 
+**Located in module:** :file:`gcpy.benchmark.modules.benchmark_funcs`
+
 This function creates column optical depth plots using the Aerosols
 diagnostic output.
 
 .. code-block:: python
 
    def make_benchmark_aod_plots(
            ref,
@@ -459,16 +499,18 @@
        """
 
 .. _bmk-funcs-plot-conc:
 
 make_benchmark_conc_plots
 -------------------------
 
-This function creates species concentration plots using the
-SpeciesConc diagnostic output by default.  In particular:
+**Located in module:** :file:`gcpy.benchmark.modules.benchmark_funcs`
+
+Generates species concentration plots using the :literal:`SpeciesConc`
+diagnostic output by default.  In particular:
 
 - This function is the only benchmark plotting function that supports
   diff-of-diffs plotting, in which 4 datasets are passed and the
   differences between two groups of :literal:`Ref` datasets vs. two
   groups of :literal:`Dev` datasets is plotted (typically used for
   comparing changes in GCHP vs. changes in GEOS-Chem Classic across
   model versions). |br|
@@ -622,20 +664,111 @@
                Directory of species_datbase.yml file
                Default value: Directory of GCPy code repository
            time_mean : bool
                Determines if we should average the datasets over time
                Default value: False
        """
 
+.. _bmk-funcs-plot-dryd:
+
+make_benchmark_drydep_plots
+---------------------------
+
+**Located in module:** :file:`gcpy.benchmark.modules.benchmark_drydep`
+
+Generates plots of dry deposition velocities using the GEOS-Chem
+:literal:`DryDep` diagnostic output.
+
+.. code-block:: python
+
+   def make_benchmark_drydep_plots(
+           ref,
+           refstr,
+           dev,
+           devstr,
+           collection="DryDep",
+           dst="./benchmark",
+           subdst=None,
+           cmpres=None,
+           overwrite=False,
+           verbose=False,
+           log_color_scale=False,
+           weightsdir=".",
+           sigdiff_files=None,
+           n_job=-1,
+           time_mean=False,
+           varlist=None,
+           spcdb_dir=os.path.join(os.path.dirname(__file__), "..", "..")
+   ):
+       """
+       Creates six-panel comparison plots (PDF format) from GEOS-Chem
+       benchmark simualtion output.  Can be used with data collections
+       that do not require special handling (e.g. concentrations).
+
+       Args:
+           ref: str
+               Path name for the "Ref" (aka "Reference") data set.
+           refstr: str
+               A string to describe ref (e.g. version number)
+           dev: str
+               Path name for the "Dev" (aka "Development") data set.
+               This data set will be compared against the "Reference"
+               data set.
+           devstr: str
+               A string to describe dev (e.g. version number)
+
+       Keyword Args (optional):
+           collection : str
+               Name of the diagnostic collection (e.g. "DryDep")
+           dst: str
+               A string denoting the destination folder where a PDF
+               file containing plots will be written.
+               Default value: ./benchmark
+           subdst: str
+               A string denoting the sub-directory of dst where PDF
+               files containing plots will be written.  In practice,
+               subdst is only needed for the 1-year benchmark output,
+               and denotes a date string (such as "Jan2016") that
+               corresponds to the month that is being plotted.
+               Default value: None
+           benchmark_type: str
+               A string denoting the type of benchmark output to plot, options are
+               FullChemBenchmark, TransportTracersBenchmark, or CH4Benchmark.
+               Default value: "FullChemBenchmark"
+           overwrite: bool
+               Set this flag to True to overwrite files in the
+               destination folder (specified by the dst argument).
+               Default value: False.
+           verbose: bool
+               Set this flag to True to print extra informational output.
+               Default value: False.
+           n_job: int
+               Defines the number of simultaneous workers for parallel plotting.
+               Set to 1 to disable parallel plotting. Value of -1 allows the
+               application to decide.
+               Default value: -1
+           spcdb_dir: str
+               Directory of species_datbase.yml file
+               Default value: Directory of GCPy code repository
+           time_mean : bool
+               Determines if we should average the datasets over time
+               Default value: False
+           varlist: list of str
+               List of variables to plot.  If varlist is None, then
+               all common variables in Ref & Dev will be plotted.
+       """
+
 .. _bmk-funcs-plot-emis:
 
 make_benchmark_emis_plots
 -------------------------
 
-This function generates plots of total emissions using output from
+**Located in module:** :file:`gcpy.benchmark.modules.benchmark_funcs`
+
+Generates plots of total emissions using output from
 :file:`HEMCO_diagnostics.*` (for GEOS-Chem Classic) and/or
 :file:`GCHP.Emissions.*` output files.
 
 .. code-block:: python
 
    def make_benchmark_emis_plots(
            ref,
@@ -759,16 +892,18 @@
    """
 
 .. _bmk-funcs-plot-jvalue:
 
 make_benchmark_jvalue_plots
 ---------------------------
 
-This function generates plots of J-values using the :literal:`JValues`
-GEOS-Chem output files.
+**Located in module:** :file:`gcpy.benchmark.modules.benchmark_funcs`
+
+Generates plots of J-values using the GEOS-Chem :literal:`JValues`
+diagnostic output.
 
 .. code-block:: python
 
    def make_benchmark_jvalue_plots(
            ref,
            refstr,
            dev,
@@ -896,21 +1031,22 @@
        """
 
 .. _bmk-funcs-plot-wetdep:
 
 make_benchmark_wetdep_plots
 ---------------------------
 
-This function generates plots of wet deposition using
-:literal:`WetLossConv` and :literal:`WetLossLS` GEOS-Chem output files.
+**Located in module:** :file:`gcpy.benchmark.modules.benchmark_funcs`
+
+Generates plots of wet deposition using the GEOS-Chem
+:literal:`WetLossConv` and :literal:`WetLossLS` diagnostic outputs.
 It is currently primarily used for 1-Year Transport Tracer benchmarks,
 plotting values for the following species as defined in
 `benchmark_categories.yml
-<https://github.com/geoschem/gcpy/blob/dev/gcpy/benchmark_categories.yml>`_
-(included in GCPY).
+<https://github.com/geoschem/gcpy/blob/dev/gcpy/benchmark/modules/benchmark_categories.yml>`_
 
 .. code-block:: python
 
    def make_benchmark_wetdep_plots(
            ref,
            refstr,
            dev,
@@ -997,58 +1133,217 @@
                Directory of species_datbase.yml file
                Default value: Directory of GCPy code repository
            time_mean : bool
                Determines if we should average the datasets over time
                Default value: False
        """
 
+.. _bmk-funcs-plot-mvo:
+
+make_benchmark_model_vs_obs_plots
+---------------------------------
+
+**Located in module:** :file:`gcpy.benchmark.modules.benchmark_models_vs_obs`
+
+Gnerates plots of monthly-averaged modeled surface
+ozone concentrations (using the GEOS-Chem :literal:`SpeciesConc`
+diagnostic outputs) vs. the `EBAS 2019 <https://ebas-data.nilu.no/>`_
+observations.
+
+.. note::
+
+   Model vs. observation plots are only available in 1-year
+   full-chemistry benchmarks.
+
+.. code-block:: python
+
+   def make_benchmark_models_vs_obs_plots(
+           obs_filepaths,
+           obs_label,
+           ref_filepaths,
+           ref_label,
+           dev_filepaths,
+           dev_label,
+           varname="SpeciesConcVV_O3",
+           dst="./benchmark",
+           verbose=False,
+           overwrite=False
+   ):
+       """
+       Driver routine to create model vs. observation plots.
+
+       Args:
+       obs_filepaths : str|list : Path(s) to the observational data.
+       obs_label     : str      : Label for the observational data
+       ref_filepaths : str      : Paths to the Ref model data
+       ref_label     : str      : Label for the Ref model data
+       dev_filepaths : str      : Paths to the Dev model data
+       dev_label     : str      : Label for the Dev model data
+       varname       : str      : Variable name for model data
+       dst           : str      : Destination folder for plots
+       verbose       : bool     : Toggles verbose output on/off
+       overwrite     : bool     : Toggles overwriting contents of dst
+
+.. _bmk-funcs-plot-mvs:
+
+make_benchmark_model_vs_sondes_plots
+------------------------------------
+
+**Located in module:** :file:`gcpy.benchmark.modules.benchmark_models_vs_sondes`
+
+.. note::
+
+   Model vs. ozonesonde plots are only available in 1-year
+   full-chemistry benchmarks.
+
+Generates vertical profiles of modeled ozone concentrations (using the
+GEOS-Chem :literal:`SpeciesConc` diagnostic outputs) vs. ozonesonde
+observations.
+
+.. code-block:: python
+
+   def make_benchmark_models_vs_sondes_plots(
+           obs_data_file,
+           obs_site_file,
+           ref_filepaths,
+           ref_label,
+           dev_filepaths,
+           dev_label,
+           dst="./benchmark",
+           overwrite=False,
+           varname="SpeciesConcVV_O3",
+
+       ):
+       """
+       Creates plots of sonde data vs. GEOS-Chem output.  For use in the
+       1-year benchmark plotting workflow.
+
+       Args
+       obs_data_file : str      : File containing sonde data
+       obs_site_file : str      : File containing sonde site metadata
+       ref_filepaths : str|list : Files for the GEOS-Chem Ref version
+       ref_label     : str      : GEOS-Chem Ref version label
+       dev_filepaths : str|list : Files for the GEOS-Chem Dev version
+       dev_label     : str      : GEOS-Chem Dev version label
+
+       Keyword Args
+       dst           : str      : Folder where PDF w/ plots will be created
+       overwrite     : bool     : Overwrite contents of dst folder?
+       varname       : str      : GEOS-Chem diagnostic variable name
+       verbose       : bool     : Activate verbose printout?
+       """
+
 .. _bmk-funcs-table:
 
 ===========================
 Benchmark tabling functions
 ===========================
 
-.. table:: **Functions creating summary tables from benchmark
-           simulation output**
+.. table:: **Functions creating summary tables**
+   :align: center
 
-   +-----------------------------------------------+----------------------------------------------+
-   | Function                                      | Type of summary table created                |
-   +===============================================+==============================================+
-   | ``make_benchmark_aerosol_tables()``           | Global aerosol burdens (1yr benchmarks only) |
-   +-----------------------------------------------+----------------------------------------------+
-   | ``make_benchmark_emis_tables()``              | Emissions (by species & inventory)           |
-   +-----------------------------------------------+----------------------------------------------+
-   | ``make_benchmark_mass_tables()``              | Total mass of each species                   |
-   +-----------------------------------------------+----------------------------------------------+
-   | ``make_benchmark_mass_accumulation_tables()`` | Mass accumulation for each species           |
-   +-----------------------------------------------+----------------------------------------------+
-   | ``make_benchmark_mass_conservation_table()``  | Total mass of a single species at hourly     |
-   |                                               | intervals (to check mass conservation)       |
-   +-----------------------------------------------+----------------------------------------------+
-   | ``make_benchmark_oh_metrics()``               | Global OH metrics (mean OH, CH4 lifetime,    |
-   |                                               | methylchloroform lifetime)                   |
-   +-----------------------------------------------+----------------------------------------------+
-   | ``make_benchmark_operations_budget()``        | Total mass of each species after each        |
-   |                                               | operation (transport, mixing, etc.)          |
-   +-----------------------------------------------+----------------------------------------------+
+   +--------------------------------------+------------------------------------------------+
+   | Function                             | Table that it creates                          |
+   +======================================+================================================+
+   | :ref:`bmk-funcs-table-oxbdg`         | Ox budget (1yr benchmarks only)                |
+   +--------------------------------------+------------------------------------------------+
+   | :ref:`bmk-funcs-table-aer`           | Global aerosol burdens (1yr benchmarks only)   |
+   +--------------------------------------+------------------------------------------------+
+   | :ref:`bmk-funcs-table-emis`          | Emissions (by species & inventory)             |
+   +--------------------------------------+------------------------------------------------+
+   | :ref:`bmk-funcs-table-gcc-timers`    | GEOS-Chem Classic timers output                |
+   +--------------------------------------+------------------------------------------------+
+   | :ref:`bmk-funcs-table-gchp-timers`   | GCHP timers output                             |
+   +--------------------------------------+------------------------------------------------+
+   | :ref:`bmk-funcs-table-mass`          | Total mass of each species                     |
+   +--------------------------------------+------------------------------------------------+
+   | :ref:`bmk-funcs-table-accum`         | Mass accumulation for each species             |
+   +--------------------------------------+------------------------------------------------+
+   | :ref:`bmk-funcs-table-cons`          | Timeseries of the PassiveTracer species        |
+   +--------------------------------------+------------------------------------------------+
+   | :ref:`bmk-funcs-table-oh`            | Global OH metrics                              |
+   +--------------------------------------+------------------------------------------------+
+   | :ref:`bmk-funcs-table-ops`           | Species mass after each operation              |
+   +--------------------------------------+------------------------------------------------+
+   | :ref:`bmk-funcs-table-ttbdg`         | Rn222, Pb210, Be7 budgets (1yr benchmarks only |
+   +--------------------------------------+------------------------------------------------+
 
 The functions listed above create summary tables for quantities such as
 total mass of species, total mass of emissions, and OH metrics.
 
 Many of these functions use pre-defined lists of variables in YAML
 files. If one dataset includes a variable but the other dataset does
 not, the data for that variable in the latter dataset will be
 considered to be NaN and will be plotted as such.
 
+.. _bmk-funcs-table-oxbdg:
+
+global_ox_budget
+----------------
+
+**Located in module:** :file:`gcpy.benchmark.modules.budget_ox`
+
+Generates a  budget table for the Ox (odd ozone) family from 1-year
+full-chemistry benchmark output.
+
+.. code-block:: python
+
+   def global_ox_budget(
+           devstr,
+           devdir,
+           devrstdir,
+           year,
+           dst='./1yr_benchmark',
+           overwrite=True,
+           spcdb_dir=None,
+           is_gchp=False,
+           gchp_res="c24",
+           gchp_is_pre_14_0=False
+   ):
+       """
+       Main program to compute Ox budgets
+
+       Arguments:
+           maindir: str
+               Top-level benchmark folder
+           devstr: str
+               Denotes the "Dev" benchmark version.
+           year: int
+               The year of the benchmark simulation (e.g. 2016).
+
+       Keyword Args (optional):
+           dst: str
+               Directory where budget tables will be created.
+               Default value: './1yr_benchmark'
+           overwrite: bool
+               Denotes whether to ovewrite existing budget tables.
+               Default value: True
+           spcdb_dir: str
+               Directory where species_database.yml is stored.
+               Default value: GCPy directory
+           is_gchp: bool
+               Denotes if data is from GCHP (True) or GCC (false).
+               Default value: False
+           gchp_res: str
+               GCHP resolution string (e.g. "c24", "c48", etc.)
+               Default value: None
+           gchp_is_pre_14_0: bool
+               Denotes if the version is prior to GCHP 14.0.0 (True)
+               or not (False).
+               Default value: False
+       """
+
 .. _bmk-funcs-table-aer:
 
 make_benchmark_aerosol_tables
 -----------------------------
 
-This function creates tables of global aerosol budgets and burdens from GEOS-Chem
+**Located in module:** :file:`gcpy.benchmark.modules.benchmark_funcs`
+
+Generates a table of global aerosol budgets and burdens from GEOS-Chem
 1-year full-chemistry benchmark simulation output.
 
 .. code-block:: python
 
    def make_benchmark_aerosol_tables(
            devdir,
            devlist_aero,
@@ -1098,16 +1393,18 @@
        """
 
 .. _bmk-funcs-table-emis:
 
 make_benchmark_emis_tables
 --------------------------
 
-This function creates tables of emissions (by species and by
-inventory) from the output of GEOS-Chem benchmark simulations.
+**Located in module:** :file:`gcpy.benchmark.modules.benchmark_funcs`
+
+Generates tables of emissions (by species and by inventory) from the
+the :literal:`HEMCO_diagnostics*` outputs.
 
 .. code-block:: python
 
    def make_benchmark_emis_tables(
            reflist,
            refstr,
            devlist,
@@ -1170,21 +1467,98 @@
                Default value: [2678400.0]
            spcdb_dir: str
                Directory of species_datbase.yml file
                Default value: Directory of GCPy code repository
 
        """
 
+.. _bmk-funcs-table-gcc-timers:
+
+make_benchmark_gcclassic_timing_table
+-------------------------------------
+
+**Located in module:**
+:file:`gcpy.benchmark.modules.benchmark_scrape_gcclassic_timers`
+
+Generates a comparison table of GEOS-Chem Classic timer values.  This
+can be used to determine if computational bottlenecks have been
+introduced.
+
+.. code-block:: python
+
+   def make_benchmark_gcclassic_timing_table(
+           ref_files,
+           ref_label,
+           dev_files,
+           dev_label,
+           dst="./benchmark",
+           overwrite=False,
+   ):
+       """
+       Creates a table of timing information for GEOS-Chem Classic
+       benchmark simulations given one or more JSON and/or text files
+       as input.
+
+       Args
+       ref_files : str|list : File(s) with timing info from the "Ref" model
+       ref_label : str      : Version string for the "Ref" model
+       dev_files : str|list : File(s) with timing info from the "Ref" model
+       dev_label : str      : Version string for the "Dev" model
+
+       Kwargs
+       dst       : str      : Directory where output will be written
+       overwrite : bool     : Overwrite existing files? (default: False)
+       """
+
+.. _bmk-funcs-table-gchp-timers:
+
+make_benchmark_gchp_timing_table
+--------------------------------
+
+**Located in module:**
+:file:`gcpy.benchmark.modules.benchmark_scrape_gchp_timers`
+
+Generates a comparison table of GCHP Classic timer values.  This
+can be used to determine if computational bottlenecks have been
+introduced.
+
+.. code-block:: python
+
+   def make_benchmark_gchp_timing_table(
+           ref_files,
+           ref_label,
+           dev_files,
+           dev_label,
+           dst="./benchmark",
+           overwrite=False,
+   ):
+       """
+       Creates a table of timing information for GCHP benchmark
+       simulations given one or more text files as input.
+
+       Args
+       ref_files : str|list : File(s) with timing info from the "Ref" model
+       ref_label : str      : Version string for the "Ref" model
+       dev_files : str|list : File(s) with timing info from the "Ref" model
+       dev_label : str      : Version string for the "Dev" model
+
+       Kwargs
+       dst       : str      : Directory where output will be written
+       overwrite : bool     : Overwrite existing files? (default: False)
+       """
+
 .. _bmk-funcs-table-mass:
 
 make_benchmark_mass_tables
 --------------------------
 
-This function creates tables of total mass for species in two
-different GEOS-Chem benchmark simulations.
+**Located in module:** :file:`gcpy.benchmark.modules.benchmark_funcs`
+
+Generates a comparison table of total mass for each GEOS-Chem species,
+using the GEOS-Chem restart file output.
 
 .. code-block:: python
 
    def make_benchmark_mass_tables(
            ref,
            refstr,
            dev,
@@ -1256,16 +1630,19 @@
        """
 
 .. _bmk-funcs-table-accum:
 
 make_benchmark_mass_accumulation_tables
 ---------------------------------------
 
-This function creates tables of mass accumulation over time for species in two
-different GEOS-Chem benchmark simulations.
+**Located in module:** :file:`gcpy.benchmark.modules.benchmark_funcs`
+
+Generates a comparison table of mass accumulation (i.e. mass difference
+between the start and end of Ref and Dev benchmark simulations), using
+GEOS-Chem restart files.
 
 .. code-block:: python
 
    def create_mass_accumulation_table(
            refdatastart,
            refdataend,
            refstr,
@@ -1337,23 +1714,25 @@
            This method is mainly intended for model benchmarking purposes,
            rather than as a general-purpose tool.
 
            Species properties (such as molecular weights) are read from a
            YAML file called "species_database.yml".
        """
 
-
 .. _bmk-funcs-table-cons:
 
 make_benchmark_mass_conservation_table
 --------------------------------------
 
-This function creates a timeseries table of the global mass of the
+**Located in module:** :file:`gcpy.benchmark.modules.benchmark_mass_cons_table`
+
+Generates a timeseries table of the global mass of the
 :literal:`PassiveTracer` species.  Usually used with output from
-1-year TransportTracers benchmark simulations.
+1-year TransportTracers benchmark simulations.  This is an important
+check for mass conservation in GEOS-Chem Classic and GCHP.
 
 .. code-block:: python
 
    def make_benchmark_mass_conservation_table(
            datafiles,
            runstr,
            dst="./benchmark",
@@ -1398,16 +1777,19 @@
        """
 
 .. _bmk-funcs-table-oh:
 
 make_benchmark_oh_metrics
 -------------------------
 
-This function generates a table of OH metrics from GEOS-Chem benchmark
-simulation output.
+**Located in module:** :file:`gcpy.benchmark.modules.oh_metrics`
+
+Generates a table of OH metrics (mean OH concentration,
+methyl chloroform lifetime, CH4 lifetime) from the GEOS-Chem
+:literal:`Metrics` diagnostic outputs.
 
 .. code-block:: python
 
    def make_benchmark_oh_metrics(
            ref,
            refmet,
            refstr,
@@ -1448,16 +1830,19 @@
        """
 
 .. _bmk-funcs-table-ops:
 
 make_benchmark_operations_budget
 --------------------------------
 
+**Located in module:** :file:`gcpy.benchmark.module.benchmark_funcs`
+
 Creates a table with the change in species mass after each GEOS-Chem
-operation, using output from GEOS-Chem benchmark simulations.
+operation, using diagnostic output from GEOS-Chem benchmark
+simulations.
 
 .. code-block:: python
 
    def make_benchmark_operations_budget(
            refstr,
            reffiles,
            devstr,
@@ -1546,8 +1931,111 @@
                Denotes whether to overwrite existing budget file.
                Default value: True
            verbose: bool
                Set this switch to True if you wish to print out extra
                informational messages.
                Default value: False
        """
-    ""
+
+.. _bmk-funcs-table-ste:
+
+make_benchmark_ste_table
+------------------------
+
+**Located in module:** :file:`gcpy.benchmark.modules.ste_flux`
+
+Generates a table with the stratosphere-troposphere flux of ozone from
+GEOS-Chem benchmark simulation output.
+
+.. note::
+
+   This table is only available for GEOS-Chem Classic benchmarks.
+
+.. code-block:: python
+
+   def make_benchmark_ste_table(devstr, files, year,
+                                dst='./1yr_benchmark',
+                                bmk_type="FullChemBenchmark",
+                                species=["O3"],
+                                overwrite=True,
+                                month=None):
+       """
+       Driver program.  Computes and prints strat-trop exchange for
+       the selected species and benchmark year.
+
+       Args:
+           devstr: str
+               Label denoting the "Dev" version.
+           files: str
+               List of files containing vertical fluxes.
+           year: str
+               Year of the benchmark simulation.
+
+       Keyword Args (optional):
+           dst: str
+               Directory where plots & tables will be created.
+           bmk_type: str
+               FullChemBenchmark or TransportTracersBenchmark.
+           species: list of str
+               Species for which STE fluxes are desired.
+           overwrite: bool
+               Denotes whether to ovewrite existing budget tables.
+           month: float
+               If passed, specifies the month of a 1-month benchmark.
+               Default: None (denotes a 1-year benchmark)
+       """
+
+.. _bmk-funcs-table-ttbdg:
+
+transport_tracers_budgets
+-------------------------
+
+**Located in module:** :file:`gcpy.benchmark.modules.budget_tt`
+
+Generates a budget table for Rn222, Pb210, and Be7 species from 1-year
+TransportTracers benchmark output.
+
+.. code-block:: python
+
+   def transport_tracers_budgets(
+           devstr,
+           devdir,
+           devrstdir,
+           year,
+           dst='./1yr_benchmark',
+           is_gchp=False,
+           gchp_res="c00",
+           gchp_is_pre_14_0=False,
+           overwrite=True,
+           spcdb_dir=os.path.dirname(__file__)):
+       """
+       Main program to compute TransportTracersBenchmark budgets
+
+       Args:
+           maindir: str
+               Top-level benchmark folder
+           devstr: str
+               Denotes the "Dev" benchmark version.
+           year: int
+               The year of the benchmark simulation (e.g. 2016).
+
+       Keyword Args (optional):
+           dst: str
+               Directory where budget tables will be created.
+               Default value: './1yr_benchmark'
+           is_gchp: bool
+               Denotes if data is from GCHP (True) or GCC (false).
+               Default value: False
+           gchp_res: str
+               A string (e.g. "c24") denoting GCHP grid resolution.
+               Default value: "c00".
+           gchp_is_pre_14_0: bool
+               Logical to indicate whether or not the GCHP data is prior
+               to GCHP 14.0.0.  Needed for restart files only.
+               Default value: False
+           overwrite: bool
+               Denotes whether to ovewrite existing budget tables.
+               Default value: True
+           spcdb_dir: str
+               Directory where species_database.yml is stored.
+               Default value: GCPy directory
+       """
```

### Comparing `geoschem-gcpy-1.4.2/docs/source/Getting-Started-with-GCPy.rst` & `geoschem_gcpy-1.5.0/docs/source/Getting-Started-with-GCPy.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,84 @@
 .. |br| raw:: html
 
    <br/>
 
-.. _install:
-
 ###############
 Installing GCPy
 ###############
 
-.. _requirements:
+.. _install:
 
 ============
 Requirements
 ============
 
 :program:`GCPy` is currently supported on the following platforms:
 
 #. Linux (x86_64)
 #. Windows Subsystem for Linux (running in Microsoft Windows 11)
 #. MacOS
 
-To install GCPy, you will need:
+You may choose one of the following methods to install GCPy on your
+system.
+
+.. _install-pip:
+
+=================================
+For most users: Install from PyPi
+=================================
+
+If you only plan on using GCPy for visualization of GEOS-Chem
+simulation results, we recommend that you install GCPy from the
+:program:`Python
+Package Index (PyPi)` using the `Pip installer
+<https://pypi.org/project/pip/>`_.
+
+If your system does not already have Pip installed, you may install it
+with the `get-pip.py
+<https://pip.pypa.io/en/stable/installation/#get-pip-py>`_ script.
+
+.. _install-pip-first:
+
+First-time installation with Pip
+--------------------------------
+
+Once you are sure that Pip is installed, you may proceed to download
+GCPy with this command:
+
+.. code-block:: console
+
+   $ pip install geoschem-gcpy
+
+To validate the installation, we recommend running the
+:ref:`test-plot` example scruot,
+
+.. _install-pip-update:
+
+Updating to a newer version with Pip
+------------------------------------
+
+Use this command to update an existing GCPy installation to a newer version:
+
+.. code-block:: console
+
+   $ pip install -U geoschem-gcpy
+
+
+You may now skip ahead to the :ref:`mpl-backend` chapter.
+
+.. _install-dev:
+
+=====================================
+For developers: Install GCPy from Git
+=====================================
+
+If you plan on actively developing GCPy, we recommend that you install
+GCPy from Git and create a :program:`Mamba` or :program:`Conda`
+environment.  You will also need:
 
 - **EITHER** a distribution of the :program:`Mamba` package manager
 - **OR** a distribution of the :program:`Conda` package manager.
 
 :program:`Mamba` is a fast drop-in replacement for the
 widely-used :program:`Conda` package manager.  We recommend using
 :program:`Mamba` to create a Python environment for GCPy.  This
@@ -35,15 +89,15 @@
 
    If your system has an existing :program:`Conda` installation, and/or
    you do not wish to upgrade from :program:`Conda` to
    :program:`Mamba`, you may create the Python environment for GCPy
    with :program:`Conda`.  See the following sections for detailed
    instructions.
 
-.. _requirements-mamba:
+.. _install-dev-req-mamba:
 
 Check if Mamba is installed
 ---------------------------
 
 Check if you already have :program:`Mamba` on your system:
 
 .. code-block:: console
@@ -53,18 +107,18 @@
 If :program:`Mamba` has been installed, you will see output similar to this:
 
 .. code-block:: console
 
    mamba version X.Y.Z
    conda version A.B.C
 
-If you see this output, you may skip ahead to the :ref:`gcpy-install`
+If you see this output, you may skip ahead to the :ref:`install-dev-gcpy-install`
 section.
 
-.. _requirements-conda:
+.. _install-dev-req-conda:
 
 Check if Conda is installed
 ---------------------------
 
 If your system does not have :program:`Mamba` installed, check if
 :program:`Conda` is already present on your system:
 
@@ -77,17 +131,17 @@
 
 .. code-block:: console
 
    conda version A.B.C
 
 If neither :program:`Conda` or :program:`Mamba` are installed, we
 recommend installing the :program:`Mamba` package manager yourself.
-Please proceed to the :ref:`mamba-install` section for instructions.
+Please proceed to the :ref:`install-dev-mamba-install` section for instructions.
 
-.. _requirements-conda-older:
+.. _install-dev-req-conda-older:
 
 Additional setup for older Conda versions
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 If your :program:`Conda` version is earlier than 23.7, you will need
 to do the following additional steps.
 
@@ -102,30 +156,29 @@
 creation considerably.
 
 .. note::
 
    The :program:`Mamba` environment solver is used by default in
    :program:`Conda` 23.7 and later.
 
-You may now skip ahead to the :ref:`gcpy-install` section.
+You may now skip ahead to the :ref:`install-dev-gcpy-install` section.
 
-.. _mamba-install:
+.. _install-dev-mamba-install:
 
-==================
 Install MambaForge
-==================
+------------------
 
 We recommend installing the :program:`MambaForge`, distribution, which
 is a full implementation of :program:`Mamba` (as opposed to the
 minimal :program:`MicroMamba` distribution).
 
 Follow the instructions below to install :program:`MambaForge`:
 
 MacOS
------
+~~~~~
 
 #. Install :program:`MambaForge` with `Homebrew <https://brew.sh/>`_:
 
    .. code-block:: console
 
       $ brew install mambaforge
 
@@ -145,19 +198,19 @@
    Python environments.
 
    |br|
 
 #. Exit your current terminal session and open a new terminal
    session.  This will apply the changes.
 
-You may now skip ahead  to the :ref:`gcpy-install` section.
+You may now skip ahead  to the :ref:`install-dev-gcpy-install` section.
 
 
 Linux and Windows Subsystem for Linux
---------------------------------------
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 #. Download the :program:`MambaForge` installer script from the
    `conda-forge GitHub releases page
    <https://github.com/conda-forge/miniforge/releases>`_:
 
    .. code-block:: console
 
@@ -239,16 +292,17 @@
    path or type a new path and then press :literal:`ENTER`.
 
    .. code-block:: console
 
       :program:`MambaForge` will downlad and install Python software
       packages into the  :file:`pkgs` subfolder of the root
       installation path.  Similarly, when you :ref:`create Python
-      environments <gcpy-install>`, these will be installed to the
-      :file:`envs` subfolder of the root installation path.
+      environments <install-dev-gcpy-install>`, these will be
+      installed to the :file:`envs` subfolder of the root installation
+      path.
 
    |br|
 
 #. You may see this warning:
 
    .. code-block:: console
 
@@ -258,15 +312,15 @@
        For best results, please verify that your PYTHONPATH only points to
        directories of packages that are compatible with the Python interpreter
        in Mambaforge: /home/YOUR-USER-NAMEb/mambaforge
 
    As long as your :envvar:`PYTHONPATH` environment variable only
    contains the path to the root-level GCPy folder, you may safely
    ignore this.  (More on :envvar:`PYTHONPATH` in the :ref:`next
-   section <gcpy-install>`.) |br|
+   section <install-dev-gcpy-install>`.) |br|
    |br|
 
 #. Tell the installer to initialize :program:`MambaForge`.
 
    .. code-block:: console
 
       Do you wish the installer to initialize Mambaforge
@@ -279,19 +333,18 @@
    environments. |br|
    |br|
 
 
 #. Exit your current terminal session.  Start a new terminal session
    to apply the updates.  You are now ready to install GCPy.
 
-.. _gcpy-install:
+.. _install-dev-gcpy-install:
 
-=================================
 Install GCPy and its dependencies
-=================================
+---------------------------------
 
 Once you have made sure that :program:`Mamba` (or :program:`Conda`) is
 present on your system, you may create a Python environment for GCPy.
 Follow these steps:
 
 #. **Download the GCPy source code.**
 
@@ -401,32 +454,32 @@
       $ source ~/.bashrc
 
    to apply the change. |br|
    |br|
 
 #. **Perform a simple test:**
 
-   Run the following commands in your terminal to check if the
-   installation was succcesful.
+   Make sure that you have specified the proper :ref:`mpl-backend` for
+   your system.  Then run the following commands in your terminal:
 
    .. code-block:: console
 
-      $ source $HOME/.bashrc     # Alternatively close and reopen your terminal
-      $ echo $PYTHONPATH         # Check it contains path to your GCPy clone
+      $ source $HOME/.bashrc                      # Alternatively close and reopen your terminal
+      $ echo $PYTHONPATH                          # Check it contains path to your GCPy clone
       $ mamba activate gcpy_env
-      $ mamba list               # Check it contains contents of gcpy env file
-      $ python
-      >>> import gcpy
+      $ mamba list                                # Check it contains contents of gcpy env file
+      $ python -m gcpy.examples.create_test_plot  # Create a test plot
+
+If the plot appears on your screen, then the GCPy installation was successful.
 
 If no error messages are displayed, you have successfully installed
 GCPy and its dependencies.
 
-=======================
 Upgrading GCPy versions
-=======================
+-----------------------
 
 Sometimes the GCPy dependency list changes with a new GCPy version,
 either through the addition of new packages or a change in the minimum
 version. You can always update to the latest GCPy version from within
 you GCPy clone, and then update your virtual environment using the
 environment.yml file included in the package.
```

### Comparing `geoschem-gcpy-1.4.2/docs/source/Guide-to-Useful-Capabilities.rst` & `geoschem_gcpy-1.5.0/docs/source/Guide-to-Useful-Capabilities.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+.. |br| raw:: html
+
+   <br/>
+
 .. _capabilities:
 
 ########################
 Overview of Capabilities
 ########################
 
-This page outlines the capabilities of GCPy with links to detailed
-function documentation.
+This page outlines the capabilities of :program:`GCPy` with links to
+detailed function documentation.
 
 .. _capabilities-spatial:
 
 ================
 Spatial plotting
 ================
 
@@ -134,25 +138,26 @@
 for :code:`compare_single_level()` and :code:`compare_zonal_mean()`.
 
 .. _capabilities-spatial-benchmark:
 
 Comprehensive benchmark plotting
 --------------------------------
 
-The GEOS-Chem Support Team uses comprehensive plotting functions from
-module :file:`gcpy.benchmark_funcs` to generate full plots of benchmark
-diagnostics. Functions like
-:ref:`gcpy.benchmark_funcs.make_benchmark_conc_plots()
-<bmk-funcs-plot-conc>` by default create plots for every variable
-in a given collection (e.g. :literal:`SpeciesConc`) at multiple
-vertical levels (surface, 500hPa, zonal mean) and divide plots into
-separate folders based on category (e.g. Chlorine, Aerosols). The
-GEOS-Chem Support Team uses benchmark plotting and tabling table
-scripts (described in our :ref:`Benchmarking <bmk>` chapter) to
-produce plots and tables for official model benchmarks.
+The `GEOS-Chem Support Team
+<https://geoschem.github.io/support-team>`_ uses comprehensive
+plotting functions (stored in modules located in the
+:file:`gcpy/benchmark/modules` folder) to generate plots and tables
+from of diagnostic output of GEOS-Chem benchmark
+simulations. Functions like :ref:`bmk-funcs-plot-conc` generate plots
+for every variable in  a given collection
+(e.g. :literal:`SpeciesConc`) at multiple vertical levels (surface,
+500hPa, zonal mean) and divide plots into separate folders based on
+category (e.g. Chlorine, Aerosols). For more information about the
+benchmark plotting and tabling scripts, please see our
+:ref:`Benchmarking <bmk>` chapter.
 
 .. _capabilities-table:
 
 ==============
 Table creation
 ==============
 
@@ -167,50 +172,55 @@
 
 Currently, budget tables can be created for "operations" (table shows
 change in mass after each category of model operation, as contained in
 the GEOS-Chem :literal:`Budget` diagnostics) or in overall averages for
 different aerosols or the Transport Tracers simulation.
 
 Operations budget tables are created using the
-:ref:`gcpy.benchmark_funcs.make_benchmark_operations_budget()
-<bmk-funcs-table-ops>` function and appear as follows:
+:ref:`bmk-funcs-table-ops` function and appear as follows:
 
 .. image:: _static/images/budget\_table.png
    :align: center
 
+|br|
+
 .. _capabilities-tables-mass:
 
 Mass tables
 -----------
 
-The :ref:`gcpy.benchmark_funcs.make_benchmark_mass_tables()
-<bmk-funcs-table-mass>` function uses species concentrations and info
-from meteorology files to generate the total mass of species in
-certain segments of the atmosphere (currently global or only the
+The :ref:`bmk-funcs-table-mass` function uses species concentrations
+and info from meteorology files to generate the total mass of species
+in certain segments of the atmosphere (currently global or only the
 troposphere). An example table is shown below:
 
 .. image:: _static/images/mass\_table.png
    :align: center
 
+|br|
+
 .. _capabilities-tables-emissions:
 
 Emissions tables
 ----------------
 
-The :ref:`gcpy.benchmark_funcs.make_benchmark_emis_tables()
-<bmk-funcs-table-emis>` function creates tables of total emissions
-categorized by species or by inventory. Examples of both emissions
-table types are shown below:
+The :ref:`bmk-funcs-table-emis` function creates tables of total
+emissions categorized by species or by inventory. Examples of both
+emissions table types are shown below:
 
 .. image:: _static/images/emissions\_totals.png
    :align: center
 
+|br|
+
 .. image:: _static/images/inventory\_totals.png
    :align: center
 
+|br|
+
 .. _capabilities-regridding:
 
 ==========
 Regridding
 ==========
 
 .. _capabilities-regridding-rules:
@@ -237,16 +247,16 @@
 
 The 72-level and 47-level vertical grids are pre-defined in
 GCPy. Other vertical grids can also be defined if you provide `the A
 and B coefficients of the hybrid vertical grid
 <wiki.seas.harvard.edu/geos-chem/index.php/GEOS-Chem_vertical_grids>`__.
 
 When plotting data of differing grid types or horizontal resolutions
-using :ref:`compare_single_level() <plot-csl-and-czm>`
-or :ref:`compare_zonal_mean() <plot-csl-and-czm>`, you
+using :ref:`compare_single_level <plot-csl>`
+or :ref:`compare_zonal_mean <plot-czm>`, you
 can specify a comparison resolution using the :literal:`cmpres`
 argument. This resolution will be used for the difference panels in
 each plot (the bottom four panels rather than the top two raw data
 panels). If you do not specify a comparison resolution, GCPy will
 automatically choose one.
 
 For more extensive regridding information, visit the :ref:`detailed
```

### Comparing `geoschem-gcpy-1.4.2/docs/source/Plotting.rst` & `geoschem_gcpy-1.5.0/docs/source/Plotting.rst`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 ==========================
 Six-panel comparison plots
 ==========================
 
 The functions listed below generate six-panel plots comparing
 variables between two datasets:
 
-+-----------------------------+------------------------------------+
-| Plotting function           | Located in GCPy module             |
-+=============================+====================================+
-| ``compare_single_level()``  | ``gcpy.plot.compare_single_level`` |
-+-----------------------------+------------------------------------+
-| ``compare_zonal_mean()``    | ``gcpy.plot.compare_zonal_mean``   |
-+-----------------------------+------------------------------------+
++----------------------------------------+------------------------------------+
+| Plotting function                      | Located in module                  |
++========================================+====================================+
+| :ref:`compare_single_level <plot-csl>` | ``gcpy.plot.compare_single_level`` |
++----------------------------------------+------------------------------------+
+| :ref:`compare_zonal_mean <plot-czm>`   | ``gcpy.plot.compare_zonal_mean``   |
++----------------------------------------+------------------------------------+
 
 Both :code:`compare_single_level()` and :code:`compare_zonal_mean()`
 generate a six panel plot for each variable passed. These plots can
 either be saved to PDFs or generated sequentially for visualization in
 the Matplotlib GUI using :code:`matplotlib.pyplot.show()`.
 Each plot uses data passed from a reference (:literal:`Ref`) dataset
 and a development (:literal:`Dev`) dataset.  Both functions share
@@ -229,15 +229,14 @@
                or imshow() (Lat/Lon).
    """
 
 and generates a comparison plot such as:
 
 .. image:: _static/images/six\_panel\_single\_level.png
    :align: center
-   :width: 80%
 
 .. _plot-czm:
 
 Function :code:`compare_zonal_mean`
 -----------------------------------
 
 .. code-block:: python
@@ -407,15 +406,14 @@
                (CS) or imshow() (Lat/Lon).
        """
 
 and generates a comparison plot such as:
 
 .. image:: _static/images/six\_panel\_zonal\_mean.png
    :align: center
-   :width: 80%
 
 .. _plot-shared:
 
 Shared structure
 ----------------
 
 Both :code:`compare_single_level()` and :code:`compare_zonal_mean()`
```

### Comparing `geoschem-gcpy-1.4.2/docs/source/Regridding.rst` & `geoschem_gcpy-1.5.0/docs/source/Regridding.rst`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
    :literal:`ESMF_RegridWeightGen`.
 #. Run the regridding operation using the :code:`regrid_restart_file`
    submodule of GCPy.
 
 .. note::
 
    As of GCPy 1.4.0, the :ref:`default GCPy environment
-   <gcpy_install>` (aka :literal:`gcpy_env`) now contains
+   <install>` (aka :literal:`gcpy_env`) now contains
    :literal:`gridspec` and :literal:`sparselt` packages.  You no
    longer need to use the separate :literal:`gchp_regridding`
    environment as in prior versions.
 
 .. _regrid-gchp-args:
 
 gcpy.regrid_restart_file required arguments:
```

### Comparing `geoschem-gcpy-1.4.2/docs/source/Single_panel.rst` & `geoschem_gcpy-1.5.0/gcpy/examples/plotting/plot_single_panel.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,123 +1,183 @@
-.. _single-panel:
+#!/usr/bin/env python
+"""
+Global and Regional Single Panel Plots
+--------------------------------------
+This example script demonstrates the core single panel plotting
+capabilities of GCPy, including global and regional single level plots
+as well as global zonal mean plots.
 
-This example script may also be found at `gcpy/examples/plotting/plot_single_panel.py <https://github.com/geoschem/gcpy/blob/feature/plot-subdir/gcpy/examples/plotting/plot_single_panel.py>`_.
+The example data described here is in lat/lon format, but the same code
+works equally well for cubed-sphere (GCHP) data.
 
-#####################
-Single Panel Plotting
-#####################
-
-.. code-block:: python
-
-   #!/usr/bin/env python
-   """
-   Global and Regional Single Panel Plots
-   --------------------------------------
-   This example script demonstrates the core single panel plotting
-   capabilities of GCPy, including global and regional single level plots
-   as well as global zonal mean plots.
-   
-   The example data described here is in lat/lon format, but the same code
-   works equally well for cubed-sphere (GCHP) data.
-   
-   For full documentation on the plotting capabilities of GCPy
-   (including full argument lists), please see the GCPy documentation
-   at https://gcpy.readthedocs.io.
-   """
-   import xarray as xr
-   import matplotlib.pyplot as plt
-   from gcpy.plot.single_panel import single_panel
-   
-   
-   def main():
-       """
-       Example routine to create single panel plots.
-       """
-   
-       # xarray allows us to read in any NetCDF file, the format of
-       # GEOS-Chem diagnostics as an xarray Dataset
-       dset = xr.open_dataset('GEOSChem.Restart.20160701_0000z.nc4')
-   
-       # You can easily view the variables available for plotting
-       # using xarray.  Each of these variables has its own xarray
-       # DataArray within the larger Dataset container.
-       print(dset.data_vars)
-   
-       # Most variables have some sort of prefix; in this example all
-       # variables are prefixed with 'SpeciesRst_'. We'll select the
-       # DataArray for ozone.
-       darr = dset.SpeciesRst_O3
-   
-       # Printing a DataArray gives a summary of the dimensions and attributes
-       # of the data.
-       print(darr)
-   
-       # This Restart file has a time dimension of size 1, with 72 vertical levels,
-       #46 latitude indicies, and 72 longitude indices.
-   
-   
-       # ==================
-       # Single-level Plots
-       # ==================
-   
-       # gcpy.single_panel is the core plotting function of GCPy, able to
-       # create a one panel zonal mean or single level plot.  Here we will
-       # create a single level plot of ozone at ~500 hPa.  We must manually
-       # index into the level that we want to plot (index 22 in the standard
-       # 72-layer and 47-layer GMAO vertical grids).
-       slice_500 = darr.isel(lev=22)
-   
-       # single_panel has many arguments which can be optionally specified.
-       # The only argument you must always pass to a call to single_panel is
-       # the DataArray that you want to plot. By default, the created plot
-       # includes a colorbar with units read from the DataArray, an
-       # automatic title (the data variable name in the DataArray), and
-       # an extent equivalent to the full lat/lon extent of the DataArray
-       single_panel(slice_500)
-       plt.show()
-   
-       #You can specify a specific area of the globe you would like plotted
-       # using the 'extent' argument, which uses the format [min_longitude,
-       # max_longitude, min_latitude, max_latitude] with bounds
-       # [-180, 180, -90, 90]
-       single_panel(slice_500, extent=[50, -90, -10, 60])
-       plt.show()
-   
-       # Other commonly used arguments include specifying a title and a
-       # colormap (defaulting to a White-Green-Yellow-Red colormap)
-       #You can find more colormaps at
-       # https://matplotlib.org/tutorials/colors/colormaps.html
-       single_panel(
-           slice_500,
-           title='500mb Ozone over the North Pacific',
-           comap=plt.get_cmap("viridis"),
-           log_color_scale=True,
-           extent=[80, -90, -10, 60]
-       )
-       plt.show()
-   
-       # ===================
-       # Zonal Mean Plotting
-       # ===================
-   
-       # Use the plot_type argument to specify zonal_mean plotting
-       single_panel(
-           darr,
-           plot_type="zonal_mean"
-       )
-       plt.show()
-   
-       #You can specify pressure ranges in hPa for zonal mean plot
-       # (by default every vertical level is plotted)
-       single_panel(
-           darr,
-           pres_range=[0, 100],
-           log_yaxis=True,
-           log_color_scale=True
-       )
-       plt.show()
-   
-   
-   
-   # Only execute when we run as a standalone script
-   if __name__ == '__main__':
-       main()
+For full documentation on the plotting capabilities of GCPy
+(including full argument lists), please see the GCPy documentation
+at https://gcpy.readthedocs.io.
+
+NOTE: If you are using GCPy from a Mac, set the environment variable:
+
+   export MPLBACKEND="MacOSX"
+
+Otherwise set:
+
+   export MPLBACKEND="tkagg"
+
+This will set the proper X11 backend (which is needed to open a plot
+window on the screen.  There is some incompatibility with the Tck/Tk
+backend "tkagg" in MacOS X operating systems.
+"""
+import argparse
+import xarray as xr
+import matplotlib.pyplot as plt
+from gcpy.plot.single_panel import single_panel
+from gcpy.util import rename_and_flip_gchp_rst_vars
+
+
+def plot_single_panel(infile, varname, level):
+    """
+    Example routine to create single panel plots.
+
+    Args:
+    -----
+    infile  (str) : Name of netCDF file to read.
+    varname (str) : Name of variable to plot
+    level   (int) : Model level for single-panel plots
+                    in Python notation (starting from 0)
+    """
+
+    # xarray allows us to read in any NetCDF file
+    dset = xr.open_dataset(infile)
+
+    # If the data is from a GCHP restart file, rename variables and
+    # flip levels to match the GEOS-Chem Classic naming and level
+    # conventions.  Otherwise no changes will be made.
+    dset = rename_and_flip_gchp_rst_vars(dset)
+
+    # You can easily view the variables available for plotting
+    # using xarray.  Each of these variables has its own xarray
+    # DataArray within the larger Dataset container.
+    print(dset.data_vars)
+
+    # Most variables have some sort of prefix; in this example all
+    # variables are prefixed with 'SpeciesRst_'. We'll select the
+    # DataArray for ozone.
+    darr = dset[varname]
+
+    # Printing a DataArray gives a summary of the dimensions and attributes
+    # of the data.
+    print(darr)
+
+    # ==================
+    # Single-level Plots
+    # ==================
+
+    # gcpy.single_panel is the core plotting function of GCPy, able to
+    # create a one panel zonal mean or single level plot.  Here we will
+    # create a single level plot. We must manually index into the level
+    # (in Python notation, starting from 0).
+    darr_single_level = darr.isel(lev=level)
+
+    # single_panel has many arguments which can be optionally specified.
+    # The only argument you must always pass to a call to single_panel is
+    # the DataArray that you want to plot. By default, the created plot
+    # includes a colorbar with units read from the DataArray, an
+    # automatic title (the data variable name in the DataArray), and
+    # an extent equivalent to the full lat/lon extent of the DataArray
+    single_panel(
+        darr_single_level,
+        title=f"{varname} at level {level}"
+    )
+    plt.show()
+
+    # You can specify a specific area of the globe you would like plotted
+    # using the 'extent' argument, which uses the format [min_longitude,
+    # max_longitude, min_latitude, max_latitude] with bounds
+    # [-180, 180, -90, 90]
+    single_panel(
+        darr_single_level,
+        extent=[50, -90, -10, 60],
+        title=f"{varname} at level {level} over N. Pacific"
+    )
+    plt.show()
+
+    # Other commonly used arguments include specifying a title and a
+    # colormap (defaulting to a White-Green-Yellow-Red colormap)
+    #You can find more colormaps at
+    # https://matplotlib.org/tutorials/colors/colormaps.html
+    single_panel(
+        darr_single_level,
+        title=f"{varname} at level {level} over N. Pacific, viridis colormap",
+        comap=plt.get_cmap("viridis"),
+        log_color_scale=True,
+        extent=[80, -90, -10, 60]
+    )
+    plt.show()
+
+    # ===================
+    # Zonal Mean Plotting
+    # ===================
+
+    # Use the plot_type argument to specify zonal_mean plotting
+    single_panel(
+        darr,
+        plot_type="zonal_mean",
+        title=f"Zonal mean plot for {varname}, full atmosphere"
+    )
+    plt.show()
+
+    # You can specify pressure ranges in hPa for zonal mean plot
+    # (by default every vertical level is plotted)
+    single_panel(
+        darr,
+        pres_range=[0, 100],
+        log_yaxis=True,
+        log_color_scale=True,
+        plot_type="zonal_mean",
+        title=f"Zonal mean plot for {varname}, stratosphere-only"
+    )
+    plt.show()
+
+
+def main():
+    """
+    Parses command-line arguments and calls plot_single_panel.
+    """
+
+    # Tell the parser which arguments to look for
+    parser = argparse.ArgumentParser(
+        description="Single-panel plotting example program"
+    )
+    parser.add_argument(
+        "-i", "--infile",
+        metavar="INF",
+        type=str,
+        required=True,
+        help="input NetCDF file"
+    )
+    parser.add_argument(
+        "-v", "--varname",
+        metavar="VARNAME",
+        type=str,
+        required=True,
+        help="variable to plot"
+    )
+    parser.add_argument(
+        "-l", "--level",
+        metavar="LEV",
+        type=int,
+        required=True,
+        help="level to plot (single-panel plots only), starting at 0"
+    )
+
+    # Parse command-line arguments
+    args = parser.parse_args()
+
+    # Call the plot_single_panel routine
+    plot_single_panel(
+        args.infile,
+        args.varname,
+        args.level
+    )
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `geoschem-gcpy-1.4.2/docs/source/_static/images/GEOS-Chem_Logo_Light_Background.png` & `geoschem_gcpy-1.5.0/docs/source/_static/images/GEOS-Chem_Logo_Light_Background.png`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/docs/source/_static/images/budget_table.png` & `geoschem_gcpy-1.5.0/docs/source/_static/images/budget_table.png`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/docs/source/_static/images/emissions_totals.png` & `geoschem_gcpy-1.5.0/docs/source/_static/images/emissions_totals.png`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/docs/source/_static/images/inventory_totals.png` & `geoschem_gcpy-1.5.0/docs/source/_static/images/inventory_totals.png`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/docs/source/_static/images/mass_table.png` & `geoschem_gcpy-1.5.0/docs/source/_static/images/mass_table.png`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/docs/source/editing_these_docs.rst` & `geoschem_gcpy-1.5.0/docs/source/editing_these_docs.rst`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/docs/source/plot_timeseries.rst` & `geoschem_gcpy-1.5.0/gcpy/examples/timeseries/plot_timeseries.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,354 +1,344 @@
-.. _plot-timeseries:
+#!/usr/bin/env python
+'''
+Example of plotting timeseries data from GEOS-Chem and saving
+the output to a PDF file.  You can modify this for your particular
+diagnostic output.  This also contains a good overview of
 
-###############
-Plot Timeseries
-###############
+This example script creates a PDF file with 2 pages.
 
-This example script may also be found at `gcpy/examples/plotting/plot_single_panel.py <https://github.com/geoschem/gcpy/blob/feature/plot-subdir/gcpy/examples/timeseries/plot_timeseries.py>`_.
-
-.. code-block:: python
-
-   #!/usr/bin/env python
-   '''
-   Example of plotting timeseries data from GEOS-Chem and saving
-   the output to a PDF file.  You can modify this for your particular
-   diagnostic output.  This also contains a good overview of
-
-   This example script creates a PDF file with 2 pages.
-
-      Page 1:
-      -------
-          O3 from the first model layer (from the "SpeciesConc"
-          diagnostic collection is) plotted in blue.
-
-          O3 at 10 meter height (from the "SpeciesConc_10m"
-          diagnostic collection) is plotted in red.
-
-      Page 2:
-      -------
-          HNO3 from the first model layer (from the SpeciesConc
-          diagnostic collection is) plotted in blue.
-
-          HNO3 at 10 meter height (from the SpeciesConc_10m
-          diagnostic collection) is plotted in red.
-
-   You can of course modify this for your own particular applications.
-
-   Author:
+   Page 1:
    -------
-   Bob Yantosca
-   yantosca@seas.harvard.edu
-   23 Aug 2019
-   '''
-
-   # Imports
-   import os
-   import warnings
-   import numpy as np
-   import matplotlib.dates as mdates
-   import matplotlib.ticker as mticker
-   import matplotlib.pyplot as plt
-   from matplotlib.backends.backend_pdf import PdfPages
-   import xarray as xr
-   from gcpy import constants
-
-
-   # Tell matplotlib not to look for an X-window, as we are plotting to
-   # a file and not to the screen.  This will avoid some warning messages.
-   os.environ['QT_QPA_PLATFORM'] = 'offscreen'
-
-   # Suppress harmless run-time warnings (mostly about underflow in division)
-   warnings.filterwarnings('ignore', category=RuntimeWarning)
-   warnings.filterwarnings('ignore', category=UserWarning)
-
-
-   def find_files_in_dir(path, substrs):
-       '''
-       Returns a list of all files in a directory that match one or more
-       substrings.
-
-       Args:
-       -----
-           path : str
-               Path to the directory in which to search for files.
-
-           substrs : list of str
-               List of substrings used in the search for files.
-
-       Returns:
-       --------
-           file_list : list of str
-               List of files in the directory (specified by path)
-               that match all substrings (specified in substrs).
-       '''
-
-       # Initialize
-       file_list = []
-
-       # Walk through the given data directory.  Then for each file found,
-       # add it to file_list if it matches text in search_list.
-       for root, directory, files in os.walk(path):
-           for f in files:
-               for s in substrs:
-                   if s in f:
-                       file_list.append(os.path.join(root, f))
-
-       # Return an alphabetically sorted list of files
-       file_list.sort()
-       return file_list
-
-
-   def find_value_index(seq, val):
-       '''
-       Finds the index of a numpy array that is close to a value.
-
-       Args:
-       -----
-           seq : numpy ndarray
-               An array of numeric values.
-
-           val : number
-               The value to search for in seq.
-
-       Returns:
-       --------
-           result : integer
-               The index of seq that has a value closest to val.
-
-       Remarks:
-       --------
-       This algorithm was found on this page:
-       https://stackoverflow.com/questions/48900977/find-all-indexes-of-a-numpy-array-closest-to-a-value
-       '''
-       r = np.where(np.diff(np.sign(seq - val)) != 0)
-       idx = r + (val - seq[r]) / (seq[r + np.ones_like(r)] - seq[r])
-       idx = np.append(idx, np.where(seq == val))
-       idx = np.sort(idx)
-       result = np.round(idx)
-
-       # NOTE: xarray needs integer values, so convert here!
-       return int(result[0])
-
-
-   def read_geoschem_data(path, collections):
-       '''
-       Returns an xarray Dataset containing timeseries data.
-
-       Args:
-       -----
-           path : str
-               Directory path where GEOS-Chem diagnostic output
-               files may be found.
-
-           collections: list of str
-               List of GEOS-Chem collections.  Files for these
-               collections will be read into the xarray Dataset.
-
-       Returns:
-       --------
-           ds : xarray Dataset
-               A Dataset object containing the GEOS-Chem diagnostic
-               output corresponding to the collections that were
-               specified.
-       '''
-
-       # Get a list of variables that GCPy should not read.
-       # These are mostly variables introduced into GCHP with the MAPL v1.0.0
-       # update.  These variables contain either repeated or non-standard
-       # dimensions that can cause problems in xarray when combining datasets.
-       skip_vars = constants.skip_these_vars
-
-       # Find all files in the given
-       file_list = find_files_in_dir(path, collections)
-
-       # Return a single xarray Dataset containing data from all files
-       # NOTE: Need to add combine="nested" for xarray 0.15 and higher
-       v = xr.__version__.split(".")
-       if int(v[0]) == 0 and int(v[1]) >= 15:
-           return xr.open_mfdataset(file_list,
-                                    drop_variables=skip_vars,
-                                    combine="nested",
-                                    concat_dim=None)
-       else:
-           return xr.open_mfdataset(file_list,
-                                    drop_variables=skip_vars)
-
-
-   def plot_timeseries_data(ds, site_coords):
-       '''
-       Plots a timseries of data at a given (lat,lon) location.
-
-       Args:
-       -----
-           ds : xarray Dataset
-               Dataset containing GEOS-Chem timeseries data.
-
-           site_coords : tuple
-               Contains the coordinate (lat, lon) of a site location
-               at which the timeseries data will be plotted.
-       '''
-
-       # ----------------------------------------------------------------------
-       # Get the GEOS-Chem data for O3 and HNO3 corresponding to the
-       # location of the observational station.  We will save these into
-       # xarray DataArray objects, which we'll need for plotting.
-       #
-       # YOU CAN EDIT THIS FOR YOUR OWN PARTICULAR APPLICATION!
-       # ----------------------------------------------------------------------
-
-       # Find the indices corresponding to the site lon and lat
-       lat_idx = find_value_index(ds.lat.values, site_coords[0])
-       lon_idx = find_value_index(ds.lon.values, site_coords[1])
-
-       # Save O3 from the first level (~60m height) (ppb) into a DataArray
-       O3_L1 = ds['SpeciesConc_O3'].isel(lon=lon_idx, lat=lat_idx, lev=0)
-       O3_L1 *= 1.0e9
-       O3_L1.attrs['units'] = 'ppbv'
-
-       # Save O3 @ 10m height into a DataArray
-       O3_10m = ds['SpeciesConc10m_O3'].isel(lon=lon_idx, lat=lat_idx)
-       O3_10m *= 1.0e9
-       O3_10m.attrs['units'] = 'ppbv'
-
-       # Save HNO3 from the first level (~60m height) into a DataArray
-       HNO3_L1 = ds['SpeciesConc_HNO3'].isel(lon=lon_idx, lat=lat_idx, lev=0)
-       HNO3_L1 *= 1.0e9
-       HNO3_L1.attrs['units'] = 'ppbv'
-
-       # Save HNO3 @ 10m height into a DataArray
-       HNO3_10m = ds['SpeciesConc10m_HNO3'].isel(lon=lon_idx, lat=lat_idx)
-       HNO3_10m *= 1.0e9
-       HNO3_10m.attrs['units'] = 'ppbv'
-
-       # ----------------------------------------------------------------------
-       # Create a PDF file of the plots
-       # ----------------------------------------------------------------------
-
-       # Get min & max days of the plot span (for setting the X-axis range).
-       # To better center the plot, add a cushion of 12 hours on either end.
-       time = ds['time'].values
-       datemin = np.datetime64(time[0]) - np.timedelta64(12, 'h')
-       datemax = np.datetime64(time[-1]) + np.timedelta64(12, 'h')
-
-       # Define a PDF object so that we can save the plots to PDF
-       pdf = PdfPages('O3_and_HNO3.pdf')
-
-       # Loop over number of desired pages (in this case, 2)
-       for i in range(0, 2):
-
-           # Create a new figure: 1 plot per page, 2x as wide as high
-           figs, ax0 = plt.subplots(1, 1, figsize=[12, 6])
-
-           # -----------------------------
-           # Plot O3 on the first page
-           # -----------------------------
-           if i == 0:
-
-               # 1st model level
-               O3_L1.plot.line(ax=ax0, x='time', color='blue',
-                               marker='o', label='O3 from 1st model level',
-                               linestyle='-')
-
-               # 10 mheight
-               O3_10m.plot.line(ax=ax0, x='time', color='red',
-                                marker='x', label='O3 at 10m height',
-                                linestyle='-')
+       O3 from the first model layer (from the "SpeciesConc"
+       diagnostic collection is) plotted in blue.
 
-               # Set title (has to be after the line plots are drawn)
-               ax0.set_title('O3 from the 1st model level and at 10m height')
+       O3 at 10 meter height (from the "SpeciesConc_10m"
+       diagnostic collection) is plotted in red.
 
-               # Set Y-axis minor tick marks at every 2 ppb (5 intervals)
-               ax0.yaxis.set_minor_locator(mticker.AutoMinorLocator(5))
-
-               # Set y-axis title
-               ax0.set_ylabel('O3 (ppbv)')
+   Page 2:
+   -------
+       HNO3 from the first model layer (from the SpeciesConc
+       diagnostic collection is) plotted in blue.
 
-           # -----------------------------
-           # Plot HNO3 on the second page
-           # -----------------------------
-           if i == 1:
+       HNO3 at 10 meter height (from the SpeciesConc_10m
+       diagnostic collection) is plotted in red.
 
-               # 1st model level
-               HNO3_L1.plot.line(ax=ax0, x='time', color='blue',
-                                 marker='o', label='HNO3 from 1st model level',
-                                 linestyle='-')
+You can of course modify this for your own particular applications.
 
-               # 10m height
-               HNO3_10m.plot.line(ax=ax0, x='time', color='red',
-                                  marker='x', label='HNO3 at 10m height',
-                                  linestyle='-')
+Author:
+-------
+Bob Yantosca
+yantosca@seas.harvard.edu
+23 Aug 2019
+'''
+
+# Imports
+import os
+import warnings
+import numpy as np
+import matplotlib.dates as mdates
+import matplotlib.ticker as mticker
+import matplotlib.pyplot as plt
+from matplotlib.backends.backend_pdf import PdfPages
+import xarray as xr
+from gcpy import constants
+
+
+# Tell matplotlib not to look for an X-window, as we are plotting to
+# a file and not to the screen.  This will avoid some warning messages.
+os.environ['QT_QPA_PLATFORM'] = 'offscreen'
+
+# Suppress harmless run-time warnings (mostly about underflow in division)
+warnings.filterwarnings('ignore', category=RuntimeWarning)
+warnings.filterwarnings('ignore', category=UserWarning)
+
+
+def find_files_in_dir(path, substrs):
+    '''
+    Returns a list of all files in a directory that match one or more
+    substrings.
+
+    Args:
+    -----
+        path : str
+            Path to the directory in which to search for files.
+
+        substrs : list of str
+            List of substrings used in the search for files.
+
+    Returns:
+    --------
+        file_list : list of str
+            List of files in the directory (specified by path)
+            that match all substrings (specified in substrs).
+    '''
+
+    # Initialize
+    file_list = []
+
+    # Walk through the given data directory.  Then for each file found,
+    # add it to file_list if it matches text in search_list.
+    for root, directory, files in os.walk(path):
+        for f in files:
+            for s in substrs:
+                if s in f:
+                    file_list.append(os.path.join(root, f))
+
+    # Return an alphabetically sorted list of files
+    file_list.sort()
+    return file_list
+
+
+def find_value_index(seq, val):
+    '''
+    Finds the index of a numpy array that is close to a value.
+
+    Args:
+    -----
+        seq : numpy ndarray
+            An array of numeric values.
+
+        val : number
+            The value to search for in seq.
+
+    Returns:
+    --------
+        result : integer
+            The index of seq that has a value closest to val.
+
+    Remarks:
+    --------
+    This algorithm was found on this page:
+    https://stackoverflow.com/questions/48900977/find-all-indexes-of-a-numpy-array-closest-to-a-value
+    '''
+    r = np.where(np.diff(np.sign(seq - val)) != 0)
+    idx = r + (val - seq[r]) / (seq[r + np.ones_like(r)] - seq[r])
+    idx = np.append(idx, np.where(seq == val))
+    idx = np.sort(idx)
+    result = np.round(idx)
+
+    # NOTE: xarray needs integer values, so convert here!
+    return int(result[0])
+
+
+def read_geoschem_data(path, collections):
+    '''
+    Returns an xarray Dataset containing timeseries data.
+
+    Args:
+    -----
+        path : str
+            Directory path where GEOS-Chem diagnostic output
+            files may be found.
+
+        collections: list of str
+            List of GEOS-Chem collections.  Files for these
+            collections will be read into the xarray Dataset.
+
+    Returns:
+    --------
+        ds : xarray Dataset
+            A Dataset object containing the GEOS-Chem diagnostic
+            output corresponding to the collections that were
+            specified.
+    '''
+
+    # Get a list of variables that GCPy should not read.
+    # These are mostly variables introduced into GCHP with the MAPL v1.0.0
+    # update.  These variables contain either repeated or non-standard
+    # dimensions that can cause problems in xarray when combining datasets.
+    skip_vars = constants.skip_these_vars
+
+    # Find all files in the given
+    file_list = find_files_in_dir(path, collections)
+
+    # Return a single xarray Dataset containing data from all files
+    # NOTE: Need to add combine="nested" for xarray 0.15 and higher
+    v = xr.__version__.split(".")
+    if int(v[0]) == 0 and int(v[1]) >= 15:
+        return xr.open_mfdataset(file_list,
+                                 drop_variables=skip_vars,
+                                 combine="nested",
+                                 concat_dim=None)
+    else:
+        return xr.open_mfdataset(file_list,
+                                 drop_variables=skip_vars)
+
+
+def plot_timeseries_data(ds, site_coords):
+    '''
+    Plots a timseries of data at a given (lat,lon) location.
+
+    Args:
+    -----
+        ds : xarray Dataset
+            Dataset containing GEOS-Chem timeseries data.
+
+        site_coords : tuple
+            Contains the coordinate (lat, lon) of a site location
+            at which the timeseries data will be plotted.
+    '''
+
+    # ----------------------------------------------------------------------
+    # Get the GEOS-Chem data for O3 and HNO3 corresponding to the
+    # location of the observational station.  We will save these into
+    # xarray DataArray objects, which we'll need for plotting.
+    #
+    # YOU CAN EDIT THIS FOR YOUR OWN PARTICULAR APPLICATION!
+    # ----------------------------------------------------------------------
+
+    # Find the indices corresponding to the site lon and lat
+    lat_idx = find_value_index(ds.lat.values, site_coords[0])
+    lon_idx = find_value_index(ds.lon.values, site_coords[1])
+
+    # Save O3 from the first level (~60m height) (ppb) into a DataArray
+    O3_L1 = ds['SpeciesConc_O3'].isel(lon=lon_idx, lat=lat_idx, lev=0)
+    O3_L1 *= 1.0e9
+    O3_L1.attrs['units'] = 'ppbv'
+
+    # Save O3 @ 10m height into a DataArray
+    O3_10m = ds['SpeciesConc10m_O3'].isel(lon=lon_idx, lat=lat_idx)
+    O3_10m *= 1.0e9
+    O3_10m.attrs['units'] = 'ppbv'
+
+    # Save HNO3 from the first level (~60m height) into a DataArray
+    HNO3_L1 = ds['SpeciesConc_HNO3'].isel(lon=lon_idx, lat=lat_idx, lev=0)
+    HNO3_L1 *= 1.0e9
+    HNO3_L1.attrs['units'] = 'ppbv'
+
+    # Save HNO3 @ 10m height into a DataArray
+    HNO3_10m = ds['SpeciesConc10m_HNO3'].isel(lon=lon_idx, lat=lat_idx)
+    HNO3_10m *= 1.0e9
+    HNO3_10m.attrs['units'] = 'ppbv'
+
+    # ----------------------------------------------------------------------
+    # Create a PDF file of the plots
+    # ----------------------------------------------------------------------
+
+    # Get min & max days of the plot span (for setting the X-axis range).
+    # To better center the plot, add a cushion of 12 hours on either end.
+    time = ds['time'].values
+    datemin = np.datetime64(time[0]) - np.timedelta64(12, 'h')
+    datemax = np.datetime64(time[-1]) + np.timedelta64(12, 'h')
+
+    # Define a PDF object so that we can save the plots to PDF
+    pdf = PdfPages('O3_and_HNO3.pdf')
+
+    # Loop over number of desired pages (in this case, 2)
+    for i in range(0, 2):
+
+        # Create a new figure: 1 plot per page, 2x as wide as high
+        figs, ax0 = plt.subplots(1, 1, figsize=[12, 6])
+
+        # -----------------------------
+        # Plot O3 on the first page
+        # -----------------------------
+        if i == 0:
+
+            # 1st model level
+            O3_L1.plot.line(ax=ax0, x='time', color='blue',
+                            marker='o', label='O3 from 1st model level',
+                            linestyle='-')
+
+            # 10 mheight
+            O3_10m.plot.line(ax=ax0, x='time', color='red',
+                             marker='x', label='O3 at 10m height',
+                             linestyle='-')
+
+            # Set title (has to be after the line plots are drawn)
+            ax0.set_title('O3 from the 1st model level and at 10m height')
+
+            # Set Y-axis minor tick marks at every 2 ppb (5 intervals)
+            ax0.yaxis.set_minor_locator(mticker.AutoMinorLocator(5))
+
+            # Set y-axis title
+            ax0.set_ylabel('O3 (ppbv)')
+
+        # -----------------------------
+        # Plot HNO3 on the second page
+        # -----------------------------
+        if i == 1:
+
+            # 1st model level
+            HNO3_L1.plot.line(ax=ax0, x='time', color='blue',
+                              marker='o', label='HNO3 from 1st model level',
+                              linestyle='-')
+
+            # 10m height
+            HNO3_10m.plot.line(ax=ax0, x='time', color='red',
+                               marker='x', label='HNO3 at 10m height',
+                               linestyle='-')
 
-               # Set title (has to be after the line plots are drawn
-               ax0.set_title('HNO3 from the 1st model level and at 10m height')
+            # Set title (has to be after the line plots are drawn
+            ax0.set_title('HNO3 from the 1st model level and at 10m height')
 
-               # Set Y-axis minor tick marks at every 0.05 ppb (4 intervals)
-               ax0.yaxis.set_minor_locator(mticker.AutoMinorLocator(4))
+            # Set Y-axis minor tick marks at every 0.05 ppb (4 intervals)
+            ax0.yaxis.set_minor_locator(mticker.AutoMinorLocator(4))
 
-               # Set y-axis title
-               ax0.set_ylabel('HNO3 (ppbv)')
+            # Set y-axis title
+            ax0.set_ylabel('HNO3 (ppbv)')
 
-           # -----------------------------
-           # Set general plot parameters
-           # -----------------------------
+        # -----------------------------
+        # Set general plot parameters
+        # -----------------------------
 
-           # Add the plot legend
-           ax0.legend()
+        # Add the plot legend
+        ax0.legend()
 
-           # Set the X-axis range
-           ax0.set_xlim(datemin, datemax)
+        # Set the X-axis range
+        ax0.set_xlim(datemin, datemax)
 
-           # Set the X-axis major tickmarks
-           locator = mdates.DayLocator()
-           formatter = mdates.DateFormatter('%d')
-           ax0.xaxis.set_major_locator(locator)
-           ax0.xaxis.set_major_formatter(formatter)
+        # Set the X-axis major tickmarks
+        locator = mdates.DayLocator()
+        formatter = mdates.DateFormatter('%d')
+        ax0.xaxis.set_major_locator(locator)
+        ax0.xaxis.set_major_formatter(formatter)
 
-           # Set X-axis minor tick marks at noon of each day
-           # (i.e. split up the major interval into 2 bins)
-           ax0.xaxis.set_minor_locator(mticker.AutoMinorLocator(2))
+        # Set X-axis minor tick marks at noon of each day
+        # (i.e. split up the major interval into 2 bins)
+        ax0.xaxis.set_minor_locator(mticker.AutoMinorLocator(2))
 
-           # Don't rotate the X-axis jtick labels
-           ax0.xaxis.set_tick_params(rotation=0)
+        # Don't rotate the X-axis jtick labels
+        ax0.xaxis.set_tick_params(rotation=0)
 
-           # Center the X-axis tick labels
-           for tick in ax0.xaxis.get_major_ticks():
-               tick.label1.set_horizontalalignment('center')
+        # Center the X-axis tick labels
+        for tick in ax0.xaxis.get_major_ticks():
+            tick.label1.set_horizontalalignment('center')
 
-           # Set X-axis and Y-axis labels
-           ax0.set_xlabel('Day of July (and August) 2016')
+        # Set X-axis and Y-axis labels
+        ax0.set_xlabel('Day of July (and August) 2016')
 
-           # -----------------------------
-           # Save this page to PDF
-           # -----------------------------
-           pdf.savefig(figs)
-           plt.close(figs)
+        # -----------------------------
+        # Save this page to PDF
+        # -----------------------------
+        pdf.savefig(figs)
+        plt.close(figs)
 
-       # ----------------------------------------------------------------------
-       # Save the PDF file to disk
-       # ----------------------------------------------------------------------
-       pdf.close()
+    # ----------------------------------------------------------------------
+    # Save the PDF file to disk
+    # ----------------------------------------------------------------------
+    pdf.close()
 
 
-   def main():
-       '''
-       Main program.
-       '''
-       # Path where the data files live
-       # (YOU MUST EDIT THIS FOR YUR OWN PARTICULAR APPLICATION!)
-       path_to_data = '/path/to/GEOS-Chem/diagnostic/data/files'
+def main():
+    '''
+    Main program.
+    '''
+    # Path where the data files live
+    # (YOU MUST EDIT THIS FOR YUR OWN PARTICULAR APPLICATION!)
+    path_to_data = '/path/to/GEOS-Chem/diagnostic/data/files'
 
-       # Get a list of files in the ConcAboveSfc and SpeciesConc collections
-       # (YOU CAN EDIT THIS FOR YOUR OWN PARTICULAR APPLICATION!)
-       collections = ['ConcAboveSfc', 'SpeciesConc']
+    # Get a list of files in the ConcAboveSfc and SpeciesConc collections
+    # (YOU CAN EDIT THIS FOR YOUR OWN PARTICULAR APPLICATION!)
+    collections = ['ConcAboveSfc', 'SpeciesConc']
 
-       # Read GEOS-Chem data into an xarray Dataset
-       ds = read_geoschem_data(path_to_data, collections)
+    # Read GEOS-Chem data into an xarray Dataset
+    ds = read_geoschem_data(path_to_data, collections)
 
-       # Plot timeseries data at Centerville, AL (32.94N, 87.18W)
-       # (YOU CAN EDIT THIS FOR YOUR OWN PARTICULAR APPLICATION!)
-       site_coords = (32.94, -87.18)
-       plot_timeseries_data(ds, site_coords)
+    # Plot timeseries data at Centerville, AL (32.94N, 87.18W)
+    # (YOU CAN EDIT THIS FOR YOUR OWN PARTICULAR APPLICATION!)
+    site_coords = (32.94, -87.18)
+    plot_timeseries_data(ds, site_coords)
 
 
-   if __name__ == "__main__":
-       main()
+if __name__ == "__main__":
+    main()
```

### Comparing `geoschem-gcpy-1.4.2/environment.yml` & `geoschem_gcpy-1.5.0/environment.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,43 @@
 ---
 # ======================================================================
 # GCPy environment file
 #
-# Recommended installation: with Mambaforge
+# If you wish to build a Mamba/Conda environment with the dependencies
+# for GCPy, use this command:
+#
 # $ mamba env create -n gcpy_env --file=/path/to/gcpy/environment.yml
 #
 # These package versions have been proven to work together.
 # See: https://github.com/geoschem/gcpy/issues/284
-# ======================================================================
+# =====================================================================
 name: gcpy_env
 channels:
   - conda-forge
   - nodefaults
 dependencies:
-  - awscli==2.13.39                 # Utilities for AWS cloud
   - cartopy==0.22.0                 # Geospatial data processing
   - cf_xarray==0.8.4                # CF conventions for xarray
   - dask==2023.9.2                  # Parallel library; backend for xarray
   - gridspec==0.1.0                 # Define Earth System Model grids
   - ipython==8.15.0                 # Interactive Python (used by Jupyter)
   - joblib==1.3.2                   # Parallelize python code
   - jupyter==1.0.0                  # Jupyter Notebook
   - matplotlib==3.8.0               # Creates plots and visualizations
   - netcdf4==1.6.0                  # Python wrapper for netCDF
   - netcdf-fortran==4.5.4           # Python wrapper for netCDF-Fortran
   - numpy==1.26.0                   # Optimized mathematical functions
   - pandas==2.1.1                   # Tables/timeseries manipulation
-  - pip==23.2.1                     # Install packages from PyPi
+  - pip==23.3                       # Install packages from PyPi
   - pylint==2.17.5                  # Python linter
   - pyproj==3.6.1                   # Python map projections library
-  - python==3.9.18                  # Any python version prior to 3.10
-  - pypdf==3.16.1                   # PDF utilities (bookmarks, etc.)
-  - recommonmark==0.7.1             # Dependency for Sphinx
+  - python==3.9.18                  # Python language
+  - pypdf==3.17.0                   # PDF utilities (bookmarks, etc.)
   - requests==2.31.0                # HTTP library
   - scipy==1.11.2                   # Scientific python package
   - sparselt==0.1.3                 # Regridding earth system model data
   - tabulate==0.9.0                 # Pretty-printing for column data
   - tk==8.6.12                      # Tcl/tk library
   - xarray==2023.8.0                # Read data from netCDF etc files
   - esmf==8.1.1                     # Earth system modeling framework
   - esmpy==8.1.1                    # Python wrapper for ESMF
   - xesmf==0.5.1                    # Universal regridder
-  - docutils==0.16                  # Convert text to other formats
-  - jinja2==3.0.3                   # Dependency for Sphinx
-  - sphinx==3.5.4                   # Generate ReadTheDocs output
-  - sphinx-autoapi==1.9.0           # Sphinx autodoc style documentation
-  - sphinx-autobuild==2021.3.14     # Build ReadTheDos live in browser
-  - sphinxcontrib-bibtex==2.2.0     # ReadTheDocs bibliography style
-  - sphinx_rtd_theme==0.5.2         # ReadTheDocs HTML theme files
```

### Comparing `geoschem-gcpy-1.4.2/gcpy/append_grid_corners.py` & `geoschem_gcpy-1.5.0/gcpy/append_grid_corners.py`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/benchmark/README.md` & `geoschem_gcpy-1.5.0/gcpy/benchmark/README.md`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/benchmark/benchmark_slurm.sh` & `geoschem_gcpy-1.5.0/gcpy/benchmark/benchmark_slurm.sh`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,14 @@
 # Specify a YAML file with benchmark options
 # Uncomment the file that you wish:
 #config="1mo_benchmark.yml"
 config="1yr_fullchem_benchmark.yml"
 #config="1yr_tt_benchmark.yml"
 
 # Call the run_benchmark script to make the plots
-python -m gcpy.benchmark.run_benchmark "${config}" > benchmark.log 2>&1
+python -m gcpy.benchmark.run_benchmark "${config}" > "${config/.yml/.log}" 2>&1
 
 # Turn off python environment
 mamba deactivate
 
 exit 0
```

### Comparing `geoschem-gcpy-1.4.2/gcpy/benchmark/cloud/template.1hr_benchmark.yml` & `geoschem_gcpy-1.5.0/gcpy/benchmark/cloud/template.1hr_benchmark.yml`

 * *Files 6% similar despite different names*

```diff
@@ -43,38 +43,46 @@
 data:
   ref:
     gcc:
       version: ${GEOSCHEM_BENCHMARK_REF_PRIMARY_KEY}
       dir: ref-gcc/run-directory
       outputs_subdir: OutputDir
       restarts_subdir: Restarts
+      logs_subdir: .
+      logs_template: runlog.txt
       bmk_start: "2019-07-01T00:00:00"
       bmk_end: "2019-07-01T01:00:00"
     gchp:
       version: ${GEOSCHEM_BENCHMARK_REF_PRIMARY_KEY}
       dir: ref-gchp/run-directory
       outputs_subdir: OutputDir
       restarts_subdir: Restarts
+      logs_subdir: .
+      logs_template: runlog.txt
       bmk_start: "2019-07-01T00:00:00"
       bmk_end: "2019-07-01T01:00:00"
       is_pre_14.0: False
       resolution: c24
   dev:
     gcc:
       version: ${GEOSCHEM_BENCHMARK_DEV_PRIMARY_KEY}
       dir: dev-gcc/run-directory
       outputs_subdir: OutputDir
       restarts_subdir: Restarts
+      logs_subdir: .
+      logs_template: runlog.txt
       bmk_start: "2019-07-01T00:00:00"
       bmk_end: "2019-07-01T01:00:00"
     gchp:
       version: ${GEOSCHEM_BENCHMARK_DEV_PRIMARY_KEY}
       dir: dev-gchp/run-directory
       outputs_subdir: OutputDir
       restarts_subdir: Restarts
+      logs_subdir: .
+      logs_template: runlog.txt
       bmk_start: "2019-07-01T00:00:00"
       bmk_end: "2019-07-01T01:00:00"
       is_pre_14.0: False
       resolution: c24
 #
 # options: Customizes the benchmark plot output
 #
@@ -106,20 +114,22 @@
   # outputs: Specifies the plots and tables to generate
   #
   outputs:
     plot_conc: False
     plot_emis: False
     emis_table: True
     plot_jvalues: False
+    plot_drydep: False
     plot_aod: False
     mass_table: True
     mass_accum_table: False
     ops_budget_table: False
     OH_metrics: True
     ste_table: True # GCC only
+    timing_table: True
     summary_table: True
     plot_options:
       by_spc_cat: True
       by_hco_cat: True
   #
   # n_cores: Specify the number of cores to use.
   # -1: Use $OMP_NUM_THREADS         cores
```

### Comparing `geoschem-gcpy-1.4.2/gcpy/benchmark/cloud/template.1mo_benchmark.yml` & `geoschem_gcpy-1.5.0/gcpy/benchmark/cloud/template.1mo_benchmark.yml`

 * *Files 5% similar despite different names*

```diff
@@ -43,38 +43,46 @@
 data:
   ref:
     gcc:
       version: ${GEOSCHEM_BENCHMARK_REF_PRIMARY_KEY}
       dir: ref-gcc/run-directory
       outputs_subdir: OutputDir
       restarts_subdir: Restarts
+      logs_subdir: .
+      logs_template: runlog.txt
       bmk_start: "2019-07-01T00:00:00"
       bmk_end: "2019-08-01T00:00:00"
     gchp:
       version: ${GEOSCHEM_BENCHMARK_REF_PRIMARY_KEY}
       dir: ref-gchp/run-directory
       outputs_subdir: OutputDir
       restarts_subdir: Restarts
+      logs_subdir: .
+      logs_template: runlog.txt
       bmk_start: "2019-07-01T00:00:00"
       bmk_end: "2019-08-01T00:00:00"
       is_pre_14.0: False
       resolution: c24
   dev:
     gcc:
       version: ${GEOSCHEM_BENCHMARK_DEV_PRIMARY_KEY}
       dir: dev-gcc/run-directory
       outputs_subdir: OutputDir
       restarts_subdir: Restarts
+      logs_subdir: .
+      logs_template: runlog.txt
       bmk_start: "2019-07-01T00:00:00"
       bmk_end: "2019-08-01T00:00:00"
     gchp:
       version: ${GEOSCHEM_BENCHMARK_DEV_PRIMARY_KEY}
       dir: dev-gchp/run-directory
       outputs_subdir: OutputDir
       restarts_subdir: Restarts
+      logs_subdir: .
+      logs_template: runlog.txt
       bmk_start: "2019-07-01T00:00:00"
       bmk_end: "2019-08-01T00:00:00"
       is_pre_14.0: False
       resolution: c24
 #
 # options: Customizes the benchmark plot output
 #
@@ -107,19 +115,21 @@
   #
   outputs:
     plot_conc: True
     plot_emis: True
     emis_table: True
     plot_jvalues: True
     plot_aod: True
+    plot_drydep: False #Hotfix (bmy, 06 Feb 2024)
     mass_table: True
     mass_accum_table: False
     ops_budget_table: False
     OH_metrics: True
     ste_table: True # GCC only
+    timing_table: True
     summary_table: True
     plot_options:
       by_spc_cat: True
       by_hco_cat: True
   #
   # n_cores: Specify the number of cores to use.
   # -1: Use $OMP_NUM_THREADS         cores
```

### Comparing `geoschem-gcpy-1.4.2/gcpy/benchmark/config/1mo_benchmark.yml` & `geoschem_gcpy-1.5.0/gcpy/benchmark/config/1mo_benchmark.yml`

 * *Files 6% similar despite different names*

```diff
@@ -43,38 +43,46 @@
 data:
   ref:
     gcc:
       version: GCC_ref
       dir: GCC_ref
       outputs_subdir: OutputDir
       restarts_subdir: Restarts
+      logs_subdir: .
+      logs_template: "GC.log"
       bmk_start: "2019-07-01T00:00:00"
       bmk_end: "2019-08-01T00:00:00"
     gchp:
       version: GCHP_ref
       dir: GCHP_ref
       outputs_subdir: OutputDir
       restarts_subdir: Restarts
+      logs_subdir: .
+      logs_template: "gchp.%Y%m%d_0000z.log"      
       bmk_start: "2019-07-01T00:00:00"
       bmk_end: "2019-08-01T00:00:00"
       is_pre_14.0: False
       resolution: c24
   dev:
     gcc:
       version: GCC_dev 
       dir: GCC_dev
       outputs_subdir: OutputDir
       restarts_subdir: Restarts
+      logs_subdir: .
+      logs_template: "GC.log"      
       bmk_start: "2019-07-01T00:00:00"
       bmk_end: "2019-08-01T00:00:00"
     gchp:
       version: GCHP_dev
       dir: GCHP_dev
       outputs_subdir: OutputDir
       restarts_subdir: Restarts
+      logs_subdir: Logs
+      logs_template: "gchp.%Y%m%d_0000z.log"
       bmk_start: "2019-07-01T00:00:00"
       bmk_end: "2019-08-01T00:00:00"
       is_pre_14.0: False
       resolution: c24
 #
 # options: Customizes the benchmark plot output
 #
@@ -107,19 +115,21 @@
   #
   outputs:
     plot_conc: True
     plot_emis: True
     emis_table: True
     plot_jvalues: True
     plot_aod: True
+    plot_drydep: False  # Need to save out DryDep collection for 1-mo
     mass_table: True
     mass_accum_table: False
     ops_budget_table: False
     OH_metrics: True
     ste_table: True # GCC only
+    timing_table: True
     summary_table: True
     plot_options:
       by_spc_cat: True
       by_hco_cat: True
   #
   # n_cores: Specify the number of cores to use.
   # -1: Use $OMP_NUM_THREADS         cores
```

### Comparing `geoschem-gcpy-1.4.2/gcpy/benchmark/config/1yr_ch4_benchmark.yml` & `geoschem_gcpy-1.5.0/gcpy/benchmark/config/1yr_tt_benchmark.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-&---
+
+---
 # =====================================================================
 # Benchmark configuration file (**EDIT AS NEEDED**)
 # customize in the following manner:
 #
 # (1) Edit the path variables so that they point to folders
 #     containing model data
 # (2) Edit the version strings for each benchmark simulation
@@ -11,27 +12,27 @@
 # (4) If necessary, edit labels for the dev and ref versions
 #
 # Note: When doing GCHP vs GCC comparisions gchp_dev will be compared
 # to gcc_dev (not gcc_ref!). This ensures consistency in version names
 # when doing GCHP vs GCC diff-of-diffs.
 # =====================================================================
 #
-# Configuration for 1-year CH4Benchmark
+# Configuration for 1-year TransportTracersBenchmark
 #
 # paths:
 #   main_dir:    High-level directory containing ref & dev rundirs
 #   results_dir: Directory where plots/tables will be created
 #   weights_dir: Path to regridding weights
 #   spcdb_dir:   Folder in which the species_database.yml file is
 #                located.  If set to "default", then will look for
 #                species_database.yml in one of the Dev rundirs.
 #
 paths:
-  main_dir: /path/to/benchmark/main/dir    # EDIT AS NEEDED
-  results_dir: /path/to/BenchmarkResults   # EDIT AS NEEDED
+  main_dir: /path/to/benchmark/main/dir
+  results_dir: /path/to/BenchmarkResults
   weights_dir: /n/holyscratch01/external_repos/GEOS-CHEM/gcgrid/data/ExtData/GCHP/RegriddingWeights
   spcdb_dir: default
 #
 # data: Contains configurations for ref and dev runs
 #   version:         Version string (must not contain spaces)
 #   dir:             Path to run directory
 #   outputs_subdir:  Subdirectory w/ GEOS-Chem diagnostic files
@@ -43,50 +44,58 @@
 data:
   ref:
     gcc:
       version: GCC_ref
       dir: GCC_ref
       outputs_subdir: OutputDir
       restarts_subdir: Restarts
+      logs_subdir: Logs
+      logs_template: "log.%Y%m%d"
       bmk_start: "2019-01-01T00:00:00"
       bmk_end: "2020-01-01T00:00:00"
     gchp:
       version: GCHP_ref
       dir: GCHP_ref
       outputs_subdir: OutputDir
       restarts_subdir: Restarts
+      logs_subdir: Logs
+      logs_template: "gchp.%Y%m%d_0000z.log"
       bmk_start: "2019-01-01T00:00:00"
       bmk_end: "2020-01-01T00:00:00"
       is_pre_14.0: False
       resolution: c24
   dev:
     gcc:
       version: GCC_dev 
       dir: GCC_dev
       outputs_subdir: OutputDir
       restarts_subdir: Restarts
+      logs_subdir: Logs
+      logs_template: "log.%Y%m%d"
       bmk_start: "2019-01-01T00:00:00"
       bmk_end: "2020-01-01T00:00:00"
     gchp:
       version: GCHP_dev
       dir: GCHP_dev
       outputs_subdir: OutputDir
       restarts_subdir: Restarts
+      logs_subdir: Logs
+      logs_template: "gchp.%Y%m%d_0000z.log"
       bmk_start: "2019-01-01T00:00:00"
       bmk_end: "2020-01-01T00:00:00"
       is_pre_14.0: False
       resolution: c24
 #
 # options: Customizes the benchmark plot output
 #
 options:
   #
   # bmk_type: Specifies the type of benchmark
   #
-  bmk_type: CH4Benchmark
+  bmk_type: TransportTracersBenchmark
   #
   # comparisons: Specifies the comparisons to perform.
   #
   comparisons:
     gcc_vs_gcc:
       run: True
       dir: GCC_version_comparison
@@ -103,27 +112,22 @@
       run: False
       dir: GCHP_GCC_diff_of_diffs
   #
   # outputs: Specifies the plots and tables to generate
   #
   outputs:
     plot_conc: True
-    plot_emis: True
-    emis_table: True
-    plot_jvalues: False
-    plot_aod: False
-    mass_table: True
+    plot_wetdep: True
+    plot_drydep: True
+    rnpbbe_budget: True
     ops_budget_table: False
-    aer_budget_table: False
-    Ox_budget_table: False
-    ste_table: False
-    OH_metrics: True
-    plot_options:
-      by_spc_cat: True
-      by_hco_cat: True
+    mass_table: True
+    ste_table: True
+    cons_table: True
+    timing_table: False
   #
   # n_cores: Specify the number of cores to use.
   # -1: Use $OMP_NUM_THREADS         cores
   # -2: Use $OMP_NUM_THREADS - 1     cores
   # -N: Use $OMP_NUM_THREADS - (N-1) cores
   #  1: Disable parallelization (use a single core)
   #
```

### Comparing `geoschem-gcpy-1.4.2/gcpy/benchmark/config/1yr_fullchem_benchmark.yml` & `geoschem_gcpy-1.5.0/gcpy/benchmark/config/1yr_ch4_benchmark.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
----
+&---
 # =====================================================================
 # Benchmark configuration file (**EDIT AS NEEDED**)
 # customize in the following manner:
 #
 # (1) Edit the path variables so that they point to folders
 #     containing model data
 # (2) Edit the version strings for each benchmark simulation
@@ -11,31 +11,40 @@
 # (4) If necessary, edit labels for the dev and ref versions
 #
 # Note: When doing GCHP vs GCC comparisions gchp_dev will be compared
 # to gcc_dev (not gcc_ref!). This ensures consistency in version names
 # when doing GCHP vs GCC diff-of-diffs.
 # =====================================================================
 #
-# Configuration for 1-year FullChemBenchmark
+# Configuration for 1-year CH4Benchmark
 #
 # paths:
-#   main_dir:     High-level directory containing ref & dev rundirs
-#   results_dir:  Directory where plots/tables will be created
-#   weights_dir:  Path to regridding weights
-#   spcdb_dir:    Folder in which the species_database.yml file is
-#                  located.  If set to "default", then will look for
-#                  species_database.yml in one of the Dev rundirs.
-#   obs_data_dir: Path to observational data (for models vs obs plots)
+#   main_dir:    High-level directory containing ref & dev rundirs
+#   results_dir: Directory where plots/tables will be created
+#   weights_dir: Path to regridding weights
+#   spcdb_dir:   Folder in which the species_database.yml file is
+#                located.  If set to "default", then will look for
+#                species_database.yml in one of the Dev rundirs.
 #
 paths:
-  main_dir: /path/to/benchmark/main/dir
-  results_dir: /path/to/BenchmarkResults
+  main_dir: /path/to/benchmark/main/dir    # EDIT AS NEEDED
+  results_dir: /path/to/BenchmarkResults   # EDIT AS NEEDED
   weights_dir: /n/holyscratch01/external_repos/GEOS-CHEM/gcgrid/data/ExtData/GCHP/RegriddingWeights
   spcdb_dir: default
-  obs_data_dir: /path/to/observational/data
+  #
+  # Observational data dirs are on Harvard Cannon, edit if necessary
+  #
+  obs_data:
+    ebas_o3:
+      data_dir: /n/jacob_lab/Lab/obs_data_for_bmk/ebas_sfc_o3_2019
+      data_label: "O3 (EBAS, 2019)"
+    sondes:
+      data_dir: /n/jacob_lab/Lab/obs_data_for_bmk/sondes_2010-2019
+      data_file: allozonesondes_2010-2019.csv
+      site_file: allozonesondes_site_elev.csv
 #
 # data: Contains configurations for ref and dev runs
 #   version:         Version string (must not contain spaces)
 #   dir:             Path to run directory
 #   outputs_subdir:  Subdirectory w/ GEOS-Chem diagnostic files
 #   restarts_subdir: Subdirectory w/ GEOS-Chem restarts
 #   bmk_start:       Simulation start date (YYYY-MM-DDThh:mm:ss)
@@ -80,15 +89,15 @@
 #
 # options: Customizes the benchmark plot output
 #
 options:
   #
   # bmk_type: Specifies the type of benchmark
   #
-  bmk_type: FullChemBenchmark
+  bmk_type: CH4Benchmark
   #
   # comparisons: Specifies the comparisons to perform.
   #
   comparisons:
     gcc_vs_gcc:
       run: True
       dir: GCC_version_comparison
@@ -98,32 +107,32 @@
       dir: GCHP_GCC_comparison
       tables_subdir: Tables
     gchp_vs_gchp:
       run: True
       dir: GCHP_version_comparison
       tables_subdir: Tables
     gchp_vs_gcc_diff_of_diffs:
-      run: True
+      run: False
       dir: GCHP_GCC_diff_of_diffs
   #
   # outputs: Specifies the plots and tables to generate
   #
   outputs:
     plot_conc: True
     plot_emis: True
     emis_table: True
-    plot_jvalues: True
-    plot_aod: True
+    plot_jvalues: False
+    plot_aod: False
+    plot_drydep: False
     mass_table: True
     ops_budget_table: False
-    aer_budget_table: True
-    Ox_budget_table: True
-    ste_table: True # GCC only
+    aer_budget_table: False
+    Ox_budget_table: False
+    ste_table: False
     OH_metrics: True
-    plot_models_vs_obs: True
     plot_options:
       by_spc_cat: True
       by_hco_cat: True
   #
   # n_cores: Specify the number of cores to use.
   # -1: Use $OMP_NUM_THREADS         cores
   # -2: Use $OMP_NUM_THREADS - 1     cores
```

### Comparing `geoschem-gcpy-1.4.2/gcpy/benchmark/config/1yr_tt_benchmark.yml` & `geoschem_gcpy-1.5.0/gcpy/benchmark/config/1yr_fullchem_benchmark.yml`

 * *Files 19% similar despite different names*

```diff
@@ -11,29 +11,41 @@
 # (4) If necessary, edit labels for the dev and ref versions
 #
 # Note: When doing GCHP vs GCC comparisions gchp_dev will be compared
 # to gcc_dev (not gcc_ref!). This ensures consistency in version names
 # when doing GCHP vs GCC diff-of-diffs.
 # =====================================================================
 #
-# Configuration for 1-year TransportTracersBenchmark
+# Configuration for 1-year FullChemBenchmark
 #
 # paths:
-#   main_dir:    High-level directory containing ref & dev rundirs
-#   results_dir: Directory where plots/tables will be created
-#   weights_dir: Path to regridding weights
-#   spcdb_dir:   Folder in which the species_database.yml file is
-#                located.  If set to "default", then will look for
-#                species_database.yml in one of the Dev rundirs.
+#   main_dir:     High-level directory containing ref & dev rundirs
+#   results_dir:  Directory where plots/tables will be created
+#   weights_dir:  Path to regridding weights
+#   spcdb_dir:    Folder in which the species_database.yml file is
+#                  located.  If set to "default", then will look for
+#                  species_database.yml in one of the Dev rundirs.
+#   obs_data:     Paths to observations (for models vs. obs plots)
 #
 paths:
   main_dir: /path/to/benchmark/main/dir
   results_dir: /path/to/BenchmarkResults
   weights_dir: /n/holyscratch01/external_repos/GEOS-CHEM/gcgrid/data/ExtData/GCHP/RegriddingWeights
   spcdb_dir: default
+  #
+  # Observational data dirs are on Harvard Cannon, edit if necessary
+  #
+  obs_data:
+    ebas_o3:
+      data_dir: /n/jacob_lab/Lab/obs_data_for_bmk/ebas_sfc_o3_2019
+      data_label: "O3 (EBAS, 2019)"
+    sondes:
+      data_dir: /n/jacob_lab/Lab/obs_data_for_bmk/sondes_2010-2019
+      data_file: allozonesondes_2010-2019.csv
+      site_file: allozonesondes_site_elev.csv
 #
 # data: Contains configurations for ref and dev runs
 #   version:         Version string (must not contain spaces)
 #   dir:             Path to run directory
 #   outputs_subdir:  Subdirectory w/ GEOS-Chem diagnostic files
 #   restarts_subdir: Subdirectory w/ GEOS-Chem restarts
 #   bmk_start:       Simulation start date (YYYY-MM-DDThh:mm:ss)
@@ -43,50 +55,58 @@
 data:
   ref:
     gcc:
       version: GCC_ref
       dir: GCC_ref
       outputs_subdir: OutputDir
       restarts_subdir: Restarts
+      logs_subdir: Logs
+      logs_template: "log.%Y%m%d"
       bmk_start: "2019-01-01T00:00:00"
       bmk_end: "2020-01-01T00:00:00"
     gchp:
       version: GCHP_ref
       dir: GCHP_ref
       outputs_subdir: OutputDir
       restarts_subdir: Restarts
+      logs_subdir: Logs
+      logs_template: "gchp.%Y%m%d_0000z.log"
       bmk_start: "2019-01-01T00:00:00"
       bmk_end: "2020-01-01T00:00:00"
       is_pre_14.0: False
       resolution: c24
   dev:
     gcc:
       version: GCC_dev 
       dir: GCC_dev
       outputs_subdir: OutputDir
       restarts_subdir: Restarts
+      logs_subdir: Logs
+      logs_template: "log.%Y%m%d"
       bmk_start: "2019-01-01T00:00:00"
       bmk_end: "2020-01-01T00:00:00"
     gchp:
       version: GCHP_dev
       dir: GCHP_dev
       outputs_subdir: OutputDir
       restarts_subdir: Restarts
+      logs_subdir: Logs
+      logs_template: "gchp.%Y%m%d_0000z.log"
       bmk_start: "2019-01-01T00:00:00"
       bmk_end: "2020-01-01T00:00:00"
       is_pre_14.0: False
       resolution: c24
 #
 # options: Customizes the benchmark plot output
 #
 options:
   #
   # bmk_type: Specifies the type of benchmark
   #
-  bmk_type: TransportTracersBenchmark
+  bmk_type: FullChemBenchmark
   #
   # comparisons: Specifies the comparisons to perform.
   #
   comparisons:
     gcc_vs_gcc:
       run: True
       dir: GCC_version_comparison
@@ -96,27 +116,37 @@
       dir: GCHP_GCC_comparison
       tables_subdir: Tables
     gchp_vs_gchp:
       run: True
       dir: GCHP_version_comparison
       tables_subdir: Tables
     gchp_vs_gcc_diff_of_diffs:
-      run: False
+      run: True
       dir: GCHP_GCC_diff_of_diffs
   #
   # outputs: Specifies the plots and tables to generate
   #
   outputs:
     plot_conc: True
-    plot_wetdep: True
-    rnpbbe_budget: True
-    operations_budget: False
+    plot_emis: True
+    emis_table: True
+    plot_jvalues: True
+    plot_aod: True
+    plot_drydep: True
     mass_table: True
-    ste_table: True
-    cons_table: True
+    ops_budget_table: False
+    aer_budget_table: True
+    Ox_budget_table: True
+    ste_table: True # GCC only
+    OH_metrics: True
+    timing_table: True
+    plot_models_vs_obs: True
+    plot_options:
+      by_spc_cat: True
+      by_hco_cat: True
   #
   # n_cores: Specify the number of cores to use.
   # -1: Use $OMP_NUM_THREADS         cores
   # -2: Use $OMP_NUM_THREADS - 1     cores
   # -N: Use $OMP_NUM_THREADS - (N-1) cores
   #  1: Disable parallelization (use a single core)
   #
```

### Comparing `geoschem-gcpy-1.4.2/gcpy/benchmark/config/README.md` & `geoschem_gcpy-1.5.0/gcpy/benchmark/config/README.md`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/benchmark/modules/GC_72_vertical_levels.csv` & `geoschem_gcpy-1.5.0/gcpy/benchmark/modules/GC_72_vertical_levels.csv`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/benchmark/modules/README.md` & `geoschem_gcpy-1.5.0/gcpy/benchmark/modules/README.md`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/benchmark/modules/benchmark_models_vs_obs.py` & `geoschem_gcpy-1.5.0/gcpy/benchmark/modules/benchmark_models_vs_obs.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,55 +8,47 @@
 O3 plots are supported, but this can be extended in the future.
 
 Author: Matt Rowlinson <matthew.rowlinson@york.ac.uk>
 
 Linted with PyLint and incorporated into GCPy
 by Bob Yantosca <yantosca@seas.harvard.edu>
 """
-import os
 import glob
 from datetime import datetime, timedelta
 from matplotlib.backends.backend_pdf import PdfPages
 from matplotlib.figure import Figure
 import matplotlib.pyplot as plt
 import pandas as pd
 import numpy as np
 import xarray as xr
 from gcpy.constants import skip_these_vars
 from gcpy.util import verify_variable_type, dataset_reader, make_directory
-from gcpy.cstools import extract_grid, find_index, is_cubed_sphere
+from gcpy.cstools import extract_grid
+from gcpy.grid import get_nearest_model_data
+from gcpy.benchmark.modules.benchmark_utils import \
+    get_geoschem_level_metadata, rename_speciesconc_to_speciesconcvv
+
 
 def read_nas(
         input_file,
         verbose=False,
 
 ):
     """
     Read NASA Ames data files from EBAS (https://ebas-data.nilu.no)
     Creates data frame of O3 values converted to ppb and dictionary
     with key site information (name, lat, lon, altitude)
 
-    Args:
-    -----
-    input_file : str
-        Path to data file with observational data (e.g. sonde data).
-
-    Keyword Args:
-    -------------
-    verbose : bool
-        Toggles verbose printout on (True) or off (False).
-        Default value: False
-
-    Returns:
-    --------
-    obs_dataframe : pandas DataFrame
-        Dataframe containing observational data from input_file.
+    Args
+    input_file      : str          : Path to observational data file
+    verbose         : bool         : Toggles verbose output on/off
 
-    obs_site_coords : dict
-        Dictionary containing formatted site name: lon, lat and altitude.
+    Returns
+    obs_dataframe   : pd.DataFrame : Observations at each station site
+    obs_site_coords : dict         : Coords (lon/lat/alt) at each site
     """
     verify_variable_type(input_file, str)
 
     if verbose:
         print(f"read_nas: Reading {input_file}")
 
     with open(input_file, encoding='UTF-8') as the_file:
@@ -138,31 +130,21 @@
     """
     Reads the observational O3 data from EBAS
     (taken from https://ebas-data.nilu.no/ on 15/05/2023)
 
     Loops over all data files (in NASA/Ames format) within
     a folder and concatenates them into a single DataFrame.
 
-    Args:
-    -----
-    path : str
-        Path to the observational data directory
-
-    verbose : bool
-        Toggles verbose printout on (True) or off (False).
-        Default value: False
-
-    Returns:
-    --------
-    obs_dataframe : pandas DataFrame
-        DataFrame object with the observational data (i.e. station
-        names, data, metadata).
+    Args
+    path            : str          : Path to the observational data dir
+    verbose         : bool         : Toggles verbose output on/off
 
-    obs_site_coords : dict
-        Dictionary with coordinates of each observation site
+    Returns
+    obs_dataframe   : pd.DataFrame : Observations at each station site
+    obs_site_coords : dict         : Coords (lon/lat/alt) at each site
     """
     verify_variable_type(path, str)
 
     first = True
     obs_site_coords = {}
     dataframe = None
     for infile in sorted(glob.glob(f"{path}/*nas")):
@@ -200,72 +182,33 @@
 ):
     """
     Reads model data from a netCDF file.  Adds special handling to look
     for species concentrations variable names starting with either
     "SpeciesConcVV" or "SpeciesConc".  This is necessary for backwards
     compatitbility with GEOS-Chem output prior to version 14.1.0.
 
-    Args:
-    -----
-    filepaths : list of str
-        List of data files to read.
-
-    varname : str or list of str
-        Variable name(s) to read from data files.
-
-    Keyword Args:
-    -------------
-    varbose : bool
-        Toggles verbose output on (True) or off (False).
-        Default value: False
+    Args
+    filepaths : list         : List of GEOS-Chem data files to read
+    varname   : str          : Variable name(s) to read
+    verbose   : bool         : Toggles verbose output on/off
 
-    Returns:
-    --------
-    dataarray : xarray DataArray
-        DataArray object containing data read from files
-        specified by the filepaths argument.
+    Returns
+    dataarray : xr.DataArray : GEOS-Chem data read from disk
     """
 
     # Read the Ref and Dev model data
     reader = dataset_reader(
         multi_files=True,
         verbose=verbose,
     )
-
-    # Set temporary variable name for use below
-    varname_tmp = varname
-
-    # First try reading the data as-is
-    try:
-        dataset = reader(
-            filepaths,
-            drop_variables=skip_these_vars,
-            data_vars=[varname_tmp]
-        ).load()
-
-    # If we encounter a ValueError, it may be because the data is
-    # older # and may have e.g. SpeciesConc fields instead of
-    # SpeciesConcVV fields.  Reset the varname_tmp and try again.
-    except ValueError:
-        varname_tmp = varname_tmp.replace("VV", "")
-        dataset = reader(
-            filepaths,
-            drop_variables=skip_these_vars,
-            data_vars=[varname_tmp]
-        ).load()
-
-        # Rename to the original name to avid confusion with data
-        # from GEOS-Chem versions prior to 14.1.0
-        with xr.set_options(keep_attrs=True):
-            dataset = dataset.rename({varname_tmp: varname})
-
-    # If we fail again, then throw an error!
-    except [FileNotFoundError, OSError, IOError] as exc:
-        msg = f"get_model_data: Could not read Ref data for {varname}!"
-        raise exc(msg) from exc
+    
+    # Read data and rename SpeciesConc_ to SpeciesConcVV_, if necessary
+    # (needed for backwards compatibility with older versions.)
+    dataset = reader(filepaths,drop_variables=skip_these_vars).load()
+    dataset = rename_speciesconc_to_speciesconcvv(dataset)
 
     # Create a DataArray object and convert to ppbv (if necessary)
     with xr.set_options(keep_attrs=True):
         dataarray = dataset[varname]
         if "mol mol-1" in dataarray.attrs["units"]:
             dataarray.values *= 1.0e9
             dataarray.attrs["units"] = "ppbv"
@@ -275,352 +218,165 @@
 
 def find_times(
         obs_dataframe,
         start_time
 ):
     """
     Convert timestamps in nasa ames data files to python datetime
-    objects  Set DataFrame index to the new datetime array
+    objects and set DataFrame index to the new datetime array.
 
-    Args:
-    ----------
-    obs_dataframe : pandas DataFrame
-        DataFrame with O3 values from GAW site
-
-    start_time : str
-        Reference start time for timestamp taken from nasa ames file
+    Args
+    obs_dataframe : pd.DataFrame : Observations from GAW sites
+    start_time    : str          : Reference start time for obs data
 
     Returns
-    ------
-    obs_dataframe: pandas DataFrame
-        O3 in ppbV with datetime index
-
-    qcflag : pandas Dataframe
-        QC flag with datetime index
+    obs_dataframe : pd.DataFrame : Observations (ppbv) w/ datetime index
+    qcflag        : pd.DataFrame : Quality control info w/ datetime index
+    start_time    : str          : Reference start time for obs data
     """
     end_time = obs_dataframe[obs_dataframe.columns[1]]
     time_x = []
 
     for index in range(len(end_time)):
         time_x.append(start_time + timedelta(days=end_time.values[index]))
 
     obs_dataframe.index = time_x
     qcflag =obs_dataframe[obs_dataframe.columns[-1]]
     obs_dataframe = obs_dataframe[obs_dataframe.columns[2]]
 
     return obs_dataframe, qcflag
 
 
-def get_nearest_model_data_to_obs_cs(
+def get_nearest_model_data_to_obs(
         gc_data,
-        gc_cs_grid,
-        gc_level_alts_m,
+        gc_levels,
         lon_value,
         lat_value,
-        alt_value
+        alt_value,
+        gc_cs_grid=None
+
 ):
     """
     Returns GEOS-Chem model data (on a cubed-sphere grid) at the
     grid box closest to an observation site location.
 
-    Args:
-    -----
-    gc_data : xarray DataArray
-        GEOS-Chem output to be processed
-
-    gc_cs_grid: xarray Dataset
-        Coordinate arrays defining the cubed-sphere grid.
+    Args
+    gc_data    : pd.DataFrame : Observations at each station site
+    gc_levels  : pd.DataFrame : Metadata for model vertical levels
+    lon_value  : float        : Longitude of station site
+    lat_value  : float        : Latitude of station site
+    alt_value  : float        : Altitude of station site
+    gc_cs_grid : xr.Dataset   : Metadata for Dev cubed-sphere grid
 
-    gc_level_alts_m: pandas Series
-        Altitudes of GEOS-Chem levels in meters
-
-    lon_value : float
-        GAW site longitude
-
-    lat_value : float
-        GAW site latitude
-
-    alt_value : float
-        GAW site altitude
-
-    Keyword Args:
-    -------------
-
-    Returns:
-    --------
-    dataframe: pandas.DataFrame
-        Model data closest to the observation site.
+    Returns
+    dataframe  : pd.DataFrame : Model data closest to the station site
     """
     verify_variable_type(gc_data, xr.DataArray)
-    verify_variable_type(gc_cs_grid, xr.Dataset)
-    verify_variable_type(gc_level_alts_m, pd.Series)
+    verify_variable_type(gc_cs_grid, (xr.Dataset, type(None)))
+    verify_variable_type(gc_levels, pd.DataFrame)
 
     # Prevent the latitude from getting too close to the N or S poles
     lat_value = max(min(lat_value, 89.75), -89.75)
 
-    # Indices (nf, yInd, xInd) of box nearest to observation site
-    cs_indices = find_index(
-        lat_value,
-        lon_value,
-        gc_cs_grid
-    )
-
-    # Index of nearest vertical levle to observation site
-    z_idx=(
-        np.abs(
-            gc_level_alts_m.values - float(alt_value)
-        )
-    ).argmin()
-
-    return gc_data.isel(
-        nf=cs_indices[0, 0],
-        Ydim=cs_indices[1, 0],
-        Xdim=cs_indices[2, 0],
-        lev=z_idx
-    ).to_dataframe()
-
-
-def get_nearest_model_data_to_obs_ll(
+    # Nearest GEOS-Chem data to (lat, lon) of observation
+    dframe = get_nearest_model_data(
         gc_data,
-        gc_cs_grid,
-        gc_level_alts_m,
         lon_value,
         lat_value,
-        alt_value,
-
-):
-    """
-    Returns GEOS-Chem model data (on a cubed-sphere grid) at the
-    grid box closest to an observation site location.
-
-    Args:
-    -----
-    gc_data : xarray DataSet
-        GEOS-Chem output to be processed
-
-    gc_cs_grid : NoneType
-        Dummy variable (needed to make the argument list the
-        same as in get_nearest_model_data_to_obs_ll).
-
-    gc_level_alts_m: pandas Series
-        Altitudes of GEOS-Chem levels in meters
-
-    lon_value : float
-        GAW site longitude
-
-    lat_value : float
-        GAW site latitude
-
-    alt_value : float
-        GAW site altitude
-
-    Returns:
-    --------
-    dataframe: pandas.DataFrame
-        Model data closest to the observation site.
-    """
-    verify_variable_type(gc_data, xr.DataArray)
-    verify_variable_type(gc_cs_grid, type(None))
-    verify_variable_type(gc_level_alts_m, pd.Series)
-
-    x_idx=(
-        np.abs(
-            gc_data.lon.values - float(lon_value)
-        )
-    ).argmin()
-
-    y_idx=(
-        np.abs(
-            gc_data.lat.values - float(lat_value)
-        )
-    ).argmin()
-
-    z_idx=(
-        np.abs(
-            gc_level_alts_m.values - float(alt_value)
-        )
-    ).argmin()
-
-    return gc_data.isel(
-        lon=x_idx,
-        lat=y_idx,
-        lev=z_idx
-    ).to_dataframe()
-
-
-def which_finder_function(
-        data
-):
-    """
-    Returns the function that will be used to get the model data nearest
-    to the observation site.  The function that is returned depends on
-    whether the model grid is lat-lon or cubed-sphere, as different
-    handling needs to be applied to each grid
-
-    Args:
-    -----
-    data : xarray.DataArray
-        Model data
-
-    Returns:
-    --------
-    A reference to the function that will read the data, depending
-    on whether the data is placed on a cubed-sphere grid or on
-    a lat-lon grid.
-    """
-    verify_variable_type(data, (xr.DataArray, xr.Dataset))
-
-    if is_cubed_sphere(data):
-        return get_nearest_model_data_to_obs_cs
-
-    return get_nearest_model_data_to_obs_ll
-
-
-def get_geoschem_level_metadata(
-        filename=None,
-        search_key=None,
-        verbose=False,
-):
-    """
-    Reads a comma-separated variable (.csv) file with GEOS-Chem vertical
-    level metadata and returns it in a pandas DataFrame object.
+        gc_cs_grid=gc_cs_grid
+    )
+    dframe = dframe.reset_index()
 
-    Args:
-    -----
-    filename : str
-        Name of the comma-separated variable to read.
-        Default value: "__file__/GC_72_vertical_levels.csv"
-
-    Keyword Args:
-    -------------
-    search_key : str
-        If present, will return metadata that matches this value.
-        Default: None
-
-    verbose : bool
-        Toggles verbose printout on (True) or off (False).
-        Default value: True
+    # Nearest GEOS-Chem level to observation
+    gc_alts = gc_levels["Altitude (m)"].values
+    n_alts = len(gc_alts)
+    z_idx =(np.abs(gc_alts - float(alt_value))).argmin()
 
-    Returns:
-    --------
-    metadata : pandas DataFrame
-        Metadata for each of the GEOS-Chem vertical levels.
-    """
-    if filename is None:
-        filename = os.path.join(
-            os.path.dirname(__file__),
-            "GC_72_vertical_levels.csv"
-        )
+    # Pick out elements of the dataframe at the nearest level to obs
+    rows = np.zeros(len(dframe), dtype=bool)
+    good = [(v * n_alts) + z_idx for v in range(12)]
+    rows[good] = True
 
-    try:
-        if verbose:
-            print(f"get_geoschem_level_metadata: Reading {filename}")
-        metadata = pd.read_csv(filename)
-    except (IOError, OSError, FileNotFoundError) as exc:
-        msg = f"Could not read GEOS-Chem level metadata in {filename}!"
-        raise exc(msg) from exc
-
-    if search_key is None:
-        return metadata
-    return metadata[search_key]
+    return dframe[rows].set_index("time")
 
 
 def prepare_data_for_plot(
         obs_dataframe,
         obs_site_coords,
         obs_site_name,
         ref_dataarray,
         ref_cs_grid,
         dev_dataarray,
         dev_cs_grid,
-        gc_level_alts_m,
+        gc_levels,
         varname="SpeciesConcVV_O3",
-        **kwargs,
 ):
     """
     Prepares data for passing to routine plot_single_frames as follows:
 
     (1) Computes the mean of observations at the given station site.
     (2) Returns the GEOS-Chem Ref and Dev data at the gridbox closest
          to the given station site.
     (3) Creates the top-of-plot title for the given station site.
 
     Args:
-    -----
-    obs_dataframe : pandas DataFrame
-        Observations at each station site.
-
-    obs_site_coords : dict
-        Coordinates (lon, lat, alt) for each observation station site.
-
-    obs_site_name : str
-        Name of the observation station site.
-
-    ref_dataarray, dev_dataarray : xarray DataArray
-        Data from the Ref and Dev model versions.
-
-    ref_cs_grid, dev_cs_grid : xarray.Dataset or NoneType
-        Dictionary containing the cubed-sphere grid definitions for
-        ref_dataarray and dev_dataarray (or None if ref_dataarray or
-        dev_dataarray are not placed on a cubed-sphere grid).
-
-    gc_level_alts_m : pandas Series
-        Metadata pertaining to GEOS-Chem vertical levels
-
-    Keyword Args (Optional)
-    -----------------------
-    varname : str
-        GEOS-Chem diagnostic name for the Ref and Dev model data.
-        Default value: "SpeciesConcVV_O3"
+    obs_dataframe   : pd.DataFrame : Observations at each station site
+    obs_site_coords : dict         : Coords (lon/lat/alt) at each site
+    obs_site_name   : str          : Names of station sites
+    ref_dataarray   : xr.DataArray : Data from the Ref model version
+    ref_label       : str          : Label for the Ref model data
+    ref_cs_grid     : xr.Dataset   : Metadata for Ref cubed-sphere grid
+    dev_dataarray   : xr.DataArray : Data from the Dev model version
+    dev_label       : str          : Label for the Dev model data
+    dev_cs_grid     : xr.Dataset   : Metadata for Dev cubed-sphere grid
+    gc_levels       : pd.DataFrame : Metadata for model vertical levels
+    varname         : str          : Variable name for model data
 
     Returns:
-    --------
-    obs_dataframe : pandas DataFrame
-        Meanb observational data at the given station site.
-
-    ref_series, dev_series : pandas Series
-        Data from the Ref and Dev model versions at the
-        closest grid box to the observation station site.
-
-    subplot_title : str
-        Plot title string for the given observation station site.
-
-    subplot_ylabel : str
-        Label for the Y-axis (e.g. species name).
+    obs_dataframe   : pd.DataFrame : Mean observational data @ station site
+    ref_series      : pd.Series    : Ref data nearest to the station site
+    dev_series      : pd.Series    : Dev data nearest to the station site
+    subplot_title   : str          : Title for the station site subplot
+    subplot_ylabel  : str          : Y-axis titel for the station site subplot
     """
     verify_variable_type(obs_dataframe, pd.DataFrame)
     verify_variable_type(obs_site_coords, dict)
     verify_variable_type(obs_site_name, str)
     verify_variable_type(ref_dataarray, xr.DataArray)
     verify_variable_type(dev_dataarray, xr.DataArray)
     verify_variable_type(ref_cs_grid, (xr.Dataset, type(None)))
     verify_variable_type(dev_cs_grid, (xr.Dataset, type(None)))
-    verify_variable_type(gc_level_alts_m, pd.Series)
+    verify_variable_type(gc_levels, pd.DataFrame)
     verify_variable_type(varname, str)
 
     # Get data from the Ref model closest to the data site
-    finder_function = which_finder_function(ref_dataarray)
-    ref_dataframe = finder_function(
+    coords = [
+        round(obs_site_coords[obs_site_name]['lon'], 2),
+        round(obs_site_coords[obs_site_name]['lat'], 2),
+        round(obs_site_coords[obs_site_name]['alt'], 1)
+    ]
+
+    # Get data from the Ref model closest to the obs site
+    ref_dataframe = get_nearest_model_data_to_obs(
         ref_dataarray,
-        ref_cs_grid,
-        gc_level_alts_m,
-        lon_value=round(obs_site_coords[obs_site_name]['lon'], 2),
-        lat_value=round(obs_site_coords[obs_site_name]['lat'], 2),
-        alt_value=round(obs_site_coords[obs_site_name]['alt'], 1)
+        gc_levels,
+        coords[0],                 # Obs site lon
+        coords[1],                 # Obs site lat
+        coords[2],                 # Obs site alt
+        gc_cs_grid=ref_cs_grid
     )
 
     # Get data from the Dev model closest to the obs site
-    finder_function = which_finder_function(dev_dataarray)
-    dev_dataframe = finder_function(
+    dev_dataframe = get_nearest_model_data_to_obs(
         dev_dataarray,
-        dev_cs_grid,
-        gc_level_alts_m,
-        lon_value=round(obs_site_coords[obs_site_name]['lon'], 2),
-        lat_value=round(obs_site_coords[obs_site_name]['lat'], 2),
-        alt_value=round(obs_site_coords[obs_site_name]['alt'], 1)
+        gc_levels,
+        coords[0],                 # Obs site lon
+        coords[1],                 # Obs site lat
+        coords[2],                 # Obs site alt
+        gc_cs_grid=dev_cs_grid,
     )
 
     # Take the monthly mean of observations for plotting
     # (since some observation sites have multiple months of data)
     obs_dataframe = obs_dataframe.resample('M').mean()
 
     # Create the top title for the subplot for this observation site
@@ -649,52 +405,37 @@
         fig,
         rows_per_page,
         cols_per_page,
         subplot_index,
         subplot_title,
         subplot_ylabel,
         obs_dataframe,
+        obs_label,
         obs_site_name,
         ref_series,
         ref_label,
         dev_series,
-        dev_label,
-        **kwargs
+        dev_label
 ):
     """
     Plots observation data vs. model data at a single station site.
 
     Args:
-    -----
-    fig : matplotlib.figure.Figure
-        Matplotlib Figure object containing the plot.
-
-    rows_per_page, cols_per_page : int
-        Number of rows and columns on each page of the plot.
-
-    subplot_index : int
-        Index of the subplot on the page.  Runs from 0 to
-        (cols_per_page * rows_per_page - 1).
-
-    subplot_title, subplot_ylabel : str
-        Top title and y-axis label for each subplot
-
-    obs_dataframe : pandas DataFrame
-        Observational data.
-
-    obs_site_name: : str
-        Name of the observation station site.
-
-    ref_series, dev_series : pandas Series
-        GEOS-Chem data at closest grid box to the observation
-        station site for the Ref and Dev model versions.
-
-    ref_label, dev_label : str
-        Descriptive labels (e.g. version numbers) for the
-        GEOS-Chem Ref and Dev model versions.
+    obs_dataframe  : mpl.figure.Figure : Figure object for the plot
+    rows_per_page  : int               : # of rows to plot on a page
+    cols_per_page  : int               : # of columns to plot on a page
+    subplot_index  : int               : Index of each subplot
+    subplot_title  : str               : Title for each subplot
+    subplot_ylabel : str               : Y-axis title for each subplot
+    obs_dataframe  : pd.DataFrame      : Observations at each station site
+    obs_site_name  : str               : Name of the station site
+    ref_series     : pd.Series         : Data from the Ref model version
+    ref_label      : str               : Label for the Ref model data
+    dev_dataarray  : pd.Series         : Data from the Dev model version
+    dev_label      : str               : Label for the Dev model data
     """
     verify_variable_type(fig, Figure)
     verify_variable_type(rows_per_page, int)
     verify_variable_type(cols_per_page, int)
     verify_variable_type(subplot_index, int)
     verify_variable_type(subplot_title, str)
     verify_variable_type(subplot_ylabel, str)
@@ -723,15 +464,15 @@
     axes_subplot.plot(
         obs_dataframe.index,
         obs_dataframe[obs_site_name],
         color='k',
         marker='^',
         markersize=4,
         lw=1,
-        label='Observations'
+        label=f"{obs_label}"
     )
 
     # Plot model data
     axes_subplot.plot(
         obs_dataframe.index,
         ref_series,
         color='r',
@@ -781,81 +522,56 @@
         labelsize=6
     )
 
 
 def plot_one_page(
         pdf,
         obs_dataframe,
+        obs_label,
         obs_site_coords,
         obs_site_names,
         ref_dataarray,
         ref_label,
         ref_cs_grid,
         dev_dataarray,
         dev_label,
         dev_cs_grid,
-        gc_level_alts_m,
+        gc_levels,
         rows_per_page=3,
         cols_per_page=3,
         varname="SpeciesConcVV_O3",
-        **kwargs
 ):
     """
     Plots a single page of models vs. observations.
 
     Args:
-    -----
-    obs_dataframe : pandas DataFrame
-        Observations at each station site.
-
-    obs_site_coords : dict
-        Coordinates (lon, lat, alt) for each observation station site.
-
-    obs_site_names : list of str
-        Names of observation station sites that fit onto a single page.
-
-    ref_dataarray, dev_dataarray : xarray DataArray
-        Data from the Ref and Dev model versions.
-
-    ref_label, dev_label: str
-        Labels describing the Ref and Dev datasets (e.g. version numbers)
-
-    ref_cs_grid, dev_cs_grid : xarray.Dataset or NoneType
-        Dictionary containing the cubed-sphere grid definitions for
-        ref_dataarray and dev_dataarray (or None if ref_dataarray or
-        dev_dataarray are not placed on a cubed-sphere grid).
-
-    gc_level_alts_m : pandas DataFrame
-        Metadata pertaining to GEOS-Chem vertical levels
-
-    Keyword Args:
-    -------------
-
-    rows_per_page, cols_per_page : int
-        Number of rows and columns to plot on a single page.
-        Default values: 3 rows, 3 columns
-
-    varname : str
-        Variable name for GEOS-Chem diagnostic data.
-        Default value: "SpeciesConcVV_O3"
-
-    verbose : bool
-        Toggles verbose printout on (True) or off (False).
-        Default value: False
+    obs_dataframe   : pd.DataFrame : Observations at each station site.
+    obs_label       : str          : Label for the observational data
+    obs_site_coords : dict         : Coords (lon/lat/alt) at each site.
+    obs_site_names  : list         : Names of station sites per page
+    ref_dataarray   : xr.DataArray : Data from the Ref model version
+    ref_label       : str          : Label for the Ref model data
+    ref_cs_grid     : str|None     : Metadata for Ref cubed-sphere grid
+    dev_dataarray   : xr.DataArray : Data from the Dev model version
+    dev_label       : str          : Label for the Dev model data
+    dev_cs_grid     : str|None     : Metadata for Dev cubed-sphere grid
+    gc_levels       : pd.DataFrame : Metadata for model vertical levels
+    rows_per_page   : int          : Number of rows to plot on a page
+    varname         : str          : Variable name for model data
     """
     verify_variable_type(obs_dataframe, pd.DataFrame)
     verify_variable_type(obs_site_coords, dict)
     verify_variable_type(obs_site_names, list)
     verify_variable_type(ref_dataarray, xr.DataArray)
     verify_variable_type(ref_label, str)
     verify_variable_type(ref_cs_grid, (xr.Dataset, type(None)))
     verify_variable_type(dev_dataarray, xr.DataArray)
     verify_variable_type(dev_label, str)
     verify_variable_type(dev_cs_grid, (xr.Dataset, type(None)))
-    verify_variable_type(gc_level_alts_m, pd.Series)
+    verify_variable_type(gc_levels, pd.DataFrame)
 
     # Define a new matplotlib.figure.Figure object for this page
     # Landscape width: 11" x 8"
     fig = plt.figure(figsize=(11, 8))
     fig.tight_layout()
 
     # Loop over all of the stations that fit on the page
@@ -870,34 +586,33 @@
             obs_dataframe,                # pandas.DataFrame
             obs_site_coords,              # dict
             obs_site_name,                # str
             ref_dataarray,                # xarray.DataArray
             ref_cs_grid,                  # dict or none
             dev_dataarray,                # xarray.DataArray
             dev_cs_grid,                  # dict or none
-            gc_level_alts_m,              # pandas.Series
-            varname=varname,              # str
-            **kwargs
+            gc_levels,                    # pandas.DataFrame
+            varname=varname               # str
         )
 
         # Plot models vs. observation for a single station site
         plot_single_station(
             fig,                          # matplotlib.figure.Figure
             rows_per_page,                # int
             cols_per_page,                # int
             subplot_index,                # int
             subplot_title,                # str
             subplot_ylabel,               # str
             obs_dataframe,                # pandas.Dataframe
+            obs_label,                    # str
             obs_site_name,                # str
             ref_series,                   # pandas.Series
             ref_label,                    # str
             dev_series,                   # pandas.Series
             dev_label,                    # str
-            **kwargs
         )
 
     # Add extra spacing around plots
     plt.subplots_adjust(
         hspace=0.4,
         top=0.9
     )
@@ -912,73 +627,54 @@
 
     # Save this page to the PDF file
     pdf.savefig(fig)
 
 
 def plot_models_vs_obs(
         obs_dataframe,
+        obs_label,
         obs_site_coords,
         ref_dataarray,
         ref_label,
         dev_dataarray,
         dev_label,
-        gc_level_alts_m,
+        gc_levels,
         varname="SpeciesConcVV_O3",
         dst="./benchmark",
-        **kwargs
 ):
     """
     Plots models vs. observations using a 3 rows x 3 column layout.
 
     Args:
-    -----
-    obs_dataframe : pandas DataFrame
-        Observations at each station site.
-
-    obs_site_coords : dict
-        Coordinates (lon, lat, alt) for each observation station site.
-
-    ref_dataarray, dev_dataarray : xarray DataArray
-        Data from the Ref and Dev model versions.
-
-    ref_label, dev_label: str
-        Labels describing the Ref and Dev datasets (e.g. version numbers)
-
-    gc_level_alts_m : pandas DataFrame
-        Metadata pertaining to GEOS-Chem vertical levels
-
-    Keyword Args:
-    -------------
-    varname : str
-        Variable name for GEOS-Chem diagnostic data.
-        Default value: "SpeciesConcVV_O3"
-
-    dst : str
-        Root folder where output will be created.
-        Default value: "./benchmark"
-
-    verbose : bool
-        Toggles verbose printout on (True) or off (False).
-        Default value: False
+    obs_dataframe   : pd.DataFrame : Observations at each station site.
+    obs_label       : str          : Label for the observational data
+    obs_site_coords : dict         : Coords (lon/lat/alt) at each site.
+    ref_dataarray   : xr.DataArray : Data from the Ref model version
+    ref_label       : str          : Label for the Ref model data
+    dev_dataarray   : xr.DataArray : Data from the Dev model version
+    dev_label       : str          : Label for the Dev model data
+    gc_levels       : pd.DataFrame : Metadata for model vertical levels
+    varname         : str          : Variable name for model data
+    dst             : str          : Destination folder for plots
     """
     verify_variable_type(obs_dataframe, pd.DataFrame)
     verify_variable_type(obs_site_coords, dict)
     verify_variable_type(ref_dataarray, xr.DataArray)
     verify_variable_type(ref_label, str)
     verify_variable_type(dev_dataarray, xr.DataArray)
     verify_variable_type(dev_label, str)
-    verify_variable_type(gc_level_alts_m, pd.Series)
+    verify_variable_type(gc_levels, pd.DataFrame)
 
     # Get the cubed-sphere grid definitions for Ref & Dev
     # (will be returned as "None" for lat/lon grids)
     ref_cs_grid = extract_grid(ref_dataarray)
     dev_cs_grid = extract_grid(dev_dataarray)
 
     # Figure setup
-    plt.style.use('seaborn-darkgrid')
+    plt.style.use("seaborn-v0_8-darkgrid")
     rows_per_page = 3
     cols_per_page = 3
     plots_per_page = rows_per_page * cols_per_page
 
     # Open the plot as a PDF document
     pdf_file = f"{dst}/models_vs_obs.surface.{varname.split('_')[1]}.pdf"
     pdf = PdfPages(pdf_file)
@@ -999,93 +695,81 @@
     for start in range(0, len(obs_site_names), plots_per_page):
         end = start + plots_per_page - 1
 
         # Plot obs sites that fit on a single page
         plot_one_page(
             pdf,                          # PdfPages
             obs_dataframe,                # pandas.DataFrame
+            obs_label,                    # str
             obs_site_coords,              # dict
             obs_site_names[start:end+1],  # list of str
             ref_dataarray,                # xarray.DataArray
             ref_label,                    # str
             ref_cs_grid,                  # xarray.DataSet or NoneType
             dev_dataarray,                # xarray.DataArray
             dev_label,                    # str
             dev_cs_grid,                  # xarray.Dataset or NoneType
-            gc_level_alts_m,              # pandas.Series
+            gc_levels,                    # pandas.DataFrame
             rows_per_page=rows_per_page,  # int
             cols_per_page=cols_per_page,  # int
             varname=varname,              # str
-            **kwargs
         )
 
     # Close the PDF file after all pages are plotted.
     pdf.close()
 
+    # Reset the plot style (this prevents the seaborn style from
+    # being applied to other model vs. obs plotting scripts)
+    plt.style.use("default")
+
 
 def make_benchmark_models_vs_obs_plots(
         obs_filepaths,
+        obs_label,
         ref_filepaths,
         ref_label,
         dev_filepaths,
         dev_label,
         varname="SpeciesConcVV_O3",
         dst="./benchmark",
         verbose=False,
         overwrite=False
 ):
     """
     Driver routine to create model vs. observation plots.
 
     Args:
-    -----
-    obs_filepaths : str or list
-        Path(s) to the observational data.
-
-    ref_filepaths, dev_filepaths: str or list
-        Path(s) to the Ref and Dev model versions to be compared.
-
-    ref_label, dev_label : str
-        Descriptive labels (e.g. for version numbers) for the
-        Ref and Dev model data.
-
-    Keyword Args (optional):
-    ------------------------
-    varname : str
-        Variable name for model data to be plotted against
-        observations.  Default value: "SpeciesConcVV_O3".
-
-    dst : str
-        Path to the root folder where plots will be created.
-
-    verbose : bool
-        Toggles verbose printout on (True) or off (False).
-        Default value: False
-
-    overwrite : bool
-        Toggles whether plots should be overwritten (True)
-        or not (False). Default value: True
+    obs_filepaths : str|list : Path(s) to the observational data.
+    obs_label     : str      : Label for the observational data
+    ref_filepaths : str      : Paths to the Ref model data
+    ref_label     : str      : Label for the Ref model data
+    dev_filepaths : str      : Paths to the Dev model data
+    dev_label     : str      : Label for the Dev model data
+    varname       : str      : Variable name for model data
+    dst           : str      : Destination folder for plots
+    verbose       : bool     : Toggles verbose output on/off
+    overwrite     : bool     : Toggles overwriting contents of dst
     """
     verify_variable_type(obs_filepaths, (str, list))
     verify_variable_type(ref_filepaths, (str, list))
     verify_variable_type(ref_label, str)
     verify_variable_type(dev_filepaths, (str, list))
     verify_variable_type(dev_label, str)
 
     # Create the destination folder
     make_directory(
         dst,
         overwrite=overwrite
     )
 
-    # Get altitude [m] of GEOS-Chem level edges
-    gc_level_alts_m = \
-        get_geoschem_level_metadata(
-            search_key="Altitude (km)"
-        ) * 1.0e3
+    # Get GEOS-Chem level metadata
+    gc_levels = get_geoschem_level_metadata(
+        search_key=["Altitude (km)", "Eta Mid"]
+    )
+    gc_levels["Altitude (m)"] = gc_levels["Altitude (km)"] * 1000.0
 
     # Read the observational data
     obs_dataframe, obs_site_coords = read_observational_data(
         obs_filepaths,
         verbose=verbose
     )
 
@@ -1098,17 +782,17 @@
         dev_filepaths,
         varname=varname
     )
 
     # Plot data vs observations
     plot_models_vs_obs(
         obs_dataframe,                    # pandas.DataFrame
+        obs_label,                        # str
         obs_site_coords,                  # dict
         ref_dataarray,                    # xarray.DataArray
         ref_label,                        # str
         dev_dataarray,                    # xarray.DataArray
         dev_label,                        # str
-        gc_level_alts_m,                  # pandas.Series
+        gc_levels,                        # pandas.DataFrame
         varname=varname,                  # str
         dst=dst,                          # str
-        verbose=verbose                   # bool
     )
```

### Comparing `geoschem-gcpy-1.4.2/gcpy/benchmark/modules/run_1yr_fullchem_benchmark.py` & `geoschem_gcpy-1.5.0/gcpy/benchmark/modules/run_1yr_fullchem_benchmark.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,27 +11,23 @@
     (3) GCHP vs GCHP
 
 You can customize this by editing the settings in the corresponding yaml
 config file (eg. 1yr_fullchem_benchmark.yml).
 
 To generate benchmark output:
 
-    (1) Copy the gcpy/benchmark/run_benchmark.py script and the
-        1yr_fullchem_benchmark.yml file anywhere you want to generate
-        output plots and tables.
+    (1) Copy the file gcpy/benchmark/config/1yr_fullchem_benchmark.yml
+        to a folder of your choice.
 
-    (2) Edit the 1yr_fullchem_benchmark.yml to point to the proper
-        file paths on your disk space.
+    (2) Edit the 1yr_fullchem_benchmark.yml to select the desired options
+        and to point to the proper file paths on your system.
 
-    (3) Make sure the /path/to/gcpy/benchmark is in your PYTHONPATH
-        shell environment variable.
+    (3) Run the command:
 
-    (4) Type at the command line
-
-        ./run_benchmark.py 1yr_fullchem_benchmark.yml
+        $ python -m gcpy.benchmark.run_benchmark.py 1yr_fullchem_benchmark.yml
 
 Remarks:
 
     By default, matplotlib will try to open an X window for plotting.
     If you are running this script in an environment where you do not have
     an active X display (such as in a computational queue), then you will
     need to use these commands to disable the X-window functionality.
@@ -39,37 +35,61 @@
         import os
         os.environ["QT_QPA_PLATFORM"]="offscreen"
 
     For more information, please see this issue posted at the ipython site:
 
         https://github.com/ipython/ipython/issues/10627
 
-This script corresponds with GCPy 1.4.2. Edit this version ID if releasing
+    Also, to disable matplotlib from trying to open X windows, you may
+    need to set the following environment variable in your shell:
+
+        $ export MPLBACKEND=agg
+
+This script corresponds with GCPy 1.5.0. Edit this version ID if releasing
 a new version of GCPy.
 """
 
 # =====================================================================
 # Imports and global settings (you should not need to edit these)
 # =====================================================================
 
 import os
 import warnings
-from shutil import copyfile
 from calendar import monthrange
 import numpy as np
 from joblib import Parallel, delayed
-from gcpy.util import get_filepath, get_filepaths
-import gcpy.ste_flux as ste
-import gcpy.oh_metrics as oh
-import gcpy.budget_ox as ox
-from gcpy import benchmark_funcs as bmk
-import gcpy.benchmark.modules.benchmark_models_vs_obs as mvo
+from gcpy.util import copy_file_to_dir, get_filepath, get_filepaths
+from gcpy.benchmark.modules.ste_flux import make_benchmark_ste_table
+from gcpy.benchmark.modules.oh_metrics import make_benchmark_oh_metrics
+from gcpy.benchmark.modules.budget_ox import global_ox_budget
+#TODO: Peel out routines from benchmark_funcs.py into smaller
+# routines in the gcpy/benchmark/modules folder, such as these:
+from gcpy.benchmark.modules.benchmark_funcs import \
+    diff_of_diffs_toprow_title, get_species_database_dir, \
+    make_benchmark_conc_plots, make_benchmark_emis_plots, \
+    make_benchmark_emis_tables, make_benchmark_jvalue_plots, \
+    make_benchmark_aod_plots, make_benchmark_mass_tables, \
+    make_benchmark_operations_budget, make_benchmark_aerosol_tables
+from gcpy.benchmark.modules.benchmark_utils import \
+    gcc_vs_gcc_dirs, gchp_vs_gcc_dirs, gchp_vs_gchp_dirs, \
+    get_log_filepaths, print_benchmark_info
+from gcpy.benchmark.modules.benchmark_models_vs_obs \
+    import make_benchmark_models_vs_obs_plots
+from gcpy.benchmark.modules.benchmark_models_vs_sondes \
+    import make_benchmark_models_vs_sondes_plots
+from gcpy.benchmark.modules.benchmark_drydep \
+    import drydepvel_species, make_benchmark_drydep_plots
+from gcpy.benchmark.modules.benchmark_scrape_gcclassic_timers import \
+    make_benchmark_gcclassic_timing_table
+from gcpy.benchmark.modules.benchmark_scrape_gchp_timers import \
+    make_benchmark_gchp_timing_table
 
 # Tell matplotlib not to look for an X-window
 os.environ["QT_QPA_PLATFORM"] = "offscreen"
+
 # Suppress annoying warning messages
 warnings.filterwarnings("ignore", category=RuntimeWarning)
 warnings.filterwarnings("ignore", category=UserWarning)
 warnings.filterwarnings("ignore", category=FutureWarning)
 
 def run_benchmark(config, bmk_year_ref, bmk_year_dev):
     """
@@ -83,88 +103,40 @@
     # This script has a fixed benchmark type
     bmk_type = config["options"]["bmk_type"]
     bmk_mon_strs = ["Jan", "Apr", "Jul", "Oct"]
     bmk_mon_inds = [0, 3, 6, 9]
     bmk_n_months = len(bmk_mon_strs)
 
     # Folder in which the species_database.yml file is found
-    spcdb_dir = bmk.get_species_database_dir(config)
+    spcdb_dir = get_species_database_dir(config)
 
     # ======================================================================
     # Data directories
     # ======================================================================
 
     # Diagnostics file directory paths
-    gcc_vs_gcc_refdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["ref"]["gcc"]["dir"],
-        config["data"]["ref"]["gcc"]["outputs_subdir"],
-    )
-    gcc_vs_gcc_devdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["dev"]["gcc"]["dir"],
-        config["data"]["dev"]["gcc"]["outputs_subdir"],
-    )
-    gchp_vs_gcc_refdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["dev"]["gcc"]["dir"],
-        config["data"]["dev"]["gcc"]["outputs_subdir"],
-    )
-    gchp_vs_gcc_devdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["dev"]["gchp"]["dir"],
-        config["data"]["dev"]["gchp"]["outputs_subdir"],
-    )
-    gchp_vs_gchp_refdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["ref"]["gchp"]["dir"],
-        config["data"]["ref"]["gchp"]["outputs_subdir"],
-    )
-    gchp_vs_gchp_devdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["dev"]["gchp"]["dir"],
-        config["data"]["dev"]["gchp"]["outputs_subdir"],
-    )
+    s = "outputs_subdir"
+    gcc_vs_gcc_refdir, gcc_vs_gcc_devdir = gcc_vs_gcc_dirs(config, s)
+    gchp_vs_gcc_refdir, gchp_vs_gcc_devdir = gchp_vs_gcc_dirs(config, s)
+    gchp_vs_gchp_refdir, gchp_vs_gchp_devdir = gchp_vs_gchp_dirs(config, s)
 
     # Restart file directory paths
-    gcc_vs_gcc_refrstdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["ref"]["gcc"]["dir"],
-        config["data"]["ref"]["gcc"]["restarts_subdir"]
-    )
-    gcc_vs_gcc_devrstdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["dev"]["gcc"]["dir"],
-        config["data"]["dev"]["gcc"]["restarts_subdir"]
-    )
-    gchp_vs_gcc_refrstdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["dev"]["gcc"]["dir"],
-        config["data"]["dev"]["gcc"]["restarts_subdir"]
-    )
-    gchp_vs_gcc_devrstdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["dev"]["gchp"]["dir"],
-        config["data"]["dev"]["gchp"]["restarts_subdir"]
-    )
-    gchp_vs_gchp_refrstdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["ref"]["gchp"]["dir"],
-        config["data"]["ref"]["gchp"]["restarts_subdir"]
-    )
-    gchp_vs_gchp_devrstdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["dev"]["gchp"]["dir"],
-        config["data"]["dev"]["gchp"]["restarts_subdir"]
-    )
+    s = "restarts_subdir"
+    gcc_vs_gcc_refrstdir, gcc_vs_gcc_devrstdir = gcc_vs_gcc_dirs(config, s)
+    gchp_vs_gcc_refrstdir, gchp_vs_gcc_devrstdir = gchp_vs_gcc_dirs(config, s)
+    gchp_vs_gchp_refrstdir, gchp_vs_gchp_devrstdir = gchp_vs_gchp_dirs(config, s)
+
+    # Log file directory paths
+    s = "logs_subdir"
+    gcc_vs_gcc_reflogdir, gcc_vs_gcc_devlogdir = gcc_vs_gcc_dirs(config, s)
+    gchp_vs_gcc_reflogdir, gchp_vs_gcc_devlogdir = gchp_vs_gcc_dirs(config, s)
+    gchp_vs_gchp_reflogdir, gchp_vs_gchp_devlogdir = gchp_vs_gchp_dirs(config, s)
 
     # Directories where plots & tables will be created
-    mainresultsdir = os.path.join(
-        config["paths"]["results_dir"]
-    )
+    mainresultsdir = os.path.join(config["paths"]["results_dir"])
     gcc_vs_gcc_resultsdir = os.path.join(
         mainresultsdir,
         config["options"]["comparisons"]["gcc_vs_gcc"]["dir"]
     )
     gchp_vs_gcc_resultsdir = os.path.join(
         mainresultsdir,
         config["options"]["comparisons"]["gchp_vs_gcc"]["dir"]
@@ -173,44 +145,39 @@
         mainresultsdir,
         config["options"]["comparisons"]["gchp_vs_gchp"]["dir"]
     )
     diff_of_diffs_resultsdir = os.path.join(
         mainresultsdir,
         "GCHP_GCC_diff_of_diffs"
     )
-    # Make copy of benchmark script in results directory
+
+    # Create the main results directory first
     if not os.path.exists(mainresultsdir):
         os.mkdir(mainresultsdir)
-        curfile = os.path.realpath(__file__)
-        dest = os.path.join(mainresultsdir, curfile.split("/")[-1])
-        if not os.path.exists(dest):
-            copyfile(curfile, dest)
 
-    # Create results directories that don't exist,
-    # and place a copy of this file in each results directory
+    # Create results directories that don't exist.  Also place a copy of
+    # this file plus the YAML configuration file in each results directory.
     results_list = [
         gcc_vs_gcc_resultsdir,
         gchp_vs_gchp_resultsdir,
         gchp_vs_gcc_resultsdir,
         diff_of_diffs_resultsdir
     ]
     comparisons_list = [
         config["options"]["comparisons"]["gcc_vs_gcc"]["run"],
         config["options"]["comparisons"]["gchp_vs_gchp"]["run"],
         config["options"]["comparisons"]["gchp_vs_gcc"]["run"],
         config["options"]["comparisons"]["gchp_vs_gcc_diff_of_diffs"]["run"]
     ]
-    for resdir, plotting_type in zip(results_list, comparisons_list):
+    for (resdir, plotting_type) in zip(results_list, comparisons_list):
         if plotting_type and not os.path.exists(resdir):
             os.mkdir(resdir)
             if resdir in results_list:
-                curfile = os.path.realpath(__file__)
-                dest = os.path.join(resdir, curfile.split("/")[-1])
-                if not os.path.exists(dest):
-                    copyfile(curfile, dest)
+                copy_file_to_dir(__file__, resdir)
+                copy_file_to_dir(config["configuration_file_name"], resdir)
 
     # Tables directories
     gcc_vs_gcc_tablesdir = os.path.join(
         gcc_vs_gcc_resultsdir,
         config["options"]["comparisons"]["gcc_vs_gcc"]["tables_subdir"],
     )
     gchp_vs_gcc_tablesdir = os.path.join(
@@ -224,35 +191,42 @@
 
     ## Budget directories
     #gcc_vs_gcc_budgetdir = os.path.join(gcc_vs_gcc_resultsdir, "Budget")
     #gchp_vs_gcc_budgetdir = os.path.join(gchp_vs_gcc_resultsdir, "Budget")
     #gchp_vs_gchp_budgetdir = os.path.join(gchp_vs_gchp_resultsdir, "Budget")
 
     # Models vs. observations directories
-    gcc_vs_gcc_models_vs_obs_dir = os.path.join(
-        gcc_vs_gcc_resultsdir, "ModelVsObs"
-    )
-    gchp_vs_gcc_models_vs_obs_dir = os.path.join(
-        gchp_vs_gcc_resultsdir, "ModelVsObs"
-    )
-    gchp_vs_gchp_models_vs_obs_dir = os.path.join(
-        gchp_vs_gchp_resultsdir, "ModelVsObs"
-    )
+    s = "ModelVsObs"
+    gcc_vs_gcc_models_vs_obs_dir = os.path.join(gcc_vs_gcc_resultsdir, s)
+    gchp_vs_gcc_models_vs_obs_dir = os.path.join(gchp_vs_gcc_resultsdir, s)
+    gchp_vs_gchp_models_vs_obs_dir = os.path.join(gchp_vs_gchp_resultsdir, s)
 
     # ======================================================================
     # Plot title strings
     # ======================================================================
     gcc_vs_gcc_refstr = config["data"]["ref"]["gcc"]["version"]
     gcc_vs_gcc_devstr = config["data"]["dev"]["gcc"]["version"]
     gchp_vs_gcc_refstr = config["data"]["dev"]["gcc"]["version"]
     gchp_vs_gcc_devstr = config["data"]["dev"]["gchp"]["version"]
     gchp_vs_gchp_refstr = config["data"]["ref"]["gchp"]["version"]
     gchp_vs_gchp_devstr = config["data"]["dev"]["gchp"]["version"]
-    diff_of_diffs_refstr = bmk.diff_of_diffs_toprow_title(config, "gcc")
-    diff_of_diffs_devstr = bmk.diff_of_diffs_toprow_title(config, "gchp")
+    diff_of_diffs_refstr = diff_of_diffs_toprow_title(config, "gcc")
+    diff_of_diffs_devstr = diff_of_diffs_toprow_title(config, "gchp")
+
+    # ======================================================================
+    # Observational data files
+    # ======================================================================
+    sondes_data_file = os.path.join(
+        config["paths"]["obs_data"]["sondes"]["data_dir"],
+        config["paths"]["obs_data"]["sondes"]["data_file"],
+    )
+    sondes_site_file = os.path.join(
+        config["paths"]["obs_data"]["sondes"]["data_dir"],
+        config["paths"]["obs_data"]["sondes"]["site_file"],
+    )
 
     ########################################################################
     ###    THE REST OF THESE SETTINGS SHOULD NOT NEED TO BE CHANGED      ###
     ########################################################################
 
     # =====================================================================
     # Dates and times -- ref data
@@ -302,49 +276,17 @@
 
     # Get subset of month datetimes and seconds per month for only benchmark months
     bmk_mons_dev = all_months_dev[bmk_mon_inds]
     bmk_mons_gchp_dev = all_months_gchp_dev[bmk_mon_inds]
     bmk_sec_per_month_dev = sec_per_month_dev[bmk_mon_inds]
 
     # ======================================================================
-    # Print the list of plots & tables to the screen
+    # Print the list of plots & tables being generated
     # ======================================================================
-
-    print(f"The following plots and tables will be created for {bmk_type}:")
-    if config["options"]["outputs"]["plot_conc"]:
-        print(" - Concentration plots")
-    if config["options"]["outputs"]["plot_emis"]:
-        print(" - Emissions plots")
-    if config["options"]["outputs"]["plot_jvalues"]:
-        print(" - J-values (photolysis rates) plots")
-    if config["options"]["outputs"]["plot_aod"]:
-        print(" - Aerosol optical depth plots")
-    if config["options"]["outputs"]["ops_budget_table"]:
-        print(" - Operations budget tables")
-    if config["options"]["outputs"]["aer_budget_table"]:
-        print(" - Aerosol budget/burden tables")
-    if config["options"]["outputs"]["emis_table"]:
-        print(" - Table of emissions totals by species and inventory")
-    if config["options"]["outputs"]["mass_table"]:
-        print(" - Table of species mass")
-    if config["options"]["outputs"]["OH_metrics"]:
-        print(" - Table of OH metrics")
-    if config["options"]["outputs"]["ste_table"]:
-        print(" - Table of strat-trop exchange")
-    if config["options"]["outputs"]["plot_models_vs_obs"]:
-        print(" - Plots of models vs. observations")
-    print("Comparisons will be made for the following combinations:")
-    if config["options"]["comparisons"]["gcc_vs_gcc"]["run"]:
-        print(" - GCC vs GCC")
-    if config["options"]["comparisons"]["gchp_vs_gcc"]["run"]:
-        print(" - GCHP vs GCC")
-    if config["options"]["comparisons"]["gchp_vs_gchp"]["run"]:
-        print(" - GCHP vs GCHP")
-    if config["options"]["comparisons"]["gchp_vs_gcc_diff_of_diffs"]["run"]:
-        print(" - GCHP vs GCC diff of diffs")
+    print_benchmark_info(config)
 
     # %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
     # Create GCC vs GCC benchmark plots and tables
     # %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
     if config["options"]["comparisons"]["gcc_vs_gcc"]["run"]:
 
         # ==================================================================
@@ -384,15 +326,15 @@
                 gcc_vs_gcc_devdir,
                 "SpeciesConc",
                 all_months_dev
             )[0]
 
             # Create plots
             print("\nCreating plots for annual mean")
-            bmk.make_benchmark_conc_plots(
+            make_benchmark_conc_plots(
                 ref,
                 gcc_vs_gcc_refstr,
                 dev,
                 gcc_vs_gcc_devstr,
                 refmet=refmet,
                 devmet=devmet,
                 dst=gcc_vs_gcc_resultsdir,
@@ -409,15 +351,15 @@
             # GCC vs GCC species concentration plots: Seasonal
             # --------------------------------------------------------------
             for mon in range(bmk_n_months):
                 print(f"\nCreating plots for {bmk_mon_strs[mon]}")
 
                 # Create plots
                 mon_ind = bmk_mon_inds[mon]
-                bmk.make_benchmark_conc_plots(
+                make_benchmark_conc_plots(
                     ref[mon_ind],
                     gcc_vs_gcc_refstr,
                     dev[mon_ind],
                     gcc_vs_gcc_devstr,
                     refmet=refmet[mon_ind],
                     devmet=devmet[mon_ind],
                     dst=gcc_vs_gcc_resultsdir,
@@ -451,15 +393,15 @@
                 gcc_vs_gcc_devdir,
                 "Emissions",
                 all_months_dev
             )[0]
 
             # Create plots
             print("\nCreating plots for annual mean")
-            bmk.make_benchmark_emis_plots(
+            make_benchmark_emis_plots(
                 ref,
                 gcc_vs_gcc_refstr,
                 dev,
                 gcc_vs_gcc_devstr,
                 dst=gcc_vs_gcc_resultsdir,
                 subdst="AnnualMean",
                 time_mean=True,
@@ -478,15 +420,15 @@
             # GCC vs GCC emissions plots: Seasonal
             # --------------------------------------------------------------
             for mon in range(bmk_n_months):
                 print(f"\nCreating plots for {bmk_mon_strs[mon]}")
 
                 # Create plots
                 mon_ind = bmk_mon_inds[mon]
-                bmk.make_benchmark_emis_plots(
+                make_benchmark_emis_plots(
                     ref[mon_ind],
                     gcc_vs_gcc_refstr,
                     dev[mon_ind],
                     gcc_vs_gcc_devstr,
                     dst=gcc_vs_gcc_resultsdir,
                     subdst=bmk_mon_yr_strs_dev[mon],
                     weightsdir=config["paths"]["weights_dir"],
@@ -515,15 +457,15 @@
             dev = get_filepaths(
                 gcc_vs_gcc_devdir,
                 "Emissions",
                 all_months_dev
             )[0]
 
             # Create table
-            bmk.make_benchmark_emis_tables(
+            make_benchmark_emis_tables(
                 ref,
                 gcc_vs_gcc_refstr,
                 dev,
                 gcc_vs_gcc_devstr,
                 dst=gcc_vs_gcc_resultsdir,
                 benchmark_type=bmk_type,
                 ref_interval=sec_per_month_ref,
@@ -552,15 +494,15 @@
                 gcc_vs_gcc_devdir,
                 "JValues",
                 all_months_dev
             )[0]
 
             # Create plots
             print("\nCreating plots for annual mean")
-            bmk.make_benchmark_jvalue_plots(
+            make_benchmark_jvalue_plots(
                 ref,
                 gcc_vs_gcc_refstr,
                 dev,
                 gcc_vs_gcc_devstr,
                 dst=gcc_vs_gcc_resultsdir,
                 subdst="AnnualMean",
                 time_mean=True,
@@ -574,15 +516,15 @@
             # GCC vs GCC J-value plots: Seasonal
             # --------------------------------------------------------------
             for mon in range(bmk_n_months):
                 print(f"\nCreating plots for {bmk_mon_strs[mon]}")
 
                 # Create plots
                 mon_ind = bmk_mon_inds[mon]
-                bmk.make_benchmark_jvalue_plots(
+                make_benchmark_jvalue_plots(
                     ref[mon_ind],
                     gcc_vs_gcc_refstr,
                     dev[mon_ind],
                     gcc_vs_gcc_devstr,
                     dst=gcc_vs_gcc_resultsdir,
                     subdst=bmk_mon_yr_strs_dev[mon],
                     weightsdir=config["paths"]["weights_dir"],
@@ -611,15 +553,15 @@
                 gcc_vs_gcc_devdir,
                 "Aerosols",
                 all_months_dev
             )[0]
 
             # Create plots
             print("\nCreating plots for annual mean")
-            bmk.make_benchmark_aod_plots(
+            make_benchmark_aod_plots(
                 ref,
                 gcc_vs_gcc_refstr,
                 dev,
                 gcc_vs_gcc_devstr,
                 dst=gcc_vs_gcc_resultsdir,
                 subdst="AnnualMean",
                 time_mean=True,
@@ -633,28 +575,89 @@
             # GCC vs GCC column AOD plots: Seasonal
             # --------------------------------------------------------------
             for mon in range(bmk_n_months):
                 print(f"\nCreating plots for {bmk_mon_strs[mon]}")
 
                 # Create plots
                 mon_ind = bmk_mon_inds[mon]
-                bmk.make_benchmark_aod_plots(
+                make_benchmark_aod_plots(
                     ref[mon_ind],
                     gcc_vs_gcc_refstr,
                     dev[mon_ind],
                     gcc_vs_gcc_devstr,
                     dst=gcc_vs_gcc_resultsdir,
                     subdst=bmk_mon_yr_strs_dev[mon],
                     weightsdir=config["paths"]["weights_dir"],
                     overwrite=True,
                     spcdb_dir=spcdb_dir,
                     n_job=config["options"]["n_cores"]
                 )
 
         # ==================================================================
+        # GCC vs. GCC drydep plots
+        # ==================================================================
+        if config["options"]["outputs"]["plot_drydep"]:
+            print("\n%%% Creating GCC vs. GCC drydep plots %%%")
+
+            # --------------------------------------------------------------
+            # GCC vs GCC drydep plots: Annual mean
+            # --------------------------------------------------------------
+
+            # Filepaths
+            ref = get_filepaths(
+                gcc_vs_gcc_refdir,
+                "DryDep",
+                all_months_ref
+            )[0]
+            dev = get_filepaths(
+                gcc_vs_gcc_devdir,
+                "DryDep",
+                all_months_dev
+            )[0]
+
+            # Create plots
+            print("\nCreating plots for annual mean")
+            make_benchmark_drydep_plots(
+                ref,
+                gcc_vs_gcc_refstr,
+                dev,
+                gcc_vs_gcc_devstr,
+                dst=gcc_vs_gcc_resultsdir,
+                subdst="AnnualMean",
+                time_mean=True,
+                weightsdir=config["paths"]["weights_dir"],
+                overwrite=True,
+                spcdb_dir=spcdb_dir,
+                n_job=config["options"]["n_cores"],
+                varlist=drydepvel_species()
+            )
+
+            # --------------------------------------------------------------
+            # GCC vs GCC drydep plots: Seasonal
+            # --------------------------------------------------------------
+            for mon in range(bmk_n_months):
+                print(f"\nCreating plots for {bmk_mon_strs[mon]}")
+
+                # Create plots
+                mon_ind = bmk_mon_inds[mon]
+                make_benchmark_drydep_plots(
+                    ref[mon_ind],
+                    gcc_vs_gcc_refstr,
+                    dev[mon_ind],
+                    gcc_vs_gcc_devstr,
+                    dst=gcc_vs_gcc_resultsdir,
+                    subdst=bmk_mon_yr_strs_dev[mon],
+                    weightsdir=config["paths"]["weights_dir"],
+                    overwrite=True,
+                    spcdb_dir=spcdb_dir,
+                    n_job=config["options"]["n_cores"],
+                    varlist=drydepvel_species()
+                )
+
+        # ==================================================================
         # GCC vs GCC mass tables
         # ==================================================================
         if config["options"]["outputs"]["mass_table"]:
             print("\n%%% Creating GCC vs. GCC mass tables %%%")
 
             def gcc_vs_gcc_mass_table(mon):
                 """
@@ -670,15 +673,15 @@
                 devpath = get_filepath(
                     gcc_vs_gcc_devrstdir,
                     "Restart",
                     bmk_mons_dev[mon]
                 )
 
                 # Create tables
-                bmk.make_benchmark_mass_tables(
+                make_benchmark_mass_tables(
                     refpath,
                     gcc_vs_gcc_refstr,
                     devpath,
                     gcc_vs_gcc_devstr,
                     dst=gcc_vs_gcc_tablesdir,
                     subdst=bmk_mon_yr_strs_dev[mon],
                     label=f"at 01{bmk_mon_yr_strs_dev[mon]}",
@@ -718,15 +721,15 @@
                 devpath = get_filepath(
                     gcc_vs_gcc_devdir,
                     "Budget",
                     bmk_mons_dev[mon]
                 )
 
                 # Create tables
-                bmk.make_benchmark_operations_budget(
+                make_benchmark_operations_budget(
                     config["data"]["ref"]["gcc"]["version"],
                     refpath,
                     config["data"]["dev"]["gcc"]["version"],
                     devpath,
                     sec_per_month_ref[mon],
                     sec_per_month_dev[mon],
                     benchmark_type=bmk_type,
@@ -761,15 +764,15 @@
             devspc = get_filepaths(
                 gcc_vs_gcc_devdir,
                 "SpeciesConc",
                 all_months_dev
             )[0]
 
             # Compute tables
-            bmk.make_benchmark_aerosol_tables(
+            make_benchmark_aerosol_tables(
                 gcc_vs_gcc_devdir,
                 devaero,
                 devspc,
                 devmet,
                 config["data"]["dev"]["gcc"]["version"],
                 bmk_year_dev,
                 days_per_month_dev,
@@ -779,15 +782,15 @@
             )
 
         # ==================================================================
         # GCC vs GCC Ox budget table
         # ==================================================================
         if config["options"]["outputs"]["Ox_budget_table"]:
             print("\n%%% Creating GCC vs. GCC Ox budget table %%%")
-            ox.global_ox_budget(
+            global_ox_budget(
                 config["data"]["dev"]["gcc"]["version"],
                 gcc_vs_gcc_devdir,
                 gcc_vs_gcc_devrstdir,
                 bmk_year_dev,
                 dst=gcc_vs_gcc_tablesdir,
                 overwrite=True,
                 spcdb_dir=spcdb_dir,
@@ -803,25 +806,53 @@
             dev = get_filepaths(
                 gcc_vs_gcc_devdir,
                 "AdvFluxVert",
                 all_months_dev
             )[0]
 
             # Compute table
-            ste.make_benchmark_ste_table(
+            make_benchmark_ste_table(
                 config["data"]["dev"]["gcc"]["version"],
                 dev,
                 bmk_year_dev,
                 dst=gcc_vs_gcc_tablesdir,
                 bmk_type=bmk_type,
                 species=["O3"],
                 overwrite=True,
             )
 
         # ==================================================================
+        # GCC vs. GCC Benchmark Timing Table
+        # ==================================================================
+        if config["options"]["outputs"]["timing_table"]:
+            print("\n%%% Creating GCC vs. GCC Benchmark Timing table %%%")
+
+            # Filepaths
+            ref = get_log_filepaths(
+                gcc_vs_gcc_reflogdir,
+                config["data"]["ref"]["gcc"]["logs_template"],
+                all_months_ref
+            )
+            dev = get_log_filepaths(
+                gcc_vs_gcc_devlogdir,
+                config["data"]["dev"]["gcc"]["logs_template"],
+                all_months_dev
+            )
+
+            # Create the table
+            make_benchmark_gcclassic_timing_table(
+                ref,
+                config["data"]["ref"]["gcc"]["version"],
+                dev,
+                config["data"]["dev"]["gcc"]["version"],
+                dst=gcc_vs_gcc_tablesdir,
+                overwrite=True,
+            )
+
+        # ==================================================================
         # GCC vs GCC Global mean OH, MCF Lifetime, CH4 Lifetime
         # ==================================================================
         if config["options"]["outputs"]["OH_metrics"]:
             print("\n%%% Creating GCC vs. GCC OH metrics %%%")
 
             # Filepaths
             ref = get_filepaths(
@@ -832,15 +863,15 @@
             dev = get_filepaths(
                 gcc_vs_gcc_devdir,
                 "Metrics",
                 all_months_dev
             )[0]
 
             # Create the OH Metrics table
-            oh.make_benchmark_oh_metrics(
+            make_benchmark_oh_metrics(
                 ref,
                 config["data"]["ref"]["gcc"]["version"],
                 dev,
                 config["data"]["dev"]["gcc"]["version"],
                 dst=gcc_vs_gcc_tablesdir,
                 overwrite=True,
                 spcdb_dir=spcdb_dir,
@@ -860,26 +891,38 @@
             )[0]
             dev = get_filepaths(
                 gcc_vs_gcc_devdir,
                 "SpeciesConc",
                 all_months_dev
             )[0]
 
-            # Plot models vs. observations (O3 for now)
-            mvo.make_benchmark_models_vs_obs_plots(
-                config["paths"]["obs_data_dir"],
+            # Plot models vs. observations
+            make_benchmark_models_vs_obs_plots(
+                config["paths"]["obs_data"]["ebas_o3"]["data_dir"],
+                config["paths"]["obs_data"]["ebas_o3"]["data_label"],
                 ref,
                 config["data"]["ref"]["gcc"]["version"],
                 dev,
                 config["data"]["dev"]["gcc"]["version"],
                 dst=gcc_vs_gcc_models_vs_obs_dir,
                 overwrite=True,
                 verbose=False
             )
 
+            # Plot models vs. sondes
+            make_benchmark_models_vs_sondes_plots(
+                sondes_data_file,
+                sondes_site_file,
+                ref,
+                config["data"]["ref"]["gcc"]["version"],
+                dev,
+                config["data"]["dev"]["gcc"]["version"],
+                dst=gcc_vs_gcc_models_vs_obs_dir,
+                overwrite=True,
+            )
 
     # %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
     # Create GCHP vs GCC benchmark plots and tables
     #
     # (1) GCHP (Dev) and GCC (Ref) use the same benchmark year.
     # (2) The GCC version in "GCHP vs GCC" is the Dev of "GCC vs GCC".
     # %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
@@ -925,15 +968,15 @@
                 "SpeciesConc",
                 all_months_gchp_dev,
                 is_gchp=True
             )[0]
 
             # Create plots
             print("\nCreating plots for annual mean")
-            bmk.make_benchmark_conc_plots(
+            make_benchmark_conc_plots(
                 ref,
                 gchp_vs_gcc_refstr,
                 dev,
                 gchp_vs_gcc_devstr,
                 refmet=refmet,
                 devmet=devmet,
                 dst=gchp_vs_gcc_resultsdir,
@@ -950,15 +993,15 @@
             # GCHP vs GCC species concentration plots: Seasonal
             # --------------------------------------------------------------
             for mon in range(bmk_n_months):
                 print(f"\nCreating plots for {bmk_mon_strs[mon]}")
 
                 # Create plots
                 mon_ind = bmk_mon_inds[mon]
-                bmk.make_benchmark_conc_plots(
+                make_benchmark_conc_plots(
                     ref[mon_ind],
                     gchp_vs_gcc_refstr,
                     dev[mon_ind],
                     gchp_vs_gcc_devstr,
                     refmet=refmet[mon_ind],
                     devmet=devmet[mon_ind],
                     dst=gchp_vs_gcc_resultsdir,
@@ -993,15 +1036,15 @@
                 "Emissions",
                 all_months_gchp_dev,
                 is_gchp=True
             )[0]
 
             # Create plots
             print("\nCreating plots for annual mean")
-            bmk.make_benchmark_emis_plots(
+            make_benchmark_emis_plots(
                 ref,
                 gchp_vs_gcc_refstr,
                 dev,
                 gchp_vs_gcc_devstr,
                 dst=gchp_vs_gcc_resultsdir,
                 subdst="AnnualMean",
                 time_mean=True,
@@ -1020,15 +1063,15 @@
             # GCHP vs GCC emissions plots: Seasonal
             # --------------------------------------------------------------
             for mon in range(bmk_n_months):
                 print(f"\nCreating plots for {bmk_mon_strs[mon]}")
 
                 # Create plots
                 mon_ind = bmk_mon_inds[mon]
-                bmk.make_benchmark_emis_plots(
+                make_benchmark_emis_plots(
                     ref[mon_ind],
                     gchp_vs_gcc_refstr,
                     dev[mon_ind],
                     gchp_vs_gcc_devstr,
                     dst=gchp_vs_gcc_resultsdir,
                     subdst=bmk_mon_yr_strs_dev[mon],
                     weightsdir=config["paths"]["weights_dir"],
@@ -1058,15 +1101,15 @@
                 gchp_vs_gcc_devdir,
                 "Emissions",
                 all_months_gchp_dev,
                 is_gchp=True
             )[0]
 
             # Create emissions table that spans entire year
-            bmk.make_benchmark_emis_tables(
+            make_benchmark_emis_tables(
                 ref,
                 gchp_vs_gcc_refstr,
                 dev,
                 gchp_vs_gcc_devstr,
                 devmet=devmet,
                 dst=gchp_vs_gcc_resultsdir,
                 ref_interval=sec_per_month_ref,
@@ -1097,15 +1140,15 @@
                 "JValues",
                 all_months_gchp_dev,
                 is_gchp=True
             )[0]
 
             # Create plots
             print("\nCreating plots for annual mean")
-            bmk.make_benchmark_jvalue_plots(
+            make_benchmark_jvalue_plots(
                 ref,
                 gchp_vs_gcc_refstr,
                 dev,
                 gchp_vs_gcc_devstr,
                 dst=gchp_vs_gcc_resultsdir,
                 subdst="AnnualMean",
                 time_mean=True,
@@ -1119,15 +1162,15 @@
             # GCHP vs GCC J-values plots: Seasonal
             # --------------------------------------------------------------
             for mon in range(bmk_n_months):
                 print(f"\nCreating plots for {bmk_mon_strs[mon]}")
 
                 # Create plots
                 mon_ind = bmk_mon_inds[mon]
-                bmk.make_benchmark_jvalue_plots(
+                make_benchmark_jvalue_plots(
                     ref[mon_ind],
                     gchp_vs_gcc_refstr,
                     dev[mon_ind],
                     gchp_vs_gcc_devstr,
                     dst=gchp_vs_gcc_resultsdir,
                     subdst=bmk_mon_yr_strs_dev[mon],
                     weightsdir=config["paths"]["weights_dir"],
@@ -1157,15 +1200,15 @@
                 "Aerosols",
                 all_months_gchp_dev,
                 is_gchp=True
             )[0]
 
             # Create plots
             print("\nCreating plots for annual mean")
-            bmk.make_benchmark_aod_plots(
+            make_benchmark_aod_plots(
                 ref,
                 gchp_vs_gcc_refstr,
                 dev,
                 gchp_vs_gcc_devstr,
                 dst=gchp_vs_gcc_resultsdir,
                 subdst="AnnualMean",
                 time_mean=True,
@@ -1179,28 +1222,90 @@
             # GCHP vs GCC column AOD plots: Seasonal
             # --------------------------------------------------------------
             for mon in range(bmk_n_months):
                 print(f"\nCreating plots for {bmk_mon_strs[mon]}")
 
                 # Create plots
                 mon_ind = bmk_mon_inds[mon]
-                bmk.make_benchmark_aod_plots(
+                make_benchmark_aod_plots(
                     ref[mon_ind],
                     gchp_vs_gcc_refstr,
                     dev[mon_ind],
                     gchp_vs_gcc_devstr,
                     dst=gchp_vs_gcc_resultsdir,
                     subdst=bmk_mon_yr_strs_dev[mon],
                     weightsdir=config["paths"]["weights_dir"],
                     overwrite=True,
                     spcdb_dir=spcdb_dir,
                     n_job=config["options"]["n_cores"]
                 )
 
         # ==================================================================
+        # GCHP vs. GCC drydep plots
+        # ==================================================================
+        if config["options"]["outputs"]["plot_drydep"]:
+            print("\n%%% Creating GCHP vs. GCC drydep plots %%%")
+
+            # --------------------------------------------------------------
+            # GCHP vs GCC drydep plots: Annual mean
+            # --------------------------------------------------------------
+
+            # Filepaths
+            ref = get_filepaths(
+                gchp_vs_gcc_refdir,
+                "DryDep",
+                all_months_dev
+            )[0]
+            dev = get_filepaths(
+                gchp_vs_gcc_devdir,
+                "DryDep",
+                all_months_gchp_dev,
+                is_gchp=True
+            )[0]
+
+            # Create plots
+            print("\nCreating plots for annual mean")
+            make_benchmark_drydep_plots(
+                ref,
+                gchp_vs_gcc_refstr,
+                dev,
+                gchp_vs_gcc_devstr,
+                dst=gchp_vs_gcc_resultsdir,
+                subdst="AnnualMean",
+                time_mean=True,
+                weightsdir=config["paths"]["weights_dir"],
+                overwrite=True,
+                spcdb_dir=spcdb_dir,
+                n_job=config["options"]["n_cores"],
+                varlist=drydepvel_species()
+            )
+
+            # --------------------------------------------------------------
+            # GCHP vs GCC drydep plots: Seasonal
+            # --------------------------------------------------------------
+            for mon in range(bmk_n_months):
+                print(f"\nCreating plots for {bmk_mon_strs[mon]}")
+
+                # Create plots
+                mon_ind = bmk_mon_inds[mon]
+                make_benchmark_drydep_plots(
+                    ref[mon_ind],
+                    gchp_vs_gcc_refstr,
+                    dev[mon_ind],
+                    gchp_vs_gcc_devstr,
+                    dst=gchp_vs_gcc_resultsdir,
+                    subdst=bmk_mon_yr_strs_dev[mon],
+                    weightsdir=config["paths"]["weights_dir"],
+                    overwrite=True,
+                    spcdb_dir=spcdb_dir,
+                    n_job=config["options"]["n_cores"],
+                    varlist=drydepvel_species()
+                )
+
+        # ==================================================================
         # GCHP vs GCC global mass tables
         # ==================================================================
         if config["options"]["outputs"]["mass_table"]:
             print("\n%%% Creating GCHP vs. GCC mass tables %%%")
 
             def gchp_vs_gcc_mass_table(mon):
                 """
@@ -1232,15 +1337,15 @@
                     is_gchp=True,
                     gchp_res=config["data"]["dev"]["gchp"]["resolution"],
                     gchp_is_pre_14_0=config["data"]["dev"]["gchp"][
                         "is_pre_14.0"]
                 )
 
                 # Create tables
-                bmk.make_benchmark_mass_tables(
+                make_benchmark_mass_tables(
                     refpath,
                     gchp_vs_gcc_refstr,
                     devpath,
                     gchp_vs_gcc_devstr,
                     dst=gchp_vs_gcc_tablesdir,
                     subdst=bmk_mon_yr_strs_dev[mon],
                     label=f"at 01{bmk_mon_yr_strs_dev[mon]}",
@@ -1282,15 +1387,15 @@
                     gchp_vs_gcc_devdir,
                     "Budget",
                     bmk_mons_gchp_dev[mon],
                     is_gchp=True
                 )
 
                 # Create tables
-                bmk.make_benchmark_operations_budget(
+                make_benchmark_operations_budget(
                     config["data"]["dev"]["gcc"]["version"],
                     refpath,
                     config["data"]["dev"]["gchp"]["version"],
                     devpath,
                     bmk_sec_per_month_dev[mon],
                     bmk_sec_per_month_dev[mon],
                     benchmark_type=bmk_type,
@@ -1335,15 +1440,15 @@
                 gchp_vs_gcc_devdir,
                 "SpeciesConc",
                 all_months_gchp_dev,
                 is_gchp=True
             )[0]
 
             # Create tables
-            bmk.make_benchmark_aerosol_tables(
+            make_benchmark_aerosol_tables(
                 gchp_vs_gcc_devdir,
                 devaero,
                 devspc,
                 devmet,
                 config["data"]["dev"]["gchp"]["version"],
                 bmk_year_dev,
                 days_per_month_dev,
@@ -1356,26 +1461,26 @@
         # ==================================================================
         # GCHP vs GCC Ox budget tables
         # ==================================================================
         if config["options"]["outputs"]["Ox_budget_table"]:
             print("\n%%% Creating GCHP vs. GCC Ox budget tables %%%")
 
             # Compute Ox budget table for GCC
-            ox.global_ox_budget(
+            global_ox_budget(
                 config["data"]["dev"]["gcc"]["version"],
                 gcc_vs_gcc_devdir,
                 gcc_vs_gcc_devrstdir,
                 bmk_year_dev,
                 dst=gcc_vs_gcc_tablesdir,
                 overwrite=True,
                 spcdb_dir=spcdb_dir
             )
 
             # Compute Ox budget table for GCHP
-            ox.global_ox_budget(
+            global_ox_budget(
                 config["data"]["dev"]["gchp"]["version"],
                 gchp_vs_gcc_devdir,
                 gchp_vs_gcc_devrstdir,
                 bmk_year_dev,
                 dst=gchp_vs_gcc_tablesdir,
                 overwrite=True,
                 spcdb_dir=spcdb_dir,
@@ -1400,15 +1505,15 @@
                 gchp_vs_gcc_devdir,
                 "Metrics",
                 all_months_gchp_dev,
                 is_gchp=True
             )[0]
 
             # Create table
-            oh.make_benchmark_oh_metrics(
+            make_benchmark_oh_metrics(
                 ref,
                 config["data"]["dev"]["gcc"]["version"],
                 dev,
                 config["data"]["dev"]["gchp"]["version"],
                 dst=gchp_vs_gcc_tablesdir,
                 overwrite=True,
                 spcdb_dir=spcdb_dir,
@@ -1435,33 +1540,47 @@
             dev = get_filepaths(
                 gchp_vs_gcc_devdir,
                 "SpeciesConc",
                 all_months_gchp_dev,
                 is_gchp=True
             )[0]
 
-            # Plot models vs. observations (O3 for now)
-            mvo.make_benchmark_models_vs_obs_plots(
-                config["paths"]["obs_data_dir"],
+            # Plot models vs. observations
+            make_benchmark_models_vs_obs_plots(
+                config["paths"]["obs_data"]["ebas_o3"]["data_dir"],
+                config["paths"]["obs_data"]["ebas_o3"]["data_label"],
                 ref,
                 config["data"]["dev"]["gcc"]["version"],
                 dev,
                 config["data"]["dev"]["gchp"]["version"],
                 dst=gchp_vs_gcc_models_vs_obs_dir,
                 overwrite=True,
                 verbose=False
             )
 
+            # Plot models vs. sondes
+            make_benchmark_models_vs_sondes_plots(
+                sondes_data_file,
+                sondes_site_file,
+                ref,
+                config["data"]["dev"]["gcc"]["version"],
+                dev,
+                config["data"]["dev"]["gchp"]["version"],
+                dst=gchp_vs_gcc_models_vs_obs_dir,
+                overwrite=True,
+            )
+
+
     # %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
     # Create GCHP vs GCHP benchmark plots and tables
     # %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
     if config["options"]["comparisons"]["gchp_vs_gchp"]["run"]:
 
         # ==================================================================
-        # GCHP vs GCC filepaths for StateMet collection data
+        # GCHP vs GCHP filepaths for StateMet collection data
         # ==================================================================
         refmet = get_filepaths(
             gchp_vs_gchp_refdir,
             "StateMet",
             all_months_gchp_ref,
             is_gchp=True
         )[0]
@@ -1504,15 +1623,15 @@
                 "SpeciesConc",
                 all_months_gchp_dev,
                 is_gchp=True
             )[0]
 
             # Create plots
             print("\nCreating plots for annual mean")
-            bmk.make_benchmark_conc_plots(
+            make_benchmark_conc_plots(
                 ref,
                 gchp_vs_gchp_refstr,
                 dev,
                 gchp_vs_gchp_devstr,
                 refmet=refmet,
                 devmet=devmet,
                 cmpres=cmpres,
@@ -1532,15 +1651,15 @@
             # GCHP vs GCHP species concentration plots: Seasonal
             # --------------------------------------------------------------
             for mon in range(bmk_n_months):
                 print(f"\nCreating plots for {bmk_mon_strs[mon]}")
 
                 # Create plots
                 mon_ind = bmk_mon_inds[mon]
-                bmk.make_benchmark_conc_plots(
+                make_benchmark_conc_plots(
                     ref[mon_ind],
                     gchp_vs_gchp_refstr,
                     dev[mon_ind],
                     gchp_vs_gchp_devstr,
                     cmpres=cmpres,
                     refmet=refmet[mon_ind],
                     devmet=devmet[mon_ind],
@@ -1577,15 +1696,15 @@
                 "Emissions",
                 all_months_gchp_dev,
                 is_gchp=True
             )[0]
 
             # Create plots
             print("\nCreating plots for annual mean")
-            bmk.make_benchmark_emis_plots(
+            make_benchmark_emis_plots(
                 ref,
                 gchp_vs_gchp_refstr,
                 dev,
                 gchp_vs_gchp_devstr,
                 dst=gchp_vs_gchp_resultsdir,
                 subdst="AnnualMean",
                 cmpres=cmpres,
@@ -1605,15 +1724,15 @@
             # GCHP vs GCHP species concentration plots: Seasonal
             # --------------------------------------------------------------
             for mon in range(bmk_n_months):
                 print(f"\nCreating plots for {bmk_mon_strs[mon]}")
 
                 # Create plots
                 mon_ind = bmk_mon_inds[mon]
-                bmk.make_benchmark_emis_plots(
+                make_benchmark_emis_plots(
                     ref[mon_ind],
                     gchp_vs_gchp_refstr,
                     dev[mon_ind],
                     gchp_vs_gchp_devstr,
                     dst=gchp_vs_gchp_resultsdir,
                     cmpres=cmpres,
                     subdst=bmk_mon_yr_strs_dev[mon],
@@ -1645,15 +1764,15 @@
                 gchp_vs_gchp_devdir,
                 "Emissions",
                 all_months_gchp_dev,
                 is_gchp=True
             )[0]
 
             # Create table
-            bmk.make_benchmark_emis_tables(
+            make_benchmark_emis_tables(
                 ref,
                 gchp_vs_gchp_refstr,
                 dev,
                 gchp_vs_gchp_devstr,
                 refmet=refmet,
                 devmet=devmet,
                 dst=gchp_vs_gchp_resultsdir,
@@ -1686,15 +1805,15 @@
                 "JValues",
                 all_months_gchp_dev,
                 is_gchp=True
             )[0]
 
             # Create plots
             print("\nCreating plots for annual mean")
-            bmk.make_benchmark_jvalue_plots(
+            make_benchmark_jvalue_plots(
                 ref,
                 gchp_vs_gchp_refstr,
                 dev,
                 gchp_vs_gchp_devstr,
                 dst=gchp_vs_gchp_resultsdir,
                 subdst='AnnualMean',
                 cmpres=cmpres,
@@ -1709,15 +1828,15 @@
             # GCHP vs GCHP J-values plots: Seasonal
             # --------------------------------------------------------------
             for mon in range(bmk_n_months):
                 print(f"\nCreating plots for {bmk_mon_strs[mon]}")
 
                 # Create plots
                 mon_ind = bmk_mon_inds[mon]
-                bmk.make_benchmark_jvalue_plots(
+                make_benchmark_jvalue_plots(
                     ref[mon_ind],
                     gchp_vs_gchp_refstr,
                     dev[mon_ind],
                     gchp_vs_gchp_devstr,
                     dst=gchp_vs_gchp_resultsdir,
                     subdst=bmk_mon_yr_strs_dev[mon],
                     cmpres=cmpres,
@@ -1749,15 +1868,15 @@
                 "Aerosols",
                 all_months_gchp_dev,
                 is_gchp=True
             )[0]
 
             # Create plots
             print("\nCreating plots for annual mean")
-            bmk.make_benchmark_aod_plots(
+            make_benchmark_aod_plots(
                 ref,
                 gchp_vs_gchp_refstr,
                 dev,
                 gchp_vs_gchp_devstr,
                 dst=gchp_vs_gchp_resultsdir,
                 subdst="AnnualMean",
                 cmpres=cmpres,
@@ -1772,29 +1891,94 @@
             # GCHP vs GCHP column AOD plots: Seasonal
             # --------------------------------------------------------------
             for mon in range(bmk_n_months):
                 print(f"\nCreating plots for {bmk_mon_strs[mon]}")
 
                 # Create plots
                 mon_ind = bmk_mon_inds[mon]
-                bmk.make_benchmark_aod_plots(
+                make_benchmark_aod_plots(
                     ref[mon_ind],
                     gchp_vs_gchp_refstr,
                     dev[mon_ind],
                     gchp_vs_gchp_devstr,
                     dst=gchp_vs_gchp_resultsdir,
                     subdst=bmk_mon_yr_strs_dev[mon],
                     cmpres=cmpres,
                     weightsdir=config["paths"]["weights_dir"],
                     overwrite=True,
                     spcdb_dir=spcdb_dir,
                     n_job=config["options"]["n_cores"]
                 )
 
         # ==================================================================
+        # GCHP vs GCHP drydep plots
+        # ==================================================================
+        if config["options"]["outputs"]["plot_drydep"]:
+            print("\n%%% Creating GCHP vs. GCHP drydep plots %%%")
+
+            # --------------------------------------------------------------
+            # GCHP vs GCHP drydep: Annual Mean
+            # --------------------------------------------------------------
+
+            # Filepaths
+            ref = get_filepaths(
+                gchp_vs_gchp_refdir,
+                "DryDep",
+                all_months_gchp_ref,
+                is_gchp=True
+            )[0]
+            dev = get_filepaths(
+                gchp_vs_gchp_devdir,
+                "DryDep",
+                all_months_gchp_dev,
+                is_gchp=True
+            )[0]
+
+            # Create plots
+            print("\nCreating plots for annual mean")
+            make_benchmark_drydep_plots(
+                ref,
+                gchp_vs_gchp_refstr,
+                dev,
+                gchp_vs_gchp_devstr,
+                dst=gchp_vs_gchp_resultsdir,
+                subdst="AnnualMean",
+                cmpres=cmpres,
+                time_mean=True,
+                weightsdir=config["paths"]["weights_dir"],
+                overwrite=True,
+                spcdb_dir=spcdb_dir,
+                n_job=config["options"]["n_cores"],
+                varlist=drydepvel_species()
+            )
+
+            # --------------------------------------------------------------
+            # GCHP vs GCHP drydep plots: Seasonal
+            # --------------------------------------------------------------
+            for mon in range(bmk_n_months):
+                print(f"\nCreating plots for {bmk_mon_strs[mon]}")
+
+                # Create plots
+                mon_ind = bmk_mon_inds[mon]
+                make_benchmark_drydep_plots(
+                    ref[mon_ind],
+                    gchp_vs_gchp_refstr,
+                    dev[mon_ind],
+                    gchp_vs_gchp_devstr,
+                    dst=gchp_vs_gchp_resultsdir,
+                    subdst=bmk_mon_yr_strs_dev[mon],
+                    cmpres=cmpres,
+                    weightsdir=config["paths"]["weights_dir"],
+                    overwrite=True,
+                    spcdb_dir=spcdb_dir,
+                    n_job=config["options"]["n_cores"],
+                    varlist=drydepvel_species()
+                )
+
+        # ==================================================================
         # GCHP vs GCHP global mass tables
         # ==================================================================
         if config["options"]["outputs"]["mass_table"]:
             print("\n%%% Creating GCHP vs. GCHP mass tables %%%")
 
             def gchp_vs_gchp_mass_table(mon):
                 """
@@ -1826,30 +2010,30 @@
                 # KLUDGE: ewl, bmy, 13 Oct 2022
                 # Use last GCHP restart file, which has correct area values
                 refareapath = get_filepath(
                     gchp_vs_gchp_refrstdir,
                     "Restart",
                     bmk_end_ref,
                     is_gchp=True,
-                    gchp_res=config["data"]["dev"]["gchp"]["resolution"],
-                    gchp_is_pre_14_0=config["data"]["dev"]["gchp"][
+                    gchp_res=config["data"]["ref"]["gchp"]["resolution"],
+                    gchp_is_pre_14_0=config["data"]["ref"]["gchp"][
                         "is_pre_14.0"]
                 )
                 devareapath = get_filepath(
                     gchp_vs_gchp_devrstdir,
                     "Restart",
                     bmk_end_dev,
                     is_gchp=True,
                     gchp_res=config["data"]["dev"]["gchp"]["resolution"],
                     gchp_is_pre_14_0=config["data"]["dev"]["gchp"][
                         "is_pre_14.0"]
                 )
 
                 # Create tables
-                bmk.make_benchmark_mass_tables(
+                make_benchmark_mass_tables(
                     refpath,
                     gchp_vs_gchp_refstr,
                     devpath,
                     gchp_vs_gchp_devstr,
                     dst=gchp_vs_gchp_tablesdir,
                     subdst=bmk_mon_yr_strs_dev[mon],
                     label=f"at 01{bmk_mon_yr_strs_dev[mon]}",
@@ -1894,15 +2078,15 @@
                     gchp_vs_gchp_devdir,
                     "Budget",
                     bmk_mons_gchp_dev[mon],
                     is_gchp=True
                 )
 
                 # Compute tables
-                bmk.make_benchmark_operations_budget(
+                make_benchmark_operations_budget(
                     config["data"]["ref"]["gchp"]["version"],
                     refpath,
                     config["data"]["dev"]["gchp"]["version"],
                     devpath,
                     bmk_sec_per_month_ref[mon],
                     bmk_sec_per_month_dev[mon],
                     benchmark_type=bmk_type,
@@ -1947,15 +2131,15 @@
                 gchp_vs_gchp_devdir,
                 "SpeciesConc",
                 all_months_gchp_dev,
                 is_gchp=True
             )[0]
 
             # Create tables
-            bmk.make_benchmark_aerosol_tables(
+            make_benchmark_aerosol_tables(
                 gchp_vs_gchp_devdir,
                 devaero,
                 devspc,
                 devmet,
                 config["data"]["dev"]["gchp"]["version"],
                 bmk_year_dev,
                 days_per_month_dev,
@@ -1968,15 +2152,15 @@
         # ==================================================================
         # GCHP vs GCHP Ox budget tables
         # ==================================================================
         if config["options"]["outputs"]["Ox_budget_table"]:
             print("\n%%% Creating GCHP Ox budget table %%%")
 
             # Compute Ox budget table for GCHP
-            ox.global_ox_budget(
+            global_ox_budget(
                 config["data"]["dev"]["gchp"]["version"],
                 gchp_vs_gchp_devdir,
                 gchp_vs_gchp_devrstdir,
                 bmk_year_dev,
                 dst=gchp_vs_gchp_tablesdir,
                 overwrite=True,
                 spcdb_dir=spcdb_dir,
@@ -2002,15 +2186,15 @@
                 gchp_vs_gchp_devdir,
                 "Metrics",
                 all_months_gchp_dev,
                 is_gchp=True
             )[0]
 
             # Create the OH Metrics table
-            oh.make_benchmark_oh_metrics(
+            make_benchmark_oh_metrics(
                 ref,
                 config["data"]["ref"]["gchp"]["version"],
                 dev,
                 config["data"]["dev"]["gchp"]["version"],
                 dst=gchp_vs_gchp_tablesdir,
                 overwrite=True,
                 spcdb_dir=spcdb_dir,
@@ -2019,45 +2203,90 @@
         # ==================================================================
         # GCHP Strat-Trop Exchange
         # ==================================================================
         if config["options"]["outputs"]["ste_table"]:
             print("\n%%% Skipping GCHP vs. GCHP Strat-Trop Exchange table %%%")
 
         # ==================================================================
+        # GCHP vs. GCHP Benchmark Timing Table
+        # ==================================================================
+        if config["options"]["outputs"]["timing_table"]:
+            print("\n%%% Creating GCHP vs. GCHP Benchmark Timing table %%%")
+
+            # Filepaths
+            # NOTE: Usually the GCHP 1-yr benchmark is run as
+            # one job, so we only need to take the 1st log file.
+            ref = get_log_filepaths(
+                gchp_vs_gchp_reflogdir,
+                config["data"]["ref"]["gchp"]["logs_template"],
+                all_months_gchp_ref,
+            )[0]
+            dev = get_log_filepaths(
+                gchp_vs_gchp_devlogdir,
+                config["data"]["dev"]["gchp"]["logs_template"],
+                all_months_gchp_dev,
+            )[0]
+
+            # Create the table
+            make_benchmark_gchp_timing_table(
+                ref,
+                config["data"]["ref"]["gchp"]["version"],
+                dev,
+                config["data"]["dev"]["gchp"]["version"],
+                dst=gchp_vs_gchp_tablesdir,
+                overwrite=True,
+            )
+
+        # ==================================================================
         # GCHP vs GCHP Model vs. Observations plots
         # ==================================================================
         if config["options"]["outputs"]["plot_models_vs_obs"]:
             print("\n%%% Creating GCHP vs. GCHP models vs. obs. plots %%%")
 
             # Filepaths
+            # NOTE: If the GCHP benchmark is done in one-shot
+            # then you need the [0] after the call to get_filepaths.
             ref = get_filepaths(
                 gchp_vs_gchp_refdir,
                 "SpeciesConc",
                 all_months_gchp_ref,
                 is_gchp=True
             )[0]
             dev = get_filepaths(
                 gchp_vs_gchp_devdir,
                 "SpeciesConc",
                 all_months_gchp_dev,
                 is_gchp=True
             )[0]
 
-            # Plot models vs. observations (O3 for now)
-            mvo.make_benchmark_models_vs_obs_plots(
-                config["paths"]["obs_data_dir"],
+            # Plot models vs. observations
+            make_benchmark_models_vs_obs_plots(
+                config["paths"]["obs_data"]["ebas_o3"]["data_dir"],
+                config["paths"]["obs_data"]["ebas_o3"]["data_label"],
                 ref,
                 config["data"]["ref"]["gchp"]["version"],
                 dev,
                 config["data"]["dev"]["gchp"]["version"],
                 dst=gchp_vs_gchp_models_vs_obs_dir,
                 overwrite=True,
                 verbose=False
             )
 
+            # Plot models vs. sondes
+            make_benchmark_models_vs_sondes_plots(
+                sondes_data_file,
+                sondes_site_file,
+                ref,
+                config["data"]["ref"]["gchp"]["version"],
+                dev,
+                config["data"]["dev"]["gchp"]["version"],
+                dst=gchp_vs_gchp_models_vs_obs_dir,
+                overwrite=True,
+            )
+
     # %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
     # Create GCHP vs GCC difference of differences benchmark plots
     # %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
     if config["options"]["comparisons"]["gchp_vs_gcc_diff_of_diffs"]["run"]:
 
         if config["options"]["outputs"]["plot_conc"]:
             print("\n%%% Creating GCHP vs. GCC diff-of-diffs conc plots %%%")
@@ -2090,15 +2319,15 @@
                 "SpeciesConc",
                 all_months_gchp_dev,
                 is_gchp=True
             )[0]
 
             # Create plots
             print("\nCreating plots for annual mean")
-            bmk.make_benchmark_conc_plots(
+            make_benchmark_conc_plots(
                 gcc_ref,
                 diff_of_diffs_refstr,
                 gchp_ref,
                 diff_of_diffs_devstr,
                 dst=diff_of_diffs_resultsdir,
                 subdst="AnnualMean",
                 time_mean=True,
@@ -2119,15 +2348,15 @@
             # GCHP vs GCC diff-of-diff species concentration plots: Seasonal
             # --------------------------------------------------------------
             for mon in range(bmk_n_months):
                 print(f"\nCreating plots for {bmk_mon_strs[mon]}")
 
                 # Create plots
                 mon_ind = bmk_mon_inds[mon]
-                bmk.make_benchmark_conc_plots(
+                make_benchmark_conc_plots(
                     gcc_ref[mon_ind],
                     diff_of_diffs_refstr,
                     gchp_ref[mon_ind],
                     diff_of_diffs_devstr,
                     dst=diff_of_diffs_resultsdir,
                     subdst=bmk_mon_yr_strs_dev[mon],
                     weightsdir=config["paths"]["weights_dir"],
@@ -2142,8 +2371,8 @@
                     spcdb_dir=spcdb_dir,
                     n_job=config["options"]["n_cores"]
                 )
 
     # ==================================================================
     # Print a message indicating that the benchmarks finished
     # ==================================================================
-    print("\n %%%% All requested benchmark plots/tables created! %%%%")
+    print("\n%%%% All requested benchmark plots/tables created! %%%%")
```

### Comparing `geoschem-gcpy-1.4.2/gcpy/benchmark/modules/run_1yr_tt_benchmark.py` & `geoschem_gcpy-1.5.0/gcpy/benchmark/modules/run_1yr_tt_benchmark.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,31 +6,28 @@
 
 Run this script to generate benchmark comparisons between:
 
     (1) GCC (aka GEOS-Chem "Classic") vs. GCC
     (2) GCHP vs GCC
     (3) GCHP vs GCHP
 
-You can customize this by editing the settings in the corresponding yaml
-config file (eg. 1yr_tt_benchmark.yml).
+You can customize this by editing the settings in the corresponding YAML
+configiration file (eg. 1yr_tt_benchmark.yml).
 
 To generate benchmark output:
 
-    (1) Copy the gcpy/benchmark/run_benchmark.py script and the
-        1yr_tt_benchmark.yml file anywhere you want to run the test.
+    (1) Copy the file gcpy/benchmark/config/1yr_tt_benchmark.yml
+        to a folder of your choice.
 
-    (2) Edit the 1yr_tt_benchmark.yml to point to the proper file paths
-        on your disk space.
+    (2) Edit the 1yr_tt_benchmark.yml to select the desired options
+        and to point to the proper file paths on your system.
 
-    (3) Make sure the /path/to/gcpy/benchmark is in your PYTHONPATH
-        shell environment variable.
+    (3) Run the command:
 
-    (4) Type at the command line
-
-        ./run_benchmark.py 1yr_tt_benchmark.yml
+        $ python -m gcpy.benchmark.run_benchmark.py 1yr_tt_benchmark.yml
 
 Remarks:
 
     By default, matplotlib will try to open an X window for plotting.
     If you are running this script in an environment where you do not have
     an active X display (such as in a computational queue), then you will
     need to use these commands to disable the X-window functionality.
@@ -38,122 +35,93 @@
         import os
         os.environ["QT_QPA_PLATFORM"]="offscreen"
 
     For more information, please see this issue posted at the ipython site:
 
         https://github.com/ipython/ipython/issues/10627
 
-This script corresponds with GCPy 1.4.2. Edit this version ID if releasing
+    Also, to disable matplotlib from trying to open X windows, you may
+    need to set the following environment variable in your shell:
+
+        $ export MPLBACKEND=agg
+
+This script corresponds with GCPy 1.5.0. Edit this version ID if releasing
 a new version of GCPy.
 """
 
 # ======================================================================
 # Imports and global settings (you should not need to edit these)
 # ======================================================================
 
 import os
 import warnings
-from shutil import copyfile
 from calendar import monthrange
 import numpy as np
 from joblib import Parallel, delayed
-from gcpy.util import get_filepath, get_filepaths
-from gcpy import benchmark_funcs as bmk
-import gcpy.budget_tt as ttbdg
-import gcpy.ste_flux as ste
+from gcpy.util import copy_file_to_dir, get_filepath, get_filepaths
+from gcpy.benchmark.modules.benchmark_funcs import \
+    get_species_database_dir, make_benchmark_conc_plots, \
+    make_benchmark_wetdep_plots, make_benchmark_mass_tables, \
+    make_benchmark_operations_budget
+from gcpy.benchmark.modules.budget_tt import transport_tracers_budgets
+from gcpy.benchmark.modules.ste_flux import make_benchmark_ste_table
+from gcpy.benchmark.modules.benchmark_utils import \
+    gcc_vs_gcc_dirs, gchp_vs_gcc_dirs, gchp_vs_gchp_dirs, \
+    get_log_filepaths, print_benchmark_info
+from gcpy.benchmark.modules.benchmark_scrape_gcclassic_timers import \
+    make_benchmark_gcclassic_timing_table
+from gcpy.benchmark.modules.benchmark_scrape_gchp_timers import \
+    make_benchmark_gchp_timing_table
+from gcpy.benchmark.modules.benchmark_mass_cons_table import \
+    make_benchmark_mass_conservation_table
 
 # Tell matplotlib not to look for an X-window
 os.environ["QT_QPA_PLATFORM"] = "offscreen"
 
 # Suppress annoying warning messages
 warnings.filterwarnings("ignore", category=RuntimeWarning)
 warnings.filterwarnings("ignore", category=UserWarning)
 warnings.filterwarnings("ignore", category=FutureWarning)
 
 
 def run_benchmark(config, bmk_year_ref, bmk_year_dev):
+    """Routine to create benchmark plots and tables"""
     # This script has a fixed benchmark type, year, and months
     bmk_type = config["options"]["bmk_type"]
     bmk_mon_strs = ["Jan", "Apr", "Jul", "Oct"]
     bmk_mon_inds = [0, 3, 6, 9]
     bmk_n_months = len(bmk_mon_strs)
 
     # =====================================================================
     # Path to species_database.yml
     # =====================================================================
-    spcdb_dir = bmk.get_species_database_dir(config)
+    spcdb_dir = get_species_database_dir(config)
 
     # ======================================================================
     # Data directories
     # For gchp_vs_gcc_refdir use config["data"]["dev"]["gcc"]["version"], not ref (mps, 6/27/19)
     # ======================================================================
 
-    # Diagnostic file directory paths
-    gcc_vs_gcc_refdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["ref"]["gcc"]["dir"],
-        config["data"]["ref"]["gcc"]["outputs_subdir"]
-    )
-    gcc_vs_gcc_devdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["dev"]["gcc"]["dir"],
-        config["data"]["dev"]["gcc"]["outputs_subdir"]
-    )
-    gchp_vs_gcc_refdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["dev"]["gcc"]["dir"],
-        config["data"]["dev"]["gcc"]["outputs_subdir"]
-    )
-    gchp_vs_gcc_devdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["dev"]["gchp"]["dir"],
-        config["data"]["dev"]["gchp"]["outputs_subdir"]
-    )
-    gchp_vs_gchp_refdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["ref"]["gchp"]["dir"],
-        config["data"]["ref"]["gchp"]["outputs_subdir"]
-    )
-    gchp_vs_gchp_devdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["dev"]["gchp"]["dir"],
-        config["data"]["dev"]["gchp"]["outputs_subdir"]
-    )
-
-    # Diagnostic file directory paths
-    gcc_vs_gcc_refrstdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["ref"]["gcc"]["dir"],
-        config["data"]["ref"]["gcc"]["restarts_subdir"]
-    )
-    gchp_vs_gcc_refrstdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["ref"]["gchp"]["dir"],
-        config["data"]["ref"]["gchp"]["restarts_subdir"]
-    )
-    gchp_vs_gchp_refrstdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["ref"]["gchp"]["dir"],
-        config["data"]["ref"]["gchp"]["restarts_subdir"]
-    )
-    gcc_vs_gcc_devrstdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["dev"]["gcc"]["dir"],
-        config["data"]["dev"]["gcc"]["restarts_subdir"]
-    )
-    gchp_vs_gcc_devrstdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["dev"]["gchp"]["dir"],
-        config["data"]["dev"]["gchp"]["restarts_subdir"]
-    )
-    gchp_vs_gchp_devrstdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["dev"]["gchp"]["dir"],
-        config["data"]["dev"]["gchp"]["restarts_subdir"]
-    )
+    # Diagnostics file directory paths
+    s = "outputs_subdir"
+    gcc_vs_gcc_refdir, gcc_vs_gcc_devdir = gcc_vs_gcc_dirs(config, s)
+    gchp_vs_gcc_refdir, gchp_vs_gcc_devdir = gchp_vs_gcc_dirs(config, s)
+    gchp_vs_gchp_refdir, gchp_vs_gchp_devdir = gchp_vs_gchp_dirs(config, s)
+
+    # Restart file directory paths
+    s = "restarts_subdir"
+    gcc_vs_gcc_refrstdir, gcc_vs_gcc_devrstdir = gcc_vs_gcc_dirs(config, s)
+    gchp_vs_gcc_refrstdir, gchp_vs_gcc_devrstdir = gchp_vs_gcc_dirs(config, s)
+    gchp_vs_gchp_refrstdir, gchp_vs_gchp_devrstdir = gchp_vs_gchp_dirs(config, s)
+
+    # Log file directory paths
+    s = "logs_subdir"
+    gcc_vs_gcc_reflogdir, gcc_vs_gcc_devlogdir = gcc_vs_gcc_dirs(config, s)
+    gchp_vs_gcc_reflogdir, gchp_vs_gcc_devlogdir = gchp_vs_gcc_dirs(config, s)
+    gchp_vs_gchp_reflogdir, gchp_vs_gchp_devlogdir = gchp_vs_gchp_dirs(config, s)
 
     # Directories where plots & tables will be created
     mainresultsdir = os.path.join(
         config["paths"]["results_dir"]
     )
     gcc_vs_gcc_resultsdir = os.path.join(
         mainresultsdir,
@@ -168,40 +136,32 @@
         config["options"]["comparisons"]["gchp_vs_gchp"]["dir"]
     )
 
     # Create the main results directory
     if not os.path.exists(mainresultsdir):
         os.mkdir(mainresultsdir)
 
-    # Make copy of benchmark script in results directory
-    curfile = os.path.realpath(__file__)
-    dest = os.path.join(mainresultsdir, curfile.split("/")[-1])
-    if not os.path.exists(dest):
-        copyfile(curfile, dest)
-
-    # Create results directories that don't exist,
-    # and place a copy of this file in each results directory
+    # Create results directories that don't exist, and place a copy of
+    # this file plus the YAML configuration file in each results directory.
     resdir_list = [
         gcc_vs_gcc_resultsdir,
         gchp_vs_gcc_resultsdir,
         gchp_vs_gchp_resultsdir
     ]
     comparisons_list =  [
         config["options"]["comparisons"]["gcc_vs_gcc"]["run"],
         config["options"]["comparisons"]["gchp_vs_gcc"]["run"],
         config["options"]["comparisons"]["gchp_vs_gchp"]["run"]
     ]
-    for resdir, plotting_type in zip(resdir_list, comparisons_list):
+    for (resdir, plotting_type) in zip(resdir_list, comparisons_list):
         if plotting_type and not os.path.exists(resdir):
             os.mkdir(resdir)
             if resdir in resdir_list:
-                curfile = os.path.realpath(__file__)
-                dest = os.path.join(resdir, curfile.split("/")[-1])
-                if not os.path.exists(dest):
-                    copyfile(curfile, dest)
+                copy_file_to_dir(__file__, resdir)
+                copy_file_to_dir(config["configuration_file_name"], resdir)
 
     # Tables directories
     gcc_vs_gcc_tablesdir = os.path.join(
         gcc_vs_gcc_resultsdir,
         config["options"]["comparisons"]["gcc_vs_gcc"]["tables_subdir"],
     )
     gchp_vs_gcc_tablesdir = os.path.join(
@@ -249,16 +209,14 @@
         dtype="datetime64[M]"
     )
     all_months_gchp_ref = all_months_ref
 
     # Get subset of month datetimes and seconds per month
     # for only benchmark months
     bmk_mons_ref = all_months_ref[bmk_mon_inds]
-    bmk_mons_gchp_ref = all_months_gchp_ref[bmk_mon_inds]
-    bmk_sec_per_month_ref = sec_per_month_ref[bmk_mon_inds]
 
     # Compute seconds in the Ref year
     sec_per_yr_ref = 0
     for t in range(12):
         days_in_mon = monthrange(int(bmk_year_ref), t + 1)[1]
         sec_per_yr_ref += days_in_mon * 86400.0
 
@@ -284,48 +242,25 @@
         bmk_end_dev,
         step=np.timedelta64(1, "M"),
         dtype="datetime64[M]"
     )
     all_months_gchp_dev = all_months_dev
 
     bmk_mons_dev = all_months_dev[bmk_mon_inds]
-    bmk_mons_gchp_dev = all_months_gchp_dev[bmk_mon_inds]
-    bmk_sec_per_month_dev = sec_per_month_dev[bmk_mon_inds]
 
     # Compute seconds in the Dev year
     sec_per_yr_dev = 0
     for t in range(12):
         days_in_mon = monthrange(int(bmk_year_dev), t + 1)[1]
         sec_per_yr_dev += days_in_mon * 86400.0
 
     # =======================================================================
-    # Print the list of plots & tables to the screen
+    # Print the list of plots & tables being generated
     # =======================================================================
-    print("The following plots and tables will be created for {}:".format(bmk_type))
-    if config["options"]["outputs"]["plot_conc"]:
-        print(" - Concentration plots")
-    if config["options"]["outputs"]["plot_wetdep"]:
-        print(" - Convective and large-scale wet deposition plots")
-    if config["options"]["outputs"]["rnpbbe_budget"]:
-        print(" - Radionuclides budget table")
-    if config["options"]["outputs"]["operations_budget"]:
-        print(" - Operations budget table")
-    if config["options"]["outputs"]["ste_table"]:
-        print(" - Table of strat-trop exchange")
-    if config["options"]["outputs"]["mass_table"]:
-        print(" - Table of species mass")
-    if config["options"]["outputs"]["cons_table"]:
-        print(" - Table of mass conservation")
-    print("Comparisons will be made for the following combinations:")
-    if config["options"]["comparisons"]["gcc_vs_gcc"]["run"]:
-        print(" - GCC vs GCC")
-    if config["options"]["comparisons"]["gchp_vs_gcc"]["run"]:
-        print(" - GCHP vs GCC")
-    if config["options"]["comparisons"]["gchp_vs_gchp"]["run"]:
-        print(" - GCHP vs GCHP")
+    print_benchmark_info(config)
 
     # %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
     # Create GCC vs GCC benchmark plots and tables
     # %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
     if config["options"]["comparisons"]["gcc_vs_gcc"]["run"]:
 
         # ==================================================================
@@ -365,15 +300,15 @@
             dev = get_filepaths(
                 gcc_vs_gcc_devdir,
                 collection,
                 all_months_dev
             )[0]
 
             # Create plots
-            bmk.make_benchmark_conc_plots(
+            make_benchmark_conc_plots(
                 ref,
                 gcc_vs_gcc_refstr,
                 dev,
                 gcc_vs_gcc_devstr,
                 collection=collection,
                 refmet=refmet,
                 devmet=devmet,
@@ -389,15 +324,15 @@
             )
 
             # --------------------------------------------------------------
             # GCC vs GCC species concentration plots: Seasonal
             # --------------------------------------------------------------
             for t in range(bmk_n_months):
                 mon_ind = bmk_mon_inds[t]
-                bmk.make_benchmark_conc_plots(
+                make_benchmark_conc_plots(
                     ref[mon_ind],
                     gcc_vs_gcc_refstr,
                     dev[mon_ind],
                     gcc_vs_gcc_devstr,
                     collection=collection,
                     refmet=refmet[mon_ind],
                     devmet=devmet[mon_ind],
@@ -436,15 +371,15 @@
                 dev = get_filepaths(
                     gcc_vs_gcc_devdir,
                     collection,
                     all_months_dev
                 )[0]
 
                 # Create plots
-                bmk.make_benchmark_wetdep_plots(
+                make_benchmark_wetdep_plots(
                     ref,
                     gcc_vs_gcc_refstr,
                     dev,
                     gcc_vs_gcc_devstr,
                     collection=collection,
                     refmet=refmet,
                     devmet=devmet,
@@ -459,15 +394,15 @@
                 )
 
                 # ----------------------------------------------------------
                 # GCC vs GCC wet deposition plots: Seasonal
                 # ----------------------------------------------------------
                 for t in range(bmk_n_months):
                     mon_ind = bmk_mon_inds[t]
-                    bmk.make_benchmark_wetdep_plots(
+                    make_benchmark_wetdep_plots(
                         ref[mon_ind],
                         gcc_vs_gcc_refstr,
                         dev[mon_ind],
                         gcc_vs_gcc_devstr,
                         collection=collection,
                         refmet=refmet[mon_ind],
                         devmet=devmet[mon_ind],
@@ -482,16 +417,29 @@
 
 
         # ==================================================================
         # GCC vs GCC radionuclides budget tables
         # ==================================================================
         if config["options"]["outputs"]["rnpbbe_budget"]:
             print("\n%%% Creating GCC vs. GCC radionuclides budget table %%%")
-            ttbdg.transport_tracers_budgets(
-                config["data"]["dev"]["gcc"]["dir"],
+
+            # Ref
+            transport_tracers_budgets(
+                config["data"]["ref"]["gcc"]["version"],
+                gcc_vs_gcc_refdir,
+                gcc_vs_gcc_refrstdir,
+                int(bmk_year_ref),
+                dst=gcc_vs_gcc_tablesdir,
+                overwrite=True,
+                spcdb_dir=spcdb_dir,
+            )
+
+            # Dev
+            transport_tracers_budgets(
+                config["data"]["dev"]["gcc"]["version"],
                 gcc_vs_gcc_devdir,
                 gcc_vs_gcc_devrstdir,
                 int(bmk_year_dev),
                 dst=gcc_vs_gcc_tablesdir,
                 overwrite=True,
                 spcdb_dir=spcdb_dir,
             )
@@ -516,15 +464,15 @@
                 devpath = get_filepath(
                     gcc_vs_gcc_devrstdir,
                     "Restart",
                     bmk_mons_dev[mon]
                 )
 
                 # Create tables
-                bmk.make_benchmark_mass_tables(
+                make_benchmark_mass_tables(
                     refpath,
                     gcc_vs_gcc_refstr,
                     devpath,
                     gcc_vs_gcc_devstr,
                     dst=gcc_vs_gcc_tablesdir,
                     subdst=bmk_mon_yr_strs_dev[mon],
                     label=f"at 01{bmk_mon_yr_strs_dev[mon]}",
@@ -543,15 +491,15 @@
                 results = []
                 for mon in range(bmk_n_months):
                     results.append(gcc_vs_gcc_mass_table(mon))
 
         # ==================================================================
         # GCC vs GCC operations budgets tables
         # ==================================================================
-        if config["options"]["outputs"]["operations_budget"]:
+        if config["options"]["outputs"]["ops_budget_table"]:
             print("\n%%% Creating GCC vs. GCC operations budget tables %%%")
 
             # Filepaths
             col = "Budget"
             refs = get_filepaths(
                 gcc_vs_gcc_refdir,
                 col,
@@ -560,15 +508,15 @@
             devs = get_filepaths(
                 gcc_vs_gcc_devdir,
                 col,
                 all_months_dev
             )[0]
 
             # Create table
-            bmk.make_benchmark_operations_budget(
+            make_benchmark_operations_budget(
                 config["data"]["ref"]["gcc"]["dir"],
                 refs,
                 config["data"]["dev"]["gcc"]["dir"],
                 devs,
                 sec_per_yr_ref,
                 sec_per_yr_dev,
                 benchmark_type=bmk_type,
@@ -588,31 +536,75 @@
         # GCC dev strat-trop exchange table
         # ==================================================================
         if config["options"]["outputs"]["ste_table"]:
             print("\n%%% Creating GCC vs. GCC Strat-Trop Exchange table %%%")
 
             # Diagnostic collection files to read (all 12 months)
             col = "AdvFluxVert"
+            refs = get_filepaths(
+                gcc_vs_gcc_refdir,
+                col,
+                all_months_ref
+            )[0]
             devs = get_filepaths(
                 gcc_vs_gcc_devdir,
                 col,
                 all_months_dev
             )[0]
 
-            # Make stat-trop exchange table for subset of species
-            ste.make_benchmark_ste_table(
-                config["data"]["dev"]["gcc"]["dir"],
+            # Ref
+            make_benchmark_ste_table(
+                config["data"]["ref"]["gcc"]["version"],
+                devs,
+                int(bmk_year_ref),
+                dst=gcc_vs_gcc_tablesdir,
+                bmk_type=bmk_type,
+                species=["Pb210", "Be7", "Be10"],
+                overwrite=True,
+            )
+
+            # Dev
+            make_benchmark_ste_table(
+                config["data"]["dev"]["gcc"]["version"],
                 devs,
                 int(bmk_year_dev),
                 dst=gcc_vs_gcc_tablesdir,
                 bmk_type=bmk_type,
                 species=["Pb210", "Be7", "Be10"],
                 overwrite=True,
             )
 
+        # ==================================================================
+        # GCC vs. GCC Benchmark Timing Table
+        # ==================================================================
+        if config["options"]["outputs"]["timing_table"]:
+            print("\n%%% Creating GCC vs. GCC Benchmark Timing table %%%")
+
+            # Filepaths
+            ref = get_log_filepaths(
+                gcc_vs_gcc_reflogdir,
+                config["data"]["ref"]["gcc"]["logs_template"],
+                all_months_ref
+            )
+            dev = get_log_filepaths(
+                gcc_vs_gcc_devlogdir,
+                config["data"]["dev"]["gcc"]["logs_template"],
+                all_months_dev
+            )
+
+            # Create the table
+            make_benchmark_gcclassic_timing_table(
+                ref,
+                config["data"]["ref"]["gcc"]["version"],
+                dev,
+                config["data"]["dev"]["gcc"]["version"],
+                dst=gcc_vs_gcc_tablesdir,
+                overwrite=True,
+            )
+
     # %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
     # Create GCHP vs GCC benchmark plots and tables
     # %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
     if config["options"]["comparisons"]["gchp_vs_gcc"]["run"]:
 
         # ==================================================================
         # GCHP vs GCC filepaths for StateMet collection data
@@ -656,15 +648,15 @@
                 gchp_vs_gcc_devdir,
                 collection,
                 all_months_gchp_dev,
                 is_gchp=True
             )[0]
 
             # Create plots
-            bmk.make_benchmark_conc_plots(
+            make_benchmark_conc_plots(
                 ref,
                 gchp_vs_gcc_refstr,
                 dev,
                 gchp_vs_gcc_devstr,
                 collection=collection,
                 refmet=refmet,
                 devmet=devmet,
@@ -680,15 +672,15 @@
             )
 
             # --------------------------------------------------------------
             # GCHP vs GCC species concentration plots: Seasonal
             # --------------------------------------------------------------
             for t in range(bmk_n_months):
                 mon_ind = bmk_mon_inds[t]
-                bmk.make_benchmark_conc_plots(
+                make_benchmark_conc_plots(
                     ref[mon_ind],
                     gchp_vs_gcc_refstr,
                     dev[mon_ind],
                     gchp_vs_gcc_devstr,
                     collection=collection,
                     refmet=refmet[mon_ind],
                     devmet=devmet[mon_ind],
@@ -728,15 +720,15 @@
                     gchp_vs_gcc_devdir,
                     collection,
                     all_months_gchp_dev,
                     is_gchp=True
                 )[0]
 
                 # Create plots
-                bmk.make_benchmark_wetdep_plots(
+                make_benchmark_wetdep_plots(
                     ref,
                     gchp_vs_gcc_refstr,
                     dev,
                     gchp_vs_gcc_devstr,
                     collection=collection,
                     devmet=devmet,
                     dst=gchp_vs_gcc_resultsdir,
@@ -751,15 +743,15 @@
                 )
 
                 # ----------------------------------------------------------
                 # GCHP vs GCC wet deposition plots: Seasonal
                 # ----------------------------------------------------------
                 for t in range(bmk_n_months):
                     mon_ind = bmk_mon_inds[t]
-                    bmk.make_benchmark_wetdep_plots(
+                    make_benchmark_wetdep_plots(
                         ref[mon_ind],
                         gchp_vs_gcc_refstr,
                         dev[mon_ind],
                         gchp_vs_gcc_devstr,
                         collection=collection,
                         refmet=refmet[mon_ind],
                         devmet=devmet[mon_ind],
@@ -774,16 +766,29 @@
                     )
 
         # ==================================================================
         # GCHP vs GCC radionuclides budget tables
         # ==================================================================
         if config["options"]["outputs"]["rnpbbe_budget"]:
             print("\n%%% Creating GCHP vs. GCC radionuclides budget table %%%")
-            ttbdg.transport_tracers_budgets(
-                config["data"]["dev"]["gchp"]["dir"],
+
+            # Ref
+            transport_tracers_budgets(
+                config["data"]["dev"]["gcc"]["version"],
+                gchp_vs_gcc_refdir,
+                gchp_vs_gcc_refrstdir,
+                int(bmk_year_dev),
+                dst=gchp_vs_gcc_tablesdir,
+                overwrite=True,
+                spcdb_dir=spcdb_dir,
+            )
+
+            # Dev
+            transport_tracers_budgets(
+                config["data"]["dev"]["gchp"]["version"],
                 gchp_vs_gcc_devdir,
                 gchp_vs_gcc_devrstdir,
                 int(bmk_year_dev),
                 dst=gchp_vs_gcc_tablesdir,
                 is_gchp=True,
                 gchp_res=config["data"]["dev"]["gchp"]["resolution"],
                 gchp_is_pre_14_0=config["data"]["dev"]["gchp"]["is_pre_14.0"],
@@ -826,14 +831,28 @@
                     bmk_end_dev,
                     is_gchp=True,
                     gchp_res=config["data"]["dev"]["gchp"]["resolution"],
                     gchp_is_pre_14_0=config["data"]["dev"]["gchp"][
                         "is_pre_14.0"]
                 )
 
+                # Create tables
+                make_benchmark_mass_tables(
+                    refpath,
+                    gchp_vs_gcc_refstr,
+                    devpath,
+                    gchp_vs_gcc_devstr,
+                    dst=gchp_vs_gcc_tablesdir,
+                    subdst=bmk_mon_yr_strs_dev[mon],
+                    label=f"at 01{bmk_mon_yr_strs_dev[mon]}",
+                    overwrite=True,
+                    spcdb_dir=spcdb_dir,
+                    dev_met_extra=devareapath
+                )
+
             # Create tables in parallel
             # Turn off parallelization if n_jobs==1
             if config["options"]["n_cores"] != 1:
                 results = Parallel(n_jobs=config["options"]["n_cores"])(
                     delayed(gchp_vs_gcc_mass_table)(mon) \
                     for mon in range(bmk_n_months)
                 )
@@ -841,15 +860,15 @@
                 results = []
                 for mon in range(bmk_n_months):
                     results.append(gchp_vs_gcc_mass_table(mon))
 
         # ==================================================================
         # GCHP vs GCC operations budgets tables
         # ==================================================================
-        if config["options"]["outputs"]["operations_budget"]:
+        if config["options"]["outputs"]["ops_budget_table"]:
             print("\n%%% Creating GCHP vs. GCC operations budget tables %%%")
 
             # Filepaths
             collection = "Budget"
             refs = get_filepaths(
                 gchp_vs_gcc_refdir,
                 collection,
@@ -859,15 +878,15 @@
                 gchp_vs_gcc_devdir,
                 collection,
                 all_months_gchp_dev,
                 is_gchp=True
             )[0]
 
             # Make operations budget table
-            bmk.make_benchmark_operations_budget(
+            make_benchmark_operations_budget(
                 config["data"]["dev"]["gcc"]["dir"],
                 refs,
                 config["data"]["dev"]["gchp"]["dir"],
                 devs,
                 sec_per_yr_ref,
                 sec_per_yr_dev,
                 benchmark_type=bmk_type,
@@ -933,15 +952,15 @@
                 gchp_vs_gchp_devdir,
                 collection,
                 all_months_gchp_dev,
                 is_gchp=True
             )[0]
 
             # Make concentration plots
-            bmk.make_benchmark_conc_plots(
+            make_benchmark_conc_plots(
                 ref,
                 gchp_vs_gchp_refstr,
                 dev,
                 gchp_vs_gchp_devstr,
                 collection=collection,
                 refmet=refmet,
                 devmet=devmet,
@@ -958,15 +977,15 @@
             )
 
             # --------------------------------------------------------------
             # GCHP vs GCHP species concentration plots: Seasonal
             # --------------------------------------------------------------
             for t in range(bmk_n_months):
                 mon_ind = bmk_mon_inds[t]
-                bmk.make_benchmark_conc_plots(
+                make_benchmark_conc_plots(
                     ref[mon_ind],
                     gchp_vs_gchp_refstr,
                     dev[mon_ind],
                     gchp_vs_gchp_devstr,
                     collection=collection,
                     refmet=refmet[mon_ind],
                     devmet=devmet[mon_ind],
@@ -1008,15 +1027,15 @@
                     gchp_vs_gchp_devdir,
                     collection,
                     all_months_gchp_dev,
                     is_gchp=True
                 )[0]
 
                 # Create plots
-                bmk.make_benchmark_wetdep_plots(
+                make_benchmark_wetdep_plots(
                     ref,
                     gchp_vs_gchp_refstr,
                     dev,
                     gchp_vs_gchp_devstr,
                     collection=collection,
                     refmet=refmet,
                     devmet=devmet,
@@ -1033,15 +1052,15 @@
                 )
 
                 # ----------------------------------------------------------
                 # GCHP vs GCHP wet deposition plots: Seasonal
                 # ----------------------------------------------------------
                 for t in range(bmk_n_months):
                     mon_ind = bmk_mon_inds[t]
-                    bmk.make_benchmark_wetdep_plots(
+                    make_benchmark_wetdep_plots(
                         ref[mon_ind],
                         gchp_vs_gchp_refstr,
                         dev[mon_ind],
                         gchp_vs_gchp_devstr,
                         collection=collection,
                         refmet=refmet[mon_ind],
                         devmet=devmet[mon_ind],
@@ -1057,16 +1076,32 @@
                     )
 
         # ==================================================================
         # GCHP vs GCHP radionuclides budget table
         # ==================================================================
         if config["options"]["outputs"]["rnpbbe_budget"]:
             print("\n%%% Creating GCHP vs. GCHP radionuclides budget table %%%")
-            ttbdg.transport_tracers_budgets(
-                config["data"]["dev"]["gchp"]["dir"],
+
+            # Ref
+            transport_tracers_budgets(
+                config["data"]["ref"]["gchp"]["version"],
+                gchp_vs_gchp_refdir,
+                gchp_vs_gchp_refrstdir,
+                int(bmk_year_ref),
+                dst=gchp_vs_gchp_tablesdir,
+                is_gchp=True,
+                gchp_res=config["data"]["ref"]["gchp"]["resolution"],
+                gchp_is_pre_14_0=config["data"]["ref"]["gchp"]["is_pre_14.0"],
+                overwrite=True,
+                spcdb_dir=spcdb_dir
+            )
+
+            # Dev
+            transport_tracers_budgets(
+                config["data"]["dev"]["gchp"]["version"],
                 gchp_vs_gchp_devdir,
                 gchp_vs_gchp_devrstdir,
                 int(bmk_year_dev),
                 dst=gchp_vs_gchp_tablesdir,
                 is_gchp=True,
                 gchp_res=config["data"]["dev"]["gchp"]["resolution"],
                 gchp_is_pre_14_0=config["data"]["dev"]["gchp"]["is_pre_14.0"],
@@ -1110,30 +1145,30 @@
                 # KLUDGE: ewl, bmy, 13 Oct 2022
                 # Use last GCHP restart file, which has correct area values
                 refareapath = get_filepath(
                     gchp_vs_gchp_refrstdir,
                     "Restart",
                     bmk_end_ref,
                     is_gchp=True,
-                    gchp_res=config["data"]["dev"]["gchp"]["resolution"],
-                    gchp_is_pre_14_0=config["data"]["dev"]["gchp"][
+                    gchp_res=config["data"]["ref"]["gchp"]["resolution"],
+                    gchp_is_pre_14_0=config["data"]["ref"]["gchp"][
                         "is_pre_14.0"]
                 )
                 devareapath = get_filepath(
                     gchp_vs_gchp_devrstdir,
                     "Restart",
                     bmk_end_dev,
                     is_gchp=True,
                     gchp_res=config["data"]["dev"]["gchp"]["resolution"],
                     gchp_is_pre_14_0=config["data"]["dev"]["gchp"][
                         "is_pre_14.0"]
                 )
 
                 # Create tables
-                bmk.make_benchmark_mass_tables(
+                make_benchmark_mass_tables(
                     refpath,
                     gchp_vs_gchp_refstr,
                     devpath,
                     gchp_vs_gchp_devstr,
                     dst=gchp_vs_gchp_tablesdir,
                     subdst=bmk_mon_yr_strs_dev[mon],
                     label=f"at 01{bmk_mon_yr_strs_dev[mon]}",
@@ -1154,15 +1189,15 @@
                 results = []
                 for mon in range(bmk_n_months):
                     results.append(gchp_vs_gchp_mass_table(mon))
 
         # ==================================================================
         # GCHP vs GCHP operations budgets tables
         # ==================================================================
-        if config["options"]["outputs"]["operations_budget"]:
+        if config["options"]["outputs"]["ops_budget_table"]:
             print("\n%%% Creating GCHP vs. GCHP operations budget tables %%%")
 
             # Filepaths
             col = "Budget"
             refs = get_filepaths(
                 gchp_vs_gchp_refdir,
                 col,
@@ -1173,15 +1208,15 @@
                 gchp_vs_gchp_devdir,
                 col,
                 all_months_gchp_dev,
                 is_gchp=True
             )[0]
 
             # Create table
-            bmk.make_benchmark_operations_budget(
+            make_benchmark_operations_budget(
                 config["data"]["dev"]["gchp"]["dir"],
                 refs,
                 config["data"]["dev"]["gchp"]["dir"],
                 devs,
                 sec_per_yr_ref,
                 sec_per_yr_dev,
                 benchmark_type=bmk_type,
@@ -1193,98 +1228,179 @@
                     "Mixing",
                     "WetDep",
                 ],
                 compute_accum=False,
                 dst=gchp_vs_gchp_tablesdir,
             )
 
+        # ==================================================================
+        # GCHP vs. GCHP Benchmark Timing Table
+        # ==================================================================
+        if config["options"]["outputs"]["timing_table"]:
+            print("\n%%% Creating GCHP vs. GCHP Benchmark Timing table %%%")
+
+            # Filepaths
+            # NOTE: Usually the GCHP 1-yr benchmark is run as
+            # one job, so we only need to take the 1st log file.
+            ref = get_log_filepaths(
+                gchp_vs_gchp_reflogdir,
+                config["data"]["ref"]["gchp"]["logs_template"],
+                all_months_gchp_ref,
+            )[0]
+            dev = get_log_filepaths(
+                gchp_vs_gchp_devlogdir,
+                config["data"]["dev"]["gchp"]["logs_template"],
+                all_months_gchp_dev,
+            )[0]
+
+            # Create the table
+            make_benchmark_gchp_timing_table(
+                ref,
+                config["data"]["ref"]["gchp"]["version"],
+                dev,
+                config["data"]["dev"]["gchp"]["version"],
+                dst=gchp_vs_gchp_tablesdir,
+                overwrite=True,
+            )
+            
     # %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
     # Create mass conservations tables for GCC and GCHP
     # %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
     if config["options"]["outputs"]["cons_table"]:
 
         # ===================================================================
-        # Create mass conservation table for GCC_dev
+        # Create mass conservation table for GCC vs GCC
         # ===================================================================
-        if (
-            config["options"]["comparisons"]["gcc_vs_gcc"]["run"]
-            or config["options"]["comparisons"]["gchp_vs_gcc"]["run"]
-        ):
-            print("\n%%% Creating GCC dev mass conservation table %%%")
+        if config["options"]["comparisons"]["gcc_vs_gcc"]["run"]:
+            print("\n%%% Creating GCC mass conservation tables %%%")
 
             # Filepaths
-            datafiles = get_filepaths(
+            ref_datafiles = get_filepaths(
+                gcc_vs_gcc_refrstdir,
+                "Restart",
+                all_months_ref
+            )[0]
+            dev_datafiles = get_filepaths(
                 gcc_vs_gcc_devrstdir,
                 "Restart",
                 all_months_dev
             )[0]
 
-            # Pick output folder
-            if config["options"]["comparisons"]["gchp_vs_gcc"]["run"]:
-                tablesdir = gchp_vs_gcc_tablesdir
-            else:
-                tablesdir = gcc_vs_gcc_tablesdir
-
             # Create table
-            bmk.make_benchmark_mass_conservation_table(
-                datafiles,
-                config["data"]["dev"]["gcc"]["dir"],
-                dst=tablesdir,
+            make_benchmark_mass_conservation_table(
+                ref_datafiles,
+                config["data"]["ref"]["gcc"]["version"],
+                dev_datafiles,
+                config["data"]["dev"]["gcc"]["version"],
+                dst=gcc_vs_gcc_tablesdir,
                 overwrite=True,
                 spcdb_dir=spcdb_dir,
             )
 
-        # =====================================================================
-        # Create mass conservation table for GCHP_dev
-        # =====================================================================
-        if (
-            config["options"]["comparisons"]["gchp_vs_gcc"]["run"]
-            or config["options"]["comparisons"]["gchp_vs_gchp"]["run"]
-        ):
-            print("\n%%% Creating GCHP dev mass conservation table %%%")
+        # ===================================================================
+        # Create mass conservation table for GCHP vs GCC
+        # ===================================================================
+        if config["options"]["comparisons"]["gchp_vs_gcc"]["run"]:
+            print("\n%%% Creating GCHP vs GCC mass conservation tables %%%")
 
             # Filepaths
-            datafiles = get_filepaths(
+            ref_datafiles = get_filepaths(
+                gchp_vs_gcc_refrstdir,
+                "Restart",
+                all_months_dev,                  # GCHP vs GCC uses GCC dev
+            )[0]
+            dev_datafiles = get_filepaths(
                 gchp_vs_gcc_devrstdir,
                 "Restart",
-                all_months_dev,
+                all_months_dev,                  # GCHP vs GCC uses GCHP dev
                 is_gchp=True,
                 gchp_res=config["data"]["dev"]["gchp"]["resolution"],
                 gchp_is_pre_14_0=config["data"]["dev"]["gchp"]["is_pre_14.0"],
             )[0]
 
             # KLUDGE: ewl, bmy, 14 Oct 2022
             # Read the AREA from the restart file at the end of the
             # simulation.  Due to a GCHP bug, intermediate restarts
             # have AREA with all zeroes.
-            areapath = get_filepath(
+            dev_areapath = get_filepath(
                 gchp_vs_gcc_devrstdir,
                 "Restart",
                 bmk_end_dev,
                 is_gchp=True,
                 gchp_res=config["data"]["dev"]["gchp"]["resolution"],
                 gchp_is_pre_14_0=config["data"]["dev"]["gchp"]["is_pre_14.0"],
             )
 
-            # Pick output folder
-            if config["options"]["comparisons"]["gchp_vs_gcc"]["run"]:
-                tablesdir = gchp_vs_gcc_tablesdir
-            else:
-                tablesdir = gchp_vs_gchp_tablesdir
+            # Create table
+            make_benchmark_mass_conservation_table(
+                ref_datafiles,
+                config["data"]["dev"]["gcc"]["version"],
+                dev_datafiles,
+                config["data"]["dev"]["gchp"]["version"],
+                dst=gchp_vs_gcc_tablesdir,
+                overwrite=True,
+                spcdb_dir=spcdb_dir,
+                dev_areapath=dev_areapath,
+            )
+
+        # =====================================================================
+        # Create mass conservation table for GCHP vs GCHP
+        # =====================================================================
+        if config["options"]["comparisons"]["gchp_vs_gchp"]["run"]:
+            print("\n%%% Creating GCHP dev mass conservation table %%%")
+
+            # Filepaths
+            ref_datafiles = get_filepaths(
+                gchp_vs_gchp_refrstdir,
+                "Restart",
+                all_months_ref,
+                is_gchp=True,
+                gchp_res=config["data"]["ref"]["gchp"]["resolution"],
+                gchp_is_pre_14_0=config["data"]["ref"]["gchp"]["is_pre_14.0"],
+            )[0]
+            dev_datafiles = get_filepaths(
+                gchp_vs_gchp_devrstdir,
+                "Restart",
+                all_months_dev,
+                is_gchp=True,
+                gchp_res=config["data"]["dev"]["gchp"]["resolution"],
+                gchp_is_pre_14_0=config["data"]["dev"]["gchp"]["is_pre_14.0"],
+            )[0]
 
             # KLUDGE: ewl, bmy, 14 Oct 2022
             # Read the AREA from the restart file at the end of the
             # simulation.  Due to a GCHP bug, intermediate restarts
             # have AREA with all zeroes.
-            bmk.make_benchmark_mass_conservation_table(
-                datafiles,
-                config["data"]["dev"]["gchp"]["dir"],
-                dst=tablesdir,
+            ref_areapath = get_filepath(
+                gchp_vs_gchp_refrstdir,
+                "Restart",
+                bmk_end_ref,
+                is_gchp=True,
+                gchp_res=config["data"]["ref"]["gchp"]["resolution"],
+                gchp_is_pre_14_0=config["data"]["ref"]["gchp"]["is_pre_14.0"],
+            )
+            dev_areapath = get_filepath(
+                gchp_vs_gchp_devrstdir,
+                "Restart",
+                bmk_end_dev,
+                is_gchp=True,
+                gchp_res=config["data"]["dev"]["gchp"]["resolution"],
+                gchp_is_pre_14_0=config["data"]["dev"]["gchp"]["is_pre_14.0"],
+            )
+
+            # Create table
+            make_benchmark_mass_conservation_table(
+                ref_datafiles,
+                config["data"]["ref"]["gchp"]["version"],
+                dev_datafiles,
+                config["data"]["dev"]["gchp"]["version"],
+                dst=gchp_vs_gchp_tablesdir,
                 overwrite=True,
                 spcdb_dir=spcdb_dir,
-                areapath=areapath
+                ref_areapath=ref_areapath,
+                dev_areapath=dev_areapath,
             )
 
     # ==================================================================
     # Print a message indicating that the benchmarks finished
     # ==================================================================
-    print("\n %%%% All requested benchmark plots/tables created! %%%%")
+    print("\n%%% All requested benchmark plots/tables created! %%%")
```

### Comparing `geoschem-gcpy-1.4.2/gcpy/benchmark/run_benchmark.py` & `geoschem_gcpy-1.5.0/gcpy/benchmark/run_benchmark.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 #!/usr/bin/env python
 """
-run_1mo_benchmark.py: Driver script for creating benchmark plots and
-                      testing gcpy 1-month benchmark capability
+run_benchmark.py: Driver script for creating benchmark plots.
 
 Run this script to generate benchmark comparisons between:
 
     (1) GCC (aka GEOS-Chem "Classic") vs. GCC
     (2) GCHP vs GCC
     (3) GCHP vs GCHP
     (4) GCHP vs GCC diff-of-diffs
 
 You can customize this by editing the settings in the corresponding yaml
-config file (eg. 1mo_benchmark.yml).
+configuration file.
 
 Calling sequence:
 
-    ./run_1mo_benchmark.py <path-to-configuration-file>
+    $ python -m gcpy.benchmark.run_benchmark <path-to-configuration-file>
 
 Remarks:
 
     By default, matplotlib will try to open an X window for plotting.
     If you are running this script in an environment where you do not have
     an active X display (such as in a computational queue), then you will
     need to use these commands to disable the X-window functionality.
@@ -27,37 +26,56 @@
         import os
         os.environ["QT_QPA_PLATFORM"]="offscreen"
 
     For more information, please see this issue posted at the ipython site:
 
         https://github.com/ipython/ipython/issues/10627
 
-This script corresponds with GCPy 1.4.2. Edit this version ID if releasing
+    Also, to disable matplotlib from trying to open X windows, you may
+    need to set the following environment variable in your shell:
+
+        $ export MPLBACKEND=agg
+
+This script corresponds with GCPy 1.5.0. Edit this version ID if releasing
 a new version of GCPy.
 """
 
-# =====================================================================
+# ======================================================================
 # Imports and global settings (you should not need to edit these)
-# ====================================q=================================
+# ======================================================================
 
 import os
 import sys
-from shutil import copyfile
 import warnings
 from datetime import datetime
 import numpy as np
-from gcpy.util import get_filepath, read_config_file
-from gcpy import ste_flux as ste
-from gcpy import oh_metrics as oh
-from gcpy import benchmark_funcs as bmk
+from gcpy.util import copy_file_to_dir, get_filepath, read_config_file
 from gcpy.date_time import add_months, is_full_year
+from gcpy.benchmark.modules.benchmark_funcs import \
+    diff_of_diffs_toprow_title, get_species_database_dir, \
+    make_benchmark_conc_plots, make_benchmark_emis_plots, \
+    make_benchmark_emis_tables, make_benchmark_jvalue_plots, \
+    make_benchmark_aod_plots, make_benchmark_mass_tables, \
+    make_benchmark_mass_accumulation_tables, \
+    make_benchmark_operations_budget, create_benchmark_summary_table
+from gcpy.benchmark.modules.ste_flux import make_benchmark_ste_table
+from gcpy.benchmark.modules.oh_metrics import make_benchmark_oh_metrics
 from gcpy.benchmark.modules.run_1yr_fullchem_benchmark \
     import run_benchmark as run_1yr_benchmark
 from gcpy.benchmark.modules.run_1yr_tt_benchmark \
     import run_benchmark as run_1yr_tt_benchmark
+from gcpy.benchmark.modules.benchmark_utils import \
+    gcc_vs_gcc_dirs, gchp_vs_gcc_dirs, gchp_vs_gchp_dirs, \
+    get_log_filepaths, print_benchmark_info
+from gcpy.benchmark.modules.benchmark_drydep \
+    import drydepvel_species, make_benchmark_drydep_plots
+from gcpy.benchmark.modules.benchmark_scrape_gcclassic_timers import \
+    make_benchmark_gcclassic_timing_table
+from gcpy.benchmark.modules.benchmark_scrape_gchp_timers import \
+    make_benchmark_gchp_timing_table
 
 # Tell matplotlib not to look for an X-window
 os.environ["QT_QPA_PLATFORM"] = "offscreen"
 
 # Suppress harmless run-time warnings (mostly about underflow in division)
 warnings.filterwarnings("ignore", category=RuntimeWarning)
 warnings.filterwarnings("ignore", category=UserWarning)
@@ -111,85 +129,39 @@
     Runs flexible date benchmark with the given configuration settings.
 
     Args:
         config : dict
             Contains configuration for 1mon benchmark from yaml file.
     """
     # Folder in which the species_database.yml file is found
-    spcdb_dir = bmk.get_species_database_dir(config)
+    spcdb_dir = get_species_database_dir(config)
 
     # =====================================================================
     # Data directories
     # For gchp_vs_gcc_refdir use config["data"]["dev"]["gcc"]["version"],
     # not ref (mps, 6/27/19)
     # =====================================================================
 
-    # Diagnostic file directory paths
-    gcc_vs_gcc_refdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["ref"]["gcc"]["dir"],
-        config["data"]["ref"]["gcc"]["outputs_subdir"],
-    )
-    gcc_vs_gcc_devdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["dev"]["gcc"]["dir"],
-        config["data"]["dev"]["gcc"]["outputs_subdir"],
-    )
-    gchp_vs_gcc_refdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["dev"]["gcc"]["dir"],
-        config["data"]["dev"]["gcc"]["outputs_subdir"],
-    )
-    gchp_vs_gcc_devdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["dev"]["gchp"]["dir"],
-        config["data"]["dev"]["gchp"]["outputs_subdir"],
-    )
-    gchp_vs_gchp_refdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["ref"]["gchp"]["dir"],
-        config["data"]["ref"]["gchp"]["outputs_subdir"],
-    )
-    gchp_vs_gchp_devdir = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["dev"]["gchp"]["dir"],
-        config["data"]["dev"]["gchp"]["outputs_subdir"],
-    )
+    # Diagnostics file directory paths
+    s = "outputs_subdir"
+    gcc_vs_gcc_refdir, gcc_vs_gcc_devdir = gcc_vs_gcc_dirs(config, s)
+    gchp_vs_gcc_refdir, gchp_vs_gcc_devdir = gchp_vs_gcc_dirs(config, s)
+    gchp_vs_gchp_refdir, gchp_vs_gchp_devdir = gchp_vs_gchp_dirs(config, s)
 
     # Restart file directory paths
-    gcc_vs_gcc_refrst = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["ref"]["gcc"]["dir"],
-        config["data"]["ref"]["gcc"]["restarts_subdir"]
-    )
-    gcc_vs_gcc_devrst = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["dev"]["gcc"]["dir"],
-        config["data"]["dev"]["gcc"]["restarts_subdir"]
-    )
-    gchp_vs_gcc_refrst = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["dev"]["gcc"]["dir"],
-        config["data"]["dev"]["gcc"]["restarts_subdir"]
-    )
-    gchp_vs_gcc_devrst = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["dev"]["gchp"]["dir"],
-        config["data"]["dev"]["gchp"]["restarts_subdir"]
-    )
-    gchp_vs_gchp_refrst = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["ref"]["gchp"]["dir"],
-        config["data"]["ref"]["gchp"]["restarts_subdir"]
-    )
-    gchp_vs_gchp_devrst = os.path.join(
-        config["paths"]["main_dir"],
-        config["data"]["dev"]["gchp"]["dir"],
-        config["data"]["dev"]["gchp"]["restarts_subdir"]
-    )
+    s = "restarts_subdir"
+    gcc_vs_gcc_refrstdir, gcc_vs_gcc_devrstdir = gcc_vs_gcc_dirs(config, s)
+    gchp_vs_gcc_refrstdir, gchp_vs_gcc_devrstdir = gchp_vs_gcc_dirs(config, s)
+    gchp_vs_gchp_refrstdir, gchp_vs_gchp_devrstdir = gchp_vs_gchp_dirs(config, s)
+
+    # Log file directory paths
+    s = "logs_subdir"
+    gcc_vs_gcc_reflogdir, gcc_vs_gcc_devlogdir = gcc_vs_gcc_dirs(config, s)
+    gchp_vs_gcc_reflogdir, gchp_vs_gcc_devlogdir = gchp_vs_gcc_dirs(config, s)
+    gchp_vs_gchp_reflogdir, gchp_vs_gchp_devlogdir = gchp_vs_gchp_dirs(config, s)
 
     # =====================================================================
     # Benchmark output directories
     # =====================================================================
     # Results directories
     gcc_vs_gcc_resultsdir = os.path.join(
         config["paths"]["main_dir"],
@@ -217,15 +189,15 @@
     base_gchp_resultsdir = os.path.join(
         config["paths"]["main_dir"],
         config["data"]["dev"]["gchp"]["dir"],
         config["paths"]["results_dir"],
     )
 
     # make results directories that don't exist
-    for resdir, plotting_type in zip(
+    for (resdir, plotting_type) in zip(
         [
             gcc_vs_gcc_resultsdir,
             base_gchp_resultsdir,
             gchp_vs_gchp_resultsdir,
             gchp_vs_gcc_resultsdir,
             diff_of_diffs_resultsdir,
         ],
@@ -237,21 +209,25 @@
             config["options"]["comparisons"]["gchp_vs_gchp"]["run"],
             config["options"]["comparisons"]["gchp_vs_gcc"]["run"],
             config["options"]["comparisons"]["gchp_vs_gcc_diff_of_diffs"]["run"],
         ],
     ):
         if plotting_type and not os.path.exists(resdir):
             os.mkdir(resdir)
-            if resdir in [gcc_vs_gcc_resultsdir, base_gchp_resultsdir]:
-                # Make copy of benchmark script in results directory
-                curfile = os.path.realpath(__file__)
-                dest = os.path.join(resdir, curfile.split("/")[-1])
-                if os.path.exists(dest):
-                    copyfile(curfile, dest)
-                    
+
+            # Copy this script and the config file to each results dir
+            if resdir in [
+                    gcc_vs_gcc_resultsdir,
+                    gchp_vs_gcc_resultsdir,
+                    gchp_vs_gchp_resultsdir,
+                    diff_of_diffs_resultsdir,
+            ]:
+                copy_file_to_dir(__file__, resdir)
+                copy_file_to_dir(config["configuration_file_name"], resdir)
+
     gcc_vs_gcc_tablesdir = os.path.join(
         gcc_vs_gcc_resultsdir,
         config["options"]["comparisons"]["gcc_vs_gcc"]["tables_subdir"],
     )
     gchp_vs_gchp_tablesdir = os.path.join(
         gchp_vs_gchp_resultsdir,
         config["options"]["comparisons"]["gchp_vs_gchp"]["tables_subdir"],
@@ -267,17 +243,17 @@
     # =====================================================================
     gcc_vs_gcc_refstr = config["data"]["ref"]["gcc"]["version"]
     gcc_vs_gcc_devstr = config["data"]["dev"]["gcc"]["version"]
     gchp_vs_gcc_refstr = config["data"]["dev"]["gcc"]["version"]
     gchp_vs_gcc_devstr = config["data"]["dev"]["gchp"]["version"]
     gchp_vs_gchp_refstr = config["data"]["ref"]["gchp"]["version"]
     gchp_vs_gchp_devstr = config["data"]["dev"]["gchp"]["version"]
-    diff_of_diffs_refstr = bmk.diff_of_diffs_toprow_title(config, "gcc")
-    diff_of_diffs_devstr = bmk.diff_of_diffs_toprow_title(config, "gchp")
-    
+    diff_of_diffs_refstr = diff_of_diffs_toprow_title(config, "gcc")
+    diff_of_diffs_devstr = diff_of_diffs_toprow_title(config, "gchp")
+
     ########################################################################
     ###    THE REST OF THESE SETTINGS SHOULD NOT NEED TO BE CHANGED      ###
     ########################################################################
 
     # =====================================================================
     # Dates and times
     # =====================================================================
@@ -324,47 +300,15 @@
         os.path.join(gchp_vs_gchp_resultsdir, "SigDiffs_zonalmean.txt"),
         os.path.join(gchp_vs_gchp_resultsdir, "SigDiffs_emissions.txt"),
     ]
 
     # ======================================================================
     # Print the list of plots & tables to the screen
     # ======================================================================
-    tmpstr = config["options"]["bmk_type"]
-    print(
-        f"The following plots and tables will be created for {tmpstr}"
-    )
-    if config["options"]["outputs"]["plot_conc"]:
-        print(" - Concentration plots")
-    if config["options"]["outputs"]["plot_emis"]:
-        print(" - Emissions plots")
-    if config["options"]["outputs"]["plot_jvalues"]:
-        print(" - J-values (photolysis rates) plots")
-    if config["options"]["outputs"]["plot_aod"]:
-        print(" - Aerosol optical depth plots")
-    if config["options"]["outputs"]["ops_budget_table"]:
-        print(" - Operations budget tables")
-    if config["options"]["outputs"]["emis_table"]:
-        print(" - Table of emissions totals by spc and inventory")
-    if config["options"]["outputs"]["mass_table"]:
-        print(" - Table of species mass")
-    if config["options"]["outputs"]["mass_accum_table"]:
-        print(" - Table of species mass accumulation")
-    if config["options"]["outputs"]["OH_metrics"]:
-        print(" - Table of OH metrics")
-    if config["options"]["outputs"]["ste_table"]:
-        print(" - Table of strat-trop exchange")
-    print("Comparisons will be made for the following combinations:")
-    if config["options"]["comparisons"]["gcc_vs_gcc"]["run"]:
-        print(" - GCC vs GCC")
-    if config["options"]["comparisons"]["gchp_vs_gcc"]["run"]:
-        print(" - GCHP vs GCC")
-    if config["options"]["comparisons"]["gchp_vs_gchp"]["run"]:
-        print(" - GCHP vs GCHP")
-    if config["options"]["comparisons"]["gchp_vs_gcc_diff_of_diffs"]["run"]:
-        print(" - GCHP vs GCC diff of diffs")
+    print_benchmark_info(config)
 
     # %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
     # Create GCC vs GCC benchmark plots and tables
     # %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
     if config["options"]["comparisons"]["gcc_vs_gcc"]["run"]:
 
         # ==================================================================
@@ -411,15 +355,15 @@
             title = "\n%%% Creating GCC vs. GCC concentration plots %%%"
 
             # Diagnostic collection files to read
             ref = get_filepath(gcc_vs_gcc_refdir, "SpeciesConc", gcc_ref_date)
             dev = get_filepath(gcc_vs_gcc_devdir, "SpeciesConc", gcc_dev_date)
 
             # Create plots
-            bmk.make_benchmark_conc_plots(
+            make_benchmark_conc_plots(
                 ref,
                 gcc_vs_gcc_refstr,
                 dev,
                 gcc_vs_gcc_devstr,
                 refmet=refmet,
                 devmet=devmet,
                 dst=gcc_vs_gcc_resultsdir,
@@ -440,15 +384,15 @@
             print("\n%%% Creating GCC vs. GCC emissions plots %%%")
 
             # Filepaths
             ref = get_filepath(gcc_vs_gcc_refdir, "Emissions", gcc_ref_date)
             dev = get_filepath(gcc_vs_gcc_devdir, "Emissions", gcc_dev_date)
 
             # Create emissions plots
-            bmk.make_benchmark_emis_plots(
+            make_benchmark_emis_plots(
                 ref,
                 gcc_vs_gcc_refstr,
                 dev,
                 gcc_vs_gcc_devstr,
                 dst=gcc_vs_gcc_resultsdir,
                 weightsdir=config["paths"]["weights_dir"],
                 plot_by_spc_cat=config["options"]["outputs"]["plot_options"][
@@ -469,15 +413,15 @@
             print("\n%%% Creating GCC vs. GCC emissions & inventory tables %%%")
 
             # Filepaths
             ref = get_filepath(gcc_vs_gcc_refdir, "Emissions", gcc_ref_date)
             dev = get_filepath(gcc_vs_gcc_devdir, "Emissions", gcc_dev_date)
 
             # Create tables
-            bmk.make_benchmark_emis_tables(
+            make_benchmark_emis_tables(
                 ref,
                 gcc_vs_gcc_refstr,
                 dev,
                 gcc_vs_gcc_devstr,
                 dst=gcc_vs_gcc_resultsdir,
                 ref_interval=[gcc_ref_sec_diff],
                 dev_interval=[gcc_dev_sec_diff],
@@ -493,15 +437,15 @@
             print("\n%%% Creating GCC vs. GCC J-value plots %%%")
 
             # Diagnostic collection files to read
             ref = get_filepath(gcc_vs_gcc_refdir, "JValues", gcc_ref_date)
             dev = get_filepath(gcc_vs_gcc_devdir, "JValues", gcc_dev_date)
 
             # Plot J-values
-            bmk.make_benchmark_jvalue_plots(
+            make_benchmark_jvalue_plots(
                 ref,
                 gcc_vs_gcc_refstr,
                 dev,
                 gcc_vs_gcc_devstr,
                 dst=gcc_vs_gcc_resultsdir,
                 weightsdir=config["paths"]["weights_dir"],
                 overwrite=True,
@@ -517,39 +461,64 @@
             print("\n%%% Creating GCC vs. GCC column AOD plots %%%")
 
             # Filepaths
             ref = get_filepath(gcc_vs_gcc_refdir, "Aerosols", gcc_ref_date)
             dev = get_filepath(gcc_vs_gcc_devdir, "Aerosols", gcc_dev_date)
 
             # Create plots
-            bmk.make_benchmark_aod_plots(
+            make_benchmark_aod_plots(
                 ref,
                 gcc_vs_gcc_refstr,
                 dev,
                 gcc_vs_gcc_devstr,
                 dst=gcc_vs_gcc_resultsdir,
                 weightsdir=config["paths"]["weights_dir"],
                 overwrite=True,
                 sigdiff_files=gcc_vs_gcc_sigdiff,
                 spcdb_dir=spcdb_dir,
                 n_job=config["options"]["n_cores"]
             )
 
         # ==================================================================
+        # GCC vs GCC drydep plots
+        # ==================================================================
+        if config["options"]["outputs"]["plot_drydep"]:
+            print("\n%%% Creating GCC vs. GCC drydep plots %%%")
+
+            # Filepaths
+            ref = get_filepath(gcc_vs_gcc_refdir, "DryDep", gcc_ref_date)
+            dev = get_filepath(gcc_vs_gcc_devdir, "DryDep", gcc_dev_date)
+
+            # Create plots
+            make_benchmark_drydep_plots(
+                ref,
+                gcc_vs_gcc_refstr,
+                dev,
+                gcc_vs_gcc_devstr,
+                dst=gcc_vs_gcc_resultsdir,
+                weightsdir=config["paths"]["weights_dir"],
+                overwrite=True,
+                sigdiff_files=gcc_vs_gcc_sigdiff,
+                spcdb_dir=spcdb_dir,
+                n_job=config["options"]["n_cores"],
+                varlist=drydepvel_species()
+            )
+
+        # ==================================================================
         # GCC vs GCC global mass tables
         # ==================================================================
         if config["options"]["outputs"]["mass_table"]:
             print("\n%%% Creating GCC vs. GCC global mass tables %%%")
 
             # Filepaths
-            ref = get_filepath(gcc_vs_gcc_refrst, "Restart", gcc_end_ref_date)
-            dev = get_filepath(gcc_vs_gcc_devrst, "Restart", gcc_end_dev_date)
+            ref = get_filepath(gcc_vs_gcc_refrstdir, "Restart", gcc_end_ref_date)
+            dev = get_filepath(gcc_vs_gcc_devrstdir, "Restart", gcc_end_dev_date)
 
             # Create tables
-            bmk.make_benchmark_mass_tables(
+            make_benchmark_mass_tables(
                 ref,
                 config["data"]["ref"]["gcc"]["version"],
                 dev,
                 config["data"]["dev"]["gcc"]["version"],
                 dst=gcc_vs_gcc_tablesdir,
                 overwrite=True,
                 spcdb_dir=spcdb_dir,
@@ -558,29 +527,29 @@
         # ==================================================================
         # GCC vs GCC global mass accumulation tables
         # ==================================================================
         if config["options"]["outputs"]["mass_accum_table"]:
             print("\n%%% Creating GCC vs. GCC mass accumulation tables %%%")
 
             # Filepaths for start and end restart files
-            refs = get_filepath(gcc_vs_gcc_refrst, "Restart", gcc_ref_date)
-            devs = get_filepath(gcc_vs_gcc_devrst, "Restart", gcc_dev_date)
-            refe = get_filepath(gcc_vs_gcc_refrst, "Restart", gcc_end_ref_date)
-            deve = get_filepath(gcc_vs_gcc_devrst, "Restart", gcc_end_dev_date)
+            refs = get_filepath(gcc_vs_gcc_refrstdir, "Restart", gcc_ref_date)
+            devs = get_filepath(gcc_vs_gcc_devrstdir, "Restart", gcc_dev_date)
+            refe = get_filepath(gcc_vs_gcc_refrstdir, "Restart", gcc_end_ref_date)
+            deve = get_filepath(gcc_vs_gcc_devrstdir, "Restart", gcc_end_dev_date)
 
             # Get period strings
             refs_str = np.datetime_as_string(gcc_ref_date, unit="s")
             devs_str = np.datetime_as_string(gcc_dev_date, unit="s")
             refe_str = np.datetime_as_string(gcc_end_ref_date, unit="s")
             deve_str = np.datetime_as_string(gcc_end_dev_date, unit="s")
             refperiod = refs_str + ' - ' + refe_str
             devperiod = devs_str + ' - ' + deve_str
 
             # Create tables
-            bmk.make_benchmark_mass_accumulation_tables(
+            make_benchmark_mass_accumulation_tables(
                 refs,
                 refe,
                 config["data"]["ref"]["gcc"]["version"],
                 refperiod,
                 devs,
                 deve,
                 config["data"]["dev"]["gcc"]["version"],
@@ -597,15 +566,15 @@
             print("\n%%% Creating GCC vs. GCC operations budget tables %%%")
 
             # Filepaths
             ref = get_filepath(gcc_vs_gcc_refdir, "Budget", gcc_ref_date)
             dev = get_filepath(gcc_vs_gcc_devdir, "Budget", gcc_dev_date)
 
             # Create table
-            bmk.make_benchmark_operations_budget(
+            make_benchmark_operations_budget(
                 config["data"]["ref"]["gcc"]["version"],
                 ref,
                 config["data"]["dev"]["gcc"]["version"],
                 dev,
                 gcc_ref_sec_diff,
                 gcc_dev_sec_diff,
                 benchmark_type=config["options"]["bmk_type"],
@@ -620,15 +589,15 @@
             print("\n%%% Creating GCC vs. GCC OH metrics table %%%")
 
             # Filepaths
             ref = get_filepath(gcc_vs_gcc_refdir, "Metrics", gcc_ref_date)
             dev = get_filepath(gcc_vs_gcc_devdir, "Metrics", gcc_dev_date)
 
             # Create table
-            oh.make_benchmark_oh_metrics(
+            make_benchmark_oh_metrics(
                 ref,
                 config["data"]["ref"]["gcc"]["version"],
                 dev,
                 config["data"]["dev"]["gcc"]["version"],
                 dst=gcc_vs_gcc_tablesdir,
                 overwrite=True,
                 spcdb_dir=spcdb_dir,
@@ -642,54 +611,72 @@
 
             # Diagnostic collection files to read
             dev = get_filepath(gcc_vs_gcc_devdir, "AdvFluxVert", gcc_dev_date)
 
             # Compute monthly and annual average strat-trop exchange of O3
             # only run if comparison is exactly 1 month
             if add_months(gcc_dev_date, 1) == gcc_end_dev_date:
-                ste.make_benchmark_ste_table(
+                make_benchmark_ste_table(
                     config["data"]["dev"]["gcc"]["version"],
                     dev,
                     gcc_dev_date.astype(datetime).year,
                     bmk_type=config["options"]["bmk_type"],
                     dst=gcc_vs_gcc_tablesdir,
                     species=["O3"],
                     overwrite=True,
                     month=gcc_dev_date.astype(datetime).month,
                 )
 
         # ==================================================================
+        # GCC vs. GCC Benchmark Timing Table
+        # ==================================================================
+        if config["options"]["outputs"]["timing_table"]:
+            print("\n%%% Creating GCC vs. GCC Benchmark Timing table %%%")
+
+            # Filepaths
+            ref = get_log_filepaths(
+                gcc_vs_gcc_reflogdir,
+                config["data"]["ref"]["gcc"]["logs_template"],
+                gcc_ref_date,
+            )
+            dev = get_log_filepaths(
+                gcc_vs_gcc_devlogdir,
+                config["data"]["dev"]["gcc"]["logs_template"],
+                gcc_dev_date,
+            )
+
+            # Create the table
+            make_benchmark_gcclassic_timing_table(
+                ref,
+                config["data"]["ref"]["gcc"]["version"],
+                dev,
+                config["data"]["dev"]["gcc"]["version"],
+                dst=gcc_vs_gcc_tablesdir,
+                overwrite=True,
+            )
+
+        # ==================================================================
         # GCC vs. GCC summary table
         # ==================================================================
         if config["options"]["outputs"]["summary_table"]:
             print("\n%%% Creating GCC vs. GCC summary table %%%")
 
-            # Diagnostic collections to check
-            collections = [
-                'AerosolMass',
-                'Aerosols',
-                'Emissions',
-                'JValues',
-                'Metrics',
-                'SpeciesConc',
-                'StateMet',
-            ]
-
             # Print summary of which collections are identical
             # between Ref & Dev, and which are not identical.
-            bmk.create_benchmark_summary_table(
+            create_benchmark_summary_table(
                 gcc_vs_gcc_refdir,
                 config["data"]["ref"]["gcc"]["version"],
                 gcc_ref_date,
                 gcc_vs_gcc_devdir,
                 config["data"]["dev"]["gcc"]["version"],
                 gcc_dev_date,
                 collections = [
                     'AerosolMass',
                     'Aerosols',
+                    #'DryDep',
                     'Emissions',
                     'JValues',
                     'Metrics',
                     'SpeciesConc',
                     'StateMet'
                 ],
                 dst=gcc_vs_gcc_tablesdir,
@@ -761,15 +748,15 @@
                 gchp_vs_gcc_devdir,
                 "SpeciesConc",
                 gchp_dev_date,
                 is_gchp=True
             )
 
             # Create plots
-            bmk.make_benchmark_conc_plots(
+            make_benchmark_conc_plots(
                 ref,
                 gchp_vs_gcc_refstr,
                 dev,
                 gchp_vs_gcc_devstr,
                 refmet=refmet,
                 devmet=devmet,
                 dst=gchp_vs_gcc_resultsdir,
@@ -795,15 +782,15 @@
                 gchp_vs_gcc_devdir,
                 "Emissions",
                 gchp_dev_date,
                 is_gchp=True
             )
 
             # Create emissions plots
-            bmk.make_benchmark_emis_plots(
+            make_benchmark_emis_plots(
                 ref,
                 gchp_vs_gcc_refstr,
                 dev,
                 gchp_vs_gcc_devstr,
                 dst=gchp_vs_gcc_resultsdir,
                 weightsdir=config["paths"]["weights_dir"],
                 plot_by_spc_cat=config["options"]["outputs"]["plot_options"][
@@ -812,15 +799,15 @@
                 plot_by_hco_cat=config["options"]["outputs"]["plot_options"][
                     "by_hco_cat"
                 ],
                 benchmark_type=config["options"]["bmk_type"],
                 overwrite=True,
                 sigdiff_files=gchp_vs_gcc_sigdiff,
                 spcdb_dir=spcdb_dir,
-                n_job=config["options"]["n_cores"]                
+                n_job=config["options"]["n_cores"]
             )
 
         # ==================================================================
         # GCHP vs. GCC tables of emission and inventory totals
         # ==================================================================
         if config["options"]["outputs"]["emis_table"]:
             print("\n%%% Creating GCHP vs. GCC emissions/inventory tables %%%")
@@ -831,15 +818,15 @@
                 gchp_vs_gcc_devdir,
                 "Emissions",
                 gchp_dev_date,
                 is_gchp=True
             )
 
             # Create plots
-            bmk.make_benchmark_emis_tables(
+            make_benchmark_emis_tables(
                 ref,
                 gchp_vs_gcc_refstr,
                 dev,
                 gchp_vs_gcc_devstr,
                 dst=gchp_vs_gcc_resultsdir,
                 ref_interval=[gcc_dev_sec_diff],
                 dev_interval=[gchp_dev_sec_diff],
@@ -861,25 +848,25 @@
                 gchp_vs_gcc_devdir,
                 "JValues",
                 gchp_dev_date,
                 is_gchp=True
             )
 
             # Create plots
-            bmk.make_benchmark_jvalue_plots(
+            make_benchmark_jvalue_plots(
                 ref,
                 gchp_vs_gcc_refstr,
                 dev,
                 gchp_vs_gcc_devstr,
                 dst=gchp_vs_gcc_resultsdir,
                 weightsdir=config["paths"]["weights_dir"],
                 overwrite=True,
                 sigdiff_files=gchp_vs_gcc_sigdiff,
                 spcdb_dir=spcdb_dir,
-                n_job=config["options"]["n_cores"]                
+                n_job=config["options"]["n_cores"]
             )
 
         # ==================================================================
         # GCHP vs GCC column AOD plots
         # ==================================================================
         if config["options"]["outputs"]["plot_aod"]:
             print("\n%%% Creating GCHP vs. GCC column AOD plots %%%")
@@ -890,50 +877,80 @@
                 gchp_vs_gcc_devdir,
                 "Aerosols",
                 gchp_dev_date,
                 is_gchp=True
             )
 
             # Create plots
-            bmk.make_benchmark_aod_plots(
+            make_benchmark_aod_plots(
+                ref,
+                gchp_vs_gcc_refstr,
+                dev,
+                gchp_vs_gcc_devstr,
+                dst=gchp_vs_gcc_resultsdir,
+                weightsdir=config["paths"]["weights_dir"],
+                overwrite=True,
+                sigdiff_files=gchp_vs_gcc_sigdiff,
+                spcdb_dir=spcdb_dir,
+                n_job=config["options"]["n_cores"]
+            )
+
+        # ==================================================================
+        # GCHP vs GCC drydep plots
+        # ==================================================================
+        if config["options"]["outputs"]["plot_drydep"]:
+            print("\n%%% Creating GCHP vs. GCC drydep plots %%%")
+
+            # Filepaths
+            ref = get_filepath(gchp_vs_gcc_refdir, "DryDep", gcc_ref_date)
+            dev = get_filepath(
+                gchp_vs_gcc_devdir,
+                "DryDep",
+                gchp_dev_date,
+                is_gchp=True
+            )
+
+            # Create plots
+            make_benchmark_drydep_plots(
                 ref,
                 gchp_vs_gcc_refstr,
                 dev,
                 gchp_vs_gcc_devstr,
                 dst=gchp_vs_gcc_resultsdir,
                 weightsdir=config["paths"]["weights_dir"],
                 overwrite=True,
                 sigdiff_files=gchp_vs_gcc_sigdiff,
                 spcdb_dir=spcdb_dir,
-                n_job=config["options"]["n_cores"]                
+                n_job=config["options"]["n_cores"],
+                varlist=drydepvel_species(),
             )
 
         # ==================================================================
         # GCHP vs GCC global mass tables
         # ==================================================================
         if config["options"]["outputs"]["mass_table"]:
             print("\n%%% Creating GCHP vs. GCC global mass tables %%%")
 
             # Filepaths
             ref = get_filepath(
-                gchp_vs_gcc_refrst,
+                gchp_vs_gcc_refrstdir,
                 "Restart",
                 gcc_end_dev_date
             )
             dev = get_filepath(
-                gchp_vs_gcc_devrst,
+                gchp_vs_gcc_devrstdir,
                 "Restart",
                 gchp_end_dev_date,
                 is_gchp=True,
                 gchp_res=config["data"]["dev"]["gchp"]["resolution"],
                 gchp_is_pre_14_0=config["data"]["dev"]["gchp"]["is_pre_14.0"]
             )
 
             # Create tables
-            bmk.make_benchmark_mass_tables(
+            make_benchmark_mass_tables(
                 ref,
                 gchp_vs_gcc_refstr,
                 dev,
                 gchp_vs_gcc_devstr,
                 dst=gchp_vs_gcc_tablesdir,
                 overwrite=True,
                 spcdb_dir=spcdb_dir,
@@ -943,33 +960,33 @@
         # GCHP vs GCC global mass accumulation tables
         # ==================================================================
         if config["options"]["outputs"]["mass_accum_table"]:
             print("\n%%% Creating GCHP vs. GCC mass accumulation tables %%%")
 
             # Filepaths for start and end restart files
             refs = get_filepath(
-                gchp_vs_gcc_refrst,
+                gchp_vs_gcc_refrstdir,
                 "Restart",
                 gcc_dev_date
             )
             devs = get_filepath(
-                gchp_vs_gcc_devrst,
+                gchp_vs_gcc_devrstdir,
                 "Restart",
                 gchp_dev_date,
                 is_gchp=True,
                 gchp_res=config["data"]["dev"]["gchp"]["resolution"],
                 gchp_is_pre_14_0=config["data"]["dev"]["gchp"]["is_pre_14.0"]
             )
             refe = get_filepath(
-                gchp_vs_gcc_refrst,
+                gchp_vs_gcc_refrstdir,
                 "Restart",
                 gcc_end_dev_date
             )
             deve = get_filepath(
-                gchp_vs_gcc_devrst,
+                gchp_vs_gcc_devrstdir,
                 "Restart",
                 gchp_end_dev_date,
                 is_gchp=True,
                 gchp_res=config["data"]["dev"]["gchp"]["resolution"],
                 gchp_is_pre_14_0=config["data"]["dev"]["gchp"]["is_pre_14.0"]
             )
 
@@ -978,15 +995,15 @@
             devs_str = np.datetime_as_string(gchp_dev_date, unit="s")
             refe_str = np.datetime_as_string(gcc_end_dev_date, unit="s")
             deve_str = np.datetime_as_string(gchp_end_dev_date, unit="s")
             refperiod = refs_str + ' - ' + refe_str
             devperiod = devs_str + ' - ' + deve_str
 
             # Create tables
-            bmk.make_benchmark_mass_accumulation_tables(
+            make_benchmark_mass_accumulation_tables(
                 refs,
                 refe,
                 config["data"]["dev"]["gcc"]["version"],
                 refperiod,
                 devs,
                 deve,
                 config["data"]["dev"]["gchp"]["version"],
@@ -1008,15 +1025,15 @@
                 gchp_vs_gcc_devdir,
                 "Budget",
                 gchp_dev_date,
                 is_gchp=True
             )
 
             # Create table
-            bmk.make_benchmark_operations_budget(
+            make_benchmark_operations_budget(
                 config["data"]["dev"]["gcc"]["version"],
                 ref,
                 config["data"]["dev"]["gchp"]["version"],
                 dev,
                 gcc_dev_sec_diff,
                 gchp_dev_sec_diff,
                 benchmark_type=config["options"]["bmk_type"],
@@ -1044,15 +1061,15 @@
                 gchp_vs_gcc_devdir,
                 "Metrics",
                 gchp_dev_date,
                 is_gchp=True
             )
 
             # Create table
-            oh.make_benchmark_oh_metrics(
+            make_benchmark_oh_metrics(
                 ref,
                 gchp_vs_gcc_refstr,
                 dev,
                 gchp_vs_gcc_devstr,
                 dst=gchp_vs_gcc_tablesdir,
                 overwrite=True,
                 spcdb_dir=spcdb_dir,
@@ -1061,24 +1078,23 @@
         # ==================================================================
         # GCHP vs GCC Strat-Trop Exchange
         # ==================================================================
         if config["options"]["outputs"]["ste_table"]:
             title = "\n%%% Skipping GCHP vs. GCC Strat-Trop Exchange table %%%"
             print(title)
 
-
         # ==================================================================
         # GCHP vs. GCC summary table
         # ==================================================================
         if config["options"]["outputs"]["summary_table"]:
             print("\n%%% Creating GCHP vs. GCC summary table %%%")
 
             # Print summary of which collections are identical
             # between Ref & Dev, and which are not identical.
-            bmk.create_benchmark_summary_table(
+            create_benchmark_summary_table(
                 gchp_vs_gcc_refdir,
                 config["data"]["dev"]["gcc"]["version"],
                 gcc_dev_date,
                 gchp_vs_gcc_devdir,
                 config["data"]["dev"]["gchp"]["version"],
                 gchp_dev_date,
                 collections=[
@@ -1169,30 +1185,30 @@
                 gchp_vs_gchp_devdir,
                 "SpeciesConc",
                 gchp_dev_date,
                 is_gchp=True
             )
 
             # Create plots
-            bmk.make_benchmark_conc_plots(
+            make_benchmark_conc_plots(
                 ref,
                 gchp_vs_gchp_refstr,
                 dev,
                 gchp_vs_gchp_devstr,
                 refmet=refmet,
                 devmet=devmet,
                 dst=gchp_vs_gchp_resultsdir,
                 weightsdir=config["paths"]["weights_dir"],
                 plot_by_spc_cat=config["options"]["outputs"]["plot_options"][
                     "by_spc_cat"],
                 benchmark_type=config["options"]["bmk_type"],
                 overwrite=True,
                 sigdiff_files=gchp_vs_gchp_sigdiff,
                 spcdb_dir=spcdb_dir,
-                n_job=config["options"]["n_cores"]                
+                n_job=config["options"]["n_cores"]
             )
 
         # ==================================================================
         # GCHP vs. GCHP Emissions plots
         # ==================================================================
         if config["options"]["outputs"]["plot_emis"]:
             print("\n%%% Creating GCHP vs. GCHP emissions plots %%%")
@@ -1208,30 +1224,30 @@
                 gchp_vs_gchp_devdir,
                 "Emissions",
                 gchp_dev_date,
                 is_gchp=True
             )
 
             # Create plots
-            bmk.make_benchmark_emis_plots(
+            make_benchmark_emis_plots(
                 ref,
                 gchp_vs_gchp_refstr,
                 dev,
                 gchp_vs_gchp_devstr,
                 dst=gchp_vs_gchp_resultsdir,
                 weightsdir=config["paths"]["weights_dir"],
                 plot_by_spc_cat=config["options"]["outputs"]["plot_options"][
                     "by_spc_cat"],
                 plot_by_hco_cat=config["options"]["outputs"]["plot_options"][
                     "by_hco_cat"],
                 benchmark_type=config["options"]["bmk_type"],
                 overwrite=True,
                 sigdiff_files=gchp_vs_gchp_sigdiff,
                 spcdb_dir=spcdb_dir,
-                n_job=config["options"]["n_cores"]                
+                n_job=config["options"]["n_cores"]
             )
 
         # ==================================================================
         # GCHP vs. GCHP tables of emission and inventory totals
         # ==================================================================
         if config["options"]["outputs"]["emis_table"]:
             print("\n%%% Creating GCHP vs. GCHP emissions/inventory tables %%%")
@@ -1247,15 +1263,15 @@
                 gchp_vs_gchp_devdir,
                 "Emissions",
                 gchp_dev_date,
                 is_gchp=True
             )
 
             # Create tables
-            bmk.make_benchmark_emis_tables(
+            make_benchmark_emis_tables(
                 ref,
                 gchp_vs_gchp_refstr,
                 dev,
                 gchp_vs_gchp_devstr,
                 dst=gchp_vs_gchp_resultsdir,
                 ref_interval=[gchp_ref_sec_diff],
                 dev_interval=[gchp_dev_sec_diff],
@@ -1283,25 +1299,25 @@
                 gchp_vs_gchp_devdir,
                 "JValues",
                 gchp_dev_date,
                 is_gchp=True
             )
 
             # Create plots
-            bmk.make_benchmark_jvalue_plots(
+            make_benchmark_jvalue_plots(
                 ref,
                 gchp_vs_gchp_refstr,
                 dev,
                 gchp_vs_gchp_devstr,
                 dst=gchp_vs_gchp_resultsdir,
                 weightsdir=config["paths"]["weights_dir"],
                 overwrite=True,
                 sigdiff_files=gchp_vs_gchp_sigdiff,
                 spcdb_dir=spcdb_dir,
-                n_job=config["options"]["n_cores"]                
+                n_job=config["options"]["n_cores"]
             )
 
         # ==================================================================
         # GCHP vs GCHP column AOD plots
         # ==================================================================
         if config["options"]["outputs"]["plot_aod"]:
             print("\n%%% Creating GCHP vs. GCHP column AOD plots %%%")
@@ -1317,53 +1333,88 @@
                 gchp_vs_gchp_devdir,
                 "Aerosols",
                 gchp_dev_date,
                 is_gchp=True
             )
 
             # Create plots
-            bmk.make_benchmark_aod_plots(
+            make_benchmark_aod_plots(
+                ref,
+                gchp_vs_gchp_refstr,
+                dev,
+                gchp_vs_gchp_devstr,
+                dst=gchp_vs_gchp_resultsdir,
+                weightsdir=config["paths"]["weights_dir"],
+                overwrite=True,
+                sigdiff_files=gchp_vs_gchp_sigdiff,
+                spcdb_dir=spcdb_dir,
+                n_job=config["options"]["n_cores"]
+            )
+
+        # ==================================================================
+        # GCHP vs GCHP drydep plots
+        # ==================================================================
+        if config["options"]["outputs"]["plot_drydep"]:
+            print("\n%%% Creating GCHP vs. GCHP drydep plots %%%")
+
+            # Filepaths
+            ref = get_filepath(
+                gchp_vs_gchp_refdir,
+                "DryDep",
+                gchp_ref_date,
+                is_gchp=True
+            )
+            dev = get_filepath(
+                gchp_vs_gchp_devdir,
+                "DryDep",
+                gchp_dev_date,
+                is_gchp=True
+            )
+
+            # Create plots
+            make_benchmark_drydep_plots(
                 ref,
                 gchp_vs_gchp_refstr,
                 dev,
                 gchp_vs_gchp_devstr,
                 dst=gchp_vs_gchp_resultsdir,
                 weightsdir=config["paths"]["weights_dir"],
                 overwrite=True,
                 sigdiff_files=gchp_vs_gchp_sigdiff,
                 spcdb_dir=spcdb_dir,
-                n_job=config["options"]["n_cores"]                
+                n_job=config["options"]["n_cores"],
+                varlist=drydepvel_species()
             )
 
         # ==================================================================
         # GCHP vs GCHP global mass tables
         # ==================================================================
         if config["options"]["outputs"]["mass_table"]:
             print("\n%%% Creating GCHP vs. GCHP global mass tables %%%")
 
             # Filepaths
             ref = get_filepath(
-                gchp_vs_gchp_refrst,
+                gchp_vs_gchp_refrstdir,
                 "Restart",
                 gchp_end_ref_date,
                 is_gchp=True,
                 gchp_res=config["data"]["ref"]["gchp"]["resolution"],
                 gchp_is_pre_14_0=config["data"]["ref"]["gchp"]["is_pre_14.0"]
             )
             dev = get_filepath(
-                gchp_vs_gchp_devrst,
+                gchp_vs_gchp_devrstdir,
                 "Restart",
                 gchp_end_dev_date,
                 is_gchp=True,
                 gchp_res=config["data"]["dev"]["gchp"]["resolution"],
                 gchp_is_pre_14_0=config["data"]["dev"]["gchp"]["is_pre_14.0"]
             )
 
             # Create tables
-            bmk.make_benchmark_mass_tables(
+            make_benchmark_mass_tables(
                 ref,
                 gchp_vs_gchp_refstr,
                 dev,
                 gchp_vs_gchp_devstr,
                 dst=gchp_vs_gchp_tablesdir,
                 overwrite=True,
                 spcdb_dir=spcdb_dir,
@@ -1373,39 +1424,39 @@
         # GCHP vs GCHP global mass accumulation tables
         # ==================================================================
         if config["options"]["outputs"]["mass_accum_table"]:
             print("\n%%% Creating GCHP vs. GCHP mass accumulation tables %%%")
 
             # Filepaths for start and end restart files
             refs = get_filepath(
-                gchp_vs_gchp_refrst,
+                gchp_vs_gchp_refrstdir,
                 "Restart",
                 gchp_ref_date,
                 is_gchp=True,
                 gchp_res=config["data"]["ref"]["gchp"]["resolution"],
                 gchp_is_pre_14_0=config["data"]["ref"]["gchp"]["is_pre_14.0"]
             )
             devs = get_filepath(
-                gchp_vs_gchp_devrst,
+                gchp_vs_gchp_devrstdir,
                 "Restart",
                 gchp_dev_date,
                 is_gchp=True,
                 gchp_res=config["data"]["dev"]["gchp"]["resolution"],
                 gchp_is_pre_14_0=config["data"]["dev"]["gchp"]["is_pre_14.0"]
             )
             refe = get_filepath(
-                gchp_vs_gchp_refrst,
+                gchp_vs_gchp_refrstdir,
                 "Restart",
                 gchp_end_ref_date,
                 is_gchp=True,
                 gchp_res=config["data"]["ref"]["gchp"]["resolution"],
                 gchp_is_pre_14_0=config["data"]["ref"]["gchp"]["is_pre_14.0"]
             )
             deve = get_filepath(
-                gchp_vs_gchp_devrst,
+                gchp_vs_gchp_devrstdir,
                 "Restart",
                 gchp_end_dev_date,
                 is_gchp=True,
                 gchp_res=config["data"]["dev"]["gchp"]["resolution"],
                 gchp_is_pre_14_0=config["data"]["dev"]["gchp"]["is_pre_14.0"]
             )
 
@@ -1414,15 +1465,15 @@
             devs_str = np.datetime_as_string(gchp_dev_date, unit="s")
             refe_str = np.datetime_as_string(gchp_end_ref_date, unit="s")
             deve_str = np.datetime_as_string(gchp_end_dev_date, unit="s")
             refperiod = refs_str + ' - ' + refe_str
             devperiod = devs_str + ' - ' + deve_str
 
             # Create tables
-            bmk.make_benchmark_mass_accumulation_tables(
+            make_benchmark_mass_accumulation_tables(
                 refs,
                 refe,
                 config["data"]["ref"]["gchp"]["version"],
                 refperiod,
                 devs,
                 deve,
                 config["data"]["dev"]["gchp"]["version"],
@@ -1449,15 +1500,15 @@
                 gchp_vs_gchp_devdir,
                 "Budget",
                 gchp_dev_date,
                 is_gchp=True
             )
 
             # Create tables
-            bmk.make_benchmark_operations_budget(
+            make_benchmark_operations_budget(
                 config["data"]["ref"]["gchp"]["version"],
                 ref,
                 config["data"]["dev"]["gchp"]["version"],
                 dev,
                 gchp_ref_sec_diff,
                 gchp_dev_sec_diff,
                 benchmark_type=config["options"]["bmk_type"],
@@ -1490,52 +1541,80 @@
                 gchp_vs_gchp_devdir,
                 "Metrics",
                 gchp_dev_date,
                 is_gchp=True
             )
 
             # Create table
-            oh.make_benchmark_oh_metrics(
+            make_benchmark_oh_metrics(
                 ref,
                 config["data"]["ref"]["gchp"]["version"],
                 dev,
                 config["data"]["dev"]["gchp"]["version"],
                 dst=gchp_vs_gchp_tablesdir,
                 overwrite=True,
                 spcdb_dir=spcdb_dir,
             )
 
         # ==================================================================
         # GCHP vs GCHP Strat-Trop Exchange
-        # --------------------------------------------------------------
+        # ==================================================================
         if config["options"]["outputs"]["ste_table"]:
             print("\n%%% Skipping GCHP vs. GCHP Strat-Trop Exchange table %%%")
 
         # ==================================================================
+        # GCHP vs. GCHP Benchmark Timing Table
+        # ==================================================================
+        if config["options"]["outputs"]["timing_table"]:
+            print("\n%%% Creating GCHP vs. GCHP Benchmark Timing table %%%")
+
+            # Filepaths
+            ref = get_log_filepaths(
+                gchp_vs_gchp_reflogdir,
+                config["data"]["ref"]["gchp"]["logs_template"],
+                gchp_ref_date,
+            )
+            dev = get_log_filepaths(
+                gchp_vs_gchp_devlogdir,
+                config["data"]["dev"]["gchp"]["logs_template"],
+                gchp_dev_date,
+            )
+
+            # Create the table
+            make_benchmark_gchp_timing_table(
+                ref,
+                config["data"]["ref"]["gchp"]["version"],
+                dev,
+                config["data"]["dev"]["gchp"]["version"],
+                dst=gchp_vs_gchp_tablesdir,
+                overwrite=True,
+            )
+            
+        # ==================================================================
         # GCHP vs. GCHP summary table
         # ==================================================================
         if config["options"]["outputs"]["summary_table"]:
             print("\n%%% Creating GCHP vs. GCHP summary table %%%")
 
             # Print summary of which collections are identical
             # between Ref & Dev, and which are not identical.
-            bmk.create_benchmark_summary_table(
+            create_benchmark_summary_table(
                 gchp_vs_gchp_refdir,
                 config["data"]["ref"]["gchp"]["version"],
                 gchp_ref_date,
                 gchp_vs_gchp_devdir,
                 config["data"]["dev"]["gchp"]["version"],
                 gchp_dev_date,
                 collections=[
                     'AerosolMass',
                     'Aerosols',
                     'Emissions',
                     'JValues',
                     'Metrics',
-                    'SpeciesConc', 
+                    'SpeciesConc',
                     'StateMet',
                 ],
                 dst=gchp_vs_gchp_tablesdir,
                 outfilename="Summary.txt",
                 overwrite=True,
                 verbose=False,
                 ref_gchp=True,
@@ -1564,29 +1643,29 @@
                 "SpeciesConc",
                 gchp_dev_date,
                 is_gchp=True
             )
 
             # Create diff-of-diff plots for species concentrations
             # NOTE: for simplicity, do not convert aerosols to ug/m3.
-            bmk.make_benchmark_conc_plots(
+            make_benchmark_conc_plots(
                 gcc_ref,
                 diff_of_diffs_refstr,
                 gchp_ref,
                 diff_of_diffs_devstr,
                 dst=diff_of_diffs_resultsdir,
                 weightsdir=config["paths"]["weights_dir"],
                 benchmark_type=config["options"]["bmk_type"],
                 overwrite=True,
                 use_cmap_RdBu=True,
                 second_ref=gcc_dev,
                 second_dev=gchp_dev,
                 cats_in_ugm3=None,
                 spcdb_dir=spcdb_dir,
-                n_job=config["options"]["n_cores"]                
+                n_job=config["options"]["n_cores"]
             )
 
 
     # ==================================================================
     # Print a message indicating that the benchmarks finished
     # ==================================================================
     print("\n%%%% All requested benchmark plots/tables created! %%%%")
@@ -1595,12 +1674,13 @@
 def main(argv):
     """
     Driver program. Determines which benchmark script script to call
     for 1-hour, 1-day, 1-month, or 1-year benchmarks.
     """
     config_filename = argv[1] if len(argv) == 2 else "1mo_benchmark.yml"
     config = read_config_file(config_filename)
+    config["configuration_file_name"] = config_filename
     choose_benchmark_type(config)
 
 
 if __name__ == "__main__":
     main(sys.argv)
```

### Comparing `geoschem-gcpy-1.4.2/gcpy/benchmark_categories.yml` & `geoschem_gcpy-1.5.0/gcpy/benchmark/modules/benchmark_categories.yml`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/benchmark_funcs.py` & `geoschem_gcpy-1.5.0/gcpy/benchmark/modules/benchmark_funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,23 +16,22 @@
 from gcpy import util
 from gcpy.regrid import create_regridders
 from gcpy.grid import get_troposphere_mask
 from gcpy.units import convert_units
 from gcpy.constants import COL_WIDTH, MW_AIR_g, skip_these_vars, TABLE_WIDTH
 from gcpy.plot.compare_single_level import compare_single_level
 from gcpy.plot.compare_zonal_mean import compare_zonal_mean
+from gcpy.benchmark.modules.benchmark_utils import \
+    AOD_SPC, EMISSION_SPC, EMISSION_INV, add_lumped_species_to_dataset, \
+    archive_lumped_species_definitions, get_species_categories, \
+    archive_species_categories, rename_speciesconc_to_speciesconcvv
 
 # Suppress numpy divide by zero warnings to prevent output spam
 np.seterr(divide="ignore", invalid="ignore")
 
-# YAML files
-AOD_SPC = "aod_species.yml"
-EMISSION_SPC = "emission_species.yml"
-EMISSION_INV = "emission_inventories.yml"
-
 
 def create_total_emissions_table(
         refdata,
         refstr,
         devdata,
         devstr,
         species,
@@ -1027,22 +1026,16 @@
 
     # Open datasets
     refds = reader(ref, drop_variables=skip_these_vars).load()
     devds = reader(dev, drop_variables=skip_these_vars).load()
 
     # Rename SpeciesConc_ to SpeciesConcVV_ for consistency with new
     # naming introduced in GEOS-Chem 14.1.0
-    for v in refds.data_vars.keys():
-        if v.startswith('SpeciesConc_'):
-            spc = v.replace('SpeciesConc_', '')
-            refds = refds.rename({v: 'SpeciesConcVV_' + spc})
-    for v in devds.data_vars.keys():
-        if v.startswith('SpeciesConc_'):
-            spc = v.replace('SpeciesConc_', '')
-            devds = devds.rename({v: 'SpeciesConcVV_' + spc})
+    refds = rename_speciesconc_to_speciesconcvv(refds)
+    devds = rename_speciesconc_to_speciesconcvv(devds)
 
     # -----------------------------------------------------------------
     # Kludge, rename wrong variable name
     if "SpeciesConcVV_PFE" in refds.data_vars.keys():
         refds = refds.rename({"SpeciesConcVV_PFE": "SpeciesConcVV_pFe"})
     if "SpeciesConcVV_PFE" in devds.data_vars.keys():
         devds = devds.rename({"SpeciesConcVV_PFE": "SpeciesConcVV_pFe"})
@@ -1225,30 +1218,30 @@
     # ==================================================================
 
     # FullChemBenchmark has lumped species (TransportTracers, CH4 do not)
     if "FullChem" in benchmark_type:
         print("\nComputing lumped species for full chemistry benchmark")
 
         print("-->Adding lumped species to ref dataset")
-        refds = util.add_lumped_species_to_dataset(refds)
+        refds = add_lumped_species_to_dataset(refds)
 
         print("-->Adding lumped species to dev dataset")
-        devds = util.add_lumped_species_to_dataset(devds)
+        devds = add_lumped_species_to_dataset(devds)
 
         if diff_of_diffs:
             print("-->Adding lumped species to dev datasets")
-            second_refds = util.add_lumped_species_to_dataset(second_refds)
-            second_devds = util.add_lumped_species_to_dataset(second_devds)
+            second_refds = add_lumped_species_to_dataset(second_refds)
+            second_devds = add_lumped_species_to_dataset(second_devds)
 
-        util.archive_lumped_species_definitions(dst)
+        archive_lumped_species_definitions(dst)
         print("Lumped species computation complete.\n")
 
     # Get the list of species categories
-    catdict = util.get_species_categories(benchmark_type)
-    util.archive_species_categories(dst)
+    catdict = get_species_categories(benchmark_type)
+    archive_species_categories(dst)
 
     # Make sure that Ref and Dev datasets have the same variables.
     # Variables that are in Ref but not in Dev will be added to Dev
     # with all missing values (NaNs). And vice-versa.
     [refds, devds] = util.add_missing_variables(refds, devds)
 
     if diff_of_diffs:
@@ -1511,17 +1504,14 @@
     dict_sfc = {list(result.keys())[0]: result[list(
         result.keys())[0]]['sfc'] for result in results}
     dict_500 = {list(result.keys())[0]: result[list(
         result.keys())[0]]['500'] for result in results}
     dict_zm = {list(result.keys())[0]: result[list(
         result.keys())[0]]['zm'] for result in results}
 
-    print("stop here")
-    quit()
-    
     # ==============================================================
     # Write the list of species having significant differences,
     # which we need to fill out the benchmark approval forms.
     # ==============================================================
     if sigdiff_files is not None:
         for filename in sigdiff_files:
             if "sfc" in plots:
@@ -1617,15 +1607,15 @@
             and denotes a date string (such as "Jan2016") that
             corresponds to the month that is being plotted.
             Default value: None
         plot_by_spc_cat: bool
             Set this flag to True to separate plots into PDF files
             according to the benchmark species categories (e.g. Oxidants,
             Aerosols, Nitrogen, etc.)  These categories are specified
-            in the YAML file benchmark_species.yml.
+            in the YAML file benchmark_categories.yml.
             Default value: False
         plot_by_hco_cat: bool
             Set this flag to True to separate plots into PDF files
             according to HEMCO emissions categories (e.g. Anthro,
             Aircraft, Bioburn, etc.)
             Default value: False
         benchmark_type: str
@@ -1897,15 +1887,15 @@
 
     # ==================================================================
     # if plot_by_spc_cat is true, make a file for each benchmark
     # species category with emissions in the diagnostics file
     # ==================================================================
     if plot_by_spc_cat:
 
-        catdict = util.get_species_categories(benchmark_type)
+        catdict = get_species_categories(benchmark_type)
         # in case any emissions are skipped (for use in nested pdf bookmarks)
         warninglist = ([])
         # for checking if emissions species not defined in benchmark category
         # file
         allcatspc = ([])
         emisdict = {}  # used for nested pdf bookmarks
         # for i, filecat in enumerate(catdict):
@@ -4036,18 +4026,19 @@
     # Molecular weights [g mol-1], as taken from the species database
     mw = {}
     for v in species_list:
         mw[v] = spcdb[v]["MW_g"]
     mw["Air"] = MW_AIR_g
 
     # Get the list of relevant AOD diagnostics from a YAML file
+    ifile= AOD_SPC
     aod = util.read_config_file(
         os.path.join(
             os.path.dirname(__file__),
-            "aod_species.yml"
+            ifile,
         ),
         quiet=True
     )
 
     aod_list = [v for v in aod.keys() if "Dust" in v or "Hyg" in v]
     # different names for GCHP
     if is_gchp:
@@ -4084,18 +4075,15 @@
         # combine="nested", concat_dim="time")
         ds_met = xr.open_mfdataset(devlist_met,
                                    drop_variables=skip_these_vars)  # ,
         # combine="nested", concat_dim="time")
 
     # Rename SpeciesConc_ to SpeciesConcVV_ for consistency with new
     # naming introduced in GEOS-Chem 14.1.0
-    for v in ds_spc.data_vars.keys():
-        if v.startswith('SpeciesConc_'):
-            spc = v.replace('SpeciesConc_', '')
-            ds_spc = ds_spc.rename({v: 'SpeciesConcVV_' + spc})
+    ds_spc = rename_speciesconc_to_speciesconcvv(ds_spc)
 
     # Get troposphere mask
     tropmask = get_troposphere_mask(ds_met)
 
     # Get number of months
     n_mon = len(days_per_mon)
 
@@ -4268,15 +4256,15 @@
         reffiles,
         devstr,
         devfiles,
         ref_interval,
         dev_interval,
         benchmark_type=None,
         label=None,
-        col_sections=["Full", "Trop", "PBL", "Strat"],
+        col_sections=["Full", "Trop", "PBL", "FixedLevs", "Strat"],
         operations=["Chemistry", "Convection", "EmisDryDep",
                     "Mixing", "Transport", "WetDep"],
         compute_accum=True,
         compute_restart=False,
         require_overlap=False,
         dst='.',
         species=None,
@@ -4308,15 +4296,15 @@
         label: str
             Contains the date or date range for each dataframe title.
             Default value: None
         col_sections: list of str
             List of column sections to calculate global budgets for. May
             include Strat eventhough not calculated in GEOS-Chem, but Full
             and Trop must also be present to calculate Strat.
-            Default value: ["Full", "Trop", "PBL", "Strat"]
+            Default value: ["Full", "Trop", "PBL", "FixedLevs", "Strat"]
         operations: list of str
             List of operations to calculate global budgets for. Accumulation
             should not be included. It will automatically be calculated if
             all GEOS-Chem budget operations are passed and optional arg
             compute_accum is True.
             Default value: ["Chemistry","Convection","EmisDryDep",
                             "Mixing","Transport","WetDep"]
@@ -4443,14 +4431,26 @@
     cmnvars = vardict["commonvars2D"]
 
     # Reduce each list to only variables containing "Budget" and not "Strat"
     refonly = [v for v in refonly if "Budget" in v and "Strat" not in v]
     devonly = [v for v in devonly if "Budget" in v and "Strat" not in v]
     cmnvars = [v for v in cmnvars if "Budget" in v and "Strat" not in v]
 
+    # Special handling for fixed level budget diagnostic
+    # Get variable name prefix, e.g. Levs1to35. Check that all fixed level
+    # vars have the same prefix. Update section names used in table.
+    fixedlevvars = [v for v in cmnvars if "Budget" in v and "Levs" in v]
+    if fixedlevvars is not None:
+        fixedlevnames = [v[v.index('Levs'):].split("_")[0] for v in fixedlevvars]
+        if len(set(fixedlevnames)) > 1:
+            msg = "Budget fixed level diagnostic name must be constant!"
+            raise ValueError(msg)
+        col_sections = [v.replace('FixedLevs',fixedlevnames[0]) for v in col_sections]
+        gc_sections = [v.replace('FixedLevs',fixedlevnames[0]) for v in gc_sections]
+
     # Get the species list, depending on if species was passed as argument.
     if species is not None:
         spclist = species
     else:
         # For each column section, get the union or intersection (depending
         # on optional argument require_overlap) of all budget diagnostic
         # species and sort alphabetically. A species is counted even if only
@@ -4557,20 +4557,23 @@
     # Populate dataframe for GEOS-Chem operations and column sections
     # ------------------------------------------
     print('Calculating budgets for all data operations and column sections...')
 
     # Loop over sections (only those with data in files)
     for gc_section in gc_sections:
 
+        # Keep track of progress in log
+        print(f"  {gc_section}")
+
         # Loop over species in that section
         for i, spc in enumerate(spclist):
 
-            # Keep track of progress
-            if (i + 1) % 50 == 0:
-                print(f"  {gc_section}: species {i + 1} of {n_spc}")
+            # Keep track of progress (debugging print)
+            #if (i + 1) % 50 == 0:
+            #    print(f"  {gc_section}: species {i + 1} of {n_spc}")
 
             # Loop over operations (only those with data in files)
             for gc_operation in gc_operations:
 
                 # Get the dataframe row to fill. Skip if not found.
                 dfrow = (df["Column_Section"] == gc_section) \
                     & (df["Species"] == spc) \
@@ -4619,22 +4622,22 @@
                 df.loc[dfrow, "Diff"] = diff
                 df.loc[dfrow, "Pct_diff"] = pctdiff
 
     # ------------------------------------------
     # Compute Strat for each data operation (if applicable)
     # ------------------------------------------
     if compute_strat:
-        print('Computing Strat budgets from Trop and Full...')
+        print('Computing Strat budgets from Trop and Full')
 
         # Loop over species
         for i, spc in enumerate(spclist):
 
-            # Keep track of progress
-            if (i + 1) % 50 == 0:
-                print(f"  Strat: species {i + 1} of {n_spc}")
+            # Keep track of progress (debugging print)
+            #if (i + 1) % 50 == 0:
+            #    print(f"  Strat: species {i + 1} of {n_spc}")
 
             # Loop over operations (only those with data in files)
             for gc_operation in gc_operations:
 
                 # Get the strat dataframe row to fill. Skip if not found.
                 dfrow = (df["Column_Section"] == "Strat") \
                     & (df["Species"] == spc) \
@@ -4686,20 +4689,23 @@
     # ------------------------------------------
     if compute_accum:
         print('Computing ACCUMULATION operation budgets...')
 
         # Loop over all column sections
         for col_section in col_sections:
 
+            # Keep track of progress in log
+            print(f"  {col_section}")
+
             # Loop over species
             for i, spc in enumerate(spclist):
 
-                # Keep track of progress
-                if (i + 1) % 50 == 0:
-                    print(f"  {col_section}: species {i + 1} of {n_spc}")
+                # Keep track of progress (debugging print)
+                #if (i + 1) % 50 == 0:
+                #    print(f"  {col_section}: species {i + 1} of {n_spc}")
 
                 # Get the accumulation dataframe row to fill.Skip if not found.
                 dfrow = (df["Column_Section"] == col_section) \
                     & (df["Species"] == spc) \
                     & (df["Operation"] == "ACCUMULATION")
                 if not any(dfrow):
                     continue
@@ -4905,189 +4911,14 @@
     # ------------------------------------------
     del df
     del ref_ds
     del dev_ds
     gc.collect()
 
 
-def make_benchmark_mass_conservation_table(
-        datafiles,
-        runstr,
-        dst="./benchmark",
-        overwrite=False,
-        areapath=None,
-        spcdb_dir=os.path.dirname(__file__)
-):
-    """
-    Creates a text file containing global mass of the PassiveTracer
-    from Transport Tracer simulations across a series of restart files.
-
-    Args:
-        datafiles: list of str
-            Path names of restart files.
-        runstr: str
-            Name to put in the filename and header of the output file
-        refstr: str
-            A string to describe ref (e.g. version number)
-        dev: str
-            Path name of "Dev" (aka "Development") data set file.
-            The "Dev" data set will be compared against the "Ref" data set.
-        devmet: list of str
-            Path name of dev meteorology data set.
-        devstr: str
-            A string to describe dev (e.g. version number)
-
-    Keyword Args (optional):
-        dst: str
-            A string denoting the destination folder where the file
-            containing emissions totals will be written.
-            Default value: "./benchmark"
-        overwrite: bool
-            Set this flag to True to overwrite files in the
-            destination folder (specified by the dst argument).
-            Default value: False
-        areapath: str
-            Path to a restart file containing surface area data.
-            Default value: None
-        spcdb_dir: str
-            Path to the species_database.yml
-            Default value: points to gcpy/gcpy folder
-    """
-
-    # ==================================================================
-    # Initialize
-    # ==================================================================
-
-    # Create the destination folder
-    util.make_directory(dst, overwrite)
-
-    # Load a YAML file containing species properties (such as
-    # molecular weights), which we will need for unit conversions.
-    properties = util.read_config_file(
-        os.path.join(
-            spcdb_dir,
-            "species_database.yml"
-        ),
-        quiet=True
-    )
-
-    # Get the species name
-    spc_name = 'PassiveTracer'
-
-    # Get a list of properties for the given species
-    species_properties = properties.get(spc_name)
-
-    # Specify target units
-    target_units = "Tg"
-
-    dates = []
-    masses = []
-
-    # ==================================================================
-    # Make sure that surface area data is found
-    # ==================================================================
-    with warnings.catch_warnings():
-        warnings.filterwarnings("ignore", category=xr.SerializationWarning)
-
-
-    # ==================================================================
-    # Calculate global mass for the tracer at all restart dates
-    # ==================================================================
-    for f in datafiles:
-        ds = xr.open_dataset(f, drop_variables=skip_these_vars)
-
-        # Save date in desired format
-        #datestr = str(pd.to_datetime(ds.time.values[0]))
-        #dates.append(datestr[:4] + '-' + datestr[5:7] + '-' + datestr[8:10])
-
-        # Find the area variable in Dev
-        if areapath is None:
-            area = util.get_area_from_dataset(ds)
-        else:
-            area = util.get_area_from_dataset(
-                xr.open_dataset(
-                    areapath,
-                    drop_variables=skip_these_vars
-                )
-            )
-
-        # Assume typical restart file name format, but avoid using dates
-        # from within files which may be incorrect for the initial restart
-        datestr = f.split('/')[-1].split('.')[2][:9]
-        dates.append(datestr[:4] + '-' + datestr[4:6] + '-' + datestr[6:8])
-
-        # Select for GCC or GCHP
-        delta_p = ds['Met_DELPDRY'] if 'Met_DELPDRY' in list(ds.data_vars) else ds['DELP_DRY']
-
-        # ==============================================================
-        # Convert units of Ref and save to a DataArray
-        # (or skip if Ref contains NaNs everywhere)
-        # ==============================================================
-        # Select for GCC or GCHP
-        if 'SpeciesRst_PassiveTracer' in list(ds.data_vars):
-            attrs = ds['SpeciesRst_PassiveTracer'].attrs
-            da = ds['SpeciesRst_PassiveTracer'].astype(np.float64)
-            da.attrs = attrs
-        else:
-            attrs = ds['SPC_PassiveTracer'].attrs
-            da = ds['SPC_PassiveTracer'].astype(np.float64)
-            da.attrs = attrs
-        da = convert_units(
-            da,
-            spc_name,
-            species_properties,
-            target_units,
-            area_m2=area,
-            delta_p=delta_p
-        )
-
-        # Save total global mass
-        masses.append(np.sum(da.values))
-
-        # Clean up
-        del ds
-        del da
-        gc.collect()
-
-    # Calclate max and min mass, absolute diff, percent diff
-    max_mass = np.max(masses)
-    min_mass = np.min(masses)
-    # Convert absdiff to grams
-    absdiff = (max_mass-min_mass) * 10**12
-    pctdiff = (max_mass-min_mass)/min_mass * 100
-
-    # ==================================================================
-    # Print masses to file
-    # ==================================================================
-    # Create file
-    outfilename = os.path.join(dst, "Passive_mass.txt")
-
-    with open(outfilename, 'w') as f:
-        titlestr = '  Global Mass of Passive Tracer in ' + runstr + '  '
-        #headers
-        print('%' * (len(titlestr)+4), file=f)
-        print(titlestr, file=f)
-        print('%' * (len(titlestr)+4), file=f)
-        print('', file=f)
-        print(' Date' + ' ' * 8 + 'Mass [Tg]', file=f)
-        print(' ' + '-' * 10 + '  ' + '-' * 16, file=f)
-        #masses
-        for i in range(len(masses)):
-            print(f" {dates[i]}  {masses[i] : 11.13f}", file=f)
-        print(' ', file=f)
-        print(' Summary', file=f)
-        print(' ' + '-' * 30, file=f)
-        print(f" Max mass =  {max_mass : 2.13f} Tg", file=f)
-        print(f" Min mass =  {min_mass : 2.13f} Tg", file=f)
-        print(f" Abs diff =  {absdiff : >16.3f} g", file=f)
-        print(f" Pct diff =  {pctdiff : >16.10f} %", file=f)
-
-    gc.collect()
-
-
 def get_species_database_dir(config):
     """
     Returns the directory in which the species_database.yml file is
     located.  If "paths:spcdb_dir" (as specified in the benchmark YAML
     configuration file) is None, then it will look for species_database.yml
     in a default location (i.e. in one of the Dev folders).
```

### Comparing `geoschem-gcpy-1.4.2/gcpy/bpch_to_nc_names.yml` & `geoschem_gcpy-1.5.0/gcpy/bpch_to_nc_names.yml`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/budget_ox.py` & `geoschem_gcpy-1.5.0/gcpy/benchmark/modules/budget_ox.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 import os
 import warnings
 from calendar import monthrange
 import numpy as np
 import xarray as xr
 import gcpy.constants as constants
 from gcpy.grid import get_troposphere_mask
-import gcpy.util as util
+from gcpy.util import get_filepath, read_config_file, \
+    rename_and_flip_gchp_rst_vars, reshape_MAPL_CS
+from gcpy.benchmark.modules.benchmark_utils import \
+    add_lumped_species_to_dataset, get_lumped_species_definitions
 import gc
 
 # Suppress harmless run-time warnings (mostly about underflow in division)
 warnings.filterwarnings("ignore", category=RuntimeWarning)
 warnings.filterwarnings("ignore", category=UserWarning)
 
 # ======================================================================
@@ -103,16 +106,16 @@
         self.ds_ini = self.read_rst(self.y0_str)
         self.ds_end = self.read_rst(self.y1_str)
 
         # Change the restart datasets into format similar to GCC, and flip
         # vertical axis.  Also test if the restart files have the BXHEIGHT
         # variable contained within them.
         if is_gchp:
-            self.ds_ini = util.rename_and_flip_gchp_rst_vars(self.ds_ini)
-            self.ds_end = util.rename_and_flip_gchp_rst_vars(self.ds_end)
+            self.ds_ini = rename_and_flip_gchp_rst_vars(self.ds_ini)
+            self.ds_end = rename_and_flip_gchp_rst_vars(self.ds_end)
 
         # Read diagnostics
         self.get_diag_paths()
         self.ds_dry = self.read_diag("DryDep", prefix="DryDep_")
         self.ds_pl = self.read_diag("ProdLoss")
         self.ds_met = self.read_diag("StateMet", prefix="Met_")
         self.ds_wcv = self.read_diag("WetLossConv", prefix="WetLossConv_")
@@ -136,36 +139,36 @@
 
         Returns
            lspc_dict : dict
         """
         # First look in the current folder
         lspc_path = "lumped_species.yml"
         if os.path.exists(lspc_path):
-            lspc_dict = util.read_config_file(lspc_path, quiet=True)
+            lspc_dict = read_config_file(lspc_path, quiet=True)
             return lspc_dict
 
         # Then look in the same folder where the species database is
         lspc_path = os.path.join(self.spcdb_dir, "lumped_species.yml")
         if os.path.exists(lspc_path):
-            lspc_dict = util.read_config_file(lspc_path, quiet=True)
+            lspc_dict = read_config_file(lspc_path, quiet=True)
             return lspc_dict
 
         # Then look in the GCPy source code folder
-        lspc_dict = util.get_lumped_species_definitions()
+        lspc_dict = get_lumped_species_definitions()
         return lspc_dict
 
 
     def rst_file_path(self, ystr):
         """
         Returns the restart file path
 
         Arguments:
             ystr : Year string (YYYY) format
         """
-        return util.get_filepath(
+        return get_filepath(
             self.devrstdir,
             "Restart",
             np.datetime64(f"{ystr}-01-01T00:00:00"),
             is_gchp=self.is_gchp,
             gchp_res=self.gchp_res,
             gchp_is_pre_14_0=self.gchp_is_pre_14_0
         )
@@ -210,15 +213,15 @@
         )
 
         if self.is_gchp:
             RstPrefix="SPC_"
         else:
             RstPrefix="SpeciesRst_"
 
-        ds = util.add_lumped_species_to_dataset(
+        ds = add_lumped_species_to_dataset(
             ds,
             lspc_dict=self.lspc_dict,
             verbose=False,
             prefix=RstPrefix
         )
 
         return ds
@@ -239,15 +242,15 @@
             self.pathlist[collection],
             drop_variables=constants.skip_these_vars,
             combine="nested",
             concat_dim="time"
         )
 
         if prefix is not None:
-            ds = util.add_lumped_species_to_dataset(
+            ds = add_lumped_species_to_dataset(
                 ds,
                 lspc_dict=self.lspc_dict,
                 verbose=False,
                 prefix=prefix
             )
 
         return ds
@@ -261,15 +264,15 @@
         # The area in cm2 is on the History diagnostic grid
         # Both grids are identical in GCClassic but differ in GCHP
         if self.is_gchp:
             if 'Met_AREAM2' not in self.ds_met.data_vars.keys():
                 msg = 'Could not find Met_AREAM2 in StateMet_avg collection!'
                 raise ValueError(msg)
             area_m2 = self.ds_met["Met_AREAM2"].isel(time=0)
-            area_m2 = util.reshape_MAPL_CS(area_m2)
+            area_m2 = reshape_MAPL_CS(area_m2)
             self.area_m2 = area_m2
             self.area_cm2 = self.ds_met["Met_AREAM2"].isel(time=0) * 1.0e4
         else:
             self.area_m2 = self.ds_met["AREA"].isel(time=0)
             self.area_cm2 = self.area_m2 * 1.0e4
 
         # Box volume [cm3]
@@ -307,15 +310,15 @@
 
         Arguments:
            spcdb_dir : str
                Path to the species_database.yml file
         """
         # Read the species database
         path = os.path.join(spcdb_dir, "species_database.yml")
-        spcdb = util.read_config_file(path, quiet=True)
+        spcdb = read_config_file(path, quiet=True)
 
         # Molecular weights [kg mol-1], as taken from the species database
         self.mw = {}
         self.mw["O3"] = spcdb["O3"]["MW_g"] * 1.0e-3
         self.mw["Ox"] = self.mw["O3"]
         self.mw["Air"] = constants.MW_AIR_g * 1.0e-3
```

### Comparing `geoschem-gcpy-1.4.2/gcpy/budget_tt.py` & `geoschem_gcpy-1.5.0/gcpy/benchmark/modules/budget_tt.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 import warnings
 from calendar import monthrange
 import numpy as np
 import xarray as xr
 import gcpy.constants as constants
 from gcpy.grid import get_troposphere_mask
 import gcpy.util as util
+from gcpy.benchmark.modules.benchmark_utils import \
+    rename_speciesconc_to_speciesconcvv
 import gc
 
 # Suppress harmless run-time warnings (mostly about underflow in division)
 warnings.filterwarnings("ignore", category=RuntimeWarning)
 warnings.filterwarnings("ignore", category=UserWarning)
 
 # ======================================================================
@@ -202,14 +204,17 @@
         )
 
         self.ds_cnc = xr.open_mfdataset(
             SpeciesConc,
             drop_variables=constants.skip_these_vars,
             **extra_kwargs
         )
+        self.ds_cnc = rename_speciesconc_to_speciesconcvv(
+            self.ds_cnc
+        )
 
         self.ds_wcv = xr.open_mfdataset(
             WetLossConv,
             drop_variables=constants.skip_these_vars,
             **extra_kwargs
         )
 
@@ -289,15 +294,15 @@
         # ------------------------------
 
         # List of species (and subsets for the trop & strat)
         self.species_list = ["Pb210", "Be7", "Be10"]
 
         # Read the species database
         path = os.path.join(spcdb_dir, "species_database.yml")
-        spcdb = util.read_config_file(path)
+        spcdb = util.read_config_file(path, quiet=True)
 
         # Molecular weights [g mol-1], as taken from the species database
         self.mw = {}
         for v in self.species_list:
             self.mw[v] = spcdb[v]["MW_g"]
         self.mw["Air"] = constants.MW_AIR_g
 
@@ -694,19 +699,22 @@
         print(f"Directory {globvars.dst} exists. {err_str}")
         return
     elif not os.path.isdir(globvars.dst):
         os.makedirs(globvars.dst)
 
     # Filename to print
     if "_f" in key:
-        filename = f"{globvars.dst}/Pb-Be_budget_trop_strat.txt"
+        filename = \
+            f"{globvars.dst}/Pb-Be_budget_trop_strat.{globvars.devstr}.txt"
     elif "_t" in key:
-        filename = f"{globvars.dst}/Pb-Be_budget_troposphere.txt"
+        filename = \
+            f"{globvars.dst}/Pb-Be_budget_troposphere.{globvars.devstr}.txt"
     elif "_s" in key:
-        filename = f"{globvars.dst}/Pb-Be_budget_stratosphere.txt"
+        filename = \
+            f"{globvars.dst}/Pb-Be_budget_stratosphere.{globvars.devstr}.txt"
 
     # Common title string
     title = "Annual Average Global Budgets of 210Pb, 7Be, and 10Be\n        "
 
     # Open file and print budgets
     with open(filename, "w+") as f:
         if "_f" in key:
```

### Comparing `geoschem-gcpy-1.4.2/gcpy/constants.py` & `geoschem_gcpy-1.5.0/gcpy/constants.py`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/cstools.py` & `geoschem_gcpy-1.5.0/gcpy/cstools.py`

 * *Files 4% similar despite different names*

```diff
@@ -716,17 +716,15 @@
         The input data.
 
     Returns:
     --------
     True if the grid has History diagnostic dimensions,
     False otherwise.
     """
-    if "nf" in data.dims:
-        return True
-    return False
+    return "nf" in data.dims
 
 
 def is_cubed_sphere_rst_grid(data):
     """
     Determines if a cubed-sphere grid has restart file dimensions.
     (i.e. lat and lon, with lat = lon*6).
 
@@ -742,20 +740,25 @@
     gcpy.util.verify_variable_type(data, (xr.DataArray, xr.Dataset))
 
     # TODO: Rethink this if we ever end up changing the GC-Classic
     # restart variables to start with SPC, or if we ever rename the
     # internal state variables in GCHP. A more robust back-up check
     # could be to see if all the lats and lons are integer, since
     # that will be the case with the GCHP restart file format.
-    if "lat" in data.dims:
-        if data.dims["lat"] == data.dims["lon"] * 6:
-            return True
-    if "SPC_" in data.data_vars.keys():
-        return True
-    return False
+
+    # NOTE: in DataArray objects, dims is a tuple but not a dict!
+    # Comparing the len of the lat & lon coords will work for both.
+    if "lat" in data.coords:
+         return len(data.coords["lat"]) == len(data.coords["lon"]) * 6
+
+    # Dataset: search data.data_vars for "SPC_"
+    # DataArray: search data.name for "SPC_"
+    if isinstance(data, xr.Dataset):
+        return "SPC_" in data.data_vars.keys()
+    return "SPC_" in data.name
 
 
 def get_cubed_sphere_res(data):
     """
     Given a Dataset or DataArray object, returns the number of
     grid cells along one side of the cubed-sphere grid face
     (e.g. 24 for grid resolution C24, which has 24x25 grid cells
@@ -772,17 +775,21 @@
         The cubed-sphere resolution.  Will return 0 if the data
         is not placed on a cubed-sphere grid.
     """
     gcpy.util.verify_variable_type(data, (xr.DataArray, xr.Dataset))
 
     if not is_cubed_sphere(data):
         return 0
+
+    # NOTE: In Dataset objects "dims" is a dict, but in DataArray
+    # objects "dims" is a tuple.  Returning the length of the
+    # corresponding coords array should work in both cases.
     if is_cubed_sphere_rst_grid(data):
-        return data.dims["lon"]
-    return data.dims["Xdim"]
+        return len(data.coords["lon"])
+    return len(data.coords["Xdim"])
 
 
 def is_gchp_lev_positive_down(data):
     """
     Determines if GCHP data is arranged vertically from the top of the
     atmosphere downwards or from the surface upwards, according to:
```

### Comparing `geoschem-gcpy-1.4.2/gcpy/date_time.py` & `geoschem_gcpy-1.5.0/gcpy/date_time.py`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/emission_species.yml` & `geoschem_gcpy-1.5.0/gcpy/benchmark/modules/emission_species.yml`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,15 @@
   DST4: Tg
   EOH: Tg
   ETNO3: Tg
   FURA: Tg
   GLYC: Tg
   GLYX: Tg
   HAC: Tg
+  HCl: Tg
   HCOOH: Tg
   HNO2: Tg
   HNO3: Tg
   ISOP: Tg
   LIMO: Tg
   MACR: Tg
   MEK: Tg
```

### Comparing `geoschem-gcpy-1.4.2/gcpy/examples/bpch_to_nc/bpch2nc.py` & `geoschem_gcpy-1.5.0/gcpy/examples/bpch_to_nc/bpch2nc.py`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/examples/bpch_to_nc/bpch_tagco_prodloss_to_nc.py` & `geoschem_gcpy-1.5.0/gcpy/examples/bpch_to_nc/bpch_tagco_prodloss_to_nc.py`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/examples/diagnostics/README.md` & `geoschem_gcpy-1.5.0/gcpy/examples/diagnostics/README.md`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/examples/diagnostics/compare_diagnostics.ipynb` & `geoschem_gcpy-1.5.0/gcpy/examples/diagnostics/compare_diagnostics.ipynb`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/examples/diagnostics/compare_diags.py` & `geoschem_gcpy-1.5.0/gcpy/examples/diagnostics/compare_diags.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 as an argument.
 """
 import os
 import sys
 import warnings
 import numpy as np
 from gcpy.util import add_missing_variables, compare_varnames, \
-    dataset_reader, read_config_file
+    dataset_reader, read_config_file, rename_and_flip_gchp_rst_vars
 from gcpy.constants import skip_these_vars
 from gcpy.plot.compare_single_level import compare_single_level
 from gcpy.plot.compare_zonal_mean import compare_zonal_mean
 
 # Tell matplotlib not to look for an X-window
 os.environ["QT_QPA_PLATFORM"] = "offscreen"
 
@@ -105,16 +105,16 @@
     except FileNotFoundError as exc:
         msg = "Error reading " + dev_file
         raise FileNotFoundError(msg) from exc
 
     # If the data is from a GCHP restart file, rename variables and
     # flip levels to match the GEOS-Chem Classic naming and level
     # conventions.  Otherwise no changes will be made.
-    refdata = util.rename_and_flip_gchp_rst_vars(refdata)
-    devdata = util.rename_and_flip_gchp_rst_vars(devdata)
+    refdata = rename_and_flip_gchp_rst_vars(refdata)
+    devdata = rename_and_flip_gchp_rst_vars(devdata)
 
     # Define dictionary for return
     data = {
         "ref": refdata,
         "dev": devdata
     }
```

### Comparing `geoschem-gcpy-1.4.2/gcpy/examples/diagnostics/compare_diags.yml` & `geoschem_gcpy-1.5.0/gcpy/examples/diagnostics/compare_diags.yml`

 * *Files 9% similar despite different names*

```diff
@@ -29,7 +29,8 @@
   totals_and_diffs:
     create_table: True
     diff_type: absdiff             # Values: percent, pctdiff, %, abs, absdiff
     print_to_screen: True
     filename: ''
     skip_small_diffs: True
     small_diff_threshold: 0.0000
+  n_cores: -1
```

### Comparing `geoschem-gcpy-1.4.2/gcpy/examples/dry_run/download_data.py` & `geoschem_gcpy-1.5.0/gcpy/examples/dry_run/download_data.py`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/examples/dry_run/download_data.yml` & `geoschem_gcpy-1.5.0/gcpy/examples/dry_run/download_data.yml`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/examples/plotting/create_test_plot.py` & `geoschem_gcpy-1.5.0/gcpy/examples/plotting/create_test_plot.py`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/examples/plotting/plot_comparisons.py` & `geoschem_gcpy-1.5.0/gcpy/examples/plotting/plot_comparisons.py`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/examples/working_with_files/add_blank_var_to_restart_file.py` & `geoschem_gcpy-1.5.0/gcpy/examples/working_with_files/add_blank_var_to_restart_file.py`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/examples/working_with_files/concatenate_files.py` & `geoschem_gcpy-1.5.0/gcpy/examples/working_with_files/concatenate_files.py`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/examples/working_with_files/insert_field_into_restart_file.py` & `geoschem_gcpy-1.5.0/gcpy/examples/working_with_files/insert_field_into_restart_file.py`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/examples/working_with_files/regrid_restart_ll_to_cs.py` & `geoschem_gcpy-1.5.0/gcpy/examples/working_with_files/regrid_restart_ll_to_cs.py`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/examples/xarray_examples/xarray_overview.ipynb` & `geoschem_gcpy-1.5.0/gcpy/examples/xarray_examples/xarray_overview.ipynb`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/file_regrid.py` & `geoschem_gcpy-1.5.0/gcpy/file_regrid.py`

 * *Files 0% similar despite different names*

```diff
@@ -741,33 +741,43 @@
 
         # Drop non-regriddable variables
         non_fields = [
             var for var in dset.variables.keys() \
             if "lat" not in dset[var].dims       \
                 and "lon" not in dset[var].dims
             ]
-        dset = dset.drop(["lat_bnds", "lon_bnds"])
+        if "lat_bnds" in dset.data_vars:
+            dset = dset.drop(["lat_bnds"])
+        if "lon_bnds" in dset.data_vars:
+            dset = dset.drop(["lon_bnds"])
         non_fields = dset[non_fields]
         dset = dset.drop(non_fields)
 
         # Set the lev:positive attribute accordingly
         dset = flip_lev_coord_if_necessary(
             dset,
             dim_format_in="classic",
             dim_format_out="classic"
         )
 
+        # Decide if we are regridding a data file or a mask
+        # by testing for the variable name "MASK"
+        method = "conservative"
+        if "MASK" in dset.data_vars:
+            method = "nearest_s2d"
+
         # Create the regridder and regrid the data
         regridder = make_regridder_L2L(
         ll_res_in,
             ll_res_out,
             reuse_weights=True,
             in_extent=in_extent,
             out_extent=out_extent,
-            weightsdir=weightsdir
+            weightsdir=weightsdir,
+            method=method,
         )
         dset = regridder(
             dset,
             keep_attrs=True
         )
 
         # Add the non-regriddable fields back
@@ -1096,32 +1106,33 @@
         old_to_new = {}
 
         # ==============================================================
         # classic/diagnostic -> checkpoint
         # ==============================================================
         if towards_gchp:
             for var in dset.data_vars.keys():
-                if "Met_DELPDRY" in var:
-                    old_to_new[var] = "DELP_DRY"
                 if var.startswith("Met_"):
-                    old_to_new[var] = var.replace("Met_", "")
+                    if "DELPDRY" in var:
+                        old_to_new[var] = "DELP_DRY"
+                    else:
+                        old_to_new[var] = var.replace("Met_", "")
                 if var.startswith("Chem_"):
                     old_to_new[var] = var.replace("Chem_", "")
                 if var.startswith("SpeciesRst_"):
                     old_to_new[var] = var.replace("SpeciesRst_", "SPC_")
                 if var.startswith("SpeciesConcVV_"):
                     old_to_new[var] = var.replace("SpeciesConcVV_", "SPC_")
 
             return dset.rename(old_to_new)
 
         # ==============================================================
         # checkpoint -> classic/diagnostic
         # ==============================================================
         for var in dset.data_vars.keys():
-            if var == "DELP_DRY":
+            if var == "DELP_DRY" or var == "DELPDRY":
                 old_to_new[var] = "Met_DELPDRY"
             if var == "BXHEIGHT":
                 old_to_new[var] = "Met_BXHEIGHT"
             if var == "StatePSC":
                 old_to_new[var] = "Chem_StatePSC"
             if var == "KPPHvalue":
                 old_to_new[var] = "Chem_KPPHvalue"
```

### Comparing `geoschem-gcpy-1.4.2/gcpy/grid.py` & `geoschem_gcpy-1.5.0/gcpy/grid.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 manipulate GEOS-Chem horizontal and vertical grids
 """
 from itertools import product
 import xarray as xr
 import numpy as np
 import scipy.sparse
 from gcpy.util import get_shape_of_data, verify_variable_type
-from .grid_stretching_transforms import scs_transform
+from gcpy.grid_stretching_transforms import scs_transform
 from gcpy.constants import R_EARTH_m
+from gcpy.cstools import find_index, is_cubed_sphere
 
 
 def get_troposphere_mask(ds):
     """
     Returns a mask array for picking out the tropospheric grid boxes.
 
     Args:
@@ -243,57 +244,66 @@
             maxlon = np.max(lon) + abs(abs(lon[-1]) - abs(lon[-2]))
             return minlon, maxlon, minlat, maxlat
     else:
         # GCHP data using MAPL v1.0.0+ has dims time, lev, nf, Ydim, and Xdim
         return -180, 180, -90, 90
 
 
-def get_vert_grid(dataset, AP=[], BP=[]):
+def get_vert_grid(
+        dataset,
+        AP=None,
+        BP=None,
+        p_sfc=1013.25):
     """
     Determine vertical grid of input dataset
 
     Args:
-        dataset: xarray Dataset
-            A GEOS-Chem output dataset
+    -----
+    dataset (xr.Dataset) : A GEOS-Chem output dataset
 
     Keyword Args (optional):
-        AP: list-like type
-            Hybrid grid parameter A in hPa
-            Default value: []
-        BP: list-like type
-            Hybrid grid parameter B (unitless)
-            Default value: []
+    ------------------------
+    AP (list-like) : Hybrid grid parameter A (hPA)
+    BP    (list-like) : Hybrid grid parameter B (unitless)
+    p_sfc (float) :
 
     Returns:
-        p_edge: numpy array
-            Edge pressure values for vertical grid
-        p_mid: numpy array
-            Midpoint pressure values for vertical grid
-        nlev: int
-            Number of levels in vertical grid
+    --------
+    pedge (np.ndarray) : Edge pressure values for vertical grid
+    p_mid (np.ndarray) : Midpoint pressure values for vertical grid
+    nlev: (int       ) : Number of levels in vertical grid
     """
 
+    # 72L GEOS grid
     if dataset.sizes["lev"] in (72, 73):
-        return GEOS_72L_grid.p_edge(), GEOS_72L_grid.p_mid(), 72
-    elif dataset.sizes["lev"] in (47, 48):
-        return GEOS_47L_grid.p_edge(), GEOS_47L_grid.p_mid(), 47
-    elif AP == [] or BP == []:
+        grid = vert_grid(_GEOS_72L_AP, _GEOS_72L_BP, p_sfc)
+        return grid.p_edge(), grid.p_mid(), 72
+
+    # 47L GEOS grid
+    if dataset.sizes["lev"] in (47, 48):
+        grid = vert_grid(_GEOS_47L_AP, _GEOS_47L_BP, p_sfc)
+        return grid.p_edge(), grid.p_mid(), 47
+
+    # Grid without specified AP, BP
+    if AP == None or BP == None:
         if dataset.sizes["lev"] == 1:
             AP = [1, 1]
             BP = [1]
-            new_grid = vert_grid(AP, BP)
-            return new_grid.p_edge(), new_grid.p_mid(), np.size(AP)
-        else:
-            raise ValueError(
-                "Only 72/73 or 47/48 level vertical grids are automatically determined" +
-                "from input dataset by get_vert_grid(), please pass grid parameters AP and BP" +
-                "as keyword arguments")
-    else:
-        new_grid = vert_grid(AP, BP)
-        return new_grid.p_edge(), new_grid.p_mid(), np.size(AP)
+            grid = vert_grid(AP, BP, p_sfc)
+            return grid.p_edge(), grid.p_mid(), np.size(AP)
+
+        raise ValueError(
+            "Only 72/73 or 47/48 level vertical grids are automatically\n" +
+            "determined from input dataset by get_vert_grid().\n" +
+            "please pass grid parameters AP and BP as keyword arguments"
+        )
+
+    # Grid with specified AP, BP
+    grid = vert_grid(AP, BP, p_sfc)
+    return grid.p_edge(), grid.p_mid(), np.size(AP)
 
 
 def get_ilev_coord(
         n_lev=72,
         AP_edge=None,
         BP_edge=None,
         top_down=False,
@@ -1573,7 +1583,184 @@
         x_new = cos_ang * x + sin_ang * y
         y_new = -sin_ang * x + cos_ang * y
         z_new = z
 
     theta_new, phi_new, r_new = cartesian_to_spherical(x_new, y_new, z_new)
 
     return theta_new, phi_new, r_new
+
+
+def get_nearest_model_data_cs(
+        gc_data,
+        gc_cs_grid,
+        lon_value,
+        lat_value,
+        varlist=None
+):
+    """
+    Returns GEOS-Chem model data (on a cubed-sphere grid) at the
+    grid box closest to a given (lat, lon) location.
+
+    Args:
+    -----
+    gc_data : xarray.DataArray or xarray.Dataset
+        GEOS-Chem model data for a single variable
+
+    gc_cs_grid: xarray Dataset
+        Coordinate arrays defining the cubed-sphere grid.
+
+    lon_value : float
+        Longitude at the location of interest
+
+    lat_value : float
+        Latitude at the location of interest
+
+
+    Keyword Args (optional):
+    ------------------------
+    varlist : list of str
+        List of data variables to include in the output
+
+    Returns:
+    --------
+    dataframe: pandas.DataFrame
+        Model data closest to the observation site.
+    """
+    verify_variable_type(gc_data, (xr.DataArray, xr.Dataset))
+    verify_variable_type(gc_cs_grid, xr.Dataset)
+
+    # Prevent the latitude from getting too close to the N or S poles
+    lat_value = max(min(lat_value, 89.75), -89.75)
+
+    # Indices (nf, yInd, xInd) of box nearest to observation site
+    cs_indices = find_index(
+        lat_value,
+        lon_value,
+        gc_cs_grid
+    )
+
+    if varlist is not None:
+        return gc_data[varlist].isel(
+            nf=cs_indices[0, 0],
+            Ydim=cs_indices[1, 0],
+            Xdim=cs_indices[2, 0],
+        ).to_dataframe()
+
+    return gc_data.isel(
+        nf=cs_indices[0, 0],
+        Ydim=cs_indices[1, 0],
+        Xdim=cs_indices[2, 0],
+    ).to_dataframe()
+
+
+def get_nearest_model_data_ll(
+        gc_data,
+        lon_value,
+        lat_value,
+        varlist=None
+
+):
+    """
+    Returns GEOS-Chem model data (on a cubed-sphere grid) at the
+    grid box closest to a given (lat, lon) location.
+
+    Args:
+    -----
+    gc_data : xarray.DataArray or xarray.Dataset
+        GEOS-Chem model data
+
+    lon_value : float
+        Longitude at the location of interest
+
+    lat_value : float
+        Latitude at the location of interest
+
+    Keyword Args (optional):
+    ------------------------
+    varlist : list of str
+        List of data variables to include in the output
+
+    Returns:
+    --------
+    dataframe: pandas.DataFrame
+        Model data closest to the observation site.
+    """
+    verify_variable_type(gc_data, (xr.DataArray, xr.Dataset))
+
+    x_idx=(
+        np.abs(
+            gc_data.lon.values - float(lon_value)
+        )
+    ).argmin()
+
+    y_idx=(
+        np.abs(
+            gc_data.lat.values - float(lat_value)
+        )
+    ).argmin()
+
+    if varlist is not None:
+        return gc_data[varlist].isel(
+            lon=x_idx,
+            lat=y_idx,
+        ).to_dataframe()
+
+    return gc_data.isel(
+        lon=x_idx,
+        lat=y_idx,
+    ).to_dataframe()
+
+
+def get_nearest_model_data(
+        gc_data,
+        lon_value,
+        lat_value,
+        gc_cs_grid=None,
+        varlist=None
+):
+    """
+    Args:
+    -----
+    gc_data : xarray.DataArray or xarray.Dataset
+        GEOS-Chem data for a single variable
+
+    gc_cs_grid: xarray.Dataset or NoneType
+        Coordinate arrays defining the cubed-sphere grid.
+
+    lon_value : float
+        Longitude at the location of interest
+
+    lat_value : float
+        Latitude at the location of interest
+
+    Keyword Args (optional):
+    ------------------------
+    gc_cs_grid : xarray.Dataset
+        Datasaet with cubed-sphere grid definition.  This can be
+        obtained as the output of function gcpy.util.extract_data().
+
+    varlist : list of str
+        List of data variables to include in the output
+
+    Returns:
+    --------
+    dataframe: pandas.DataFrame
+        Model data closest to the observation site.
+    """
+    verify_variable_type(gc_data, (xr.DataArray, xr.Dataset))
+    verify_variable_type(gc_cs_grid, (xr.Dataset, type(None)))
+
+    if is_cubed_sphere(gc_data):
+        return get_nearest_model_data_cs(
+            gc_data,
+            gc_cs_grid,
+            lon_value,
+            lat_value,
+            varlist=varlist
+        )
+
+    return get_nearest_model_data_ll(
+        gc_data,
+        lon_value,
+        lat_value,
+        varlist=varlist,
+    )
```

### Comparing `geoschem-gcpy-1.4.2/gcpy/grid_stretching_transforms.py` & `geoschem_gcpy-1.5.0/gcpy/grid_stretching_transforms.py`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/lumped_species.yml` & `geoschem_gcpy-1.5.0/gcpy/benchmark/modules/lumped_species.yml`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/oh_metrics.py` & `geoschem_gcpy-1.5.0/gcpy/benchmark/modules/oh_metrics.py`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/plot/colormaps/WhGrYlRd.txt` & `geoschem_gcpy-1.5.0/gcpy/plot/colormaps/WhGrYlRd.txt`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/plot/compare_single_level.py` & `geoschem_gcpy-1.5.0/gcpy/plot/compare_single_level.py`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/plot/compare_zonal_mean.py` & `geoschem_gcpy-1.5.0/gcpy/plot/compare_zonal_mean.py`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/plot/core.py` & `geoschem_gcpy-1.5.0/gcpy/plot/core.py`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/plot/gcpy_plot_style` & `geoschem_gcpy-1.5.0/gcpy/plot/gcpy_plot_style`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/plot/single_panel.py` & `geoschem_gcpy-1.5.0/gcpy/plot/single_panel.py`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/plot/six_plot.py` & `geoschem_gcpy-1.5.0/gcpy/plot/six_plot.py`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/raveller_1D.py` & `geoschem_gcpy-1.5.0/gcpy/raveller_1D.py`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/regrid.py` & `geoschem_gcpy-1.5.0/gcpy/regrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -422,15 +422,15 @@
             cmpgridtype = refgridtype
         elif refgridtype == "cs" and devgridtype == "cs":
             if zm:
                 print(
                     "Warning: zonal mean comparison must be lat-lon. Defaulting to 1x1.25")
                 cmpres = '1x1.25'
                 cmpgridtype = "ll"
-            elif sg_ref_params != [] or sg_dev_params != []:
+            elif sg_ref_params != [1, 170, -90] or sg_dev_params != [1, 170, -90]:
                 # pick ref grid when a stretched-grid and non-stretched-grid
                 # are passed
                 cmpres = refres
                 cmpgridtype = "cs"
                 sg_cmp_params = sg_ref_params
             else:
                 # pick higher resolution CS grid out of two standard
@@ -754,14 +754,20 @@
             cs_res = ds_out['lon'].size
         ds_out = ds_out.stack(lat=['lat_level_0', 'lat_level_1'])
         ds_out = ds_out.assign_coords({
             'lat': np.linspace(1, 6 * cs_res, 6 * cs_res),
         })
         return ds_out
 
+    # Filter non-existent coordinates/dimensions
+    def rename_existing(ds, rename_dict):
+        existing_keys = set(ds.coords) | set(ds.dims)
+        filtered_rename_dict = {key: value for key, value in rename_dict.items() if key in existing_keys}
+        return ds.rename(filtered_rename_dict)
+
     dim_formats = {
         'checkpoint': {
             'unravel': [unravel_checkpoint_lat],
             'ravel': [ravel_checkpoint_lat],
             'rename': {
                 'lon': 'X',
                 'lat_level_0': 'F',
@@ -775,49 +781,41 @@
             'rename': {
                 'nf': 'F',
                 'lev': 'Z',
                 'Xdim': 'X',
                 'Ydim': 'Y',
                 'time': 'T',
             },
-            'transpose': ('time', 'lev', 'nf', 'Xdim', 'Ydim')
+            # match format of GCHP output
+            'transpose': ('time', 'lev', 'nf', 'Ydim', 'Xdim')
         }
     }
 
     # %%%% Renaming toward the common format %%%%
     if towards_common:
         # Unravel dimensions
         for unravel_callback in dim_formats[format].get('unravel', []):
             ds = unravel_callback(ds)
 
         # Rename dimensions
-        ds = ds.rename(dim_formats[format].get('rename', {}))
+        ds = rename_existing(ds, dim_formats[format].get('rename', {}))
         return ds
 
 
     # %%%% Renaming from the common format %%%%
     # Reverse rename
-    ds = ds.rename(
+    ds = rename_existing(ds, 
         {v: k for k, v in dim_formats[format].get('rename', {}).items()})
 
     # Ravel dimensions
     for ravel_callback in dim_formats[format].get('ravel', []):
         ds = ravel_callback(ds)
 
     # Transpose
-    if len(ds.dims) == 5 or (len(ds.dims) == 4 and 'lev' in list(
-            ds.dims) and 'time' in list(ds.dims)):
-        # full dim dataset
-        ds = ds.transpose(*dim_formats[format].get('transpose', []))
-    elif len(ds.dims) == 4:
-        # single time
-        ds = ds.transpose(*dim_formats[format].get('transpose', [])[1:])
-    elif len(ds.dims) == 3:
-        # single level / time
-        ds = ds.transpose(*dim_formats[format].get('transpose', [])[2:])
+    ds = ds.transpose(*[x for x in dim_formats[format].get('transpose', []) if x in list(ds.dims)])
     return ds
 
 
 def sg_hash(
         cs_res,
         stretch_factor: float,
         target_lat: float,
```

### Comparing `geoschem-gcpy-1.4.2/gcpy/regrid_restart_file.py` & `geoschem_gcpy-1.5.0/gcpy/regrid_restart_file.py`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/species_database.yml` & `geoschem_gcpy-1.5.0/gcpy/benchmark/modules/species_database.yml`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/ste_flux.py` & `geoschem_gcpy-1.5.0/gcpy/benchmark/modules/ste_flux.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,15 @@
         df: pandas DataFrame
             Strat-trop exchange table
     """
     # Create plot directory hierarchy if necessary
     make_directory(globvars.dst, globvars.overwrite)
 
     # Save the file in the Tables folder of dst
-    filename = f"{globvars.dst}/Strat_trop_exchange.txt"
+    filename = f"{globvars.dst}/Strat_trop_exchange.{globvars.devstr}.txt"
 
     # Set numeric format to be 11 chars wide with 4 decimals
     pd.options.display.float_format = '{:11.4f}'.format
 
     # Open filename for output
     with open(filename, "w+") as f:
```

### Comparing `geoschem-gcpy-1.4.2/gcpy/units.py` & `geoschem_gcpy-1.5.0/gcpy/units.py`

 * *Files identical despite different names*

### Comparing `geoschem-gcpy-1.4.2/gcpy/util.py` & `geoschem_gcpy-1.5.0/gcpy/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Internal utilities for helping to manage xarray and numpy
 objects used throughout GCPy
 """
 import os
+from shutil import copyfile
 import warnings
-import shutil
 from textwrap import wrap
 from yaml import safe_load
 import numpy as np
 import xarray as xr
 from pypdf import PdfWriter, PdfReader
 from gcpy.constants import ENCODING, TABLE_WIDTH
 from gcpy.cstools import is_cubed_sphere_rst_grid
@@ -343,65 +343,14 @@
     pctdiff_fmt = format_number_for_table(pctdiff)
 
     print(f"{display_name[0:19].ljust(19)}: {ref_fmt}  {dev_fmt}  {diff_fmt}  {pctdiff_fmt}  {diff_str}", file=ofile)
 
     return diff_list
 
 
-def get_species_categories(
-        benchmark_type="FullChemBenchmark"
-):
-    """
-    Returns the list of benchmark categories that each species
-    belongs to.  This determines which PDF files will contain the
-    plots for the various species.
-
-    Args:
-        benchmark_type: str
-            Specifies the type of the benchmark (either
-            FullChemBenchmark (default) or TransportTracersBenchmark).
-
-    Returns:
-        spc_cat_dict: dict
-            A nested dictionary of categories (and sub-categories)
-            and the species belonging to each.
-
-    NOTE: The benchmark categories are specified in YAML file
-    benchmark_species.yml.
-    """
-    spc_cat_dict = read_config_file(
-        os.path.join(
-            os.path.dirname(__file__),
-            "benchmark_categories.yml"
-        )
-    )
-    return spc_cat_dict[benchmark_type]
-
-
-def archive_species_categories(
-        dst
-):
-    """
-    Writes the list of benchmark categories to a YAML file
-    named "benchmark_species.yml".
-
-    Args:
-        dst: str
-            Name of the folder where the YAML file containing
-            benchmark categories ("benchmark_species.yml")
-            will be written.
-    """
-    spc_categories = "benchmark_categories.yml"
-    src = os.path.join(os.path.dirname(__file__), spc_categories)
-    copy = os.path.join(dst, spc_categories)
-    if not os.path.exists(copy):
-        print(f"\nArchiving {spc_categories} in {dst}")
-        shutil.copyfile(src, copy)
-
-
 def add_bookmarks_to_pdf(
         pdfname,
         varlist,
         remove_prefix="",
         verbose=False
 ):
     """
@@ -835,14 +784,16 @@
         # TODO: Think of better algorithm in case we ever change
         # the internal state to start with something else than "SPC_".
         if var.startswith("SPC_"):
             spc = var.replace('SPC_', '')
             old_to_new[var] = 'SpeciesRst_' + spc
         if var == "DELP_DRY":
             old_to_new["DELP_DRY"] = "Met_DELPDRY"
+        if var == "DELPDRY":
+            old_to_new["DELPDRY"] = "Met_DELPDRY"
         if var == "BXHEIGHT":
             old_to_new["BXHEIGHT"] = "Met_BXHEIGHT"
         if var == "TropLev":
             old_to_new["TropLev"] = "Met_TropLev"
 
     # Replace variable names in one operation
     dset = dset.rename(old_to_new)
@@ -1246,180 +1197,14 @@
     with xr.set_options(keep_attrs=True):
         dset = dset.rename(name_dict=old_to_new)
 
     # Return the dataset
     return dset
 
 
-def get_lumped_species_definitions():
-    """
-    Returns lumped species definitions from a YAML file.
-
-    Returns:
-        lumped_spc_dict : dict of str
-            Dictionary of lumped species
-    """
-    return read_config_file(
-        os.path.join(
-            os.path.dirname(__file__),
-            "lumped_species.yml"
-        ),
-        quiet=True
-    )
-
-
-def archive_lumped_species_definitions(
-        dst
-):
-    """
-    Archives lumped species definitions to a YAML file.
-
-    Args:
-        dst : str
-            Name of the folder where the YAML file containing
-            benchmark categories ("benchmark_species.yml")
-            will be written.
-    """
-    lumped_spc = "lumped_species.yml"
-    src = os.path.join(os.path.dirname(__file__), lumped_spc)
-    copy = os.path.join(dst, lumped_spc)
-    if not os.path.exists(copy):
-        print(f"\nArchiving {lumped_spc} in {dst}")
-        shutil.copyfile(src, copy)
-
-
-def add_lumped_species_to_dataset(
-        dset,
-        lspc_dict=None,
-        lspc_yaml="",
-        verbose=False,
-        overwrite=False,
-        prefix="SpeciesConcVV_",
-):
-    """
-    Function to calculate lumped species concentrations and add
-    them to an xarray Dataset. Lumped species definitions may be passed
-    as a dictionary or a path to a yaml file. If neither is passed then
-    the lumped species yaml file stored in gcpy is used. This file is
-    customized for use with benchmark simuation SpeciesConc diagnostic
-    collection output.
-
-    Args:
-        dset: xarray Dataset
-            An xarray Dataset object prior to adding lumped species.
-
-    Keyword Args (optional):
-        lspc_dict: dictionary
-            Dictionary containing list of constituent species and their
-            integer scale factors per lumped species.
-            Default value: False
-        lspc_yaml: str
-            Name of the YAML file containing the list of constituent s
-            species and their integer scale factors per lumped species.
-            Default value: ""
-        verbose: bool
-            Whether to print informational output.
-            Default value: False
-        overwrite: bool
-            Whether to overwrite an existing species dataarray in a dataset
-            if it has the same name as a new lumped species. If False and
-            overlapping names are found then the function will raise an error.
-            Default value: False
-        prefix: str
-            Prefix to prepend to new lumped species names. This argument is
-            also used to extract an existing dataarray in the dataset with
-            the correct size and dimensions to use during initialization of
-            new lumped species dataarrays.
-            Default value: "SpeciesConcVV_"
-
-    Returns:
-        dset: xarray Dataset
-            A new xarray Dataset object containing all of the original
-            species plus new lumped species.
-    """
-
-    # Default is to add all benchmark lumped species.
-    # Can overwrite by passing a dictionary
-    # or a yaml file path containing one
-    assert not (
-        lspc_dict is not None and lspc_yaml != ""
-    ), "Cannot pass both lspc_dict and lspc_yaml. Choose one only."
-    if lspc_dict is None and lspc_yaml == "":
-        lspc_dict = get_lumped_species_definitions()
-    elif lspc_dict is None and lspc_yaml != "":
-        lspc_dict = read_config_file(lspc_yaml)
-
-    # Make sure attributes are transferred when copying dataset / dataarrays
-    with xr.set_options(keep_attrs=True):
-
-        # Get a dummy DataArray to use for initialization
-        dummy_darr = None
-        for var in dset.data_vars:
-            if prefix in var or prefix.replace("VV", "") in var:
-                dummy_darr = dset[var]
-                dummy_type = dummy_darr.dtype
-                dummy_shape = dummy_darr.shape
-                break
-        if dummy_darr is None:
-            msg = "Invalid prefix: " + prefix
-            raise ValueError(msg)
-
-        # Create a list with a copy of the dummy DataArray object
-        n_lumped_spc = len(lspc_dict)
-        lumped_spc = [None] * n_lumped_spc
-        for var, spcname in enumerate(lspc_dict):
-            lumped_spc[var] = dummy_darr.copy(deep=False)
-            lumped_spc[var].name = prefix + spcname
-            lumped_spc[var].values = np.full(dummy_shape, 0.0, dtype=dummy_type)
-
-        # Loop over lumped species list
-        for var, lspc in enumerate(lumped_spc):
-
-            # Search key for lspc_dict is lspc.name minus the prefix
-            cidx = lspc.name.find("_")
-            key = lspc.name[cidx+1:]
-
-            # Check if overlap with existing species
-            if lspc.name in dset.data_vars and overwrite:
-                dset.drop(lspc.name)
-            else:
-                assert(lspc.name not in dset.data_vars), \
-                    f"{lspc.name} already in dataset. To overwrite pass overwrite=True."
-
-            # Verbose prints
-            if verbose:
-                print(f"Creating {lspc.name}")
-
-            # Loop over and sum constituent species values
-            num_spc = 0
-            for _, spcname in enumerate(lspc_dict[key]):
-                varname = prefix + spcname
-                if varname not in dset.data_vars:
-                    if verbose:
-                        print(f"Warning: {varname} needed for {lspc_dict[key][spcname]} not in dataset")
-                    continue
-                if verbose:
-                    print(f" -> adding {varname} with scale {lspc_dict[key][spcname]}")
-                lspc.values += dset[varname].values * lspc_dict[key][spcname]
-                num_spc += 1
-
-            # Replace values with NaN if no species found in dataset
-            if num_spc == 0:
-                if verbose:
-                    print("No constituent species found! Setting to NaN.")
-                lspc.values = np.full(lspc.shape, np.nan)
-
-        # Insert the DataSet into the list of DataArrays
-        # so that we can only do the merge operation once
-        lumped_spc.insert(0, dset)
-        dset = xr.merge(lumped_spc)
-
-    return dset
-
-
 def filter_names(
         names,
         text=""):
     """
     Returns elements in a list that match a given substring.
     Can be used in conjnction with compare_varnames to return a subset
     of variable names pertaining to a given diagnostic type or species.
@@ -2430,7 +2215,46 @@
     var_type : type or tuple of types
         A single type definition (list, str, pandas.Series, etc.)
         or a tuple of type definitions.
     """
     if isinstance(var, var_type):
         return
     raise TypeError( f"{var} is not of type: {var_type}!")
+
+
+def copy_file_to_dir(
+        ifile,
+        dest,
+):
+    """
+    Convenience wrapper for shutil.copyfile, used to copy a file to
+    a directory.
+
+    Args
+    ifile : str : Input file in original location
+    dest  : str : Destination folder where ifile will be copied.
+    """
+    ifile = os.path.realpath(ifile)
+    ofile = os.path.join(dest, os.path.basename(ifile))
+    if not os.path.exists(ofile):
+        copyfile(ifile, ofile)
+
+
+def replace_whitespace(
+        string,
+        repl_char="_"
+):
+    """
+    Replaces whitespace in a string with underscores.
+    Useful for removing spaces in filename strings.
+
+    Args
+    string    : str : The input string
+    repl_char : str : Replacement character (default is "_")
+
+    Returns
+    string    : str : String with whitespace replaced
+    """
+    verify_variable_type(string, str)
+    verify_variable_type(repl_char, str)
+
+    return repl_char.join(string.split())
```

### Comparing `geoschem-gcpy-1.4.2/geoschem_gcpy.egg-info/PKG-INFO` & `geoschem_gcpy-1.5.0/geoschem_gcpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoschem-gcpy
-Version: 1.4.2
+Version: 1.5.0
 Home-page: https://github.com/geoschem/gcpy
 Author: GEOS-Chem Support Team
 Author-email: geos-chem-support@g.harvard.edu
 Maintainer: GEOS-Chem Support Team
 Maintainer-email: geos-chem-support@g.harvard.edu
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,21 +25,21 @@
 Requires-Dist: joblib==1.3.2
 Requires-Dist: jupyter==1.0.0
 Requires-Dist: matplotlib==3.8.0
 Requires-Dist: netcdf4==1.6.0
 Requires-Dist: netcdf-fortran==4.5.4
 Requires-Dist: numpy==1.26.0
 Requires-Dist: pandas==2.1.1
-Requires-Dist: pip==23.2.1
+Requires-Dist: pip==23.3
 Requires-Dist: pylint==2.17.5
 Requires-Dist: pyproj==3.6.1
 Requires-Dist: python==3.9.18
-Requires-Dist: pypdf==3.16.1
+Requires-Dist: pypdf==3.17.0
 Requires-Dist: recommonmark==0.7.1
-Requires-Dist: requests==2.31.0
+Requires-Dist: requests==2.32.0
 Requires-Dist: scipy==1.11.2
 Requires-Dist: sparselt==0.1.3
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: tk==8.6.12
 Requires-Dist: xarray==2023.8.0
 Requires-Dist: esmf==8.1.1
 Requires-Dist: esmpy==8.1.1
```

### Comparing `geoschem-gcpy-1.4.2/geoschem_gcpy.egg-info/SOURCES.txt` & `geoschem_gcpy-1.5.0/geoschem_gcpy.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -2,63 +2,58 @@
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE.txt
 MANIFEST.in
 README.md
 SUPPORT.md
 environment.yml
+requirements.txt
 setup.py
 docs/Makefile
 docs/make.bat
 docs/source/About-GCPy.rst
 docs/source/Benchmarking.rst
+docs/source/Compare-Diags.rst
 docs/source/Getting-Started-with-GCPy.rst
 docs/source/Guide-to-Useful-Capabilities.rst
+docs/source/Hemco-Formatting.rst
+docs/source/Known-Bugs.rst
+docs/source/Matplotlib-Backend.rst
+docs/source/ObsPack.rst
 docs/source/Plotting.rst
 docs/source/Regridding.rst
-docs/source/Release_guide.rst
-docs/source/Single_panel.rst
-docs/source/Six_panel.rst
+docs/source/Release-Guide.rst
+docs/source/Single-Panel.rst
+docs/source/Six-Panel.rst
+docs/source/Test-Plot.rst
 docs/source/editing_these_docs.rst
 docs/source/index.rst
-docs/source/plot_timeseries.rst
 docs/source/_static/images/GEOS-Chem_Logo_Light_Background.png
 docs/source/_static/images/budget_table.png
+docs/source/_static/images/create_test_plot.png
 docs/source/_static/images/emissions_totals.png
 docs/source/_static/images/inventory_totals.png
 docs/source/_static/images/mass_table.png
 docs/source/_static/images/single_panel_single_level.png
 docs/source/_static/images/single_panel_zonal_mean.png
 docs/source/_static/images/six_panel_single_level.png
 docs/source/_static/images/six_panel_zonal_mean.png
 gcpy/__init__.py
 gcpy/_version.py
-gcpy/aod_species.yml
 gcpy/append_grid_corners.py
-gcpy/benchmark_categories.yml
-gcpy/benchmark_funcs.py
 gcpy/bpch_to_nc_names.yml
-gcpy/budget_ox.py
-gcpy/budget_tt.py
 gcpy/constants.py
 gcpy/cstools.py
 gcpy/date_time.py
-gcpy/emission_inventories.yml
-gcpy/emission_species.yml
 gcpy/file_regrid.py
 gcpy/grid.py
 gcpy/grid_stretching_transforms.py
-gcpy/lumped_species.yml
-gcpy/mean_oh_from_logs.py
-gcpy/oh_metrics.py
 gcpy/raveller_1D.py
 gcpy/regrid.py
 gcpy/regrid_restart_file.py
-gcpy/species_database.yml
-gcpy/ste_flux.py
 gcpy/units.py
 gcpy/util.py
 gcpy/benchmark/README.md
 gcpy/benchmark/__init__.py
 gcpy/benchmark/benchmark_slurm.sh
 gcpy/benchmark/run_benchmark.py
 gcpy/benchmark/cloud/README.md
@@ -68,37 +63,61 @@
 gcpy/benchmark/config/1yr_ch4_benchmark.yml
 gcpy/benchmark/config/1yr_fullchem_benchmark.yml
 gcpy/benchmark/config/1yr_tt_benchmark.yml
 gcpy/benchmark/config/README.md
 gcpy/benchmark/modules/GC_72_vertical_levels.csv
 gcpy/benchmark/modules/README.md
 gcpy/benchmark/modules/__init__.py
+gcpy/benchmark/modules/aod_species.yml
+gcpy/benchmark/modules/benchmark_categories.yml
+gcpy/benchmark/modules/benchmark_drydep.py
+gcpy/benchmark/modules/benchmark_funcs.py
+gcpy/benchmark/modules/benchmark_mass_cons_table.py
 gcpy/benchmark/modules/benchmark_models_vs_obs.py
+gcpy/benchmark/modules/benchmark_models_vs_sondes.py
+gcpy/benchmark/modules/benchmark_scrape_gcclassic_timers.py
+gcpy/benchmark/modules/benchmark_scrape_gchp_timers.py
+gcpy/benchmark/modules/benchmark_utils.py
+gcpy/benchmark/modules/budget_ox.py
+gcpy/benchmark/modules/budget_tt.py
+gcpy/benchmark/modules/emission_inventories.yml
+gcpy/benchmark/modules/emission_species.yml
+gcpy/benchmark/modules/lumped_species.yml
+gcpy/benchmark/modules/oh_metrics.py
 gcpy/benchmark/modules/run_1yr_fullchem_benchmark.py
 gcpy/benchmark/modules/run_1yr_tt_benchmark.py
-gcpy/examples/README.txt
+gcpy/benchmark/modules/species_database.yml
+gcpy/benchmark/modules/ste_flux.py
+gcpy/community/README.md
+gcpy/community/__init__.py
+gcpy/community/create_obspack_coords_file.py
+gcpy/community/format_hemco_data.py
+gcpy/examples/README.md
 gcpy/examples/__init__.py
 gcpy/examples/bpch_to_nc/__init__.py
 gcpy/examples/bpch_to_nc/bpch2nc.py
 gcpy/examples/bpch_to_nc/bpch_tagco_prodloss_to_nc.py
 gcpy/examples/diagnostics/README.md
 gcpy/examples/diagnostics/__init__.py
 gcpy/examples/diagnostics/compare_diagnostics.ipynb
 gcpy/examples/diagnostics/compare_diags.py
 gcpy/examples/diagnostics/compare_diags.yml
 gcpy/examples/dry_run/__init__.py
 gcpy/examples/dry_run/download_data.py
 gcpy/examples/dry_run/download_data.yml
+gcpy/examples/hemco/.gitignore
+gcpy/examples/hemco/__init__.py
+gcpy/examples/hemco/format_hemco_demo.py
+gcpy/examples/hemco/make_mask_file.py
 gcpy/examples/plotting/__init__.py
 gcpy/examples/plotting/create_test_plot.py
 gcpy/examples/plotting/plot_comparisons.py
 gcpy/examples/plotting/plot_single_panel.py
 gcpy/examples/timeseries/README.txt
 gcpy/examples/timeseries/__init__.py
-gcpy/examples/timeseries/mda8_o3_timeseries.py
 gcpy/examples/timeseries/plot_timeseries.py
 gcpy/examples/working_with_files/__init__.py
 gcpy/examples/working_with_files/add_blank_var_to_restart_file.py
 gcpy/examples/working_with_files/concatenate_files.py
 gcpy/examples/working_with_files/insert_field_into_restart_file.py
 gcpy/examples/working_with_files/regrid_restart_ll_to_cs.py
 gcpy/examples/xarray_examples/__init__.py
```

### Comparing `geoschem-gcpy-1.4.2/geoschem_gcpy.egg-info/requires.txt` & `geoschem_gcpy-1.5.0/geoschem_gcpy.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 joblib==1.3.2
 jupyter==1.0.0
 matplotlib==3.8.0
 netcdf4==1.6.0
 netcdf-fortran==4.5.4
 numpy==1.26.0
 pandas==2.1.1
-pip==23.2.1
+pip==23.3
 pylint==2.17.5
 pyproj==3.6.1
 python==3.9.18
-pypdf==3.16.1
+pypdf==3.17.0
 recommonmark==0.7.1
-requests==2.31.0
+requests==2.32.0
 scipy==1.11.2
 sparselt==0.1.3
 tabulate==0.9.0
 tk==8.6.12
 xarray==2023.8.0
 esmf==8.1.1
 esmpy==8.1.1
```

### Comparing `geoschem-gcpy-1.4.2/setup.py` & `geoschem_gcpy-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     'Intended Audience :: Science/Research',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3.9',
     'Topic :: Scientific/Engineering',
 ]
 
 MAJOR = 1
-MINOR = 4
-MICRO = 2
+MINOR = 5
+MICRO = 0
 EXTRA = '' # for alpha (aN), beta (bN), rc (rcN) versions
 
 VERSION = f"{MAJOR}.{MINOR}.{MICRO}{EXTRA}"
 '''
 #DEV format (using git hash) is intriguing but incompatible with PEP 440
 #No hashes can be used in version field
 DEV = True
@@ -99,21 +99,21 @@
         "joblib==1.3.2",
         "jupyter==1.0.0",
         "matplotlib==3.8.0",
         "netcdf4==1.6.0",
         "netcdf-fortran==4.5.4",
         "numpy==1.26.0",
         "pandas==2.1.1",
-        "pip==23.2.1",
+        "pip==23.3",
         "pylint==2.17.5",
         "pyproj==3.6.1",
         "python==3.9.18",
-        "pypdf==3.16.1",
+        "pypdf==3.17.0",
         "recommonmark==0.7.1",
-        "requests==2.31.0",
+        "requests==2.32.0",
         "scipy==1.11.2",
         "sparselt==0.1.3",
         "tabulate==0.9.0",
         "tk==8.6.12",
         "xarray==2023.8.0",
         "esmf==8.1.1",
         "esmpy==8.1.1",
```

