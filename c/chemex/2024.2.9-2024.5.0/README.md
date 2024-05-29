# Comparing `tmp/chemex-2024.2.9.tar.gz` & `tmp/chemex-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemex-2024.2.9.tar", last modified: Fri Feb  9 16:07:17 2024, max compression
+gzip compressed data, was "chemex-2024.5.0.tar", last modified: Tue May 28 21:51:25 2024, max compression
```

## Comparing `chemex-2024.2.9.tar` & `chemex-2024.5.0.tar`

### file list

```diff
@@ -1,135 +1,135 @@
--rw-r--r--   0        0        0    34916 2024-02-09 16:07:10.428516 chemex-2024.2.9/LICENSE.md
--rw-r--r--   0        0        0     2833 2024-02-09 16:07:10.428516 chemex-2024.2.9/README.md
--rw-r--r--   0        0        0      326 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/__init__.py
--rw-r--r--   0        0        0      185 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/__main__.py
--rw-r--r--   0        0        0     2395 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/chemex.py
--rw-r--r--   0        0        0     5947 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/cli.py
--rw-r--r--   0        0        0        0 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/configuration/__init__.py
--rw-r--r--   0        0        0     1350 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/configuration/base.py
--rw-r--r--   0        0        0     6549 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/configuration/conditions.py
--rw-r--r--   0        0        0     1291 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/configuration/data.py
--rw-r--r--   0        0        0      642 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/configuration/experiment.py
--rw-r--r--   0        0        0     2902 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/configuration/methods.py
--rw-r--r--   0        0        0     1757 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/configuration/parameters.py
--rw-r--r--   0        0        0     1799 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/configuration/utils.py
--rw-r--r--   0        0        0        0 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/containers/__init__.py
--rw-r--r--   0        0        0     5153 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/containers/data.py
--rw-r--r--   0        0        0     2616 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/containers/dataset.py
--rw-r--r--   0        0        0     5670 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/containers/experiment.py
--rw-r--r--   0        0        0     8387 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/containers/experiments.py
--rw-r--r--   0        0        0     5007 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/containers/profile.py
--rw-r--r--   0        0        0        0 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/__init__.py
--rw-r--r--   0        0        0     4477 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/builder.py
--rw-r--r--   0        0        0        0 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/__init__.py
--rw-r--r--   0        0        0     3710 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/cest_13c.py
--rw-r--r--   0        0        0     3621 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/cest_15n.py
--rw-r--r--   0        0        0     4031 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/cest_15n_cw.py
--rw-r--r--   0        0        0     4353 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/cest_15n_tr.py
--rw-r--r--   0        0        0     3708 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/cest_1hn_ap.py
--rw-r--r--   0        0        0     4755 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/cest_1hn_ip_ap.py
--rw-r--r--   0        0        0     4062 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/cest_ch3_1h_ip_ap.py
--rw-r--r--   0        0        0     5203 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/coscest_13c.py
--rw-r--r--   0        0        0     5485 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/coscest_1hn_ip_ap.py
--rw-r--r--   0        0        0     4729 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/cpmg_13c_ip.py
--rw-r--r--   0        0        0     5123 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/cpmg_13co_ap.py
--rw-r--r--   0        0        0     4813 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/cpmg_15n_ip.py
--rw-r--r--   0        0        0     5683 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/cpmg_15n_ip_0013.py
--rw-r--r--   0        0        0     5385 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/cpmg_15n_tr.py
--rw-r--r--   0        0        0     7510 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/cpmg_15n_tr_0013.py
--rw-r--r--   0        0        0     5143 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/cpmg_1hn_ap.py
--rw-r--r--   0        0        0     7690 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/cpmg_1hn_ap_0013.py
--rw-r--r--   0        0        0     4967 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/cpmg_ch3_13c_h2c.py
--rw-r--r--   0        0        0     5822 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/cpmg_ch3_1h_dq.py
--rw-r--r--   0        0        0     6654 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/cpmg_ch3_1h_sq.py
--rw-r--r--   0        0        0     5824 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/cpmg_ch3_1h_tq.py
--rw-r--r--   0        0        0     7360 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/cpmg_ch3_1h_tq_diff.py
--rw-r--r--   0        0        0     4239 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/cpmg_ch3_mq.py
--rw-r--r--   0        0        0     4858 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/cpmg_chd2_1h_ap.py
--rw-r--r--   0        0        0     5383 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/cpmg_hn_dq_zq.py
--rw-r--r--   0        0        0     4389 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/dcest_13c.py
--rw-r--r--   0        0        0     4661 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/dcest_15n.py
--rw-r--r--   0        0        0     3064 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/noesyfpgpph19.py
--rw-r--r--   0        0        0     3281 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/relaxation_hznz.py
--rw-r--r--   0        0        0     2953 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/relaxation_nz.py
--rw-r--r--   0        0        0     2893 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/shift_15n_sq.py
--rw-r--r--   0        0        0     3317 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/catalog/shift_15n_sqmq.py
--rw-r--r--   0        0        0     3318 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/factories.py
--rw-r--r--   0        0        0      957 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/experiments/loader.py
--rw-r--r--   0        0        0     2599 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/filterers.py
--rw-r--r--   0        0        0    20310 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/messages.py
--rw-r--r--   0        0        0        0 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/__init__.py
--rw-r--r--   0        0        0     2916 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/constraints.py
--rw-r--r--   0        0        0     1072 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/factory.py
--rw-r--r--   0        0        0        0 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/kinetic/__init__.py
--rw-r--r--   0        0        0      482 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/kinetic/settings_1st.py
--rw-r--r--   0        0        0     1223 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/kinetic/settings_2st.py
--rw-r--r--   0        0        0     3351 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/kinetic/settings_2st_binding.py
--rw-r--r--   0        0        0     2792 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/kinetic/settings_2st_eyring.py
--rw-r--r--   0        0        0     1891 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/kinetic/settings_2st_hd.py
--rw-r--r--   0        0        0     3094 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/kinetic/settings_2st_monomer_dimer.py
--rw-r--r--   0        0        0     3124 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/kinetic/settings_2st_monomer_tetramer.py
--rw-r--r--   0        0        0     3104 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/kinetic/settings_2st_monomer_trimer.py
--rw-r--r--   0        0        0     1224 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/kinetic/settings_2st_rs.py
--rw-r--r--   0        0        0     5751 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/kinetic/settings_3st_binding_2st_partner.py
--rw-r--r--   0        0        0     4408 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/kinetic/settings_3st_binding_cs.py
--rw-r--r--   0        0        0     4256 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/kinetic/settings_3st_binding_if.py
--rw-r--r--   0        0        0     5067 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/kinetic/settings_3st_double_binding.py
--rw-r--r--   0        0        0     4528 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/kinetic/settings_3st_eyring.py
--rw-r--r--   0        0        0     4382 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/kinetic/settings_3st_monomer_dimer_tetramer.py
--rw-r--r--   0        0        0     4851 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/kinetic/settings_3st_monomer_dimer_trimer.py
--rw-r--r--   0        0        0     7001 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/kinetic/settings_4st_binding_2st_partner.py
--rw-r--r--   0        0        0     6471 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/kinetic/settings_4st_binding_3_bound_states.py
--rw-r--r--   0        0        0     3901 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/kinetic/settings_4st_hd.py
--rw-r--r--   0        0        0     4695 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/kinetic/settings_nst.py
--rw-r--r--   0        0        0      933 2024-02-09 16:07:10.428516 chemex-2024.2.9/chemex/models/loader.py
--rw-r--r--   0        0        0     1250 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/models/model.py
--rw-r--r--   0        0        0        0 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/nmr/__init__.py
--rw-r--r--   0        0        0    10954 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/nmr/basis.py
--rw-r--r--   0        0        0     6405 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/nmr/constants.py
--rw-r--r--   0        0        0     9526 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/nmr/liouvillian.py
--rw-r--r--   0        0        0     8914 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/nmr/rates.py
--rw-r--r--   0        0        0    14523 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/nmr/spectrometer.py
--rw-r--r--   0        0        0        0 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/optimize/__init__.py
--rw-r--r--   0        0        0     5179 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/optimize/fitting.py
--rw-r--r--   0        0        0     8757 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/optimize/gridding.py
--rw-r--r--   0        0        0     4299 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/optimize/grouping.py
--rw-r--r--   0        0        0     5332 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/optimize/helper.py
--rw-r--r--   0        0        0     4449 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/optimize/minimizer.py
--rw-r--r--   0        0        0        0 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/parameters/__init__.py
--rw-r--r--   0        0        0    22058 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/parameters/database.py
--rw-r--r--   0        0        0     3335 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/parameters/factory.py
--rw-r--r--   0        0        0     4748 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/parameters/name.py
--rw-r--r--   0        0        0     3959 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/parameters/setting.py
--rw-r--r--   0        0        0       78 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/parameters/spin_system/__init__.py
--rw-r--r--   0        0        0     2304 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/parameters/spin_system/atom.py
--rw-r--r--   0        0        0     1727 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/parameters/spin_system/constants.py
--rw-r--r--   0        0        0     4141 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/parameters/spin_system/group.py
--rw-r--r--   0        0        0     1567 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/parameters/spin_system/nucleus.py
--rw-r--r--   0        0        0     2139 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/parameters/spin_system/spin.py
--rw-r--r--   0        0        0     6517 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/parameters/spin_system/spin_system.py
--rw-r--r--   0        0        0     1058 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/parameters/spin_system/utilities.py
--rw-r--r--   0        0        0    10123 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/parameters/spins.py
--rw-r--r--   0        0        0      977 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/parameters/userfunctions.py
--rw-r--r--   0        0        0        0 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/plotters/__init__.py
--rw-r--r--   0        0        0     8227 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/plotters/cest.py
--rw-r--r--   0        0        0     6909 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/plotters/cpmg.py
--rw-r--r--   0        0        0     4944 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/plotters/exsy.py
--rw-r--r--   0        0        0     2440 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/plotters/plot.py
--rw-r--r--   0        0        0      329 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/plotters/plotter.py
--rw-r--r--   0        0        0     3854 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/plotters/relaxation.py
--rw-r--r--   0        0        0     1680 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/plotters/shift.py
--rw-r--r--   0        0        0        0 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/printers/__init__.py
--rw-r--r--   0        0        0     4199 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/printers/data.py
--rw-r--r--   0        0        0     4518 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/printers/parameters.py
--rw-r--r--   0        0        0     2975 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/printers/plot.py
--rw-r--r--   0        0        0     2795 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/toml.py
--rw-r--r--   0        0        0        0 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/tools/__init__.py
--rw-r--r--   0        0        0       60 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/tools/pick_cest/__init__.py
--rw-r--r--   0        0        0     6546 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/tools/pick_cest/buttons.py
--rw-r--r--   0        0        0     3875 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/tools/pick_cest/cest_picker.py
--rw-r--r--   0        0        0     1496 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/tools/pick_cest/curve.py
--rw-r--r--   0        0        0     1862 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/tools/plot_param.py
--rw-r--r--   0        0        0      144 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/typing.py
--rw-r--r--   0        0        0     3649 2024-02-09 16:07:10.432517 chemex-2024.2.9/chemex/uncertainty.py
--rw-r--r--   0        0        0     1469 2024-02-09 16:07:17.348557 chemex-2024.2.9/pyproject.toml
--rw-r--r--   0        0        0     3753 1970-01-01 00:00:00.000000 chemex-2024.2.9/PKG-INFO
+-rw-r--r--   0        0        0    34916 2024-05-28 21:51:20.687304 chemex-2024.5.0/LICENSE.md
+-rw-r--r--   0        0        0     2833 2024-05-28 21:51:20.687304 chemex-2024.5.0/README.md
+-rw-r--r--   0        0        0      326 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/__init__.py
+-rw-r--r--   0        0        0      185 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/__main__.py
+-rw-r--r--   0        0        0     2395 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/chemex.py
+-rw-r--r--   0        0        0     5947 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/cli.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/configuration/__init__.py
+-rw-r--r--   0        0        0     1350 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/configuration/base.py
+-rw-r--r--   0        0        0     6524 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/configuration/conditions.py
+-rw-r--r--   0        0        0     1291 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/configuration/data.py
+-rw-r--r--   0        0        0      642 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/configuration/experiment.py
+-rw-r--r--   0        0        0     2920 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/configuration/methods.py
+-rw-r--r--   0        0        0     1757 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/configuration/parameters.py
+-rw-r--r--   0        0        0     1799 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/configuration/utils.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/containers/__init__.py
+-rw-r--r--   0        0        0     5097 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/containers/data.py
+-rw-r--r--   0        0        0     2621 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/containers/dataset.py
+-rw-r--r--   0        0        0     5686 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/containers/experiment.py
+-rw-r--r--   0        0        0     8270 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/containers/experiments.py
+-rw-r--r--   0        0        0     4994 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/containers/profile.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/__init__.py
+-rw-r--r--   0        0        0     4511 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/builder.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/__init__.py
+-rw-r--r--   0        0        0     3710 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cest_13c.py
+-rw-r--r--   0        0        0     3621 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cest_15n.py
+-rw-r--r--   0        0        0     4031 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cest_15n_cw.py
+-rw-r--r--   0        0        0     4353 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cest_15n_tr.py
+-rw-r--r--   0        0        0     3708 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cest_1hn_ap.py
+-rw-r--r--   0        0        0     4755 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cest_1hn_ip_ap.py
+-rw-r--r--   0        0        0     4062 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cest_ch3_1h_ip_ap.py
+-rw-r--r--   0        0        0     5203 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/coscest_13c.py
+-rw-r--r--   0        0        0     5485 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/coscest_1hn_ip_ap.py
+-rw-r--r--   0        0        0     4729 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_13c_ip.py
+-rw-r--r--   0        0        0     5123 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_13co_ap.py
+-rw-r--r--   0        0        0     4813 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_15n_ip.py
+-rw-r--r--   0        0        0     5683 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_15n_ip_0013.py
+-rw-r--r--   0        0        0     5385 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_15n_tr.py
+-rw-r--r--   0        0        0     7510 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_15n_tr_0013.py
+-rw-r--r--   0        0        0     5143 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_1hn_ap.py
+-rw-r--r--   0        0        0     7690 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_1hn_ap_0013.py
+-rw-r--r--   0        0        0     4967 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_ch3_13c_h2c.py
+-rw-r--r--   0        0        0     5822 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_ch3_1h_dq.py
+-rw-r--r--   0        0        0     6654 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_ch3_1h_sq.py
+-rw-r--r--   0        0        0     5824 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_ch3_1h_tq.py
+-rw-r--r--   0        0        0     7360 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_ch3_1h_tq_diff.py
+-rw-r--r--   0        0        0     4239 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_ch3_mq.py
+-rw-r--r--   0        0        0     4858 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_chd2_1h_ap.py
+-rw-r--r--   0        0        0     5383 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_hn_dq_zq.py
+-rw-r--r--   0        0        0     4389 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/catalog/dcest_13c.py
+-rw-r--r--   0        0        0     4661 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/catalog/dcest_15n.py
+-rw-r--r--   0        0        0     3064 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/catalog/noesyfpgpph19.py
+-rw-r--r--   0        0        0     3281 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/catalog/relaxation_hznz.py
+-rw-r--r--   0        0        0     2953 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/catalog/relaxation_nz.py
+-rw-r--r--   0        0        0     2892 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/catalog/shift_15n_sq.py
+-rw-r--r--   0        0        0     3313 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/catalog/shift_15n_sqmq.py
+-rw-r--r--   0        0        0     3327 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/factories.py
+-rw-r--r--   0        0        0      957 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/loader.py
+-rw-r--r--   0        0        0     2606 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/filterers.py
+-rw-r--r--   0        0        0    20310 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/messages.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/__init__.py
+-rw-r--r--   0        0        0     2916 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/constraints.py
+-rw-r--r--   0        0        0     1080 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/factory.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/__init__.py
+-rw-r--r--   0        0        0      482 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_1st.py
+-rw-r--r--   0        0        0     1223 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_2st.py
+-rw-r--r--   0        0        0     3351 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_2st_binding.py
+-rw-r--r--   0        0        0     2792 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_2st_eyring.py
+-rw-r--r--   0        0        0     1891 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_2st_hd.py
+-rw-r--r--   0        0        0     3094 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_2st_monomer_dimer.py
+-rw-r--r--   0        0        0     3124 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_2st_monomer_tetramer.py
+-rw-r--r--   0        0        0     3104 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_2st_monomer_trimer.py
+-rw-r--r--   0        0        0     1224 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_2st_rs.py
+-rw-r--r--   0        0        0     5751 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_3st_binding_2st_partner.py
+-rw-r--r--   0        0        0     4255 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_3st_binding_cs.py
+-rw-r--r--   0        0        0     4179 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_3st_binding_if.py
+-rw-r--r--   0        0        0     5067 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_3st_double_binding.py
+-rw-r--r--   0        0        0     4528 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_3st_eyring.py
+-rw-r--r--   0        0        0     4382 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_3st_monomer_dimer_tetramer.py
+-rw-r--r--   0        0        0     4851 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_3st_monomer_dimer_trimer.py
+-rw-r--r--   0        0        0     7001 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_4st_binding_2st_partner.py
+-rw-r--r--   0        0        0     6471 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_4st_binding_3_bound_states.py
+-rw-r--r--   0        0        0     3901 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_4st_hd.py
+-rw-r--r--   0        0        0     4695 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_nst.py
+-rw-r--r--   0        0        0      933 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/loader.py
+-rw-r--r--   0        0        0     1250 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/model.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/nmr/__init__.py
+-rw-r--r--   0        0        0    10954 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/nmr/basis.py
+-rw-r--r--   0        0        0     6405 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/nmr/constants.py
+-rw-r--r--   0        0        0     9646 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/nmr/liouvillian.py
+-rw-r--r--   0        0        0    10512 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/nmr/rates.py
+-rw-r--r--   0        0        0    14637 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/nmr/spectrometer.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/optimize/__init__.py
+-rw-r--r--   0        0        0     5179 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/optimize/fitting.py
+-rw-r--r--   0        0        0     8773 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/optimize/gridding.py
+-rw-r--r--   0        0        0     4299 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/optimize/grouping.py
+-rw-r--r--   0        0        0     5332 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/optimize/helper.py
+-rw-r--r--   0        0        0     4449 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/optimize/minimizer.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/parameters/__init__.py
+-rw-r--r--   0        0        0    22058 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/parameters/database.py
+-rw-r--r--   0        0        0     3335 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/parameters/factory.py
+-rw-r--r--   0        0        0     4737 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/parameters/name.py
+-rw-r--r--   0        0        0     3959 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/parameters/setting.py
+-rw-r--r--   0        0        0       78 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/parameters/spin_system/__init__.py
+-rw-r--r--   0        0        0     2304 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/parameters/spin_system/atom.py
+-rw-r--r--   0        0        0     1727 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/parameters/spin_system/constants.py
+-rw-r--r--   0        0        0     4141 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/parameters/spin_system/group.py
+-rw-r--r--   0        0        0     1567 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/parameters/spin_system/nucleus.py
+-rw-r--r--   0        0        0     2139 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/parameters/spin_system/spin.py
+-rw-r--r--   0        0        0     6488 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/parameters/spin_system/spin_system.py
+-rw-r--r--   0        0        0     1058 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/parameters/spin_system/utilities.py
+-rw-r--r--   0        0        0    10123 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/parameters/spins.py
+-rw-r--r--   0        0        0      977 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/parameters/userfunctions.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/plotters/__init__.py
+-rw-r--r--   0        0        0     8235 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/plotters/cest.py
+-rw-r--r--   0        0        0     6917 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/plotters/cpmg.py
+-rw-r--r--   0        0        0     4952 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/plotters/exsy.py
+-rw-r--r--   0        0        0     2574 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/plotters/plot.py
+-rw-r--r--   0        0        0      329 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/plotters/plotter.py
+-rw-r--r--   0        0        0     3862 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/plotters/relaxation.py
+-rw-r--r--   0        0        0     1688 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/plotters/shift.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/printers/__init__.py
+-rw-r--r--   0        0        0     4220 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/printers/data.py
+-rw-r--r--   0        0        0     4577 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/printers/parameters.py
+-rw-r--r--   0        0        0     2975 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/printers/plot.py
+-rw-r--r--   0        0        0     2794 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/toml.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/tools/__init__.py
+-rw-r--r--   0        0        0       60 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/tools/pick_cest/__init__.py
+-rw-r--r--   0        0        0     6575 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/tools/pick_cest/buttons.py
+-rw-r--r--   0        0        0     3875 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/tools/pick_cest/cest_picker.py
+-rw-r--r--   0        0        0     1496 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/tools/pick_cest/curve.py
+-rw-r--r--   0        0        0     1867 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/tools/plot_param.py
+-rw-r--r--   0        0        0      144 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/typing.py
+-rw-r--r--   0        0        0     3649 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/uncertainty.py
+-rw-r--r--   0        0        0     1447 2024-05-28 21:51:25.931302 chemex-2024.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 chemex-2024.5.0/PKG-INFO
```

### Comparing `chemex-2024.2.9/LICENSE.md` & `chemex-2024.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/README.md` & `chemex-2024.5.0/README.md`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/chemex.py` & `chemex-2024.5.0/chemex/chemex.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/cli.py` & `chemex-2024.5.0/chemex/cli.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/configuration/base.py` & `chemex-2024.5.0/chemex/configuration/base.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/configuration/conditions.py` & `chemex-2024.5.0/chemex/configuration/conditions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from __future__ import annotations
 
 from collections.abc import Hashable
 from functools import total_ordering
-from typing import Annotated, Literal, TypeVar
+from typing import Annotated, Literal, Self, TypeVar
 
 from pydantic import (
     BaseModel,
     BeforeValidator,
     Field,
     NonNegativeFloat,
     ValidationError,
     field_validator,
     model_validator,
 )
-from typing_extensions import Self
 
 from chemex.configuration.utils import key_to_lower, to_lower
 
 T = TypeVar("T")
 LabelType = Annotated[Literal["1h", "2h", "13c", "15n"], BeforeValidator(to_lower)]
 
 
@@ -69,17 +68,17 @@
         """Helper method to create a list of condition keys and values."""
         conditions: list[tuple[str, str]] = []
         if self.temperature is not None:
             conditions.append(("T", f"{self.temperature:.1f}C"))
         if self.h_larmor_frq is not None:
             conditions.append(("B0", f"{self.h_larmor_frq:.1f}MHz"))
         if self.p_total is not None:
-            conditions.append(("[P]", f"{self.p_total:e}M"))
+            conditions.append(("[P]", f"{self.p_total:.3e}M"))
         if self.l_total is not None:
-            conditions.append(("[L]", f"{self.l_total:e}M"))
+            conditions.append(("[L]", f"{self.l_total:.3e}M"))
         if self.d2o is not None:
             conditions.append(("D2O", f"{self.d2o:.4f}"))
 
         return conditions
 
     @property
     def section(self) -> str:
```

### Comparing `chemex-2024.2.9/chemex/configuration/data.py` & `chemex-2024.5.0/chemex/configuration/data.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/configuration/experiment.py` & `chemex-2024.5.0/chemex/configuration/experiment.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/configuration/methods.py` & `chemex-2024.5.0/chemex/configuration/methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,16 @@
         if isinstance(value, list):
             for residue in value:
                 if isinstance(residue, str) and residue.lower() in ("*", "all"):
                     return "*"
             return [SpinSystem.from_name(residue) for residue in value]
         if isinstance(value, str) and value.lower() in ("*", "all"):
             return "*"
-        raise ValueError(f"Invalid residue list: {value}")
+        msg = f"Invalid residue list: {value}"
+        raise ValueError(msg)
 
     @property
     def selection(self) -> Selection:
         return Selection(include=self.include, exclude=self.exclude)
 
 
 Methods = dict[str, Method]
```

### Comparing `chemex-2024.2.9/chemex/configuration/parameters.py` & `chemex-2024.5.0/chemex/configuration/parameters.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/configuration/utils.py` & `chemex-2024.5.0/chemex/configuration/utils.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/containers/data.py` & `chemex-2024.5.0/chemex/containers/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-from __future__ import annotations
-
 from copy import deepcopy
 from dataclasses import dataclass, field
 from functools import cached_property
 from random import choices
-from typing import Any
+from typing import Any, Self
 
 import numpy as np
 from numpy.typing import NDArray
-from typing_extensions import Self
 
 from chemex.typing import ArrayBool, ArrayFloat
 
 rng = np.random.default_rng()
 
 
 @dataclass
@@ -20,15 +17,15 @@
     """Dataset with experimental, calculated data and metadata.
 
     Attributes:
         exp (ArrayFloat): Experimental data array.
         err (ArrayFloat): Error array for experimental data.
         metadata (NDArray[Any]): Metadata for data points.
         calc (ArrayFloat): Calculated data, set after instantiation.
-        calc (ArrayFloat): Unscaled calculated data, set after instantiation.
+        calc_unscaled (ArrayFloat): Unscaled calculated data, set after instantiation.
         mask (ArrayBool): Mask array for data selection, set after instantiation.
         refs (ArrayBool): Array of reference points, set after instantiation.
     """
 
     exp: ArrayFloat
     err: ArrayFloat
     metadata: NDArray[Any] = field(default_factory=lambda: np.array([]))
```

### Comparing `chemex-2024.2.9/chemex/containers/dataset.py` & `chemex-2024.5.0/chemex/containers/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,10 +74,10 @@
 
     shifts = np.loadtxt(
         data_path,
         dtype=[("spin_system", "U15"), ("exp", "f8"), ("err", "f8")],
     )
 
     return [
-        (SpinSystem(spin_system), Data(exp=np.array([exp]), err=np.array([err])))
+        (SpinSystem(name=spin_system), Data(exp=np.array([exp]), err=np.array([err])))
         for spin_system, exp, err in shifts
     ]
```

### Comparing `chemex-2024.2.9/chemex/containers/experiment.py` & `chemex-2024.5.0/chemex/containers/experiment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,57 @@
 from __future__ import annotations
 
 from collections.abc import Iterator
 from dataclasses import dataclass, field
-from itertools import chain
 from pathlib import Path
+from typing import Self
 
 import numpy as np
 from lmfit import Parameters as ParametersLF
-from typing_extensions import Self
 
 from chemex.configuration.methods import Selection
 from chemex.containers.profile import Profile
 from chemex.messages import (
     print_no_duplicate_warning,
     print_not_implemented_noise_method_warning,
 )
 from chemex.parameters import database
 from chemex.parameters.spin_system import Group
 from chemex.plotters.plotter import Plotter
 from chemex.printers.data import Printer
+from chemex.typing import ArrayFloat
 from chemex.uncertainty import estimate_noise_variance
 
 
 @dataclass
 class Experiment:
     filename: Path
     name: str
     profiles: list[Profile]
     filtered_profiles: list[Profile] = field(init=False, default_factory=list)
     printer: Printer
     plotter: Plotter
 
-    def residuals(self, params: ParametersLF) -> list[float]:
-        return list(
-            chain.from_iterable(profile.residuals(params) for profile in self.profiles),
-        )
+    def residuals(self, params: ParametersLF) -> ArrayFloat:
+        return np.concatenate([profile.residuals(params) for profile in self.profiles])
 
-    def plot(self, path: Path):
+    def plot(self, path: Path) -> None:
         self.plotter.plot(path, self.profiles)
 
-    def plot_simulation(self, path: Path):
+    def plot_simulation(self, path: Path) -> None:
         self.plotter.plot_simulation(path, self.profiles)
 
-    def write(self, path: Path):
+    def write(self, path: Path) -> None:
         filename = (path / self.filename.name).with_suffix(".dat")
         with filename.open("w", encoding="utf-8") as file_dat:
             file_dat.write(self.printer.header)
             for profile in sorted(self.profiles):
                 file_dat.write(str(profile))
 
-    def select(self, selection: Selection):
+    def select(self, selection: Selection) -> None:
         include = selection.include
         exclude = selection.exclude
         profiles_all = [*self.profiles, *self.filtered_profiles]
         profiles: list[Profile] = []
         filtered: list[Profile] = []
         for profile in profiles_all:
             included = include is None or profile.spin_system.part_of(include)
@@ -61,22 +59,22 @@
             if included and not excluded:
                 profiles.append(profile)
             else:
                 filtered.append(profile)
         self.profiles = profiles
         self.filtered_profiles = filtered
 
-    def filter(self, params: ParametersLF):
+    def filter(self, params: ParametersLF) -> None:
         for profile in self.profiles:
             profile.filter(params)
 
-    def _any_duplicate(self):
+    def _any_duplicate(self) -> bool:
         return any(profile.any_duplicate() for profile in self.profiles)
 
-    def estimate_noise(self, kind: str, global_error: bool = True) -> None:
+    def estimate_noise(self, kind: str, *, global_error: bool = True) -> None:
         # TODO: Validation should be moved to the configuration file module
         implemented = ("file", "scatter", "duplicates")
         if kind not in implemented:
             print_not_implemented_noise_method_warning(self.filename, kind, implemented)
             kind = "file"
         if kind == "duplicates" and not self._any_duplicate():
             print_no_duplicate_warning(self.filename)
```

### Comparing `chemex-2024.2.9/chemex/containers/experiments.py` & `chemex-2024.5.0/chemex/containers/experiments.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Module for managing and manipulating collections of NMR experiments.
 
 This module contains the Experiments class and functions for generating different
 types of simulated experiment datasets for statistical analysis.
 """
+
 from __future__ import annotations
 
 from collections.abc import Iterator
 from itertools import chain
 from pathlib import Path
 from random import choices
-from typing import Literal
+from typing import Literal, Self
 
 import numpy as np
 from lmfit.parameter import Parameters
-from typing_extensions import Self
 
 from chemex.configuration.methods import Selection
 from chemex.containers.experiment import Experiment
 from chemex.messages import print_selecting_profiles
 from chemex.parameters import database
 from chemex.parameters.spin_system import Group, SpinSystem
 from chemex.typing import ArrayFloat
@@ -63,54 +63,48 @@
 
         Args:
             params (Parameters): Parameters for residual calculation.
 
         Returns:
             ArrayFloat: Residuals as a NumPy array.
         """
-        return np.asarray(
-            list(
-                chain.from_iterable(
-                    experiment.residuals(params) for experiment in self
-                ),
-            ),
-        )
+        return np.concatenate([experiment.residuals(params) for experiment in self])
 
     def back_calculate(self) -> None:
         """Back calculate experiments' parameters from the database."""
         params_lf = database.build_lmfit_params(self.param_ids)
         self.residuals(params_lf)
 
     def prepare_for_simulation(self) -> None:
         """Prepare each experiment in the collection for simulation."""
         self.back_calculate()
         for experiment in self:
             experiment.prepare_for_simulation()
 
-    def write(self, path: Path):
+    def write(self, path: Path) -> None:
         """Write experiment data to a specified path.
 
         Args:
             path (Path): Directory path to write data.
         """
         path_dat = path / "Data"
         path_dat.mkdir(parents=True, exist_ok=True)
         for experiment in self:
             experiment.write(path_dat)
 
-    def plot(self, path: Path):
+    def plot(self, path: Path) -> None:
         """Plot each experiment in the collection.
 
         Args:
             path (Path): Directory path for saving plots.
         """
         for experiment in self:
             experiment.plot(path)
 
-    def plot_simulation(self, path: Path):
+    def plot_simulation(self, path: Path) -> None:
         """Plot simulations for each experiment.
 
         Args:
             path (Path): Directory path for saving simulation plots.
         """
         for experiment in self:
             experiment.plot_simulation(path)
```

### Comparing `chemex-2024.2.9/chemex/containers/profile.py` & `chemex-2024.5.0/chemex/containers/profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from __future__ import annotations
 
 from collections.abc import Hashable
 from copy import deepcopy
 from dataclasses import dataclass, field
 from functools import cached_property
 from operator import attrgetter
-from typing import Protocol
+from typing import Protocol, Self
 
 from cachetools import LRUCache, cachedmethod
 from lmfit import Parameters as ParametersLF
-from typing_extensions import Self
 
 from chemex.containers.data import Data
 from chemex.nmr.spectrometer import Spectrometer
 from chemex.parameters.spin_system import SpinSystem
 from chemex.printers.data import Printer
 from chemex.typing import ArrayBool, ArrayFloat
 
@@ -51,18 +50,18 @@
     is_scaled: bool = field(compare=False, default=True)
     spin_system: SpinSystem = field(compare=True, init=False)
     cache: LRUCache = field(compare=False, init=False)
 
     def _cache_key(self, params: ParametersLF) -> tuple[Hashable, ...]:
         return (
             *(params[param_id].value for param_id in self.param_ids),
-            self.data.metadata.tostring(),
+            self.data.metadata.tobytes(),
         )
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         """Initialize derived attributes."""
         self.spin_system = self.spectrometer.liouvillian.spin_system
         self.data.refs = self.pulse_sequence.is_reference(self.data.metadata)
         self.cache = LRUCache(maxsize=5)
 
     @cached_property
     def param_ids(self) -> set[str]:
@@ -122,20 +121,21 @@
 
     def bootstrap(self) -> Self:
         """Generate a bootstrap variant of the profile."""
         profile = deepcopy(self)
         profile.data = profile.data.bootstrap()
         return profile
 
-    def any_duplicate(self):
+    def any_duplicate(self) -> bool:
         """Check for duplicate data points."""
         return self.data.any_duplicate()
 
     def __add__(self, other: Self) -> Self:
         """Combine two profiles."""
         profile = deepcopy(self)
         profile.data = self.data + other.data
         return profile
 
     def __str__(self) -> str:
         """String representation of the Profile."""
         return self.printer.print(str(self.spin_system), self.data)
+
```

### Comparing `chemex-2024.2.9/chemex/experiments/builder.py` & `chemex-2024.5.0/chemex/experiments/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,20 +130,22 @@
                     config.data.scaled,
                 ),
             )
 
         live.update(get_reading_exp_text(filename, experiment_name, len(profiles)))
 
     experiment = Experiment(filename, experiment_name, profiles, printer, plotter)
-    experiment.estimate_noise(config.data.error, config.data.global_error)
+    experiment.estimate_noise(config.data.error, global_error=config.data.global_error)
 
     return experiment
 
 
-def build_experiments(filenames: list[Path] | None, selection: Selection):
+def build_experiments(
+    filenames: list[Path] | None, selection: Selection
+) -> Experiments:
     if not filenames:
         return Experiments()
 
     print_loading_experiments()
 
     experiments = Experiments()
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/cest_13c.py` & `chemex-2024.5.0/chemex/experiments/catalog/cest_13c.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,8 +115,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=Cest13CSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=CestFilterer,
         printer_creator=CestPrinter,
         plotter_creator=CestPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/cest_15n.py` & `chemex-2024.5.0/chemex/experiments/catalog/cest_15n.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,8 +114,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=Cest15NSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=CestFilterer,
         printer_creator=CestPrinter,
         plotter_creator=CestPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/cest_15n_cw.py` & `chemex-2024.5.0/chemex/experiments/catalog/cest_15n_cw.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,8 +129,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=Cest15NCwSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=CestFilterer,
         printer_creator=CestPrinter,
         plotter_creator=CestPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/cest_15n_tr.py` & `chemex-2024.5.0/chemex/experiments/catalog/cest_15n_tr.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,8 +136,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=Cest15NTrSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=CestFilterer,
         printer_creator=CestPrinter,
         plotter_creator=CestPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/cest_1hn_ap.py` & `chemex-2024.5.0/chemex/experiments/catalog/cest_1hn_ap.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,8 +117,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=Cest1HnApSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=CestFilterer,
         printer_creator=CestPrinter,
         plotter_creator=CestPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/cest_1hn_ip_ap.py` & `chemex-2024.5.0/chemex/experiments/catalog/cest_1hn_ip_ap.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,8 +139,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=Cest1HnIpApSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=CestFilterer,
         printer_creator=CestPrinter,
         plotter_creator=CestPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/cest_ch3_1h_ip_ap.py` & `chemex-2024.5.0/chemex/experiments/catalog/cest_ch3_1h_ip_ap.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,8 +123,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=CestCh31HIpApSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=CestFilterer,
         printer_creator=CestPrinter,
         plotter_creator=CestPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/coscest_13c.py` & `chemex-2024.5.0/chemex/experiments/catalog/coscest_13c.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,8 +162,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=CosCest13CSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=CestFilterer,
         printer_creator=CestPrinter,
         plotter_creator=CestPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/coscest_1hn_ip_ap.py` & `chemex-2024.5.0/chemex/experiments/catalog/coscest_1hn_ip_ap.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,8 +166,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=CosCest1HnIpApSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=CestFilterer,
         printer_creator=CestPrinter,
         plotter_creator=CestPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/cpmg_13c_ip.py` & `chemex-2024.5.0/chemex/experiments/catalog/cpmg_13c_ip.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,8 +132,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=Cpmg13CIpSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=PlanesFilterer,
         printer_creator=CpmgPrinter,
         plotter_creator=CpmgPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/cpmg_13co_ap.py` & `chemex-2024.5.0/chemex/experiments/catalog/cpmg_13co_ap.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 def build_spectrometer(
     config: Cpmg13CoApConfig,
     spin_system: SpinSystem,
 ) -> Spectrometer:
     settings = config.experiment
     conditions = config.conditions
 
-    basis = Basis(type="ixyzsz", spin_system="hn")
+    basis = Basis(type="ixyzsz", spin_system="cn")
     liouvillian = LiouvillianIS(spin_system, basis, conditions)
     spectrometer = Spectrometer(liouvillian)
 
     spectrometer.carrier_i = settings.carrier
     spectrometer.b1_i = 1 / (4.0 * settings.pw90)
     spectrometer.detection = settings.detection
 
@@ -152,8 +152,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=Cpmg13CoApSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=PlanesFilterer,
         printer_creator=CpmgPrinter,
         plotter_creator=CpmgPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/cpmg_15n_ip.py` & `chemex-2024.5.0/chemex/experiments/catalog/cpmg_15n_ip.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,8 +136,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=Cpmg15NIpSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=PlanesFilterer,
         printer_creator=CpmgPrinter,
         plotter_creator=CpmgPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/cpmg_15n_ip_0013.py` & `chemex-2024.5.0/chemex/experiments/catalog/cpmg_15n_ip_0013.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,8 +169,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=Cpmg15N0013IpSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=PlanesFilterer,
         printer_creator=CpmgPrinter,
         plotter_creator=CpmgPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/cpmg_15n_tr.py` & `chemex-2024.5.0/chemex/experiments/catalog/cpmg_15n_tr.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,8 +156,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=Cpmg15NTrSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=PlanesFilterer,
         printer_creator=CpmgPrinter,
         plotter_creator=CpmgPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/cpmg_15n_tr_0013.py` & `chemex-2024.5.0/chemex/experiments/catalog/cpmg_15n_tr_0013.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,8 +219,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=Cpmg15NTr0013Sequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=PlanesFilterer,
         printer_creator=CpmgPrinter,
         plotter_creator=CpmgPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/cpmg_1hn_ap.py` & `chemex-2024.5.0/chemex/experiments/catalog/cpmg_1hn_ap.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,8 +147,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=Cpmg1HnApSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=PlanesFilterer,
         printer_creator=CpmgPrinter,
         plotter_creator=CpmgPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/cpmg_1hn_ap_0013.py` & `chemex-2024.5.0/chemex/experiments/catalog/cpmg_1hn_ap_0013.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,8 +219,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=Cpmg1HnAp0013Sequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=PlanesFilterer,
         printer_creator=CpmgPrinter,
         plotter_creator=CpmgPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/cpmg_ch3_13c_h2c.py` & `chemex-2024.5.0/chemex/experiments/catalog/cpmg_ch3_13c_h2c.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,8 +145,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=CpmgCh313CH2cSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=PlanesFilterer,
         printer_creator=CpmgPrinter,
         plotter_creator=CpmgPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/cpmg_ch3_1h_dq.py` & `chemex-2024.5.0/chemex/experiments/catalog/cpmg_ch3_1h_dq.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,8 +158,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=CpmgCh31HDqSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=PlanesFilterer,
         printer_creator=CpmgPrinter,
         plotter_creator=CpmgPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/cpmg_ch3_1h_sq.py` & `chemex-2024.5.0/chemex/experiments/catalog/cpmg_ch3_1h_sq.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,8 +179,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=CpmgCh31HSqSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=PlanesFilterer,
         printer_creator=CpmgPrinter,
         plotter_creator=CpmgPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/cpmg_ch3_1h_tq.py` & `chemex-2024.5.0/chemex/experiments/catalog/cpmg_ch3_1h_tq.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,8 +158,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=CpmgCh31HTqSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=PlanesFilterer,
         printer_creator=CpmgPrinter,
         plotter_creator=CpmgPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/cpmg_ch3_1h_tq_diff.py` & `chemex-2024.5.0/chemex/experiments/catalog/cpmg_ch3_1h_tq_diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,8 +192,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=CpmgCh31HTqDiffSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=PlanesFilterer,
         printer_creator=CpmgPrinter,
         plotter_creator=CpmgPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/cpmg_ch3_mq.py` & `chemex-2024.5.0/chemex/experiments/catalog/cpmg_ch3_mq.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,8 +116,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=CpmgCh3MqSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=PlanesFilterer,
         printer_creator=CpmgPrinter,
         plotter_creator=CpmgPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/cpmg_chd2_1h_ap.py` & `chemex-2024.5.0/chemex/experiments/catalog/cpmg_chd2_1h_ap.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,8 +134,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=CpmgChd21HApSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=PlanesFilterer,
         printer_creator=CpmgPrinter,
         plotter_creator=CpmgPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/cpmg_hn_dq_zq.py` & `chemex-2024.5.0/chemex/experiments/catalog/cpmg_hn_dq_zq.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,8 +152,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=CpmgHNDqZqSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=PlanesFilterer,
         printer_creator=CpmgPrinter,
         plotter_creator=CpmgPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/dcest_13c.py` & `chemex-2024.5.0/chemex/experiments/catalog/dcest_13c.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,8 +138,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=DCest13CSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=CestFilterer,
         printer_creator=CestPrinter,
         plotter_creator=CestPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/dcest_15n.py` & `chemex-2024.5.0/chemex/experiments/catalog/dcest_15n.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,8 +146,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=DCest15NSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=CestFilterer,
         printer_creator=CestPrinter,
         plotter_creator=CestPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/noesyfpgpph19.py` & `chemex-2024.5.0/chemex/experiments/catalog/noesyfpgpph19.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,8 +90,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=Noesyfpgpph19Sequence,
         dataset_creator=load_exsy_dataset,
         filterer_creator=PlanesFilterer,
         printer_creator=EXSYPrinter,
         plotter_creator=EXSYPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/relaxation_hznz.py` & `chemex-2024.5.0/chemex/experiments/catalog/relaxation_hznz.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,8 +97,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=RelaxationHzNzSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=PlanesFilterer,
         printer_creator=RelaxationPrinter,
         plotter_creator=RelaxationPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/relaxation_nz.py` & `chemex-2024.5.0/chemex/experiments/catalog/relaxation_nz.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,8 +88,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=RelaxationNzSequence,
         dataset_creator=load_relaxation_dataset,
         filterer_creator=PlanesFilterer,
         printer_creator=RelaxationPrinter,
         plotter_creator=RelaxationPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/shift_15n_sq.py` & `chemex-2024.5.0/chemex/experiments/catalog/shift_15n_sq.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     return array[idx]
 
 
 @dataclass
 class Shift15NSqSequence:
     settings: Shift15NSqSettings
 
-    def calculate(self, spectrometer: Spectrometer, _data: Data) -> ArrayFloat:
+    def calculate(self, spectrometer: Spectrometer, data: Data) -> ArrayFloat:
         ppm_i = spectrometer.liouvillian.ppm_i
         ref_shift_i = spectrometer.par_values[self.settings.cs_i_name] * ppm_i
         shifts = spectrometer.calculate_shifts()
         shift_sq = _find_nearest(shifts, ref_shift_i)
         return np.array([shift_sq / ppm_i])
 
     def is_reference(self, metadata: ArrayFloat) -> ArrayBool:
@@ -84,8 +84,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=Shift15NSqSequence,
         dataset_creator=load_shift_dataset,
         filterer_creator=NoFilterer,
         printer_creator=ShiftPrinter,
         plotter_creator=ShiftPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/catalog/shift_15n_sqmq.py` & `chemex-2024.5.0/chemex/experiments/catalog/shift_15n_sqmq.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,16 +38,15 @@
 
 class Shift15NSqMqConfig(
     ExperimentConfiguration[
         Shift15NSqMqSettings,
         ConditionsWithValidations,
         ShiftDataSettings,
     ],
-):
-    ...
+): ...
 
 
 def build_spectrometer(
     config: Shift15NSqMqConfig,
     spin_system: SpinSystem,
 ) -> Spectrometer:
     conditions = config.conditions
@@ -100,8 +99,8 @@
         spectrometer_creator=build_spectrometer,
         sequence_creator=Shift15NSqMqSequence,
         dataset_creator=load_shift_dataset,
         filterer_creator=NoFilterer,
         printer_creator=ShiftPrinter,
         plotter_creator=ShiftPlotter,
     )
-    factories.register(type=EXPERIMENT_NAME, creators=creators)
+    factories.register(name=EXPERIMENT_NAME, creators=creators)
```

### Comparing `chemex-2024.2.9/chemex/experiments/factories.py` & `chemex-2024.5.0/chemex/experiments/factories.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Factories for creating different parts of an experiment."""
+
 from __future__ import annotations
 
 from collections.abc import Callable, MutableMapping
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, ClassVar
 
@@ -76,20 +77,20 @@
 
 
 class Factories:
     """Factory for creating all parts of an experiment."""
 
     creators_registry: ClassVar[dict[str, Creators]] = {}
 
-    def register(self, type: str, creators: Creators):
+    def register(self, name: str, creators: Creators) -> None:
         """Register a new propagtor type."""
-        self.creators_registry[type] = creators
+        self.creators_registry[name] = creators
 
-    def get(self, type: str) -> Creators:
+    def get(self, name: str) -> Creators:
         try:
-            return self.creators_registry[type]
+            return self.creators_registry[name]
         except KeyError:
-            msg = f"Unknown  type {type!r}"
+            msg = f"Unknown  type {name!r}"
             raise ValueError(msg) from None
 
 
 factories = Factories()
```

### Comparing `chemex-2024.2.9/chemex/experiments/loader.py` & `chemex-2024.5.0/chemex/experiments/loader.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/filterers.py` & `chemex-2024.5.0/chemex/filterers.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class NoFilterer:
     """Filterer that does no filtering."""
 
     def __init__(self, **_extra: Any) -> None:
         return
 
-    def filter(self, _data: Data) -> None:
+    def filter(self, data: Data) -> None:
         return
 
 
 class PlanesDataSettings(Protocol):
     filter_planes: list[int]
 
 
@@ -83,14 +83,14 @@
 
 
 class CestFilterer(Generic[T]):
     def __init__(self, config: T, spectrometer: Spectrometer, **_extra: Any) -> None:
         self.config = config
         self.spectrometer = spectrometer
 
-    def filter(self, data: Data):
+    def filter(self, data: Data) -> None:
         _filter_planes(data, self.config.data.filter_planes)
 
         if self.config.data.filter_ref_planes:
             _filter_ref_planes(data)
 
         _filter_offsets(data, self.config, self.spectrometer)
```

### Comparing `chemex-2024.2.9/chemex/messages.py` & `chemex-2024.5.0/chemex/messages.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/models/constraints.py` & `chemex-2024.5.0/chemex/models/constraints.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/models/factory.py` & `chemex-2024.5.0/chemex/models/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 class Factory:
     """Factory for creating all parts of an experiment."""
 
     setting_makers_registry: ClassVar[dict[str, SettingMakerType]] = {}
 
-    def register(self, name: str, setting_maker: SettingMakerType):
+    def register(self, name: str, setting_maker: SettingMakerType) -> None:
         """Register a new setting maker."""
         self.setting_makers_registry[name] = setting_maker
 
     def create(self, name: str, conditions: Conditions) -> SettingsType:
         try:
             return self.setting_makers_registry[name](conditions)
         except KeyError:
```

### Comparing `chemex-2024.2.9/chemex/models/kinetic/settings_2st.py` & `chemex-2024.5.0/chemex/models/kinetic/settings_2st.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/models/kinetic/settings_2st_binding.py` & `chemex-2024.5.0/chemex/models/kinetic/settings_2st_binding.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/models/kinetic/settings_2st_eyring.py` & `chemex-2024.5.0/chemex/models/kinetic/settings_2st_eyring.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/models/kinetic/settings_2st_hd.py` & `chemex-2024.5.0/chemex/models/kinetic/settings_2st_hd.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/models/kinetic/settings_2st_monomer_dimer.py` & `chemex-2024.5.0/chemex/models/kinetic/settings_2st_monomer_dimer.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/models/kinetic/settings_2st_monomer_tetramer.py` & `chemex-2024.5.0/chemex/models/kinetic/settings_2st_monomer_tetramer.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/models/kinetic/settings_2st_monomer_trimer.py` & `chemex-2024.5.0/chemex/models/kinetic/settings_2st_monomer_trimer.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/models/kinetic/settings_2st_rs.py` & `chemex-2024.5.0/chemex/models/kinetic/settings_2st_rs.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/models/kinetic/settings_3st_binding_2st_partner.py` & `chemex-2024.5.0/chemex/models/kinetic/settings_3st_binding_2st_partner.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/models/kinetic/settings_3st_binding_cs.py` & `chemex-2024.5.0/chemex/models/kinetic/settings_3st_binding_cs.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,108 +19,105 @@
 
 def calculate_residuals(
     concentrations: ArrayFloat,
     p_total: float,
     l_total: float,
     kab: float,
     kba: float,
-    kd: float,
+    kd_bc: float,
 ) -> ArrayFloat:
     p1, p2, pl, l_ = concentrations
     return np.array(
         [
             p_total - p1 - p2 - pl,
             l_total - l_ - pl,
             kab * p1 - kba * p2,
-            kd * pl - p2 * l_,
+            kd_bc * pl - p2 * l_,
         ],
     )
 
 
 @lru_cache(maxsize=100)
 def calculate_concentrations(
     p_total: float,
     l_total: float,
-    kd: float,
     kab: float,
     kba: float,
+    kd_bc: float,
 ) -> dict[str, float]:
-    concentrations_start = (p_total, 0.0, 0.0, l_total)
+    p1 = p2 = 0.5 * (p_total - 0.5 * l_total)
+    pl = l_ = 0.5 * l_total
+    concentrations_start = (p1, p2, pl, l_)
     results = root(
         calculate_residuals,
         concentrations_start,
-        args=(p_total, l_total, kab, kba, kd),
+        args=(p_total, l_total, kab, kba, kd_bc),
     )
     p1, p2, pl, l_ = results["x"]
     return {"p1": p1, "p2": p2, "pl": pl, "l": l_}
 
 
 def make_settings_3st_binding_cs(
     conditions: Conditions,
 ) -> dict[str, ParamLocalSetting]:
-    p0 = conditions.p_total
-    l0 = conditions.l_total
-    if p0 is None:
+    p_total = conditions.p_total
+    l_total = conditions.l_total
+    if p_total is None:
         msg = f"'p_total' must be specified to use the '{NAME}' model"
         raise ValueError(msg)
-    if l0 is None:
+    if l_total is None:
         msg = f"'l_total' must be specified to use the '{NAME}' model"
         raise ValueError(msg)
+    concentrations_string = (
+        f"concentrations({p_total}, {l_total}, {{kab}}, {{kba}}, {{kd_bc}})"
+    )
     return {
         "kab": ParamLocalSetting(
             name_setting=NameSetting("kab", "", ("temperature",)),
             value=100.0,
             min=0.0,
             vary=True,
         ),
         "kba": ParamLocalSetting(
             name_setting=NameSetting("kba", "", ("temperature",)),
             value=100.0,
             min=0.0,
             vary=True,
         ),
-        "koff": ParamLocalSetting(
-            name_setting=NameSetting("koff", "", ("temperature",)),
+        "koff_bc": ParamLocalSetting(
+            name_setting=NameSetting("koff_bc", "", ("temperature",)),
             value=100.0,
             min=0.0,
             vary=True,
         ),
-        "kd": ParamLocalSetting(
-            name_setting=NameSetting("kd", "", ("temperature",)),
-            value=1e-3,
+        "kd_app": ParamLocalSetting(
+            name_setting=NameSetting("kd_app", "", ("temperature",)),
+            value=1e-6,
             min=0.0,
             vary=True,
         ),
-        "kon": ParamLocalSetting(
-            name_setting=NameSetting("kon", "", ("temperature",)),
-            expr="{koff} / max({kd}, 1e-100)",
+        "kd_bc": ParamLocalSetting(
+            name_setting=NameSetting("kd_bc", "", ("temperature",)),
+            expr="{kd_app} * {kab} / max({kab} + {kba}, 1e-16)",
+        ),
+        "kon_bc": ParamLocalSetting(
+            name_setting=NameSetting("kon_bc", "", ("temperature",)),
+            expr="{koff_bc} / max({kd_bc}, 1e-16)",
         ),
         "c_l": ParamLocalSetting(
             name_setting=NameSetting("c_l", "", TPL),
-            expr=f"concentrations({p0}, {l0}, {{kab}}, {{kba}}, {{kd}})['l']",
-        ),
-        "c_p1": ParamLocalSetting(
-            name_setting=NameSetting("c_p1", "", TPL),
-            expr=f"concentrations({p0}, {l0}, {{kab}}, {{kba}}, {{kd}})['p1']",
-        ),
-        "c_p2": ParamLocalSetting(
-            name_setting=NameSetting("c_p2", "", TPL),
-            expr=f"concentrations({p0}, {l0}, {{kab}}, {{kba}}, {{kd}})['p2']",
-        ),
-        "c_pl": ParamLocalSetting(
-            name_setting=NameSetting("c_pl", "", TPL),
-            expr=f"concentrations({p0}, {l0}, {{kab}}, {{kba}}, {{kd}})['pl']",
+            expr=f"{concentrations_string}['l']",
         ),
         "kbc": ParamLocalSetting(
             name_setting=NameSetting("kbc", "", TPL),
-            expr="{kon} * {c_l}",
+            expr="{kon_bc} * {c_l}",
         ),
         "kcb": ParamLocalSetting(
             name_setting=NameSetting("kcb", "", TPL),
-            expr="{koff}",
+            expr="{koff_bc}",
         ),
         "pa": ParamLocalSetting(
             name_setting=NameSetting("pa", "", TPL),
             expr="pop_3st({kab}, {kba}, 0.0, 0.0, {kbc}, {kcb})['pa']",
         ),
         "pb": ParamLocalSetting(
             name_setting=NameSetting("pb", "", TPL),
```

### Comparing `chemex-2024.2.9/chemex/models/kinetic/settings_3st_binding_if.py` & `chemex-2024.5.0/chemex/models/kinetic/settings_3st_binding_if.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,40 +21,43 @@
     populations: ArrayFloat,
     p_total: float,
     l_total: float,
     kd_ab: float,
     kbc: float,
     kcb: float,
 ) -> ArrayFloat:
-    pfree, pl1, pl2 = populations
-    lfree = l_total - p_total + pfree
+    p_, pl1, pl2, l_ = populations
     return np.array(
         [
-            pfree + pl1 + pl2 - p_total,
-            lfree * pfree - kd_ab * pl1,
+            p_ + pl1 + pl2 - p_total,
+            l_ + pl1 + pl2 - l_total,
+            l_ * p_ - kd_ab * pl1,
             kbc * pl1 - kcb * pl2,
         ],
     )
 
 
 @lru_cache(maxsize=100)
 def calculate_concentrations(
     p_total: float,
     l_total: float,
     kd_ab: float,
     kbc: float,
     kcb: float,
 ) -> dict[str, float]:
-    concentrations_start = (p_total, 0.0, 0.0)
+    p_ = p_total - 0.5 * l_total
+    pl1 = pl2 = 0.5 * (p_total - p_)
+    l_ = 0.5 * l_total
+    concentrations_start = (p_, pl1, pl2, l_)
     results = root(
         calculate_residuals,
         concentrations_start,
         args=(p_total, l_total, kd_ab, kbc, kcb),
     )
-    return dict(zip(("pfree", "pl1", "pl2"), results["x"], strict=True))
+    return dict(zip(("p", "pl1", "pl2", "l"), results["x"], strict=True))
 
 
 def make_settings_3st_induced_fit(
     conditions: Conditions,
 ) -> dict[str, ParamLocalSetting]:
     p_total = conditions.p_total
     l_total = conditions.l_total
@@ -89,29 +92,25 @@
             min=0.0,
             vary=True,
         ),
         "kd_ab": ParamLocalSetting(
             name_setting=NameSetting("kd_ab", "", ("temperature",)),
             expr="{kd_app} * (1 + {kbc} / {kcb})",
         ),
-        "kon": ParamLocalSetting(
-            name_setting=NameSetting("kon", "", ("temperature",)),
+        "kon_ab": ParamLocalSetting(
+            name_setting=NameSetting("kon_ab", "", ("temperature",)),
             expr="{koff_ab} / max({kd_ab}, 1e-100)",
         ),
-        "pfree": ParamLocalSetting(
-            name_setting=NameSetting("pfree", "", TPL),
-            expr=(f"calc_conc({p_total},{l_total},{{kd_ab}},{{kbc}},{{kcb}})['pfree']"),
-        ),
-        "l_free": ParamLocalSetting(
-            name_setting=NameSetting("l_free", "", TPL),
-            expr=f"{l_total} - {p_total} + {{pfree}}",
+        "c_l": ParamLocalSetting(
+            name_setting=NameSetting("c_l", "", TPL),
+            expr=(f"calc_conc({p_total},{l_total},{{kd_ab}},{{kbc}},{{kcb}})['l']"),
         ),
         "kab": ParamLocalSetting(
             name_setting=NameSetting("kab", "", TPL),
-            expr="{kon} * {l_free}",
+            expr="{kon_ab} * {c_l}",
         ),
         "kba": ParamLocalSetting(
             name_setting=NameSetting("kba", "", TPL),
             expr="{koff_ab}",
         ),
         "pa": ParamLocalSetting(
             name_setting=NameSetting("pa", "", TPL),
```

### Comparing `chemex-2024.2.9/chemex/models/kinetic/settings_3st_double_binding.py` & `chemex-2024.5.0/chemex/models/kinetic/settings_3st_double_binding.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/models/kinetic/settings_3st_eyring.py` & `chemex-2024.5.0/chemex/models/kinetic/settings_3st_eyring.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/models/kinetic/settings_3st_monomer_dimer_tetramer.py` & `chemex-2024.5.0/chemex/models/kinetic/settings_3st_monomer_dimer_tetramer.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/models/kinetic/settings_3st_monomer_dimer_trimer.py` & `chemex-2024.5.0/chemex/models/kinetic/settings_3st_monomer_dimer_trimer.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/models/kinetic/settings_4st_binding_2st_partner.py` & `chemex-2024.5.0/chemex/models/kinetic/settings_4st_binding_2st_partner.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/models/kinetic/settings_4st_binding_3_bound_states.py` & `chemex-2024.5.0/chemex/models/kinetic/settings_4st_binding_3_bound_states.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/models/kinetic/settings_4st_hd.py` & `chemex-2024.5.0/chemex/models/kinetic/settings_4st_hd.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/models/kinetic/settings_nst.py` & `chemex-2024.5.0/chemex/models/kinetic/settings_nst.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/models/loader.py` & `chemex-2024.5.0/chemex/models/loader.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/models/model.py` & `chemex-2024.5.0/chemex/models/model.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/nmr/basis.py` & `chemex-2024.5.0/chemex/nmr/basis.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/nmr/constants.py` & `chemex-2024.5.0/chemex/nmr/constants.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/nmr/liouvillian.py` & `chemex-2024.5.0/chemex/nmr/liouvillian.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 { Eq,
 Ix, Iy, Iz, Sx, Sy, Sz,
 2IxSz, 2IySz, 2IzSx, 2IzSy,
 2IxSx, 2IxSy, 2IySx, 2IySy,
 2IzSz }
 
 """
+
 from __future__ import annotations
 
 import re
 from collections.abc import Iterable
 from itertools import product
 
 import numpy as np
@@ -43,15 +44,15 @@
         dist = np.array([1.0])
     weights = stats.norm.pdf(grid)
     weights /= weights.sum()
     return dist * value, weights
 
 
 class LiouvillianIS:
-    def _scale_matrix(self, name: str, value: float):
+    def _scale_matrix(self, name: str, value: float) -> None:
         state_names = {name.format(state=state) for state in model.states}
         for state_name in state_names & set(self.matrices):
             self.matrices[state_name] = np.sign(self._matrices_ref[state_name]) * value
 
     def __init__(
         self,
         spin_system: SpinSystem,
@@ -99,93 +100,93 @@
         self._build_base_liouvillian()
 
     @property
     def ppm_i(self) -> float:
         return self._ppm_i
 
     @ppm_i.setter
-    def ppm_i(self, value: float):
+    def ppm_i(self, value: float) -> None:
         self._ppm_i = value
         self._scale_matrix("cs_i_{state}", self._q_order_i * value)
         self._scale_matrix("carrier_i", self._q_order_i * value)
 
     @property
     def ppm_s(self) -> float:
         return self._ppm_s
 
     @ppm_s.setter
-    def ppm_s(self, value: float):
+    def ppm_s(self, value: float) -> None:
         self._ppm_s = value
         self._scale_matrix("cs_s_{state}", value)
         self._scale_matrix("carrier_s", value)
 
     @property
     def carrier_i(self) -> float:
         return float(self._carrier_i)
 
     @carrier_i.setter
-    def carrier_i(self, value: float):
+    def carrier_i(self, value: float) -> None:
         self._carrier_i = np.array(value)
         self._l_carrier_i = self.matrices.get("carrier_i", np.array(0.0)) * value
 
     @property
     def carrier_s(self) -> float:
         return float(self._carrier_s)
 
     @carrier_s.setter
-    def carrier_s(self, value: float):
+    def carrier_s(self, value: float) -> None:
         self._carrier_s = np.array(value)
         self._l_carrier_s = self.matrices.get("carrier_s", np.array(0.0)) * value
 
     @property
     def offset_i(self) -> float:
         return float(self._offset_i)
 
     @offset_i.setter
-    def offset_i(self, value: float):
+    def offset_i(self, value: float) -> None:
         self._offset_i = np.array(value)
         self._l_offset_i = (
             self.matrices.get("offset_i", np.array(0.0)) * value * np.sign(self.ppm_i)
         )
 
     @property
     def offset_s(self) -> float:
         return float(self._offset_s)
 
     @offset_s.setter
-    def offset_s(self, value: float):
+    def offset_s(self, value: float) -> None:
         self._offset_s = np.array(value)
         self._l_offset_s = (
             self.matrices.get("offset_s", 0.0) * value * np.sign(self.ppm_s)
         )
 
     @property
     def b1_i_inh_scale(self) -> float:
         return self._b1_i_inh_scale
 
     @b1_i_inh_scale.setter
-    def b1_i_inh_scale(self, value: float):
+    def b1_i_inh_scale(self, value: float) -> None:
         self._b1_i_inh_scale = value
         self.b1_i = self._b1_i
 
     @property
     def b1_i_inh_res(self) -> int:
         return self._b1_i_inh_res
 
     @b1_i_inh_res.setter
-    def b1_i_inh_res(self, value: int):
+    def b1_i_inh_res(self, value: int) -> None:
         self._b1_i_inh_res = value
         self.b1_i = self._b1_i
 
     @property
     def b1_i(self) -> float:
         return self._b1_i
 
     @b1_i.setter
-    def b1_i(self, value: float):
+    def b1_i(self, value: float) -> None:
         self._b1_i = value
         self._b1_i_dist, self._b1_i_weights = _make_gaussian(
             self.b1_i,
             self.b1_i_inh_scale,
             self.b1_i_inh_res,
         )
         self._b1_i_dist = self._b1_i_dist.reshape((-1, 1, 1))
@@ -194,36 +195,36 @@
         self.l_b1y_i = self.matrices.get("b1y_i", 0.0) * self._b1_i_dist
 
     @property
     def b1_s(self) -> float:
         return self._b1_s
 
     @b1_s.setter
-    def b1_s(self, value: float):
+    def b1_s(self, value: float) -> None:
         self._b1_s = value
         self.l_b1x_s = self.matrices.get("b1x_s", 0.0) * value
         self.l_b1y_s = self.matrices.get("b1y_s", 0.0) * value
 
     @property
     def jeff_i(self) -> Distribution:
         return self._jeff_i
 
     @jeff_i.setter
-    def jeff_i(self, distribution: Distribution):
+    def jeff_i(self, distribution: Distribution) -> None:
         self._jeff_i = distribution
         values = distribution.values.reshape((-1, 1, 1, 1))
         self._l_jeff_i = self.matrices.get("jeff_i", np.array(0.0)) * values
         self._jeff_i_weights = distribution.weights.reshape((-1, 1, 1, 1))
 
     @property
     def gradient_dephasing(self) -> float:
         return self._gradient_dephasing
 
     @gradient_dephasing.setter
-    def gradient_dephasing(self, value: float):
+    def gradient_dephasing(self, value: float) -> None:
         self._gradient_dephasing = value
         self._scale_matrix("d_{state}", value * 1e-12)
         self._build_base_liouvillian()
 
     @property
     def l_free(self) -> ArrayFloat:
         return sum(
@@ -239,19 +240,19 @@
         )
 
     @property
     def weights(self) -> ArrayFloat:
         return self._b1_i_weights * self._jeff_i_weights
 
     @property
-    def detection(self):
+    def detection(self) -> str:
         return self._detection
 
     @detection.setter
-    def detection(self, value: str):
+    def detection(self, value: str) -> None:
         self._detection = value
         expr = _RE_COMP.sub(r'self.vectors.get("\g<1>")', value)
         vector: ArrayFloat = eval(expr)
         self._detect_vector = vector.transpose()
 
     def detect(self, magnetization: ArrayFloat) -> float:
         shape = -1, *magnetization.shape[-2:]
```

### Comparing `chemex-2024.2.9/chemex/nmr/rates.py` & `chemex-2024.5.0/chemex/nmr/rates.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,30 +13,48 @@
 from chemex.typing import ArrayFloat
 
 # Type definition
 T = TypeVar("T", float, ArrayFloat)
 
 
 def _calculate_jw(tauc: float, s2: float, w: T) -> T:
+    """Calculates J(w) for given tau_c, s2, and angular frequency w.
+
+    Args:
+        tauc (float): Correlation time in seconds.
+        s2 (float): Order parameter squared, amplitude of motion measure.
+        w (T): Angular frequency/frequencies for J(w) calculation. Can be float or
+               ArrayFloat.
+
+    Returns:
+        T: Spectral density function(s) J(w).
+    """
     tauc_ = tauc * 1e-9
     return 2.0 / 5.0 * tauc_ * s2 / (1.0 + (w * tauc_) ** 2)
 
 
 class RatesIS:
+    """Base class for calculating relaxation rates in IS spin systems.
+
+    Attributes describe gyromagnetic ratios, distances, CSA parameters, and Euler angles
+    for nuclei I and S.
+    """
+
     gi: float
     gs: float
     ris3: float
     rih3: float
     rsh3: float
     csa_i: ArrayFloat
     csa_s: ArrayFloat
     phi_i: ArrayFloat
     phi_s: ArrayFloat
 
     def __init__(self) -> None:
+        """Initializes RatesIS object with default gyromagnetic ratios and distances."""
         self.gh = GAMMA["h"]
 
         # Dipolar factors
         self.dis = -mu_0 * hbar * self.gi * self.gs / (8.0 * np.pi * self.ris3)
         dih = -mu_0 * hbar * self.gi * self.gh / (8.0 * np.pi * self.rih3)
         dsh = -mu_0 * hbar * self.gs * self.gh / (8.0 * np.pi * self.rsh3)
         self.dis2 = self.dis * self.dis
@@ -44,14 +62,24 @@
         self.dsh2 = dsh * dsh
 
         # CSA factors
         self.delta_i = self.csa_i[:2] - self.csa_i[2]
         self.delta_s = self.csa_s[:2] - self.csa_s[2]
 
     def __call__(self, h_frq: float, tauc: float, s2: float) -> dict[str, float]:
+        """Calculates relaxation rates for given Larmor frequency, tau_c, and s2.
+
+        Args:
+            h_frq (float): Proton Larmor frequency in MHz.
+            tauc (float): Correlation time in seconds.
+            s2 (float): Order parameter squared.
+
+        Returns:
+            dict[str, float]: Dictionary of relaxation rates (R2, R1 for I and S).
+        """
         # B0 in Tesla
         b0 = 2.0 * np.pi * 1e6 * h_frq / self.gh
 
         # Larmor angular frequencies
         wi, ws, wh = -np.array([self.gi, self.gs, self.gh]) * b0
 
         # CSA factors
@@ -130,14 +158,16 @@
             "etaz_s": self.dis * cs * 6 * js,
             "sigma_is": self.dis2 * (-jmis + 6.0 * jpis),
             "mu_is": 0.5 * self.dis2 * (-jmis + 6.0 * jpis),
         }
 
 
 class RateNH(RatesIS):
+    """Class for calculating relaxation rates in NH group using model-free approach."""
+
     gi = GAMMA["n"]
     gs = GAMMA["h"]
     ris3 = 1.04e-10**3
     rih3 = 1.79e-10**3
     rsh3 = 1.85e-10**3
     csa_i = np.array([69.0, 42.0, -111.0]) * 1e-6
     csa_s = np.array([5.7, 0.5, -6.2]) * 1e-6
@@ -147,14 +177,25 @@
     def __call__(
         self,
         h_frq: float,
         tauc: float,
         s2: float,
         khh: float = 0.0,
     ) -> dict[str, float]:
+        """Calculates rates for NH systems, including exchange contributions if any.
+
+        Args:
+            h_frq (float): Proton Larmor frequency in MHz.
+            tauc (float): Correlation time in seconds.
+            s2 (float): Order parameter squared.
+            khh (float, optional): Exchange rate between H atoms. Defaults to 0.
+
+        Returns:
+            dict[str, float]: Relaxation rates for NH systems, including exchanges.
+        """
         rates = super().__call__(h_frq, tauc, s2)
         if khh == 0:
             return rates
         # Make a copy of rates before adding 'khh' due to lru_cache"
         # on 'super().__call__'
         rates = rates.copy()
         rates["r2_s"] += khh
@@ -248,14 +289,16 @@
     "nh_d": RateNH_D(),
     "hn": RateHN(),
     "hn_d": RateHN_D(),
     "ch": RateCH(),
     "ch_d": RateCH_D(),
     "hc": RateHC(),
     "hc_d": RateHC_D(),
+    "cn": RateCH(),
+    "cn_d": RateCH_D(),
 }
 
 _RATE_NAMES = [
     "r2_i",
     "r2_s",
     "r1_i",
     "r1_s",
@@ -269,28 +312,22 @@
     "etaz_s",
     "sigma_is",
     "mu_is",
 ]
 
 
 def get_model_free_expressions(basis: Basis, conditions: Conditions) -> dict[str, str]:
-    """It takes a basis and a set of conditions,
-    and returns a dictionary of rate expressions.
+    """Generates expressions for model-free analysis based on basis and conditions.
 
-    Parameters
-    ----------
-    basis : Basis
-        The basis set to use for the model-free analysis.
-    conditions : Conditions
-        The conditions for the fitting.
+    Args:
+        basis (Basis): Basis set for model-free analysis.
+        conditions (Conditions): Conditions including Larmor frequency and deuteration.
 
     Returns:
-    -------
-        A dictionary of rate names and their corresponding expressions.
-
+        dict[str, str]: Mapping of rate names to expressions for model-free analysis.
     """
     deuterated_extension = "_d" if conditions.is_deuterated else ""
     rate_function_name = f"{basis.spin_system}{deuterated_extension}"
 
     h_frq_str = f"{conditions.h_larmor_frq}"
     has_h_exchange = basis.spin_system in {"nh", "hn"}
```

### Comparing `chemex-2024.2.9/chemex/nmr/spectrometer.py` & `chemex-2024.5.0/chemex/nmr/spectrometer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from collections.abc import Iterable, Sequence
+from collections.abc import Hashable, Iterable, Sequence
 from functools import reduce
 from itertools import product
 
 import numpy as np
 from cachetools import cached
 from cachetools.keys import hashkey
 from scipy.linalg import expm
@@ -18,14 +18,15 @@
 # A small value used for numerical stability
 SMALL_VALUE = 1e-6
 
 
 def calculate_propagators(
     liouv: ArrayFloat,
     delays: float | Iterable[float],
+    *,
     dephasing: bool = False,
 ) -> ArrayFloat:
     """Calculate the propagators for the given delays.
 
     Parameters
     ----------
     liouv : ArrayFloat
@@ -42,15 +43,15 @@
     """
     # Ensure delays is a 1D NumPy array
     delays = np.asarray(delays).flatten()
 
     if delays.size == 1 and not dephasing:
         # If there's only one delay and no dephasing, calculate the propagator directly
         # using scipy expm function
-        return expm(liouv * delays[0])
+        return expm(liouv * delays[0]).astype(np.float64)
 
     # Calculate eigenvalues and eigenvectors of the Liouvillian matrices
     eigenvalues, eigenvectors = np.linalg.eig(liouv)
 
     if dephasing:
         # If dephasing is requested, adjust eigenvalues
         eigenvalues = np.where(
@@ -76,15 +77,17 @@
         # If there's only one propagator, return it with no extra time dimension
         propagators = propagators[0]
 
     # Return the real part of the propagators
     return propagators.real
 
 
-def _get_key(liouvillian: LiouvillianIS, *args, **kwargs):
+def _get_key(
+    liouvillian: LiouvillianIS, *args: Hashable, **kwargs: Hashable
+) -> tuple[Hashable, ...]:
     return hashkey(liouvillian.basis, *args, **kwargs)
 
 
 @cached(cache={}, key=_get_key)
 def _make_perfect180(liouvillian: LiouvillianIS, spin: str) -> ArrayFloat:
     size = liouvillian.size
     identity = np.eye(size).reshape((1, 1, size, size))
@@ -101,15 +104,15 @@
 
 
 @cached(cache={}, key=_get_key)
 def _make_perfect90(liouvillian: LiouvillianIS, spin: str) -> ArrayFloat:
     size = liouvillian.size
     zeros = np.zeros((size, size))
     rot = liouvillian.matrices.get(f"b1x_{spin}", zeros)
-    return np.asarray(expm(0.25 * rot)).reshape((1, 1, size, size))
+    return expm(0.25 * rot).reshape(1, 1, size, size).astype(np.float64)
 
 
 @cached(cache={}, key=_get_key)
 def _get_phases(liouvillian: LiouvillianIS) -> DictArrayFloat:
     phases = {}
     size = liouvillian.size
     zeros = np.zeros((size, size))
@@ -293,15 +296,15 @@
         dephased = self.b1_i_inh_scale == np.inf
         rad = phase * np.pi * 0.5
         liouv = (
             self.liouvillian.l_free
             + scale * np.cos(rad) * self.liouvillian.l_b1x_i
             + scale * np.sin(rad) * self.liouvillian.l_b1y_i
         )
-        return calculate_propagators(liouv, times, dephased)
+        return calculate_propagators(liouv, times, dephasing=dephased)
 
     def pulse_s(
         self,
         times: float | Iterable[float],
         phase: float,
         scale: float = 1.0,
     ) -> ArrayFloat:
@@ -323,15 +326,15 @@
         liouv = (
             self.liouvillian.l_free
             + np.cos(phase_i * np.pi * 0.5) * self.liouvillian.l_b1x_i
             + np.sin(phase_i * np.pi * 0.5) * self.liouvillian.l_b1y_i
             + np.cos(phase_s * np.pi * 0.5) * self.liouvillian.l_b1x_s
             + np.sin(phase_s * np.pi * 0.5) * self.liouvillian.l_b1y_s
         )
-        return calculate_propagators(liouv, times, dephased)
+        return calculate_propagators(liouv, times, dephasing=dephased)
 
     def shaped_pulse_i(
         self,
         pw: float,
         amplitudes: Sequence[float],
         phases: Iterable[float],
     ) -> ArrayFloat:
@@ -389,15 +392,15 @@
             self._p180_s = pulses.swapaxes(0, 1)
 
     @property
     def p180_s(self) -> ArrayFloat:
         self._calculate_base_pulses_s()
         return self._p180_s
 
-    def p9024090_nh(self, reverse: bool = False) -> ArrayFloat:
+    def p9024090_nh(self, *, reverse: bool = False) -> ArrayFloat:
         ph_n = 1 if reverse else 3
         ph_h = 3 if reverse else 1
         pw240i, pw9024090i = np.array([8.0, 14.0]) * self._pw90_i / 3.0
         pw240s, pw9024090s = np.array([8.0, 14.0]) * self._pw90_s / 3.0
         t0, t1, t2, t3 = 0.5 * np.diff(
             np.sort([pw240i, pw240s, pw9024090i, pw9024090s]),
             prepend=0.0,
```

### Comparing `chemex-2024.2.9/chemex/optimize/fitting.py` & `chemex-2024.5.0/chemex/optimize/fitting.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/optimize/gridding.py` & `chemex-2024.5.0/chemex/optimize/gridding.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     chisqr: ArrayFloat
 
 
 def _set_param_values(
     params: Parameters,
     fnames: Iterable[str],
     values: tuple[float, ...],
-):
+) -> None:
     for fname, value in zip(fnames, values, strict=True):
         params[fname].value = value
 
 
 def run_group_grid(
     group: Group,
     grid: dict[str, ArrayFloat],
@@ -144,15 +144,15 @@
 
         result = GridResult(grid_ref, chisqr_sum)
         results.append(result)
 
     return results
 
 
-def set_params_from_grid(grids_1d: Iterable[GridResult]):
+def set_params_from_grid(grids_1d: Iterable[GridResult]) -> None:
     par_values = {}
     for grid_result in grids_1d:
         id_, values = next(iter(grid_result.grid.items()))
         par_values[id_] = values[grid_result.chisqr.argmin()]
     database.set_param_values(par_values)
```

### Comparing `chemex-2024.2.9/chemex/optimize/grouping.py` & `chemex-2024.5.0/chemex/optimize/grouping.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/optimize/helper.py` & `chemex-2024.5.0/chemex/optimize/helper.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/optimize/minimizer.py` & `chemex-2024.5.0/chemex/optimize/minimizer.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/parameters/database.py` & `chemex-2024.5.0/chemex/parameters/database.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/parameters/factory.py` & `chemex-2024.5.0/chemex/parameters/factory.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/parameters/name.py` & `chemex-2024.5.0/chemex/parameters/name.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 import re
 from collections.abc import Hashable, Iterable
 from dataclasses import dataclass, field
 from functools import cached_property
 from re import Pattern
+from typing import Self
 
 from rapidfuzz.process import extractOne
-from typing_extensions import Self
 
 from chemex.configuration.conditions import Conditions
 from chemex.parameters.spin_system import SpinSystem
 
 _EXPAND = {"-": "_", "+": "_", ".": "_"}
 
 _FLOAT = r"[-+]?(\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?"
```

### Comparing `chemex-2024.2.9/chemex/parameters/setting.py` & `chemex-2024.5.0/chemex/parameters/setting.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/parameters/spin_system/atom.py` & `chemex-2024.5.0/chemex/parameters/spin_system/atom.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/parameters/spin_system/constants.py` & `chemex-2024.5.0/chemex/parameters/spin_system/constants.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/parameters/spin_system/group.py` & `chemex-2024.5.0/chemex/parameters/spin_system/group.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/parameters/spin_system/nucleus.py` & `chemex-2024.5.0/chemex/parameters/spin_system/nucleus.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/parameters/spin_system/spin.py` & `chemex-2024.5.0/chemex/parameters/spin_system/spin.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/parameters/spin_system/spin_system.py` & `chemex-2024.5.0/chemex/parameters/spin_system/spin_system.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 from collections.abc import Hashable, Iterable, Sequence
 from functools import cache, cached_property, total_ordering
-from typing import TYPE_CHECKING, Any, Literal
+from typing import TYPE_CHECKING, Any, Literal, Self
 
 from pydantic import BaseModel, Field, InstanceOf, computed_field, model_validator
-from typing_extensions import Self
 
 from chemex.parameters.spin_system.atom import Atom
 from chemex.parameters.spin_system.group import Group
 from chemex.parameters.spin_system.nucleus import Nucleus
 from chemex.parameters.spin_system.spin import Spin
 from chemex.parameters.spin_system.utilities import powerset
```

### Comparing `chemex-2024.2.9/chemex/parameters/spin_system/utilities.py` & `chemex-2024.5.0/chemex/parameters/spin_system/utilities.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/parameters/spins.py` & `chemex-2024.5.0/chemex/parameters/spins.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/parameters/userfunctions.py` & `chemex-2024.5.0/chemex/parameters/userfunctions.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/plotters/cest.py` & `chemex-2024.5.0/chemex/plotters/cest.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 def plot_dcest(
     file_pdf: PdfPages,
     name: str,
     data_exp: Data,
     data_calc: Data,
     cs_values: ArrayFloat,
     circular_shift: CircularShift,
-):
+) -> None:
     if data_exp.size > 0:
         residuals = data_exp.exp - data_exp.calc
         sigma = estimate_sigma(residuals)
     else:
         sigma = 0.0
     centre = float(np.mean(cs_values))
     data_exp.metadata = circular_shift.centre(data_exp.metadata, centre)
```

### Comparing `chemex-2024.2.9/chemex/plotters/cpmg.py` & `chemex-2024.5.0/chemex/plotters/cpmg.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 class CpmgExperimentConfig(Protocol):
     experiment: CpmgExperimentSettings
 
 
 T = TypeVar("T", bound=CpmgExperimentConfig)
 
 
-def plot_cpmg(file_pdf: PdfPages, name: str, data_exp: Data, data_calc: Data):
+def plot_cpmg(file_pdf: PdfPages, name: str, data_exp: Data, data_calc: Data) -> None:
     fig = plot_profile(name, data_exp, data_calc)
     ax2 = fig.axes[1]
     ax2.set_xlabel(r"$\nu_\mathregular{CPMG}$ (Hz)")
     ax2.set_ylabel(r"$R_{2,\mathregular{eff}}$ (s$^{-1}$)")
     ax2.set_xlim(0.0, max(data_calc.metadata) + min(data_calc.metadata))
     if data_exp.size == 0:
         fig.delaxes(fig.axes[0])
```

### Comparing `chemex-2024.2.9/chemex/plotters/exsy.py` & `chemex-2024.5.0/chemex/plotters/exsy.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from chemex.containers.data import Data
 from chemex.containers.profile import Profile
 from chemex.messages import print_plot_filename
 from chemex.plotters.plot import get_grid, plot_profile
 from chemex.printers.plot import PlotPrinter, data_plot_printers
 
 
-def plot_exsy(file_pdf: PdfPages, name: str, data_exp: Data, data_calc: Data):
+def plot_exsy(file_pdf: PdfPages, name: str, data_exp: Data, data_calc: Data) -> None:
     fig = plot_profile(name, data_exp, data_calc)
     ax2 = fig.axes[1]
     ax2.set_xlabel(r"Time (s)")
     ax2.set_ylabel(r"Intensity")
     ax2.set_xlim(0.0, max(data_exp.metadata) + min(data_calc.metadata))
     file_pdf.savefig(fig)
```

### Comparing `chemex-2024.2.9/chemex/plotters/plot.py` & `chemex-2024.5.0/chemex/plotters/plot.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,23 +28,23 @@
 def get_grid(values: ArrayFloat, size: int = 400, extension: float = 0.0) -> ArrayFloat:
     value_min = np.min(values)
     value_max = np.max(values)
     extra = (value_max - value_min) * extension
     return np.linspace(value_min - extra, value_max + extra, size)
 
 
-def _plot_fit(data_calc: Data, ax2: Axes):
+def _plot_fit(data_calc: Data, ax2: Axes) -> None:
     fit_x = data_calc.metadata
     fit_y = data_calc.calc
     range_x = get_grid(fit_x, 2, 0.02)
     ax2.set_xlim(*range_x)
     ax2.plot(fit_x, fit_y, linestyle="-", color=_RED300)
 
 
-def _plot_exp(data_exp: Data, ax1: Axes, ax2: Axes):
+def _plot_exp(data_exp: Data, ax1: Axes, ax2: Axes) -> None:
     exp_x = data_exp.metadata
     exp_y = data_exp.exp
     exp_e = abs(data_exp.err)
     res_y = data_exp.exp - data_exp.calc
 
     m_sel = data_exp.mask
     m_inf = exp_e.sum(axis=1) > LARGE_VALUE
@@ -73,11 +73,17 @@
     fig, ax1, ax2 = _create_fig(name)
 
     _plot_fit(data_calc, ax2)
 
     if data_exp.size:
         _plot_exp(data_exp, ax1, ax2)
 
+    range1_y = ax1.get_ylim()
+    range2_y = ax2.get_ylim()
+
     for axis in (ax1, ax2):
         axis.axhline(0, color="k", linewidth=0.5, zorder=1)
 
+    ax1.set_ylim(*range1_y)
+    ax2.set_ylim(*range2_y)
+
     return fig
```

### Comparing `chemex-2024.2.9/chemex/plotters/relaxation.py` & `chemex-2024.5.0/chemex/plotters/relaxation.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from chemex.containers.data import Data
 from chemex.containers.profile import Profile
 from chemex.messages import print_plot_filename
 from chemex.plotters.plot import get_grid, plot_profile
 from chemex.printers.plot import PlotPrinter, data_plot_printers
 
 
-def plot_relaxation(file_pdf: PdfPages, name: str, data_exp: Data, data_calc: Data):
+def plot_relaxation(file_pdf: PdfPages, name: str, data_exp: Data, data_calc: Data) -> None:
     fig = plot_profile(name, data_exp, data_calc)
     ax2 = fig.axes[1]
     ax2.set_xlabel(r"Time (s)")
     ax2.set_ylabel(r"Intensity")
     ax2.set_xlim(0.0, max(data_exp.metadata) + min(data_calc.metadata))
     file_pdf.savefig(fig)
```

### Comparing `chemex-2024.2.9/chemex/plotters/shift.py` & `chemex-2024.5.0/chemex/plotters/shift.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from chemex.containers.data import Data
 from chemex.containers.profile import Profile
 from chemex.messages import print_plot_filename
 
 _RED700 = "#D32F2F"
 
 
-def plot_shift(name_pdf: Path, data: Data):
+def plot_shift(name_pdf: Path, data: Data) -> None:
     fig = Figure()
     ax = fig.subplots(1, 1)
     fig.align_labels()
     ax.errorbar(data.calc, data.exp, yerr=data.err, fmt=".", color=_RED700)
     val_min = min(ax.get_xlim()[0], ax.get_ylim()[0])
     val_max = max(ax.get_xlim()[1], ax.get_ylim()[1])
     ax.set_aspect("equal", "box")
```

### Comparing `chemex-2024.2.9/chemex/printers/data.py` & `chemex-2024.5.0/chemex/printers/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 from chemex.containers.data import Data
 
 
 class Printer(Protocol):
     header: str
     simulation: bool
 
-    def print(self, name: str, data: Data) -> str:
-        ...
+    def print(self, name: str, data: Data) -> str: ...
 
 
 @dataclass
 class ShiftPrinter:
     header = "\n".join(
         [
             "#",
@@ -23,14 +22,15 @@
             "#",
             (
                 f"# {'NAME':>16s} {'SHIFT (EXP)':>17s}"
                 f" {'ERROR (EXP)':>17s} {'SHIFT (CALC)':>17s}\n"
             ),
         ],
     )
+    simulation: bool = False
 
     def print(self, name: str, data: Data) -> str:
         return (
             f"{name:>18s} {data.exp[0]: 17.3f} {data.err[0]: 17.3f}"
             f" {data.calc[0]: 17.3f}\n"
         )
```

### Comparing `chemex-2024.2.9/chemex/printers/parameters.py` & `chemex-2024.5.0/chemex/printers/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,16 @@
     return text if RE_GROUPNAME.match(text) else f'"{text}"'
 
 
 def _format_strings(par_strings: dict[str, dict[str, str]]) -> str:
     result: list[str] = []
     for section, key_values in par_strings.items():
         result.append(f"[{_quote(section)}]")
-        width = len(max(key_values, key=len))
+        quoted_keys = [_quote(key) for key in key_values]
+        width = len(max(quoted_keys, key=len))
         result.extend(
             f"{_quote(key):<{width}} = {value}" for key, value in key_values.items()
         )
         result.append("")
     return "\n".join(result)
```

### Comparing `chemex-2024.2.9/chemex/printers/plot.py` & `chemex-2024.5.0/chemex/printers/plot.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/toml.py` & `chemex-2024.5.0/chemex/toml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 
 import sys
+import tomllib
 from collections.abc import Iterable, MutableMapping
 from pathlib import Path
 from typing import Any
 
-import tomllib
-
 from chemex.messages import print_file_not_found, print_toml_error
 
 
 def read_toml(filename: Path) -> dict[str, Any]:
     """Read and parse the experiment configuration file with 'toml."""
     with filename.open(mode="rb") as file:
         try:
```

### Comparing `chemex-2024.2.9/chemex/tools/pick_cest/buttons.py` & `chemex-2024.5.0/chemex/tools/pick_cest/buttons.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                 spin_system = profile.spin_system
                 spin_systems.add(spin_system)
                 self.data.setdefault(spin_system, []).append(Curve(profile, sw))
 
         self.spin_systems = sorted(spin_systems)
         self.out = path
 
-        self.spin_system = SpinSystem("")
+        self.spin_system = SpinSystem(name="")
         self.curves: list[Curve] = []
         self.cs_a: dict[SpinSystem, float | None] = {}
         self.cs_b: dict[SpinSystem, float | None] = {}
         self.artists: list[Artist] = []
         self.sw = sw
 
         self.cursor = Cursor(self.axis, horizOn=False, useblit=True)
@@ -91,15 +91,15 @@
     def _get_click_position(self, event: Event) -> float | None:
         if not isinstance(event, LocationEvent):
             return None
         if event.inaxes != self.axis:
             return None
         return event.xdata
 
-    def _add_line(self, position: float, state: Literal["a", "b"]):
+    def _add_line(self, position: float, state: Literal["a", "b"]) -> None:
         text_ = rf"$\varpi_{state}$ = {position:.3f} ppm"
         text = self.fig.text(0.82, TEXT_Y[state], text_)
         line = self.axis.axvline(
             x=position,
             linestyle=LSTYLE[state],
             color="0.74",
             linewidth=1.0,
@@ -107,15 +107,15 @@
         self.artists.extend([line, text])
 
     def _add_text_dw(self, dw_ab: float) -> None:
         text_ = rf"$\Delta\varpi_{{ab}}$ = {dw_ab:.3f} ppm"
         text = self.fig.text(0.82, 0.7, text_)
         self.artists.append(text)
 
-    def _save(self):
+    def _save(self) -> None:
         self.out.mkdir(parents=True, exist_ok=True)
 
         fname1 = self.out / "cs_a.toml"
         fname2 = self.out / "dw_ab.toml"
 
         with contextlib.ExitStack() as stack:
             file1 = stack.enter_context(fname1.open("w", encoding="utf-8"))
@@ -175,15 +175,15 @@
 
     def _plot(self, event: Event | None = None) -> None:
         self._clear_axis()
         self._plot_lines()
         self._plot_profiles()
         self.fig.canvas.draw_idle()
 
-    def _shift(self, step: int):
+    def _shift(self, step: int) -> None:
         self.index += step
         self.index %= len(self.spin_systems)
         self.spin_system = self.spin_systems[self.index]
         self.curves = self.data[self.spin_system]
         self._clear_axis()
         self._plot()
```

### Comparing `chemex-2024.2.9/chemex/tools/pick_cest/cest_picker.py` & `chemex-2024.5.0/chemex/tools/pick_cest/cest_picker.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/tools/pick_cest/curve.py` & `chemex-2024.5.0/chemex/tools/pick_cest/curve.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/chemex/tools/plot_param.py` & `chemex-2024.5.0/chemex/tools/plot_param.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         section_name = cpn.ParamName.from_section(section.strip('"'))
         if param_name.match(section_name):
             print_section(section)
             residues: list[int] = []
             values: list[float] = []
             errors: list[float] = []
             for key, entry in params.items(section):
-                residues.append(int(cns.SpinSystem(key).numbers["i"]))
+                residues.append(int(cns.SpinSystem(name=key).numbers["i"]))
                 split = entry.split()
                 values.append(float(split[0]))
                 try:
                     error = float(split[2].strip("±"))
                 except ValueError:
                     error = 0.0
                 errors.append(error)
```

### Comparing `chemex-2024.2.9/chemex/uncertainty.py` & `chemex-2024.5.0/chemex/uncertainty.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.2.9/pyproject.toml` & `chemex-2024.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -7,31 +7,30 @@
 [project]
 name = "chemex"
 description = "An analysis program for chemical exchange detected by NMR"
 authors = [
     { name = "Guillaume Bouvignies", email = "guillaume.bouvignies@ens.psl.eu" },
 ]
 dependencies = [
-    "numpy>=1.26.1",
-    "scipy>=1.11.3",
-    "matplotlib>=3.8.0",
+    "numpy>=1.26.4",
+    "scipy>=1.13.0",
+    "matplotlib>=3.8.4",
     "lmfit>=1.2.2",
-    "pydantic>=2.4.2",
-    "cachetools>=5.3.2",
-    "rich>=13.6.0",
-    "tomli>=2.0.1",
-    "rapidfuzz>=3.4.0",
+    "pydantic>=2.6.4",
+    "cachetools>=5.3.3",
+    "rich>=13.7.1",
+    "rapidfuzz>=3.7.0",
     "emcee>=3.1.4",
-    "typing-extensions>=4.9.0",
     "numdifftools>=0.9.41",
+    "annotated-types>=0.6.0",
 ]
-requires-python = ">=3.10,<3.13"
+requires-python = ">=3.11,<3.13"
 readme = "README.md"
 dynamic = []
-version = "2024.2.9"
+version = "2024.5.0"
 
 [project.license]
 text = "GPL-3.0-or-later"
 
 [project.urls]
 Homepage = "http://gbouvignies.github.io/ChemEx/"
 Documentation = "http://gbouvignies.github.io/ChemEx/"
```

### Comparing `chemex-2024.2.9/PKG-INFO` & `chemex-2024.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: chemex
-Version: 2024.2.9
+Version: 2024.5.0
 Summary: An analysis program for chemical exchange detected by NMR
 Author-Email: Guillaume Bouvignies <guillaume.bouvignies@ens.psl.eu>
 License: GPL-3.0-or-later
 Project-URL: Homepage, http://gbouvignies.github.io/ChemEx/
 Project-URL: Documentation, http://gbouvignies.github.io/ChemEx/
 Project-URL: Repository, https://github.com/gbouvignies/chemex
 Project-URL: Changelog, https://github.com/gbouvignies/chemex/releases
-Requires-Python: <3.13,>=3.10
-Requires-Dist: numpy>=1.26.1
-Requires-Dist: scipy>=1.11.3
-Requires-Dist: matplotlib>=3.8.0
+Requires-Python: <3.13,>=3.11
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: scipy>=1.13.0
+Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: lmfit>=1.2.2
-Requires-Dist: pydantic>=2.4.2
-Requires-Dist: cachetools>=5.3.2
-Requires-Dist: rich>=13.6.0
-Requires-Dist: tomli>=2.0.1
-Requires-Dist: rapidfuzz>=3.4.0
+Requires-Dist: pydantic>=2.6.4
+Requires-Dist: cachetools>=5.3.3
+Requires-Dist: rich>=13.7.1
+Requires-Dist: rapidfuzz>=3.7.0
 Requires-Dist: emcee>=3.1.4
-Requires-Dist: typing-extensions>=4.9.0
 Requires-Dist: numdifftools>=0.9.41
+Requires-Dist: annotated-types>=0.6.0
 Description-Content-Type: text/markdown
 
 # ChemEx: NMR Chemical Exchange Analysis Tool
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 ## Table of Contents
```

