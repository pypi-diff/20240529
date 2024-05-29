# Comparing `tmp/ecoengine-1.6.3.tar.gz` & `tmp/ecoengine-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoengine-1.6.3.tar", last modified: Thu May 23 23:53:32 2024, max compression
+gzip compressed data, was "ecoengine-1.6.4.tar", last modified: Wed May 29 19:48:53 2024, max compression
```

## Comparing `ecoengine-1.6.3.tar` & `ecoengine-1.6.4.tar`

### file list

```diff
@@ -1,300 +1,300 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.958510 ecoengine-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-23 23:51:43.000000 ecoengine-1.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-23 23:53:32.958510 ecoengine-1.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-23 23:51:43.000000 ecoengine-1.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-23 23:51:43.000000 ecoengine-1.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-23 23:53:32.958510 ecoengine-1.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-23 23:51:43.000000 ecoengine-1.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.866510 ecoengine-1.6.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.866510 ecoengine-1.6.3/src/ecoengine/
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.870509 ecoengine-1.6.3/src/ecoengine/constants/
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/constants/Constants.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.870509 ecoengine-1.6.3/src/ecoengine/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.874509 ecoengine-1.6.3/src/ecoengine/data/climate_data/
--rw-r--r--   0 runner    (1001) docker     (127)  3784790 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/climate_data/DryBulbTemperatures_ByClimateZone.csv
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/climate_data/InletWaterTemperatures_ByClimateZone.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/climate_data/WeatherStation_ClimateZone_Lookup.csv
--rw-r--r--   0 runner    (1001) docker     (127)    22793 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/climate_data/ZipCode_ClimateZone_Lookup.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/climate_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1728735 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/climate_data/kGperkWh_ByClimateZone.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.878509 ecoengine-1.6.3/src/ecoengine/data/load_shapes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/apartment.json
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/elementary_school.json
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/food_service_a.json
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/food_service_b.json
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/junior_high.json
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/mens_dorm.json
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/motel.json
--rw-r--r--   0 runner    (1001) docker     (127)   262011 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/multi_family.json
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/nursing_home.json
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/office_building.json
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/senior_high.json
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/womens_dorm.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.878509 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58109 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/maps.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.954510 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19141 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   374730 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   374730 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19113 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19445 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   387706 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   387706 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19113 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15039 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15039 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18191 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   353846 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   353846 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14787 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14787 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19680 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   387526 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   387526 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18648 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   364494 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   364494 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19558 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   383718 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   383718 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14667 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14667 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19121 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   376446 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   376446 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19272 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   373434 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   373434 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19737 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   383822 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   383822 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18589 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   364226 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   364226 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18505 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   358582 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   358582 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19243 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   374554 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   374554 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18911 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   368874 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   368874 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    17837 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   349178 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   349178 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13935 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13935 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   399586 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   399586 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18580 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   365854 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   365854 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19946 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   390254 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   390254 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18932 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   372098 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   372098 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18228 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   356322 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   356322 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    17964 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   354146 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   354146 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14103 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14103 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18022 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   359030 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   359030 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    21000 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   411666 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   411666 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    21627 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   414014 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   414014 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13698 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   121180 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   121180 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    24604 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    24604 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    26588 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    26588 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_power_in_interpolator.pkl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.958510 ecoengine-1.6.3/src/ecoengine/engine/
--rw-r--r--   0 runner    (1001) docker     (127)    12289 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/engine/BuildingCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)    44309 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/engine/EcosizerEngine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/engine/Simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/engine/SystemCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.958510 ecoengine-1.6.3/src/ecoengine/objects/
--rw-r--r--   0 runner    (1001) docker     (127)    22619 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/Building.py
--rw-r--r--   0 runner    (1001) docker     (127)    30767 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/PrefMapTracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    34828 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/SimulationRun.py
--rw-r--r--   0 runner    (1001) docker     (127)    48946 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/SystemConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/UtilityCostTracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/systemConfigUtils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.958510 ecoengine-1.6.3/src/ecoengine/objects/systems/
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/systems/MultiPass.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/systems/MultiPassRecirc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/systems/ParallelLoopTank.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/systems/PrimaryWithRecirc.py
--rw-r--r--   0 runner    (1001) docker     (127)    26558 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/systems/SwingTank.py
--rw-r--r--   0 runner    (1001) docker     (127)    14033 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/systems/SwingTankER.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/systems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.958510 ecoengine-1.6.3/src/ecoengine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-23 23:53:32.000000 ecoengine-1.6.3/src/ecoengine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23016 2024-05-23 23:53:32.000000 ecoengine-1.6.3/src/ecoengine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 23:53:32.000000 ecoengine-1.6.3/src/ecoengine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-23 23:53:32.000000 ecoengine-1.6.3/src/ecoengine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 23:53:32.000000 ecoengine-1.6.3/src/ecoengine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:48:53.258673 ecoengine-1.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-29 19:47:02.000000 ecoengine-1.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-29 19:48:53.258673 ecoengine-1.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-29 19:47:02.000000 ecoengine-1.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-29 19:47:02.000000 ecoengine-1.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-29 19:48:53.258673 ecoengine-1.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-29 19:47:02.000000 ecoengine-1.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:48:53.162673 ecoengine-1.6.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:48:53.166673 ecoengine-1.6.4/src/ecoengine/
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:48:53.166673 ecoengine-1.6.4/src/ecoengine/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/constants/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:48:53.166673 ecoengine-1.6.4/src/ecoengine/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:48:53.174673 ecoengine-1.6.4/src/ecoengine/data/climate_data/
+-rw-r--r--   0 runner    (1001) docker     (127)  3784790 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/climate_data/DryBulbTemperatures_ByClimateZone.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/climate_data/InletWaterTemperatures_ByClimateZone.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/climate_data/WeatherStation_ClimateZone_Lookup.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    22793 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/climate_data/ZipCode_ClimateZone_Lookup.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/climate_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1728735 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/climate_data/kGperkWh_ByClimateZone.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:48:53.178673 ecoengine-1.6.4/src/ecoengine/data/load_shapes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/load_shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/load_shapes/apartment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/load_shapes/elementary_school.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/load_shapes/food_service_a.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/load_shapes/food_service_b.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/load_shapes/junior_high.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/load_shapes/mens_dorm.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/load_shapes/motel.json
+-rw-r--r--   0 runner    (1001) docker     (127)   262011 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/load_shapes/multi_family.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/load_shapes/nursing_home.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/load_shapes/office_building.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/load_shapes/senior_high.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/load_shapes/womens_dorm.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:48:53.178673 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58109 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/maps.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:48:53.254673 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19141 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   374730 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   374730 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19113 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19445 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   387706 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   387706 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19113 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15039 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15039 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18191 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   353846 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   353846 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14787 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14787 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19680 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   387526 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   387526 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18648 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   364494 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   364494 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19558 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   383718 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   383718 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14667 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14667 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19121 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   376446 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   376446 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19272 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   373434 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   373434 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19737 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   383822 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   383822 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18589 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   364226 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   364226 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18505 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   358582 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   358582 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19243 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   374554 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   374554 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18911 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   368874 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   368874 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    17837 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   349178 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   349178 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13935 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13935 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   399586 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   399586 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18580 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   365854 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   365854 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19946 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   390254 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   390254 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18932 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   372098 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   372098 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18228 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   356322 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   356322 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    17964 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   354146 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   354146 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14103 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14103 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18022 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   359030 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   359030 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    21000 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   411666 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   411666 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    21627 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   414014 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   414014 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13698 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   121180 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   121180 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    24604 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    24604 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    26588 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    26588 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_power_in_interpolator.pkl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:48:53.254673 ecoengine-1.6.4/src/ecoengine/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)    12289 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/engine/BuildingCreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44309 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/engine/EcosizerEngine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/engine/Simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/engine/SystemCreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:48:53.258673 ecoengine-1.6.4/src/ecoengine/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)    22619 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/objects/Building.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30767 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/objects/PrefMapTracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34828 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/objects/SimulationRun.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48946 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/objects/SystemConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/objects/UtilityCostTracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/objects/systemConfigUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:48:53.258673 ecoengine-1.6.4/src/ecoengine/objects/systems/
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/objects/systems/MultiPass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/objects/systems/MultiPassRecirc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/objects/systems/ParallelLoopTank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/objects/systems/PrimaryWithRecirc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26558 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/objects/systems/SwingTank.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11825 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/objects/systems/SwingTankER.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:47:02.000000 ecoengine-1.6.4/src/ecoengine/objects/systems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:48:53.258673 ecoengine-1.6.4/src/ecoengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-29 19:48:53.000000 ecoengine-1.6.4/src/ecoengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23016 2024-05-29 19:48:53.000000 ecoengine-1.6.4/src/ecoengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 19:48:53.000000 ecoengine-1.6.4/src/ecoengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 19:48:53.000000 ecoengine-1.6.4/src/ecoengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 19:48:53.000000 ecoengine-1.6.4/src/ecoengine.egg-info/top_level.txt
```

### Comparing `ecoengine-1.6.3/PKG-INFO` & `ecoengine-1.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoengine
-Version: 1.6.3
+Version: 1.6.4
 Summary: A software for sizing Heat Pump Water Heaters for buildings
 Home-page: https://ecosizer.ecotope.com/sizer/
 Author: Nolan
 Author-email: nolan@ecotope.com
 Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecoengine-1.6.3/README.md` & `ecoengine-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/setup.cfg` & `ecoengine-1.6.4/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ecoengine
-version = 1.6.3
+version = 1.6.4
 author = Nolan
 author_email = nolan@ecotope.com
 description = A software for sizing Heat Pump Water Heaters for buildings
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://ecosizer.ecotope.com/sizer/
 project_urls =
```

### Comparing `ecoengine-1.6.3/src/ecoengine/__init__.py` & `ecoengine-1.6.4/src/ecoengine/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/constants/Constants.py` & `ecoengine-1.6.4/src/ecoengine/constants/Constants.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/climate_data/DryBulbTemperatures_ByClimateZone.csv` & `ecoengine-1.6.4/src/ecoengine/data/climate_data/DryBulbTemperatures_ByClimateZone.csv`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/climate_data/InletWaterTemperatures_ByClimateZone.csv` & `ecoengine-1.6.4/src/ecoengine/data/climate_data/InletWaterTemperatures_ByClimateZone.csv`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/climate_data/WeatherStation_ClimateZone_Lookup.csv` & `ecoengine-1.6.4/src/ecoengine/data/climate_data/WeatherStation_ClimateZone_Lookup.csv`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/climate_data/ZipCode_ClimateZone_Lookup.csv` & `ecoengine-1.6.4/src/ecoengine/data/climate_data/ZipCode_ClimateZone_Lookup.csv`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/climate_data/kGperkWh_ByClimateZone.csv` & `ecoengine-1.6.4/src/ecoengine/data/climate_data/kGperkWh_ByClimateZone.csv`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/load_shapes/apartment.json` & `ecoengine-1.6.4/src/ecoengine/data/load_shapes/apartment.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/load_shapes/elementary_school.json` & `ecoengine-1.6.4/src/ecoengine/data/load_shapes/elementary_school.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/load_shapes/food_service_a.json` & `ecoengine-1.6.4/src/ecoengine/data/load_shapes/food_service_a.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/load_shapes/food_service_b.json` & `ecoengine-1.6.4/src/ecoengine/data/load_shapes/food_service_b.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/load_shapes/junior_high.json` & `ecoengine-1.6.4/src/ecoengine/data/load_shapes/junior_high.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/load_shapes/mens_dorm.json` & `ecoengine-1.6.4/src/ecoengine/data/load_shapes/mens_dorm.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/load_shapes/motel.json` & `ecoengine-1.6.4/src/ecoengine/data/load_shapes/motel.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/load_shapes/multi_family.json` & `ecoengine-1.6.4/src/ecoengine/data/load_shapes/multi_family.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/load_shapes/nursing_home.json` & `ecoengine-1.6.4/src/ecoengine/data/load_shapes/nursing_home.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/load_shapes/office_building.json` & `ecoengine-1.6.4/src/ecoengine/data/load_shapes/office_building.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/load_shapes/senior_high.json` & `ecoengine-1.6.4/src/ecoengine/data/load_shapes/senior_high.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/load_shapes/womens_dorm.json` & `ecoengine-1.6.4/src/ecoengine/data/load_shapes/womens_dorm.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/maps.json` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/maps.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_bounds.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_capacity_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_power_in_interpolator.pkl` & `ecoengine-1.6.4/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/engine/BuildingCreator.py` & `ecoengine-1.6.4/src/ecoengine/engine/BuildingCreator.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/engine/EcosizerEngine.py` & `ecoengine-1.6.4/src/ecoengine/engine/EcosizerEngine.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/engine/Simulator.py` & `ecoengine-1.6.4/src/ecoengine/engine/Simulator.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/engine/SystemCreator.py` & `ecoengine-1.6.4/src/ecoengine/engine/SystemCreator.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/engine/__init__.py` & `ecoengine-1.6.4/src/ecoengine/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/objects/Building.py` & `ecoengine-1.6.4/src/ecoengine/objects/Building.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/objects/PrefMapTracker.py` & `ecoengine-1.6.4/src/ecoengine/objects/PrefMapTracker.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/objects/SimulationRun.py` & `ecoengine-1.6.4/src/ecoengine/objects/SimulationRun.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/objects/SystemConfig.py` & `ecoengine-1.6.4/src/ecoengine/objects/SystemConfig.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/objects/UtilityCostTracker.py` & `ecoengine-1.6.4/src/ecoengine/objects/UtilityCostTracker.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/objects/__init__.py` & `ecoengine-1.6.4/src/ecoengine/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/objects/systemConfigUtils.py` & `ecoengine-1.6.4/src/ecoengine/objects/systemConfigUtils.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/objects/systems/MultiPass.py` & `ecoengine-1.6.4/src/ecoengine/objects/systems/MultiPass.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/objects/systems/MultiPassRecirc.py` & `ecoengine-1.6.4/src/ecoengine/objects/systems/MultiPassRecirc.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/objects/systems/ParallelLoopTank.py` & `ecoengine-1.6.4/src/ecoengine/objects/systems/ParallelLoopTank.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/objects/systems/PrimaryWithRecirc.py` & `ecoengine-1.6.4/src/ecoengine/objects/systems/PrimaryWithRecirc.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/objects/systems/SwingTank.py` & `ecoengine-1.6.4/src/ecoengine/objects/systems/SwingTank.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.3/src/ecoengine/objects/systems/SwingTankER.py` & `ecoengine-1.6.4/src/ecoengine/objects/systems/SwingTankER.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,37 +63,14 @@
 
         self.TMCap_kBTUhr = self.original_TMCap_kBTUhr + (((self.TMVol_G * (60/minuteIntervals) * rhoCp * (max(tempDeficit))) / 1000.) * saftey_factor)
         # set performance map back to its original form
         self.perfMap = perfMap_holder
         self.resetToDefaultCapacity()
         return self.TMCap_kBTUhr
 
-    def _findNextIndexOfHWDeficit(self, simRun : SimulationRun, i):
-        incomingWater_T = simRun.building.getDesignInlet()
-        while i < len(simRun.hwDemand):
-            if simRun.pV[i-1] >= 0:
-                # The following is esentially the normal swing tank runOneSystemStep() execpt uses design IWT instead of the climate-informed one
-                # there is already no preSystemStepSetUp() because simulation is very basic
-                simRun.hw_outSwing[i] = convertVolume(simRun.hwDemand[i], simRun.tmT_F[i-1], incomingWater_T, simRun.building.supplyT_F)    
-                simRun.tmheating, simRun.tmT_F[i], simRun.tmRun[i] = self._runOneSwingStep(simRun.building, 
-                    simRun.tmheating, simRun.tmT_F[i-1], simRun.hw_outSwing[i], self.storageT_F, minuteIntervals = simRun.minuteIntervals, erCalc = True)
-                mixedGHW = convertVolume(simRun.hwGenRate, self.storageT_F, incomingWater_T, simRun.building.supplyT_F)
-                simRun.pheating, simRun.pV[i], simRun.pGen[i], simRun.pRun[i] = self.runOnePrimaryStep(pheating = simRun.pheating,
-                                                                                                        Vcurr = simRun.pV[i-1], 
-                                                                                                        hw_out = simRun.hw_outSwing[i], 
-                                                                                                        hw_in = mixedGHW, 
-                                                                                                        mode = simRun.getLoadShiftMode(i),
-                                                                                                        modeChanged = (simRun.getLoadShiftMode(i) != simRun.getLoadShiftMode(i-1)),
-                                                                                                        minuteIntervals = simRun.minuteIntervals,
-                                                                                                        erCalc = True)
-            else:
-                return i-1
-            i += 1
-        return i
-
     def runOneSystemStep(self, simRun : SimulationRun, i, minuteIntervals = 1, oat = None, erCalc=False):
         incomingWater_T = simRun.getIncomingWaterT(i)
         self.preSystemStepSetUp(simRun, i, incomingWater_T + 15.0, minuteIntervals, oat) # CHPWH IWT is assumed 15°F (adjustable) warmer than DCW temperature on average, based on lab test data. 
 
         # aquire draw amount for time step
         last_temp = simRun.tmT_F[i-1]
         simRun.hw_outSwing[i] = convertVolume(simRun.hwDemand[i], last_temp, incomingWater_T, simRun.building.supplyT_F)
@@ -160,17 +137,17 @@
                 building.magnitude = original_magnitude * fract
                 er_cap_kBTUhr = self.sizeERElement(building, additionalERSaftey, 1)
             er_cap_kW.append(round(er_cap_kBTUhr/W_TO_BTUHR,0))
             fract_covered.append(i)
             i -= 10
 
         # reverse the lists because they are backwards:
-        # fract_covered.reverse()
-        # er_cap_kW.reverse()
-        # startind = (len(fract_covered)-1)-startind
+        fract_covered.reverse()
+        er_cap_kW.reverse()
+        startind = (len(fract_covered)-1)-startind
 
         building.magnitude = original_magnitude
         self.TMCap_kBTUhr = original_erSize_kBTUhr
         return [er_cap_kW, fract_covered, startind] # TODO edge cases around start index
     
     
     def getERCurveAndSlider(self, x, y, startind, returnAsDiv = True):
@@ -197,31 +174,31 @@
         """
         fig = createERSizingCurvePlot(x, y, startind)
     
         # Create and add sliderbar steps
         steps = []
         for i in range(1,len(fig.data)):
         
-            labelText = "Percent Coverage: <b id='point_x'>" + str(float(x[len(fig.data)-i-1])) + "</b> %, Electric Resistance Heating Capacity: <b id='point_y'>" + \
-                str(round(y[len(fig.data)-i-1],1)) + "</b> kW" 
+            labelText = "Percent Coverage: <b id='point_x'>" + str(float(x[i-1])) + "</b> %, Electric Resistance Heating Capacity: <b id='point_y'>" + \
+                str(round(y[i-1],1)) + "</b> kW" 
         
             step = dict(
                 # this value must match the values in x = loads(form['x_data']) #json loads
                 label = labelText,
                 method="update",
                 args=[{"visible": [False] * len(fig.data)},
                     ],  # layout attribute
             )
             step["args"][0]["visible"][0] = True  # Make sure first trace is visible since its the line
-            step["args"][0]["visible"][len(fig.data)-i] = True  # Toggle i'th trace to "visible"
+            step["args"][0]["visible"][i] = True  # Toggle i'th trace to "visible"
             steps.append(step)
 
         sliders = [dict(    
             steps=steps,
-            active=len(x)-startind-1,
+            active=startind,
             currentvalue=dict({
                 'font': {'size': 16},
                 'prefix': '<b>Electric Resistance Size</b> ',
                 'visible': True,
                 'xanchor': 'left'
                 }), 
             pad={"t": 50},
```

### Comparing `ecoengine-1.6.3/src/ecoengine.egg-info/PKG-INFO` & `ecoengine-1.6.4/src/ecoengine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoengine
-Version: 1.6.3
+Version: 1.6.4
 Summary: A software for sizing Heat Pump Water Heaters for buildings
 Home-page: https://ecosizer.ecotope.com/sizer/
 Author: Nolan
 Author-email: nolan@ecotope.com
 Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecoengine-1.6.3/src/ecoengine.egg-info/SOURCES.txt` & `ecoengine-1.6.4/src/ecoengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

