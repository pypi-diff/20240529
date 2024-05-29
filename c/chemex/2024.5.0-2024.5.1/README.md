# Comparing `tmp/chemex-2024.5.0.tar.gz` & `tmp/chemex-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemex-2024.5.0.tar", last modified: Tue May 28 21:51:25 2024, max compression
+gzip compressed data, was "chemex-2024.5.1.tar", last modified: Wed May 29 10:48:12 2024, max compression
```

## Comparing `chemex-2024.5.0.tar` & `chemex-2024.5.1.tar`

### file list

```diff
@@ -1,135 +1,135 @@
--rw-r--r--   0        0        0    34916 2024-05-28 21:51:20.687304 chemex-2024.5.0/LICENSE.md
--rw-r--r--   0        0        0     2833 2024-05-28 21:51:20.687304 chemex-2024.5.0/README.md
--rw-r--r--   0        0        0      326 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/__init__.py
--rw-r--r--   0        0        0      185 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/__main__.py
--rw-r--r--   0        0        0     2395 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/chemex.py
--rw-r--r--   0        0        0     5947 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/cli.py
--rw-r--r--   0        0        0        0 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/configuration/__init__.py
--rw-r--r--   0        0        0     1350 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/configuration/base.py
--rw-r--r--   0        0        0     6524 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/configuration/conditions.py
--rw-r--r--   0        0        0     1291 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/configuration/data.py
--rw-r--r--   0        0        0      642 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/configuration/experiment.py
--rw-r--r--   0        0        0     2920 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/configuration/methods.py
--rw-r--r--   0        0        0     1757 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/configuration/parameters.py
--rw-r--r--   0        0        0     1799 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/configuration/utils.py
--rw-r--r--   0        0        0        0 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/containers/__init__.py
--rw-r--r--   0        0        0     5097 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/containers/data.py
--rw-r--r--   0        0        0     2621 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/containers/dataset.py
--rw-r--r--   0        0        0     5686 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/containers/experiment.py
--rw-r--r--   0        0        0     8270 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/containers/experiments.py
--rw-r--r--   0        0        0     4994 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/containers/profile.py
--rw-r--r--   0        0        0        0 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/__init__.py
--rw-r--r--   0        0        0     4511 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/builder.py
--rw-r--r--   0        0        0        0 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/__init__.py
--rw-r--r--   0        0        0     3710 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cest_13c.py
--rw-r--r--   0        0        0     3621 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cest_15n.py
--rw-r--r--   0        0        0     4031 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cest_15n_cw.py
--rw-r--r--   0        0        0     4353 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cest_15n_tr.py
--rw-r--r--   0        0        0     3708 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cest_1hn_ap.py
--rw-r--r--   0        0        0     4755 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cest_1hn_ip_ap.py
--rw-r--r--   0        0        0     4062 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cest_ch3_1h_ip_ap.py
--rw-r--r--   0        0        0     5203 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/coscest_13c.py
--rw-r--r--   0        0        0     5485 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/coscest_1hn_ip_ap.py
--rw-r--r--   0        0        0     4729 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_13c_ip.py
--rw-r--r--   0        0        0     5123 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_13co_ap.py
--rw-r--r--   0        0        0     4813 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_15n_ip.py
--rw-r--r--   0        0        0     5683 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_15n_ip_0013.py
--rw-r--r--   0        0        0     5385 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_15n_tr.py
--rw-r--r--   0        0        0     7510 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_15n_tr_0013.py
--rw-r--r--   0        0        0     5143 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_1hn_ap.py
--rw-r--r--   0        0        0     7690 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_1hn_ap_0013.py
--rw-r--r--   0        0        0     4967 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_ch3_13c_h2c.py
--rw-r--r--   0        0        0     5822 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_ch3_1h_dq.py
--rw-r--r--   0        0        0     6654 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_ch3_1h_sq.py
--rw-r--r--   0        0        0     5824 2024-05-28 21:51:20.687304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_ch3_1h_tq.py
--rw-r--r--   0        0        0     7360 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_ch3_1h_tq_diff.py
--rw-r--r--   0        0        0     4239 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_ch3_mq.py
--rw-r--r--   0        0        0     4858 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_chd2_1h_ap.py
--rw-r--r--   0        0        0     5383 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/catalog/cpmg_hn_dq_zq.py
--rw-r--r--   0        0        0     4389 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/catalog/dcest_13c.py
--rw-r--r--   0        0        0     4661 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/catalog/dcest_15n.py
--rw-r--r--   0        0        0     3064 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/catalog/noesyfpgpph19.py
--rw-r--r--   0        0        0     3281 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/catalog/relaxation_hznz.py
--rw-r--r--   0        0        0     2953 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/catalog/relaxation_nz.py
--rw-r--r--   0        0        0     2892 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/catalog/shift_15n_sq.py
--rw-r--r--   0        0        0     3313 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/catalog/shift_15n_sqmq.py
--rw-r--r--   0        0        0     3327 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/factories.py
--rw-r--r--   0        0        0      957 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/experiments/loader.py
--rw-r--r--   0        0        0     2606 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/filterers.py
--rw-r--r--   0        0        0    20310 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/messages.py
--rw-r--r--   0        0        0        0 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/__init__.py
--rw-r--r--   0        0        0     2916 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/constraints.py
--rw-r--r--   0        0        0     1080 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/factory.py
--rw-r--r--   0        0        0        0 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/__init__.py
--rw-r--r--   0        0        0      482 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_1st.py
--rw-r--r--   0        0        0     1223 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_2st.py
--rw-r--r--   0        0        0     3351 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_2st_binding.py
--rw-r--r--   0        0        0     2792 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_2st_eyring.py
--rw-r--r--   0        0        0     1891 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_2st_hd.py
--rw-r--r--   0        0        0     3094 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_2st_monomer_dimer.py
--rw-r--r--   0        0        0     3124 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_2st_monomer_tetramer.py
--rw-r--r--   0        0        0     3104 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_2st_monomer_trimer.py
--rw-r--r--   0        0        0     1224 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_2st_rs.py
--rw-r--r--   0        0        0     5751 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_3st_binding_2st_partner.py
--rw-r--r--   0        0        0     4255 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_3st_binding_cs.py
--rw-r--r--   0        0        0     4179 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_3st_binding_if.py
--rw-r--r--   0        0        0     5067 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_3st_double_binding.py
--rw-r--r--   0        0        0     4528 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_3st_eyring.py
--rw-r--r--   0        0        0     4382 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_3st_monomer_dimer_tetramer.py
--rw-r--r--   0        0        0     4851 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_3st_monomer_dimer_trimer.py
--rw-r--r--   0        0        0     7001 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_4st_binding_2st_partner.py
--rw-r--r--   0        0        0     6471 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_4st_binding_3_bound_states.py
--rw-r--r--   0        0        0     3901 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_4st_hd.py
--rw-r--r--   0        0        0     4695 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/kinetic/settings_nst.py
--rw-r--r--   0        0        0      933 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/loader.py
--rw-r--r--   0        0        0     1250 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/models/model.py
--rw-r--r--   0        0        0        0 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/nmr/__init__.py
--rw-r--r--   0        0        0    10954 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/nmr/basis.py
--rw-r--r--   0        0        0     6405 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/nmr/constants.py
--rw-r--r--   0        0        0     9646 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/nmr/liouvillian.py
--rw-r--r--   0        0        0    10512 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/nmr/rates.py
--rw-r--r--   0        0        0    14637 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/nmr/spectrometer.py
--rw-r--r--   0        0        0        0 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/optimize/__init__.py
--rw-r--r--   0        0        0     5179 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/optimize/fitting.py
--rw-r--r--   0        0        0     8773 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/optimize/gridding.py
--rw-r--r--   0        0        0     4299 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/optimize/grouping.py
--rw-r--r--   0        0        0     5332 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/optimize/helper.py
--rw-r--r--   0        0        0     4449 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/optimize/minimizer.py
--rw-r--r--   0        0        0        0 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/parameters/__init__.py
--rw-r--r--   0        0        0    22058 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/parameters/database.py
--rw-r--r--   0        0        0     3335 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/parameters/factory.py
--rw-r--r--   0        0        0     4737 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/parameters/name.py
--rw-r--r--   0        0        0     3959 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/parameters/setting.py
--rw-r--r--   0        0        0       78 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/parameters/spin_system/__init__.py
--rw-r--r--   0        0        0     2304 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/parameters/spin_system/atom.py
--rw-r--r--   0        0        0     1727 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/parameters/spin_system/constants.py
--rw-r--r--   0        0        0     4141 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/parameters/spin_system/group.py
--rw-r--r--   0        0        0     1567 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/parameters/spin_system/nucleus.py
--rw-r--r--   0        0        0     2139 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/parameters/spin_system/spin.py
--rw-r--r--   0        0        0     6488 2024-05-28 21:51:20.691304 chemex-2024.5.0/chemex/parameters/spin_system/spin_system.py
--rw-r--r--   0        0        0     1058 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/parameters/spin_system/utilities.py
--rw-r--r--   0        0        0    10123 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/parameters/spins.py
--rw-r--r--   0        0        0      977 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/parameters/userfunctions.py
--rw-r--r--   0        0        0        0 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/plotters/__init__.py
--rw-r--r--   0        0        0     8235 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/plotters/cest.py
--rw-r--r--   0        0        0     6917 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/plotters/cpmg.py
--rw-r--r--   0        0        0     4952 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/plotters/exsy.py
--rw-r--r--   0        0        0     2574 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/plotters/plot.py
--rw-r--r--   0        0        0      329 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/plotters/plotter.py
--rw-r--r--   0        0        0     3862 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/plotters/relaxation.py
--rw-r--r--   0        0        0     1688 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/plotters/shift.py
--rw-r--r--   0        0        0        0 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/printers/__init__.py
--rw-r--r--   0        0        0     4220 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/printers/data.py
--rw-r--r--   0        0        0     4577 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/printers/parameters.py
--rw-r--r--   0        0        0     2975 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/printers/plot.py
--rw-r--r--   0        0        0     2794 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/toml.py
--rw-r--r--   0        0        0        0 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/tools/__init__.py
--rw-r--r--   0        0        0       60 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/tools/pick_cest/__init__.py
--rw-r--r--   0        0        0     6575 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/tools/pick_cest/buttons.py
--rw-r--r--   0        0        0     3875 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/tools/pick_cest/cest_picker.py
--rw-r--r--   0        0        0     1496 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/tools/pick_cest/curve.py
--rw-r--r--   0        0        0     1867 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/tools/plot_param.py
--rw-r--r--   0        0        0      144 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/typing.py
--rw-r--r--   0        0        0     3649 2024-05-28 21:51:20.695304 chemex-2024.5.0/chemex/uncertainty.py
--rw-r--r--   0        0        0     1447 2024-05-28 21:51:25.931302 chemex-2024.5.0/pyproject.toml
--rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 chemex-2024.5.0/PKG-INFO
+-rw-r--r--   0        0        0    34916 2024-05-29 10:48:09.604230 chemex-2024.5.1/LICENSE.md
+-rw-r--r--   0        0        0     2833 2024-05-29 10:48:09.604230 chemex-2024.5.1/README.md
+-rw-r--r--   0        0        0      326 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/__init__.py
+-rw-r--r--   0        0        0      185 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/__main__.py
+-rw-r--r--   0        0        0     2395 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/chemex.py
+-rw-r--r--   0        0        0     5947 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/cli.py
+-rw-r--r--   0        0        0        0 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/configuration/__init__.py
+-rw-r--r--   0        0        0     1350 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/configuration/base.py
+-rw-r--r--   0        0        0     6524 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/configuration/conditions.py
+-rw-r--r--   0        0        0     1291 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/configuration/data.py
+-rw-r--r--   0        0        0      642 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/configuration/experiment.py
+-rw-r--r--   0        0        0     2920 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/configuration/methods.py
+-rw-r--r--   0        0        0     1757 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/configuration/parameters.py
+-rw-r--r--   0        0        0     1799 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/configuration/utils.py
+-rw-r--r--   0        0        0        0 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/containers/__init__.py
+-rw-r--r--   0        0        0     5097 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/containers/data.py
+-rw-r--r--   0        0        0     2621 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/containers/dataset.py
+-rw-r--r--   0        0        0     5686 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/containers/experiment.py
+-rw-r--r--   0        0        0     8270 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/containers/experiments.py
+-rw-r--r--   0        0        0     4994 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/containers/profile.py
+-rw-r--r--   0        0        0        0 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/__init__.py
+-rw-r--r--   0        0        0     4511 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/builder.py
+-rw-r--r--   0        0        0        0 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/__init__.py
+-rw-r--r--   0        0        0     3710 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/cest_13c.py
+-rw-r--r--   0        0        0     3621 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/cest_15n.py
+-rw-r--r--   0        0        0     4031 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/cest_15n_cw.py
+-rw-r--r--   0        0        0     4353 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/cest_15n_tr.py
+-rw-r--r--   0        0        0     3708 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/cest_1hn_ap.py
+-rw-r--r--   0        0        0     4755 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/cest_1hn_ip_ap.py
+-rw-r--r--   0        0        0     4062 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/cest_ch3_1h_ip_ap.py
+-rw-r--r--   0        0        0     5203 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/coscest_13c.py
+-rw-r--r--   0        0        0     5485 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/coscest_1hn_ip_ap.py
+-rw-r--r--   0        0        0     4729 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/cpmg_13c_ip.py
+-rw-r--r--   0        0        0     5123 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/cpmg_13co_ap.py
+-rw-r--r--   0        0        0     4813 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/cpmg_15n_ip.py
+-rw-r--r--   0        0        0     5683 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/cpmg_15n_ip_0013.py
+-rw-r--r--   0        0        0     5385 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/cpmg_15n_tr.py
+-rw-r--r--   0        0        0     7510 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/cpmg_15n_tr_0013.py
+-rw-r--r--   0        0        0     5143 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/cpmg_1hn_ap.py
+-rw-r--r--   0        0        0     7690 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/cpmg_1hn_ap_0013.py
+-rw-r--r--   0        0        0     4967 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/cpmg_ch3_13c_h2c.py
+-rw-r--r--   0        0        0     5822 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/cpmg_ch3_1h_dq.py
+-rw-r--r--   0        0        0     6654 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/cpmg_ch3_1h_sq.py
+-rw-r--r--   0        0        0     5824 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/cpmg_ch3_1h_tq.py
+-rw-r--r--   0        0        0     7360 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/cpmg_ch3_1h_tq_diff.py
+-rw-r--r--   0        0        0     4239 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/cpmg_ch3_mq.py
+-rw-r--r--   0        0        0     4858 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/cpmg_chd2_1h_ap.py
+-rw-r--r--   0        0        0     5383 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/cpmg_hn_dq_zq.py
+-rw-r--r--   0        0        0     4389 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/dcest_13c.py
+-rw-r--r--   0        0        0     4661 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/dcest_15n.py
+-rw-r--r--   0        0        0     3064 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/noesyfpgpph19.py
+-rw-r--r--   0        0        0     3281 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/relaxation_hznz.py
+-rw-r--r--   0        0        0     2953 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/relaxation_nz.py
+-rw-r--r--   0        0        0     2892 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/shift_15n_sq.py
+-rw-r--r--   0        0        0     3313 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/catalog/shift_15n_sqmq.py
+-rw-r--r--   0        0        0     3327 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/factories.py
+-rw-r--r--   0        0        0      957 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/experiments/loader.py
+-rw-r--r--   0        0        0     2606 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/filterers.py
+-rw-r--r--   0        0        0    20310 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/messages.py
+-rw-r--r--   0        0        0        0 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/models/__init__.py
+-rw-r--r--   0        0        0     2916 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/models/constraints.py
+-rw-r--r--   0        0        0     1080 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/models/factory.py
+-rw-r--r--   0        0        0        0 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/models/kinetic/__init__.py
+-rw-r--r--   0        0        0      482 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/models/kinetic/settings_1st.py
+-rw-r--r--   0        0        0     1223 2024-05-29 10:48:09.604230 chemex-2024.5.1/chemex/models/kinetic/settings_2st.py
+-rw-r--r--   0        0        0     3351 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/models/kinetic/settings_2st_binding.py
+-rw-r--r--   0        0        0     2792 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/models/kinetic/settings_2st_eyring.py
+-rw-r--r--   0        0        0     1891 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/models/kinetic/settings_2st_hd.py
+-rw-r--r--   0        0        0     3094 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/models/kinetic/settings_2st_monomer_dimer.py
+-rw-r--r--   0        0        0     3124 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/models/kinetic/settings_2st_monomer_tetramer.py
+-rw-r--r--   0        0        0     3104 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/models/kinetic/settings_2st_monomer_trimer.py
+-rw-r--r--   0        0        0     1224 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/models/kinetic/settings_2st_rs.py
+-rw-r--r--   0        0        0     5751 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/models/kinetic/settings_3st_binding_2st_partner.py
+-rw-r--r--   0        0        0     4255 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/models/kinetic/settings_3st_binding_cs.py
+-rw-r--r--   0        0        0     4179 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/models/kinetic/settings_3st_binding_if.py
+-rw-r--r--   0        0        0     5067 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/models/kinetic/settings_3st_double_binding.py
+-rw-r--r--   0        0        0     4528 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/models/kinetic/settings_3st_eyring.py
+-rw-r--r--   0        0        0     4382 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/models/kinetic/settings_3st_monomer_dimer_tetramer.py
+-rw-r--r--   0        0        0     4851 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/models/kinetic/settings_3st_monomer_dimer_trimer.py
+-rw-r--r--   0        0        0     7001 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/models/kinetic/settings_4st_binding_2st_partner.py
+-rw-r--r--   0        0        0     6471 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/models/kinetic/settings_4st_binding_3_bound_states.py
+-rw-r--r--   0        0        0     3901 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/models/kinetic/settings_4st_hd.py
+-rw-r--r--   0        0        0     4695 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/models/kinetic/settings_nst.py
+-rw-r--r--   0        0        0      933 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/models/loader.py
+-rw-r--r--   0        0        0     1250 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/models/model.py
+-rw-r--r--   0        0        0        0 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/nmr/__init__.py
+-rw-r--r--   0        0        0    10954 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/nmr/basis.py
+-rw-r--r--   0        0        0     6405 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/nmr/constants.py
+-rw-r--r--   0        0        0     9646 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/nmr/liouvillian.py
+-rw-r--r--   0        0        0    10512 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/nmr/rates.py
+-rw-r--r--   0        0        0    14637 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/nmr/spectrometer.py
+-rw-r--r--   0        0        0        0 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/optimize/__init__.py
+-rw-r--r--   0        0        0     5179 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/optimize/fitting.py
+-rw-r--r--   0        0        0     8777 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/optimize/gridding.py
+-rw-r--r--   0        0        0     4299 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/optimize/grouping.py
+-rw-r--r--   0        0        0     5332 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/optimize/helper.py
+-rw-r--r--   0        0        0     4449 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/optimize/minimizer.py
+-rw-r--r--   0        0        0        0 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/parameters/__init__.py
+-rw-r--r--   0        0        0    22058 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/parameters/database.py
+-rw-r--r--   0        0        0     3335 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/parameters/factory.py
+-rw-r--r--   0        0        0     4737 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/parameters/name.py
+-rw-r--r--   0        0        0     3959 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/parameters/setting.py
+-rw-r--r--   0        0        0       78 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/parameters/spin_system/__init__.py
+-rw-r--r--   0        0        0     2304 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/parameters/spin_system/atom.py
+-rw-r--r--   0        0        0     1727 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/parameters/spin_system/constants.py
+-rw-r--r--   0        0        0     4141 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/parameters/spin_system/group.py
+-rw-r--r--   0        0        0     1567 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/parameters/spin_system/nucleus.py
+-rw-r--r--   0        0        0     2139 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/parameters/spin_system/spin.py
+-rw-r--r--   0        0        0     6488 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/parameters/spin_system/spin_system.py
+-rw-r--r--   0        0        0     1058 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/parameters/spin_system/utilities.py
+-rw-r--r--   0        0        0    10123 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/parameters/spins.py
+-rw-r--r--   0        0        0      977 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/parameters/userfunctions.py
+-rw-r--r--   0        0        0        0 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/plotters/__init__.py
+-rw-r--r--   0        0        0     8235 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/plotters/cest.py
+-rw-r--r--   0        0        0     6917 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/plotters/cpmg.py
+-rw-r--r--   0        0        0     4952 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/plotters/exsy.py
+-rw-r--r--   0        0        0     2574 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/plotters/plot.py
+-rw-r--r--   0        0        0      329 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/plotters/plotter.py
+-rw-r--r--   0        0        0     3862 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/plotters/relaxation.py
+-rw-r--r--   0        0        0     1688 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/plotters/shift.py
+-rw-r--r--   0        0        0        0 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/printers/__init__.py
+-rw-r--r--   0        0        0     4220 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/printers/data.py
+-rw-r--r--   0        0        0     4577 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/printers/parameters.py
+-rw-r--r--   0        0        0     2975 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/printers/plot.py
+-rw-r--r--   0        0        0     2794 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/toml.py
+-rw-r--r--   0        0        0        0 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/tools/__init__.py
+-rw-r--r--   0        0        0       60 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/tools/pick_cest/__init__.py
+-rw-r--r--   0        0        0     6575 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/tools/pick_cest/buttons.py
+-rw-r--r--   0        0        0     3875 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/tools/pick_cest/cest_picker.py
+-rw-r--r--   0        0        0     1496 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/tools/pick_cest/curve.py
+-rw-r--r--   0        0        0     1867 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/tools/plot_param.py
+-rw-r--r--   0        0        0      144 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/typing.py
+-rw-r--r--   0        0        0     3649 2024-05-29 10:48:09.608230 chemex-2024.5.1/chemex/uncertainty.py
+-rw-r--r--   0        0        0     1447 2024-05-29 10:48:12.680220 chemex-2024.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 chemex-2024.5.1/PKG-INFO
```

### Comparing `chemex-2024.5.0/LICENSE.md` & `chemex-2024.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/README.md` & `chemex-2024.5.1/README.md`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/chemex.py` & `chemex-2024.5.1/chemex/chemex.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/cli.py` & `chemex-2024.5.1/chemex/cli.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/configuration/base.py` & `chemex-2024.5.1/chemex/configuration/base.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/configuration/conditions.py` & `chemex-2024.5.1/chemex/configuration/conditions.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/configuration/data.py` & `chemex-2024.5.1/chemex/configuration/data.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/configuration/experiment.py` & `chemex-2024.5.1/chemex/configuration/experiment.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/configuration/methods.py` & `chemex-2024.5.1/chemex/configuration/methods.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/configuration/parameters.py` & `chemex-2024.5.1/chemex/configuration/parameters.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/configuration/utils.py` & `chemex-2024.5.1/chemex/configuration/utils.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/containers/data.py` & `chemex-2024.5.1/chemex/containers/data.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/containers/dataset.py` & `chemex-2024.5.1/chemex/containers/dataset.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/containers/experiment.py` & `chemex-2024.5.1/chemex/containers/experiment.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/containers/experiments.py` & `chemex-2024.5.1/chemex/containers/experiments.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/containers/profile.py` & `chemex-2024.5.1/chemex/containers/profile.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/builder.py` & `chemex-2024.5.1/chemex/experiments/builder.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/cest_13c.py` & `chemex-2024.5.1/chemex/experiments/catalog/cest_13c.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/cest_15n.py` & `chemex-2024.5.1/chemex/experiments/catalog/cest_15n.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/cest_15n_cw.py` & `chemex-2024.5.1/chemex/experiments/catalog/cest_15n_cw.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/cest_15n_tr.py` & `chemex-2024.5.1/chemex/experiments/catalog/cest_15n_tr.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/cest_1hn_ap.py` & `chemex-2024.5.1/chemex/experiments/catalog/cest_1hn_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/cest_1hn_ip_ap.py` & `chemex-2024.5.1/chemex/experiments/catalog/cest_1hn_ip_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/cest_ch3_1h_ip_ap.py` & `chemex-2024.5.1/chemex/experiments/catalog/cest_ch3_1h_ip_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/coscest_13c.py` & `chemex-2024.5.1/chemex/experiments/catalog/coscest_13c.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/coscest_1hn_ip_ap.py` & `chemex-2024.5.1/chemex/experiments/catalog/coscest_1hn_ip_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/cpmg_13c_ip.py` & `chemex-2024.5.1/chemex/experiments/catalog/cpmg_13c_ip.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/cpmg_13co_ap.py` & `chemex-2024.5.1/chemex/experiments/catalog/cpmg_13co_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/cpmg_15n_ip.py` & `chemex-2024.5.1/chemex/experiments/catalog/cpmg_15n_ip.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/cpmg_15n_ip_0013.py` & `chemex-2024.5.1/chemex/experiments/catalog/cpmg_15n_ip_0013.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/cpmg_15n_tr.py` & `chemex-2024.5.1/chemex/experiments/catalog/cpmg_15n_tr.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/cpmg_15n_tr_0013.py` & `chemex-2024.5.1/chemex/experiments/catalog/cpmg_15n_tr_0013.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/cpmg_1hn_ap.py` & `chemex-2024.5.1/chemex/experiments/catalog/cpmg_1hn_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/cpmg_1hn_ap_0013.py` & `chemex-2024.5.1/chemex/experiments/catalog/cpmg_1hn_ap_0013.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/cpmg_ch3_13c_h2c.py` & `chemex-2024.5.1/chemex/experiments/catalog/cpmg_ch3_13c_h2c.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/cpmg_ch3_1h_dq.py` & `chemex-2024.5.1/chemex/experiments/catalog/cpmg_ch3_1h_dq.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/cpmg_ch3_1h_sq.py` & `chemex-2024.5.1/chemex/experiments/catalog/cpmg_ch3_1h_sq.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/cpmg_ch3_1h_tq.py` & `chemex-2024.5.1/chemex/experiments/catalog/cpmg_ch3_1h_tq.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/cpmg_ch3_1h_tq_diff.py` & `chemex-2024.5.1/chemex/experiments/catalog/cpmg_ch3_1h_tq_diff.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/cpmg_ch3_mq.py` & `chemex-2024.5.1/chemex/experiments/catalog/cpmg_ch3_mq.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/cpmg_chd2_1h_ap.py` & `chemex-2024.5.1/chemex/experiments/catalog/cpmg_chd2_1h_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/cpmg_hn_dq_zq.py` & `chemex-2024.5.1/chemex/experiments/catalog/cpmg_hn_dq_zq.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/dcest_13c.py` & `chemex-2024.5.1/chemex/experiments/catalog/dcest_13c.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/dcest_15n.py` & `chemex-2024.5.1/chemex/experiments/catalog/dcest_15n.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/noesyfpgpph19.py` & `chemex-2024.5.1/chemex/experiments/catalog/noesyfpgpph19.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/relaxation_hznz.py` & `chemex-2024.5.1/chemex/experiments/catalog/relaxation_hznz.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/relaxation_nz.py` & `chemex-2024.5.1/chemex/experiments/catalog/relaxation_nz.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/shift_15n_sq.py` & `chemex-2024.5.1/chemex/experiments/catalog/shift_15n_sq.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/catalog/shift_15n_sqmq.py` & `chemex-2024.5.1/chemex/experiments/catalog/shift_15n_sqmq.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/factories.py` & `chemex-2024.5.1/chemex/experiments/factories.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/experiments/loader.py` & `chemex-2024.5.1/chemex/experiments/loader.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/filterers.py` & `chemex-2024.5.1/chemex/filterers.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/messages.py` & `chemex-2024.5.1/chemex/messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 Typical usage example:
 
   from your_module import print_logo, print_loading_experiments
   print_logo()
   print_loading_experiments()
 """
+
 from __future__ import annotations
 
 from collections import Counter
 from pathlib import Path
 
 from pydantic import ValidationError
 from rich import box
@@ -30,15 +31,15 @@
 
 from chemex import __version__
 
 console = Console()
 
 
 LOGO = r"""
-    ________                   ______
+   ________                   ______
   / ____/ /_  ___  ____ ___  / ____/  __
  / /   / __ \/ _ \/ __ `__ \/ __/ | |/_/
 / /___/ / / /  __/ / / / / / /____>  <
 \____/_/ /_/\___/_/ /_/ /_/_____/_/|_|
 
 
 """
```

### Comparing `chemex-2024.5.0/chemex/models/constraints.py` & `chemex-2024.5.1/chemex/models/constraints.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/models/factory.py` & `chemex-2024.5.1/chemex/models/factory.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/models/kinetic/settings_2st.py` & `chemex-2024.5.1/chemex/models/kinetic/settings_2st.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/models/kinetic/settings_2st_binding.py` & `chemex-2024.5.1/chemex/models/kinetic/settings_2st_binding.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/models/kinetic/settings_2st_eyring.py` & `chemex-2024.5.1/chemex/models/kinetic/settings_2st_eyring.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/models/kinetic/settings_2st_hd.py` & `chemex-2024.5.1/chemex/models/kinetic/settings_2st_hd.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/models/kinetic/settings_2st_monomer_dimer.py` & `chemex-2024.5.1/chemex/models/kinetic/settings_2st_monomer_dimer.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/models/kinetic/settings_2st_monomer_tetramer.py` & `chemex-2024.5.1/chemex/models/kinetic/settings_2st_monomer_tetramer.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/models/kinetic/settings_2st_monomer_trimer.py` & `chemex-2024.5.1/chemex/models/kinetic/settings_2st_monomer_trimer.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/models/kinetic/settings_2st_rs.py` & `chemex-2024.5.1/chemex/models/kinetic/settings_2st_rs.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/models/kinetic/settings_3st_binding_2st_partner.py` & `chemex-2024.5.1/chemex/models/kinetic/settings_3st_binding_2st_partner.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/models/kinetic/settings_3st_binding_cs.py` & `chemex-2024.5.1/chemex/models/kinetic/settings_3st_binding_cs.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/models/kinetic/settings_3st_binding_if.py` & `chemex-2024.5.1/chemex/models/kinetic/settings_3st_binding_if.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/models/kinetic/settings_3st_double_binding.py` & `chemex-2024.5.1/chemex/models/kinetic/settings_3st_double_binding.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/models/kinetic/settings_3st_eyring.py` & `chemex-2024.5.1/chemex/models/kinetic/settings_3st_eyring.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/models/kinetic/settings_3st_monomer_dimer_tetramer.py` & `chemex-2024.5.1/chemex/models/kinetic/settings_3st_monomer_dimer_tetramer.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/models/kinetic/settings_3st_monomer_dimer_trimer.py` & `chemex-2024.5.1/chemex/models/kinetic/settings_3st_monomer_dimer_trimer.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/models/kinetic/settings_4st_binding_2st_partner.py` & `chemex-2024.5.1/chemex/models/kinetic/settings_4st_binding_2st_partner.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/models/kinetic/settings_4st_binding_3_bound_states.py` & `chemex-2024.5.1/chemex/models/kinetic/settings_4st_binding_3_bound_states.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/models/kinetic/settings_4st_hd.py` & `chemex-2024.5.1/chemex/models/kinetic/settings_4st_hd.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/models/kinetic/settings_nst.py` & `chemex-2024.5.1/chemex/models/kinetic/settings_nst.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/models/loader.py` & `chemex-2024.5.1/chemex/models/loader.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/models/model.py` & `chemex-2024.5.1/chemex/models/model.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/nmr/basis.py` & `chemex-2024.5.1/chemex/nmr/basis.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/nmr/constants.py` & `chemex-2024.5.1/chemex/nmr/constants.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/nmr/liouvillian.py` & `chemex-2024.5.1/chemex/nmr/liouvillian.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/nmr/rates.py` & `chemex-2024.5.1/chemex/nmr/rates.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/nmr/spectrometer.py` & `chemex-2024.5.1/chemex/nmr/spectrometer.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/optimize/fitting.py` & `chemex-2024.5.1/chemex/optimize/fitting.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/optimize/gridding.py` & `chemex-2024.5.1/chemex/optimize/gridding.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from itertools import combinations, permutations, product
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 import numpy as np
 from lmfit.parameter import Parameters
 from matplotlib.backends.backend_pdf import PdfPages
-from matplotlib.cm import get_cmap
 from matplotlib.colors import LogNorm
+from matplotlib.pyplot import get_cmap
 from rich.progress import track
 
 from chemex.containers.experiments import Experiments
 from chemex.messages import print_group_name, print_running_grid
 from chemex.optimize.grouping import Group, create_groups
 from chemex.optimize.helper import (
     calculate_statistics,
```

### Comparing `chemex-2024.5.0/chemex/optimize/grouping.py` & `chemex-2024.5.1/chemex/optimize/grouping.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/optimize/helper.py` & `chemex-2024.5.1/chemex/optimize/helper.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/optimize/minimizer.py` & `chemex-2024.5.1/chemex/optimize/minimizer.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/parameters/database.py` & `chemex-2024.5.1/chemex/parameters/database.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/parameters/factory.py` & `chemex-2024.5.1/chemex/parameters/factory.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/parameters/name.py` & `chemex-2024.5.1/chemex/parameters/name.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/parameters/setting.py` & `chemex-2024.5.1/chemex/parameters/setting.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/parameters/spin_system/atom.py` & `chemex-2024.5.1/chemex/parameters/spin_system/atom.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/parameters/spin_system/constants.py` & `chemex-2024.5.1/chemex/parameters/spin_system/constants.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/parameters/spin_system/group.py` & `chemex-2024.5.1/chemex/parameters/spin_system/group.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/parameters/spin_system/nucleus.py` & `chemex-2024.5.1/chemex/parameters/spin_system/nucleus.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/parameters/spin_system/spin.py` & `chemex-2024.5.1/chemex/parameters/spin_system/spin.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/parameters/spin_system/spin_system.py` & `chemex-2024.5.1/chemex/parameters/spin_system/spin_system.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/parameters/spin_system/utilities.py` & `chemex-2024.5.1/chemex/parameters/spin_system/utilities.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/parameters/spins.py` & `chemex-2024.5.1/chemex/parameters/spins.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/parameters/userfunctions.py` & `chemex-2024.5.1/chemex/parameters/userfunctions.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/plotters/cest.py` & `chemex-2024.5.1/chemex/plotters/cest.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/plotters/cpmg.py` & `chemex-2024.5.1/chemex/plotters/cpmg.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/plotters/exsy.py` & `chemex-2024.5.1/chemex/plotters/exsy.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/plotters/plot.py` & `chemex-2024.5.1/chemex/plotters/plot.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/plotters/relaxation.py` & `chemex-2024.5.1/chemex/plotters/relaxation.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/plotters/shift.py` & `chemex-2024.5.1/chemex/plotters/shift.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/printers/data.py` & `chemex-2024.5.1/chemex/printers/data.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/printers/parameters.py` & `chemex-2024.5.1/chemex/printers/parameters.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/printers/plot.py` & `chemex-2024.5.1/chemex/printers/plot.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/toml.py` & `chemex-2024.5.1/chemex/toml.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/tools/pick_cest/buttons.py` & `chemex-2024.5.1/chemex/tools/pick_cest/buttons.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/tools/pick_cest/cest_picker.py` & `chemex-2024.5.1/chemex/tools/pick_cest/cest_picker.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/tools/pick_cest/curve.py` & `chemex-2024.5.1/chemex/tools/pick_cest/curve.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/tools/plot_param.py` & `chemex-2024.5.1/chemex/tools/plot_param.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/chemex/uncertainty.py` & `chemex-2024.5.1/chemex/uncertainty.py`

 * *Files identical despite different names*

### Comparing `chemex-2024.5.0/pyproject.toml` & `chemex-2024.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "emcee>=3.1.4",
     "numdifftools>=0.9.41",
     "annotated-types>=0.6.0",
 ]
 requires-python = ">=3.11,<3.13"
 readme = "README.md"
 dynamic = []
-version = "2024.5.0"
+version = "2024.5.1"
 
 [project.license]
 text = "GPL-3.0-or-later"
 
 [project.urls]
 Homepage = "http://gbouvignies.github.io/ChemEx/"
 Documentation = "http://gbouvignies.github.io/ChemEx/"
```

### Comparing `chemex-2024.5.0/PKG-INFO` & `chemex-2024.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemex
-Version: 2024.5.0
+Version: 2024.5.1
 Summary: An analysis program for chemical exchange detected by NMR
 Author-Email: Guillaume Bouvignies <guillaume.bouvignies@ens.psl.eu>
 License: GPL-3.0-or-later
 Project-URL: Homepage, http://gbouvignies.github.io/ChemEx/
 Project-URL: Documentation, http://gbouvignies.github.io/ChemEx/
 Project-URL: Repository, https://github.com/gbouvignies/chemex
 Project-URL: Changelog, https://github.com/gbouvignies/chemex/releases
```

