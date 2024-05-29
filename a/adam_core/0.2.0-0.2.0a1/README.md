# Comparing `tmp/adam_core-0.2.0.tar.gz` & `tmp/adam_core-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adam_core-0.2.0.tar", last modified: Wed May 29 14:48:57 2024, max compression
+gzip compressed data, was "adam_core-0.2.0a1.tar", last modified: Tue May 28 18:15:50 2024, max compression
```

## Comparing `adam_core-0.2.0.tar` & `adam_core-0.2.0a1.tar`

### file list

```diff
@@ -1,187 +1,187 @@
--rw-r--r--   0        0        0     2782 2024-05-28 17:05:15.871265 adam_core-0.2.0/LICENSE.md
--rw-r--r--   0        0        0    12438 2024-05-29 13:21:17.950452 adam_core-0.2.0/README.md
--rw-r--r--   0        0        0     2949 2024-05-29 14:48:57.387395 adam_core-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       93 2024-05-28 17:06:44.754921 adam_core-0.2.0/src/adam_core/__init__.py
--rw-r--r--   0        0        0       21 2024-05-29 14:48:57.377458 adam_core-0.2.0/src/adam_core/_version.py
--rw-r--r--   0        0        0     1377 2024-05-28 17:06:44.755022 adam_core-0.2.0/src/adam_core/constants.py
--rw-r--r--   0        0        0      396 2024-05-28 17:06:44.755170 adam_core-0.2.0/src/adam_core/coordinates/__init__.py
--rw-r--r--   0        0        0    10810 2024-05-28 17:06:44.755290 adam_core-0.2.0/src/adam_core/coordinates/cartesian.py
--rw-r--r--   0        0        0    10202 2024-05-28 17:06:44.755414 adam_core-0.2.0/src/adam_core/coordinates/cometary.py
--rw-r--r--   0        0        0     6505 2024-05-28 17:06:44.755532 adam_core-0.2.0/src/adam_core/coordinates/conversions.py
--rw-r--r--   0        0        0    14285 2024-05-28 17:06:44.755677 adam_core-0.2.0/src/adam_core/coordinates/covariances.py
--rw-r--r--   0        0        0     2634 2024-05-28 17:06:44.755755 adam_core-0.2.0/src/adam_core/coordinates/jacobian.py
--rw-r--r--   0        0        0     9250 2024-05-28 17:06:44.755872 adam_core-0.2.0/src/adam_core/coordinates/keplerian.py
--rw-r--r--   0        0        0     4194 2024-05-28 17:06:44.755988 adam_core-0.2.0/src/adam_core/coordinates/origin.py
--rw-r--r--   0        0        0    16741 2024-05-28 17:06:44.756119 adam_core-0.2.0/src/adam_core/coordinates/residuals.py
--rw-r--r--   0        0        0     7681 2024-05-28 17:06:44.756311 adam_core-0.2.0/src/adam_core/coordinates/spherical.py
--rw-r--r--   0        0        0        0 2024-05-28 17:06:44.756376 adam_core-0.2.0/src/adam_core/coordinates/tests/__init__.py
--rw-r--r--   0        0        0     1211 2024-05-28 17:06:44.756514 adam_core-0.2.0/src/adam_core/coordinates/tests/conftest.py
--rw-r--r--   0        0        0     2327 2024-05-28 17:06:44.756610 adam_core-0.2.0/src/adam_core/coordinates/tests/test_benchmarks.py
--rw-r--r--   0        0        0     6568 2024-05-28 17:06:44.756722 adam_core-0.2.0/src/adam_core/coordinates/tests/test_cartesian.py
--rw-r--r--   0        0        0     5367 2024-05-28 17:06:44.756850 adam_core-0.2.0/src/adam_core/coordinates/tests/test_cometary.py
--rw-r--r--   0        0        0     6052 2024-05-28 17:06:44.757031 adam_core-0.2.0/src/adam_core/coordinates/tests/test_covariances.py
--rw-r--r--   0        0        0     5444 2024-05-28 17:06:44.757227 adam_core-0.2.0/src/adam_core/coordinates/tests/test_keplerian.py
--rw-r--r--   0        0        0     2948 2024-05-28 17:06:44.757314 adam_core-0.2.0/src/adam_core/coordinates/tests/test_origin.py
--rw-r--r--   0        0        0    34081 2024-05-28 17:06:44.757510 adam_core-0.2.0/src/adam_core/coordinates/tests/test_residuals.py
--rw-r--r--   0        0        0     1918 2024-05-28 17:06:44.757618 adam_core-0.2.0/src/adam_core/coordinates/tests/test_spherical.py
--rw-r--r--   0        0        0     7646 2024-05-28 17:06:44.759302 adam_core-0.2.0/src/adam_core/coordinates/tests/test_transforms_cometary.py
--rw-r--r--   0        0        0    10063 2024-05-28 17:06:44.759458 adam_core-0.2.0/src/adam_core/coordinates/tests/test_transforms_keplerian.py
--rw-r--r--   0        0        0     4866 2024-05-28 17:06:44.759616 adam_core-0.2.0/src/adam_core/coordinates/tests/test_transforms_rotation.py
--rw-r--r--   0        0        0     3243 2024-05-28 17:06:44.759769 adam_core-0.2.0/src/adam_core/coordinates/tests/test_transforms_spherical.py
--rw-r--r--   0        0        0    11020 2024-05-28 17:06:44.759897 adam_core-0.2.0/src/adam_core/coordinates/tests/test_transforms_spice.py
--rw-r--r--   0        0        0     8044 2024-05-28 17:06:44.760004 adam_core-0.2.0/src/adam_core/coordinates/tests/test_transforms_translation.py
--rw-r--r--   0        0        0    49595 2024-05-28 17:06:44.760222 adam_core-0.2.0/src/adam_core/coordinates/transform.py
--rw-r--r--   0        0        0      691 2024-05-28 17:06:44.760362 adam_core-0.2.0/src/adam_core/coordinates/types.py
--rw-r--r--   0        0        0     6647 2024-05-28 17:06:44.760507 adam_core-0.2.0/src/adam_core/coordinates/variants.py
--rw-r--r--   0        0        0      110 2024-05-28 17:06:44.760609 adam_core-0.2.0/src/adam_core/dynamics/__init__.py
--rw-r--r--   0        0        0   218508 2022-12-23 16:41:41.356795 adam_core-0.2.0/src/adam_core/dynamics/__pycache__/aberrations.add_light_time-15.py310.1.nbc
--rw-r--r--   0        0        0     1014 2022-12-23 16:41:41.347089 adam_core-0.2.0/src/adam_core/dynamics/__pycache__/aberrations.add_light_time-15.py310.nbi
--rw-r--r--   0        0        0   105441 2022-12-23 16:41:42.665228 adam_core-0.2.0/src/adam_core/dynamics/__pycache__/aberrations.add_stellar_aberration-86.py310.1.nbc
--rw-r--r--   0        0        0      983 2022-12-23 16:41:42.645978 adam_core-0.2.0/src/adam_core/dynamics/__pycache__/aberrations.add_stellar_aberration-86.py310.nbi
--rw-r--r--   0        0        0    76611 2022-12-23 16:41:30.071415 adam_core-0.2.0/src/adam_core/dynamics/__pycache__/chi.calc_chi-13.py310.1.nbc
--rw-r--r--   0        0        0      981 2022-12-23 16:41:30.059411 adam_core-0.2.0/src/adam_core/dynamics/__pycache__/chi.calc_chi-13.py310.nbi
--rw-r--r--   0        0        0    49303 2022-12-23 16:41:31.578450 adam_core-0.2.0/src/adam_core/dynamics/__pycache__/lagrange.apply_lagrange_coefficients-92.py310.1.nbc
--rw-r--r--   0        0        0     1008 2022-12-23 16:41:31.568284 adam_core-0.2.0/src/adam_core/dynamics/__pycache__/lagrange.apply_lagrange_coefficients-92.py310.nbi
--rw-r--r--   0        0        0    98285 2022-12-23 16:41:31.179470 adam_core-0.2.0/src/adam_core/dynamics/__pycache__/lagrange.calc_lagrange_coefficients-14.py310.1.nbc
--rw-r--r--   0        0        0     1034 2022-12-23 16:41:31.167530 adam_core-0.2.0/src/adam_core/dynamics/__pycache__/lagrange.calc_lagrange_coefficients-14.py310.nbi
--rw-r--r--   0        0        0    82910 2022-12-23 16:41:32.415608 adam_core-0.2.0/src/adam_core/dynamics/__pycache__/state_transition._calc_M_matrix-15.py310.1.nbc
--rw-r--r--   0        0        0     1022 2022-12-23 16:41:32.397995 adam_core-0.2.0/src/adam_core/dynamics/__pycache__/state_transition._calc_M_matrix-15.py310.nbi
--rw-r--r--   0        0        0   276594 2022-12-23 16:41:37.239361 adam_core-0.2.0/src/adam_core/dynamics/__pycache__/state_transition.calc_state_transition_matrix-112.py310.1.nbc
--rw-r--r--   0        0        0     1000 2022-12-23 16:41:37.220517 adam_core-0.2.0/src/adam_core/dynamics/__pycache__/state_transition.calc_state_transition_matrix-112.py310.nbi
--rw-r--r--   0        0        0    29452 2022-12-23 16:41:27.944024 adam_core-0.2.0/src/adam_core/dynamics/__pycache__/stumpff.calc_stumpff-8.py310.1.nbc
--rw-r--r--   0        0        0      962 2022-12-23 16:41:27.932619 adam_core-0.2.0/src/adam_core/dynamics/__pycache__/stumpff.calc_stumpff-8.py310.nbi
--rw-r--r--   0        0        0   156824 2022-12-23 16:41:38.691950 adam_core-0.2.0/src/adam_core/dynamics/__pycache__/universal_propagate.propagate_universal-14.py310.1.nbc
--rw-r--r--   0        0        0     1005 2022-12-23 16:41:38.679195 adam_core-0.2.0/src/adam_core/dynamics/__pycache__/universal_propagate.propagate_universal-14.py310.nbi
--rw-r--r--   0        0        0     6601 2024-05-28 17:06:44.760697 adam_core-0.2.0/src/adam_core/dynamics/aberrations.py
--rw-r--r--   0        0        0      780 2024-05-28 17:06:44.761711 adam_core-0.2.0/src/adam_core/dynamics/barker.py
--rw-r--r--   0        0        0     3387 2024-05-28 17:06:44.761806 adam_core-0.2.0/src/adam_core/dynamics/chi.py
--rw-r--r--   0        0        0    10553 2024-05-28 17:06:44.761912 adam_core-0.2.0/src/adam_core/dynamics/ephemeris.py
--rw-r--r--   0        0        0     9796 2024-05-28 17:06:44.762068 adam_core-0.2.0/src/adam_core/dynamics/impacts.py
--rw-r--r--   0        0        0     7728 2024-05-28 17:06:44.762231 adam_core-0.2.0/src/adam_core/dynamics/kepler.py
--rw-r--r--   0        0        0     3747 2024-05-28 17:06:44.762306 adam_core-0.2.0/src/adam_core/dynamics/lagrange.py
--rw-r--r--   0        0        0     5212 2024-05-28 17:06:44.762584 adam_core-0.2.0/src/adam_core/dynamics/moid.py
--rw-r--r--   0        0        0     5614 2024-05-28 17:06:44.762865 adam_core-0.2.0/src/adam_core/dynamics/propagation.py
--rw-r--r--   0        0        0     2250 2024-05-28 17:06:44.762960 adam_core-0.2.0/src/adam_core/dynamics/stumpff.py
--rw-r--r--   0        0        0        0 2024-05-28 17:06:44.763001 adam_core-0.2.0/src/adam_core/dynamics/tests/__init__.py
--rw-r--r--   0        0        0     1115 2024-05-28 17:06:44.763131 adam_core-0.2.0/src/adam_core/dynamics/tests/conftest.py
--rw-r--r--   0        0        0     5413 2024-05-28 17:06:44.763230 adam_core-0.2.0/src/adam_core/dynamics/tests/test_ephemeris.py
--rw-r--r--   0        0        0     7108 2024-05-28 17:06:44.763477 adam_core-0.2.0/src/adam_core/dynamics/tests/test_impacts.py
--rw-r--r--   0        0        0     8775 2024-05-28 17:06:44.763611 adam_core-0.2.0/src/adam_core/dynamics/tests/test_kepler.py
--rw-r--r--   0        0        0     5555 2024-05-28 17:06:44.763838 adam_core-0.2.0/src/adam_core/dynamics/tests/test_moid.py
--rw-r--r--   0        0        0    16189 2024-05-28 17:06:44.763985 adam_core-0.2.0/src/adam_core/dynamics/tests/test_propagation.py
--rw-r--r--   0        0        0     1311 2024-05-28 17:06:44.764071 adam_core-0.2.0/src/adam_core/dynamics/tests/test_tisserand.py
--rw-r--r--   0        0        0     1953 2024-05-28 17:06:44.764170 adam_core-0.2.0/src/adam_core/dynamics/tisserand.py
--rw-r--r--   0        0        0      316 2024-05-28 17:06:44.764241 adam_core-0.2.0/src/adam_core/observations/__init__.py
--rw-r--r--   0        0        0     2086 2024-05-28 17:06:44.764347 adam_core-0.2.0/src/adam_core/observations/associations.py
--rw-r--r--   0        0        0     2616 2024-05-28 17:06:44.764474 adam_core-0.2.0/src/adam_core/observations/detections.py
--rw-r--r--   0        0        0     2578 2024-05-28 17:06:44.764600 adam_core-0.2.0/src/adam_core/observations/exposures.py
--rw-r--r--   0        0        0        0 2024-05-28 17:06:44.764638 adam_core-0.2.0/src/adam_core/observations/tests/__init__.py
--rw-r--r--   0        0        0     1582 2024-05-28 17:06:44.764744 adam_core-0.2.0/src/adam_core/observations/tests/test_associations.py
--rw-r--r--   0        0        0     3349 2024-05-28 17:06:44.764818 adam_core-0.2.0/src/adam_core/observations/tests/test_detections.py
--rw-r--r--   0        0        0     3623 2024-05-28 17:06:44.764947 adam_core-0.2.0/src/adam_core/observations/tests/test_exposures.py
--rw-r--r--   0        0        0      139 2024-05-28 17:06:44.765039 adam_core-0.2.0/src/adam_core/observers/__init__.py
--rw-r--r--   0        0        0     3703 2024-05-28 17:06:44.765147 adam_core-0.2.0/src/adam_core/observers/observers.py
--rw-r--r--   0        0        0     6357 2024-05-28 17:06:44.765242 adam_core-0.2.0/src/adam_core/observers/state.py
--rw-r--r--   0        0        0        0 2024-05-28 17:06:44.765286 adam_core-0.2.0/src/adam_core/observers/tests/__init__.py
--rw-r--r--   0        0        0     1339 2024-05-28 17:06:44.765452 adam_core-0.2.0/src/adam_core/observers/tests/test_benchmarks.py
--rw-r--r--   0        0        0     3141 2024-05-28 17:06:44.765577 adam_core-0.2.0/src/adam_core/observers/tests/test_state.py
--rw-r--r--   0        0        0    26467 2024-05-28 17:06:44.765793 adam_core-0.2.0/src/adam_core/observers/tests/testdata/000_ssb.parquet
--rw-r--r--   0        0        0    26327 2024-05-28 17:06:44.765999 adam_core-0.2.0/src/adam_core/observers/tests/testdata/000_sun.parquet
--rw-r--r--   0        0        0    26467 2024-05-28 17:06:44.766172 adam_core-0.2.0/src/adam_core/observers/tests/testdata/500_ssb.parquet
--rw-r--r--   0        0        0    26327 2024-05-28 17:06:44.766349 adam_core-0.2.0/src/adam_core/observers/tests/testdata/500_sun.parquet
--rw-r--r--   0        0        0    26467 2024-05-28 17:06:44.766573 adam_core-0.2.0/src/adam_core/observers/tests/testdata/F51_ssb.parquet
--rw-r--r--   0        0        0    26327 2024-05-28 17:06:44.766750 adam_core-0.2.0/src/adam_core/observers/tests/testdata/F51_sun.parquet
--rw-r--r--   0        0        0    26467 2024-05-28 17:06:44.766928 adam_core-0.2.0/src/adam_core/observers/tests/testdata/I41_ssb.parquet
--rw-r--r--   0        0        0    26327 2024-05-28 17:06:44.767125 adam_core-0.2.0/src/adam_core/observers/tests/testdata/I41_sun.parquet
--rw-r--r--   0        0        0     1638 2024-05-28 17:06:44.767218 adam_core-0.2.0/src/adam_core/observers/tests/testdata/README.md
--rw-r--r--   0        0        0    26467 2024-05-28 17:06:44.767391 adam_core-0.2.0/src/adam_core/observers/tests/testdata/W84_ssb.parquet
--rw-r--r--   0        0        0    26327 2024-05-28 17:06:44.767550 adam_core-0.2.0/src/adam_core/observers/tests/testdata/W84_sun.parquet
--rw-r--r--   0        0        0    26467 2024-05-28 17:06:44.767718 adam_core-0.2.0/src/adam_core/observers/tests/testdata/X05_ssb.parquet
--rw-r--r--   0        0        0    26327 2024-05-28 17:06:44.767896 adam_core-0.2.0/src/adam_core/observers/tests/testdata/X05_sun.parquet
--rw-r--r--   0        0        0     1475 2024-05-28 17:06:44.767981 adam_core-0.2.0/src/adam_core/observers/tests/testdata/get_states.py
--rw-r--r--   0        0        0      266 2024-05-28 17:06:44.768062 adam_core-0.2.0/src/adam_core/orbit_determination/__init__.py
--rw-r--r--   0        0        0     7438 2024-05-28 17:06:44.768223 adam_core-0.2.0/src/adam_core/orbit_determination/differential_correction.py
--rw-r--r--   0        0        0     5219 2024-05-28 17:06:44.768382 adam_core-0.2.0/src/adam_core/orbit_determination/evaluate.py
--rw-r--r--   0        0        0     1310 2024-05-28 17:06:44.768466 adam_core-0.2.0/src/adam_core/orbit_determination/fitted_orbits.py
--rw-r--r--   0        0        0     2420 2024-05-28 17:06:44.768559 adam_core-0.2.0/src/adam_core/orbit_determination/outliers.py
--rw-r--r--   0        0        0        0 2024-05-28 17:06:44.768598 adam_core-0.2.0/src/adam_core/orbit_determination/tests/__init__.py
--rw-r--r--   0        0        0      810 2024-05-28 17:06:44.768716 adam_core-0.2.0/src/adam_core/orbit_determination/tests/conftest.py
--rw-r--r--   0        0        0     8261 2024-05-28 17:06:44.768898 adam_core-0.2.0/src/adam_core/orbit_determination/tests/data/pure_iod_orbit.parquet
--rw-r--r--   0        0        0     3659 2024-05-28 17:06:44.769010 adam_core-0.2.0/src/adam_core/orbit_determination/tests/data/pure_iod_orbit_members.parquet
--rw-r--r--   0        0        0    16284 2024-05-28 17:06:44.769171 adam_core-0.2.0/src/adam_core/orbit_determination/tests/data/pure_iod_orbit_observations.parquet
--rw-r--r--   0        0        0     1081 2024-05-29 13:18:47.023785 adam_core-0.2.0/src/adam_core/orbit_determination/tests/test_differential_correction.py
--rw-r--r--   0        0        0     4512 2024-05-29 13:18:47.024136 adam_core-0.2.0/src/adam_core/orbit_determination/tests/test_evaluate.py
--rw-r--r--   0        0        0     6049 2024-05-28 17:06:44.770121 adam_core-0.2.0/src/adam_core/orbit_determination/tests/test_outliers.py
--rw-r--r--   0        0        0      275 2024-05-28 17:06:44.770264 adam_core-0.2.0/src/adam_core/orbits/__init__.py
--rw-r--r--   0        0        0     2111 2024-05-28 17:06:44.770355 adam_core-0.2.0/src/adam_core/orbits/classification.py
--rw-r--r--   0        0        0     4294 2024-05-28 17:06:44.770496 adam_core-0.2.0/src/adam_core/orbits/ephemeris.py
--rw-r--r--   0        0        0     1381 2024-05-28 17:06:44.770648 adam_core-0.2.0/src/adam_core/orbits/orbits.py
--rw-r--r--   0        0        0       87 2024-05-28 17:06:44.770738 adam_core-0.2.0/src/adam_core/orbits/query/__init__.py
--rw-r--r--   0        0        0    11927 2024-05-28 17:06:44.770874 adam_core-0.2.0/src/adam_core/orbits/query/horizons.py
--rw-r--r--   0        0        0     8414 2024-05-28 17:06:44.771011 adam_core-0.2.0/src/adam_core/orbits/query/sbdb.py
--rw-r--r--   0        0        0     1726 2024-05-28 17:06:44.771084 adam_core-0.2.0/src/adam_core/orbits/query/tests/__init__.py
--rw-r--r--   0        0        0     3686 2024-05-28 17:06:44.771155 adam_core-0.2.0/src/adam_core/orbits/query/tests/test_sbdb.py
--rw-r--r--   0        0        0     2953 2024-05-28 17:06:44.771303 adam_core-0.2.0/src/adam_core/orbits/query/tests/testdata/sbdb/2001VB.json
--rw-r--r--   0        0        0     5115 2024-05-28 17:06:44.771401 adam_core-0.2.0/src/adam_core/orbits/query/tests/testdata/sbdb/54509.json
--rw-r--r--   0        0        0     3908 2024-05-28 17:06:44.771484 adam_core-0.2.0/src/adam_core/orbits/query/tests/testdata/sbdb/Ceres.json
--rw-r--r--   0        0        0      442 2024-05-28 17:06:44.771558 adam_core-0.2.0/src/adam_core/orbits/query/tests/testdata/sbdb/README.md
--rw-r--r--   0        0        0      114 2024-05-28 17:06:44.771632 adam_core-0.2.0/src/adam_core/orbits/query/tests/testdata/sbdb/missing.json
--rw-r--r--   0        0        0        0 2024-05-28 17:06:44.771667 adam_core-0.2.0/src/adam_core/orbits/tests/__init__.py
--rw-r--r--   0        0        0      254 2024-05-28 17:06:44.771783 adam_core-0.2.0/src/adam_core/orbits/tests/test_benchmarks.py
--rw-r--r--   0        0        0     5773 2024-05-28 17:06:44.771901 adam_core-0.2.0/src/adam_core/orbits/tests/test_classification.py
--rw-r--r--   0        0        0     3160 2024-05-28 17:06:44.771970 adam_core-0.2.0/src/adam_core/orbits/tests/test_ephemeris.py
--rw-r--r--   0        0        0     1394 2024-05-28 17:06:44.772044 adam_core-0.2.0/src/adam_core/orbits/tests/test_orbits.py
--rw-r--r--   0        0        0     1132 2024-05-28 17:06:44.772129 adam_core-0.2.0/src/adam_core/orbits/tests/test_variants.py
--rw-r--r--   0        0        0        0 2024-05-28 17:06:44.772238 adam_core-0.2.0/src/adam_core/orbits/tests/testdata/__init__.py
--rw-r--r--   0        0        0     2209 2024-05-28 17:06:44.772434 adam_core-0.2.0/src/adam_core/orbits/tests/testdata/amo.csv
--rw-r--r--   0        0        0     2222 2024-05-28 17:06:44.772547 adam_core-0.2.0/src/adam_core/orbits/tests/testdata/apo.csv
--rw-r--r--   0        0        0     2168 2024-05-28 17:06:44.772648 adam_core-0.2.0/src/adam_core/orbits/tests/testdata/ast.csv
--rw-r--r--   0        0        0     2195 2024-05-28 17:06:44.772906 adam_core-0.2.0/src/adam_core/orbits/tests/testdata/ate.csv
--rw-r--r--   0        0        0     2218 2024-05-28 17:06:44.773120 adam_core-0.2.0/src/adam_core/orbits/tests/testdata/cen.csv
--rw-r--r--   0        0        0      613 2024-05-28 17:06:44.773190 adam_core-0.2.0/src/adam_core/orbits/tests/testdata/hya.csv
--rw-r--r--   0        0        0     2178 2024-05-28 17:06:44.773377 adam_core-0.2.0/src/adam_core/orbits/tests/testdata/ieo.csv
--rw-r--r--   0        0        0     2243 2024-05-28 17:06:44.773469 adam_core-0.2.0/src/adam_core/orbits/tests/testdata/imb.csv
--rw-r--r--   0        0        0     2197 2024-05-28 17:06:44.773536 adam_core-0.2.0/src/adam_core/orbits/tests/testdata/mba.csv
--rw-r--r--   0        0        0     2219 2024-05-28 17:06:44.773696 adam_core-0.2.0/src/adam_core/orbits/tests/testdata/mca.csv
--rw-r--r--   0        0        0     2211 2024-05-28 17:06:44.773778 adam_core-0.2.0/src/adam_core/orbits/tests/testdata/omb.csv
--rw-r--r--   0        0        0     2226 2024-05-28 17:06:44.773869 adam_core-0.2.0/src/adam_core/orbits/tests/testdata/tjn.csv
--rw-r--r--   0        0        0     2161 2024-05-28 17:06:44.773946 adam_core-0.2.0/src/adam_core/orbits/tests/testdata/tno.csv
--rw-r--r--   0        0        0    10048 2024-05-28 17:06:44.774074 adam_core-0.2.0/src/adam_core/orbits/variants.py
--rw-r--r--   0        0        0      226 2024-05-28 17:06:44.774231 adam_core-0.2.0/src/adam_core/propagator/__init__.py
--rw-r--r--   0        0        0    15904 2024-05-28 17:06:44.774376 adam_core-0.2.0/src/adam_core/propagator/propagator.py
--rw-r--r--   0        0        0        0 2024-05-28 17:06:44.774411 adam_core-0.2.0/src/adam_core/propagator/tests/__init__.py
--rw-r--r--   0        0        0     3663 2024-05-28 17:06:44.774551 adam_core-0.2.0/src/adam_core/propagator/tests/test_propagator.py
--rw-r--r--   0        0        0     1523 2024-05-28 17:06:44.774620 adam_core-0.2.0/src/adam_core/propagator/tests/test_utils.py
--rw-r--r--   0        0        0     1899 2024-05-28 17:06:44.774927 adam_core-0.2.0/src/adam_core/propagator/utils.py
--rw-r--r--   0        0        0     1556 2024-05-28 17:06:44.775025 adam_core-0.2.0/src/adam_core/ray_cluster.py
--rw-r--r--   0        0        0      933 2024-05-28 17:06:44.775357 adam_core-0.2.0/src/adam_core/tests/test_imports.py
--rw-r--r--   0        0        0     1276 2024-05-28 17:06:44.775455 adam_core-0.2.0/src/adam_core/tests/test_ray_cluster.py
--rw-r--r--   0        0        0       60 2024-05-28 17:06:44.775645 adam_core-0.2.0/src/adam_core/time/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 17:06:44.775689 adam_core-0.2.0/src/adam_core/time/tests/__init__.py
--rw-r--r--   0        0        0    21981 2024-05-28 17:06:44.775853 adam_core-0.2.0/src/adam_core/time/tests/test_time.py
--rw-r--r--   0        0        0    19352 2024-05-28 17:06:44.776037 adam_core-0.2.0/src/adam_core/time/time.py
--rw-r--r--   0        0        0      123 2024-05-28 17:06:44.776124 adam_core-0.2.0/src/adam_core/utils/__init__.py
--rw-r--r--   0        0        0      212 2024-05-28 17:06:44.776209 adam_core-0.2.0/src/adam_core/utils/helpers/__init__.py
--rw-r--r--   0        0        0     1245 2024-05-28 17:06:44.776453 adam_core-0.2.0/src/adam_core/utils/helpers/data/README.md
--rw-r--r--   0        0        0        0 2024-05-28 17:06:44.776489 adam_core-0.2.0/src/adam_core/utils/helpers/data/__init__.py
--rw-r--r--   0        0        0    10395 2024-05-28 17:06:44.776652 adam_core-0.2.0/src/adam_core/utils/helpers/data/elements_ssb_ec.csv
--rw-r--r--   0        0        0    10398 2024-05-28 17:06:44.776772 adam_core-0.2.0/src/adam_core/utils/helpers/data/elements_ssb_eq.csv
--rw-r--r--   0        0        0    10402 2024-05-28 17:06:44.776892 adam_core-0.2.0/src/adam_core/utils/helpers/data/elements_sun_ec.csv
--rw-r--r--   0        0        0    10385 2024-05-28 17:06:44.776997 adam_core-0.2.0/src/adam_core/utils/helpers/data/elements_sun_eq.csv
--rw-r--r--   0        0        0  1797474 2024-05-28 17:06:44.780662 adam_core-0.2.0/src/adam_core/utils/helpers/data/ephemeris.csv
--rw-r--r--   0        0        0     6919 2024-05-28 17:06:44.780870 adam_core-0.2.0/src/adam_core/utils/helpers/data/get_test_data.py
--rw-r--r--   0        0        0      504 2024-05-28 17:06:44.780949 adam_core-0.2.0/src/adam_core/utils/helpers/data/objects.csv
--rw-r--r--   0        0        0    15438 2024-05-28 17:06:44.781091 adam_core-0.2.0/src/adam_core/utils/helpers/data/orbits.parquet
--rw-r--r--   0        0        0   156180 2024-05-28 17:06:44.781753 adam_core-0.2.0/src/adam_core/utils/helpers/data/propagated_orbits.parquet
--rw-r--r--   0        0        0     5273 2024-05-28 17:06:44.781932 adam_core-0.2.0/src/adam_core/utils/helpers/observations.py
--rw-r--r--   0        0        0     2836 2024-05-28 17:06:44.782022 adam_core-0.2.0/src/adam_core/utils/helpers/orbits.py
--rw-r--r--   0        0        0        0 2024-05-28 17:06:44.782055 adam_core-0.2.0/src/adam_core/utils/helpers/tests/__init__.py
--rw-r--r--   0        0        0     2096 2024-05-28 17:06:44.782161 adam_core-0.2.0/src/adam_core/utils/helpers/tests/test_observations.py
--rw-r--r--   0        0        0      698 2024-05-28 17:06:44.782222 adam_core-0.2.0/src/adam_core/utils/helpers/tests/test_orbits.py
--rw-r--r--   0        0        0    13599 2024-05-28 17:06:44.782348 adam_core-0.2.0/src/adam_core/utils/mpc.py
--rw-r--r--   0        0        0     5263 2024-05-28 17:06:44.782462 adam_core-0.2.0/src/adam_core/utils/spice.py
--rw-r--r--   0        0        0        0 2024-05-28 17:06:44.782504 adam_core-0.2.0/src/adam_core/utils/tests/__init__.py
--rw-r--r--   0        0        0     1455 2024-05-28 17:06:44.782631 adam_core-0.2.0/src/adam_core/utils/tests/test_benchmarks.py
--rw-r--r--   0        0        0     7211 2024-05-28 17:06:44.782845 adam_core-0.2.0/src/adam_core/utils/tests/test_mpc.py
--rw-r--r--   0        0        0      550 2024-05-28 17:06:44.782919 adam_core-0.2.0/src/adam_core/utils/tests/test_spice.py
--rw-r--r--   0        0        0    17794 1970-01-01 00:00:00.000000 adam_core-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2782 2024-05-28 17:05:15.871265 adam_core-0.2.0a1/LICENSE.md
+-rw-r--r--   0        0        0    12890 2024-05-28 17:06:44.754473 adam_core-0.2.0a1/README.md
+-rw-r--r--   0        0        0     2910 2024-05-28 18:15:50.395839 adam_core-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0       93 2024-05-28 17:06:44.754921 adam_core-0.2.0a1/src/adam_core/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-28 18:15:50.388175 adam_core-0.2.0a1/src/adam_core/_version.py
+-rw-r--r--   0        0        0     1377 2024-05-28 17:06:44.755022 adam_core-0.2.0a1/src/adam_core/constants.py
+-rw-r--r--   0        0        0      396 2024-05-28 17:06:44.755170 adam_core-0.2.0a1/src/adam_core/coordinates/__init__.py
+-rw-r--r--   0        0        0    10810 2024-05-28 17:06:44.755290 adam_core-0.2.0a1/src/adam_core/coordinates/cartesian.py
+-rw-r--r--   0        0        0    10202 2024-05-28 17:06:44.755414 adam_core-0.2.0a1/src/adam_core/coordinates/cometary.py
+-rw-r--r--   0        0        0     6505 2024-05-28 17:06:44.755532 adam_core-0.2.0a1/src/adam_core/coordinates/conversions.py
+-rw-r--r--   0        0        0    14285 2024-05-28 17:06:44.755677 adam_core-0.2.0a1/src/adam_core/coordinates/covariances.py
+-rw-r--r--   0        0        0     2634 2024-05-28 17:06:44.755755 adam_core-0.2.0a1/src/adam_core/coordinates/jacobian.py
+-rw-r--r--   0        0        0     9250 2024-05-28 17:06:44.755872 adam_core-0.2.0a1/src/adam_core/coordinates/keplerian.py
+-rw-r--r--   0        0        0     4194 2024-05-28 17:06:44.755988 adam_core-0.2.0a1/src/adam_core/coordinates/origin.py
+-rw-r--r--   0        0        0    16741 2024-05-28 17:06:44.756119 adam_core-0.2.0a1/src/adam_core/coordinates/residuals.py
+-rw-r--r--   0        0        0     7681 2024-05-28 17:06:44.756311 adam_core-0.2.0a1/src/adam_core/coordinates/spherical.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:06:44.756376 adam_core-0.2.0a1/src/adam_core/coordinates/tests/__init__.py
+-rw-r--r--   0        0        0     1211 2024-05-28 17:06:44.756514 adam_core-0.2.0a1/src/adam_core/coordinates/tests/conftest.py
+-rw-r--r--   0        0        0     2327 2024-05-28 17:06:44.756610 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_benchmarks.py
+-rw-r--r--   0        0        0     6568 2024-05-28 17:06:44.756722 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_cartesian.py
+-rw-r--r--   0        0        0     5367 2024-05-28 17:06:44.756850 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_cometary.py
+-rw-r--r--   0        0        0     6052 2024-05-28 17:06:44.757031 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_covariances.py
+-rw-r--r--   0        0        0     5444 2024-05-28 17:06:44.757227 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_keplerian.py
+-rw-r--r--   0        0        0     2948 2024-05-28 17:06:44.757314 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_origin.py
+-rw-r--r--   0        0        0    34081 2024-05-28 17:06:44.757510 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_residuals.py
+-rw-r--r--   0        0        0     1918 2024-05-28 17:06:44.757618 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_spherical.py
+-rw-r--r--   0        0        0     7646 2024-05-28 17:06:44.759302 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_transforms_cometary.py
+-rw-r--r--   0        0        0    10063 2024-05-28 17:06:44.759458 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_transforms_keplerian.py
+-rw-r--r--   0        0        0     4866 2024-05-28 17:06:44.759616 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_transforms_rotation.py
+-rw-r--r--   0        0        0     3243 2024-05-28 17:06:44.759769 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_transforms_spherical.py
+-rw-r--r--   0        0        0    11020 2024-05-28 17:06:44.759897 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_transforms_spice.py
+-rw-r--r--   0        0        0     8044 2024-05-28 17:06:44.760004 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_transforms_translation.py
+-rw-r--r--   0        0        0    49595 2024-05-28 17:06:44.760222 adam_core-0.2.0a1/src/adam_core/coordinates/transform.py
+-rw-r--r--   0        0        0      691 2024-05-28 17:06:44.760362 adam_core-0.2.0a1/src/adam_core/coordinates/types.py
+-rw-r--r--   0        0        0     6647 2024-05-28 17:06:44.760507 adam_core-0.2.0a1/src/adam_core/coordinates/variants.py
+-rw-r--r--   0        0        0      110 2024-05-28 17:06:44.760609 adam_core-0.2.0a1/src/adam_core/dynamics/__init__.py
+-rw-r--r--   0        0        0   218508 2022-12-23 16:41:41.356795 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/aberrations.add_light_time-15.py310.1.nbc
+-rw-r--r--   0        0        0     1014 2022-12-23 16:41:41.347089 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/aberrations.add_light_time-15.py310.nbi
+-rw-r--r--   0        0        0   105441 2022-12-23 16:41:42.665228 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/aberrations.add_stellar_aberration-86.py310.1.nbc
+-rw-r--r--   0        0        0      983 2022-12-23 16:41:42.645978 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/aberrations.add_stellar_aberration-86.py310.nbi
+-rw-r--r--   0        0        0    76611 2022-12-23 16:41:30.071415 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/chi.calc_chi-13.py310.1.nbc
+-rw-r--r--   0        0        0      981 2022-12-23 16:41:30.059411 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/chi.calc_chi-13.py310.nbi
+-rw-r--r--   0        0        0    49303 2022-12-23 16:41:31.578450 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/lagrange.apply_lagrange_coefficients-92.py310.1.nbc
+-rw-r--r--   0        0        0     1008 2022-12-23 16:41:31.568284 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/lagrange.apply_lagrange_coefficients-92.py310.nbi
+-rw-r--r--   0        0        0    98285 2022-12-23 16:41:31.179470 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/lagrange.calc_lagrange_coefficients-14.py310.1.nbc
+-rw-r--r--   0        0        0     1034 2022-12-23 16:41:31.167530 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/lagrange.calc_lagrange_coefficients-14.py310.nbi
+-rw-r--r--   0        0        0    82910 2022-12-23 16:41:32.415608 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/state_transition._calc_M_matrix-15.py310.1.nbc
+-rw-r--r--   0        0        0     1022 2022-12-23 16:41:32.397995 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/state_transition._calc_M_matrix-15.py310.nbi
+-rw-r--r--   0        0        0   276594 2022-12-23 16:41:37.239361 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/state_transition.calc_state_transition_matrix-112.py310.1.nbc
+-rw-r--r--   0        0        0     1000 2022-12-23 16:41:37.220517 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/state_transition.calc_state_transition_matrix-112.py310.nbi
+-rw-r--r--   0        0        0    29452 2022-12-23 16:41:27.944024 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/stumpff.calc_stumpff-8.py310.1.nbc
+-rw-r--r--   0        0        0      962 2022-12-23 16:41:27.932619 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/stumpff.calc_stumpff-8.py310.nbi
+-rw-r--r--   0        0        0   156824 2022-12-23 16:41:38.691950 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/universal_propagate.propagate_universal-14.py310.1.nbc
+-rw-r--r--   0        0        0     1005 2022-12-23 16:41:38.679195 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/universal_propagate.propagate_universal-14.py310.nbi
+-rw-r--r--   0        0        0     6601 2024-05-28 17:06:44.760697 adam_core-0.2.0a1/src/adam_core/dynamics/aberrations.py
+-rw-r--r--   0        0        0      780 2024-05-28 17:06:44.761711 adam_core-0.2.0a1/src/adam_core/dynamics/barker.py
+-rw-r--r--   0        0        0     3387 2024-05-28 17:06:44.761806 adam_core-0.2.0a1/src/adam_core/dynamics/chi.py
+-rw-r--r--   0        0        0    10553 2024-05-28 17:06:44.761912 adam_core-0.2.0a1/src/adam_core/dynamics/ephemeris.py
+-rw-r--r--   0        0        0     9796 2024-05-28 17:06:44.762068 adam_core-0.2.0a1/src/adam_core/dynamics/impacts.py
+-rw-r--r--   0        0        0     7728 2024-05-28 17:06:44.762231 adam_core-0.2.0a1/src/adam_core/dynamics/kepler.py
+-rw-r--r--   0        0        0     3747 2024-05-28 17:06:44.762306 adam_core-0.2.0a1/src/adam_core/dynamics/lagrange.py
+-rw-r--r--   0        0        0     5212 2024-05-28 17:06:44.762584 adam_core-0.2.0a1/src/adam_core/dynamics/moid.py
+-rw-r--r--   0        0        0     5614 2024-05-28 17:06:44.762865 adam_core-0.2.0a1/src/adam_core/dynamics/propagation.py
+-rw-r--r--   0        0        0     2250 2024-05-28 17:06:44.762960 adam_core-0.2.0a1/src/adam_core/dynamics/stumpff.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:06:44.763001 adam_core-0.2.0a1/src/adam_core/dynamics/tests/__init__.py
+-rw-r--r--   0        0        0     1115 2024-05-28 17:06:44.763131 adam_core-0.2.0a1/src/adam_core/dynamics/tests/conftest.py
+-rw-r--r--   0        0        0     5413 2024-05-28 17:06:44.763230 adam_core-0.2.0a1/src/adam_core/dynamics/tests/test_ephemeris.py
+-rw-r--r--   0        0        0     7108 2024-05-28 17:06:44.763477 adam_core-0.2.0a1/src/adam_core/dynamics/tests/test_impacts.py
+-rw-r--r--   0        0        0     8775 2024-05-28 17:06:44.763611 adam_core-0.2.0a1/src/adam_core/dynamics/tests/test_kepler.py
+-rw-r--r--   0        0        0     5555 2024-05-28 17:06:44.763838 adam_core-0.2.0a1/src/adam_core/dynamics/tests/test_moid.py
+-rw-r--r--   0        0        0    16189 2024-05-28 17:06:44.763985 adam_core-0.2.0a1/src/adam_core/dynamics/tests/test_propagation.py
+-rw-r--r--   0        0        0     1311 2024-05-28 17:06:44.764071 adam_core-0.2.0a1/src/adam_core/dynamics/tests/test_tisserand.py
+-rw-r--r--   0        0        0     1953 2024-05-28 17:06:44.764170 adam_core-0.2.0a1/src/adam_core/dynamics/tisserand.py
+-rw-r--r--   0        0        0      316 2024-05-28 17:06:44.764241 adam_core-0.2.0a1/src/adam_core/observations/__init__.py
+-rw-r--r--   0        0        0     2086 2024-05-28 17:06:44.764347 adam_core-0.2.0a1/src/adam_core/observations/associations.py
+-rw-r--r--   0        0        0     2616 2024-05-28 17:06:44.764474 adam_core-0.2.0a1/src/adam_core/observations/detections.py
+-rw-r--r--   0        0        0     2578 2024-05-28 17:06:44.764600 adam_core-0.2.0a1/src/adam_core/observations/exposures.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:06:44.764638 adam_core-0.2.0a1/src/adam_core/observations/tests/__init__.py
+-rw-r--r--   0        0        0     1582 2024-05-28 17:06:44.764744 adam_core-0.2.0a1/src/adam_core/observations/tests/test_associations.py
+-rw-r--r--   0        0        0     3349 2024-05-28 17:06:44.764818 adam_core-0.2.0a1/src/adam_core/observations/tests/test_detections.py
+-rw-r--r--   0        0        0     3623 2024-05-28 17:06:44.764947 adam_core-0.2.0a1/src/adam_core/observations/tests/test_exposures.py
+-rw-r--r--   0        0        0      139 2024-05-28 17:06:44.765039 adam_core-0.2.0a1/src/adam_core/observers/__init__.py
+-rw-r--r--   0        0        0     3703 2024-05-28 17:06:44.765147 adam_core-0.2.0a1/src/adam_core/observers/observers.py
+-rw-r--r--   0        0        0     6357 2024-05-28 17:06:44.765242 adam_core-0.2.0a1/src/adam_core/observers/state.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:06:44.765286 adam_core-0.2.0a1/src/adam_core/observers/tests/__init__.py
+-rw-r--r--   0        0        0     1339 2024-05-28 17:06:44.765452 adam_core-0.2.0a1/src/adam_core/observers/tests/test_benchmarks.py
+-rw-r--r--   0        0        0     3141 2024-05-28 17:06:44.765577 adam_core-0.2.0a1/src/adam_core/observers/tests/test_state.py
+-rw-r--r--   0        0        0    26467 2024-05-28 17:06:44.765793 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/000_ssb.parquet
+-rw-r--r--   0        0        0    26327 2024-05-28 17:06:44.765999 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/000_sun.parquet
+-rw-r--r--   0        0        0    26467 2024-05-28 17:06:44.766172 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/500_ssb.parquet
+-rw-r--r--   0        0        0    26327 2024-05-28 17:06:44.766349 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/500_sun.parquet
+-rw-r--r--   0        0        0    26467 2024-05-28 17:06:44.766573 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/F51_ssb.parquet
+-rw-r--r--   0        0        0    26327 2024-05-28 17:06:44.766750 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/F51_sun.parquet
+-rw-r--r--   0        0        0    26467 2024-05-28 17:06:44.766928 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/I41_ssb.parquet
+-rw-r--r--   0        0        0    26327 2024-05-28 17:06:44.767125 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/I41_sun.parquet
+-rw-r--r--   0        0        0     1638 2024-05-28 17:06:44.767218 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/README.md
+-rw-r--r--   0        0        0    26467 2024-05-28 17:06:44.767391 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/W84_ssb.parquet
+-rw-r--r--   0        0        0    26327 2024-05-28 17:06:44.767550 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/W84_sun.parquet
+-rw-r--r--   0        0        0    26467 2024-05-28 17:06:44.767718 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/X05_ssb.parquet
+-rw-r--r--   0        0        0    26327 2024-05-28 17:06:44.767896 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/X05_sun.parquet
+-rw-r--r--   0        0        0     1475 2024-05-28 17:06:44.767981 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/get_states.py
+-rw-r--r--   0        0        0      266 2024-05-28 17:06:44.768062 adam_core-0.2.0a1/src/adam_core/orbit_determination/__init__.py
+-rw-r--r--   0        0        0     7438 2024-05-28 17:06:44.768223 adam_core-0.2.0a1/src/adam_core/orbit_determination/differential_correction.py
+-rw-r--r--   0        0        0     5219 2024-05-28 17:06:44.768382 adam_core-0.2.0a1/src/adam_core/orbit_determination/evaluate.py
+-rw-r--r--   0        0        0     1310 2024-05-28 17:06:44.768466 adam_core-0.2.0a1/src/adam_core/orbit_determination/fitted_orbits.py
+-rw-r--r--   0        0        0     2420 2024-05-28 17:06:44.768559 adam_core-0.2.0a1/src/adam_core/orbit_determination/outliers.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:06:44.768598 adam_core-0.2.0a1/src/adam_core/orbit_determination/tests/__init__.py
+-rw-r--r--   0        0        0      810 2024-05-28 17:06:44.768716 adam_core-0.2.0a1/src/adam_core/orbit_determination/tests/conftest.py
+-rw-r--r--   0        0        0     8261 2024-05-28 17:06:44.768898 adam_core-0.2.0a1/src/adam_core/orbit_determination/tests/data/pure_iod_orbit.parquet
+-rw-r--r--   0        0        0     3659 2024-05-28 17:06:44.769010 adam_core-0.2.0a1/src/adam_core/orbit_determination/tests/data/pure_iod_orbit_members.parquet
+-rw-r--r--   0        0        0    16284 2024-05-28 17:06:44.769171 adam_core-0.2.0a1/src/adam_core/orbit_determination/tests/data/pure_iod_orbit_observations.parquet
+-rw-r--r--   0        0        0      937 2024-05-28 17:06:44.769596 adam_core-0.2.0a1/src/adam_core/orbit_determination/tests/test_differential_correction.py
+-rw-r--r--   0        0        0     4281 2024-05-28 17:06:44.770015 adam_core-0.2.0a1/src/adam_core/orbit_determination/tests/test_evaluate.py
+-rw-r--r--   0        0        0     6049 2024-05-28 17:06:44.770121 adam_core-0.2.0a1/src/adam_core/orbit_determination/tests/test_outliers.py
+-rw-r--r--   0        0        0      275 2024-05-28 17:06:44.770264 adam_core-0.2.0a1/src/adam_core/orbits/__init__.py
+-rw-r--r--   0        0        0     2111 2024-05-28 17:06:44.770355 adam_core-0.2.0a1/src/adam_core/orbits/classification.py
+-rw-r--r--   0        0        0     4294 2024-05-28 17:06:44.770496 adam_core-0.2.0a1/src/adam_core/orbits/ephemeris.py
+-rw-r--r--   0        0        0     1381 2024-05-28 17:06:44.770648 adam_core-0.2.0a1/src/adam_core/orbits/orbits.py
+-rw-r--r--   0        0        0       87 2024-05-28 17:06:44.770738 adam_core-0.2.0a1/src/adam_core/orbits/query/__init__.py
+-rw-r--r--   0        0        0    11927 2024-05-28 17:06:44.770874 adam_core-0.2.0a1/src/adam_core/orbits/query/horizons.py
+-rw-r--r--   0        0        0     8414 2024-05-28 17:06:44.771011 adam_core-0.2.0a1/src/adam_core/orbits/query/sbdb.py
+-rw-r--r--   0        0        0     1726 2024-05-28 17:06:44.771084 adam_core-0.2.0a1/src/adam_core/orbits/query/tests/__init__.py
+-rw-r--r--   0        0        0     3686 2024-05-28 17:06:44.771155 adam_core-0.2.0a1/src/adam_core/orbits/query/tests/test_sbdb.py
+-rw-r--r--   0        0        0     2953 2024-05-28 17:06:44.771303 adam_core-0.2.0a1/src/adam_core/orbits/query/tests/testdata/sbdb/2001VB.json
+-rw-r--r--   0        0        0     5115 2024-05-28 17:06:44.771401 adam_core-0.2.0a1/src/adam_core/orbits/query/tests/testdata/sbdb/54509.json
+-rw-r--r--   0        0        0     3908 2024-05-28 17:06:44.771484 adam_core-0.2.0a1/src/adam_core/orbits/query/tests/testdata/sbdb/Ceres.json
+-rw-r--r--   0        0        0      442 2024-05-28 17:06:44.771558 adam_core-0.2.0a1/src/adam_core/orbits/query/tests/testdata/sbdb/README.md
+-rw-r--r--   0        0        0      114 2024-05-28 17:06:44.771632 adam_core-0.2.0a1/src/adam_core/orbits/query/tests/testdata/sbdb/missing.json
+-rw-r--r--   0        0        0        0 2024-05-28 17:06:44.771667 adam_core-0.2.0a1/src/adam_core/orbits/tests/__init__.py
+-rw-r--r--   0        0        0      254 2024-05-28 17:06:44.771783 adam_core-0.2.0a1/src/adam_core/orbits/tests/test_benchmarks.py
+-rw-r--r--   0        0        0     5773 2024-05-28 17:06:44.771901 adam_core-0.2.0a1/src/adam_core/orbits/tests/test_classification.py
+-rw-r--r--   0        0        0     3160 2024-05-28 17:06:44.771970 adam_core-0.2.0a1/src/adam_core/orbits/tests/test_ephemeris.py
+-rw-r--r--   0        0        0     1394 2024-05-28 17:06:44.772044 adam_core-0.2.0a1/src/adam_core/orbits/tests/test_orbits.py
+-rw-r--r--   0        0        0     1132 2024-05-28 17:06:44.772129 adam_core-0.2.0a1/src/adam_core/orbits/tests/test_variants.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:06:44.772238 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     2209 2024-05-28 17:06:44.772434 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/amo.csv
+-rw-r--r--   0        0        0     2222 2024-05-28 17:06:44.772547 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/apo.csv
+-rw-r--r--   0        0        0     2168 2024-05-28 17:06:44.772648 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/ast.csv
+-rw-r--r--   0        0        0     2195 2024-05-28 17:06:44.772906 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/ate.csv
+-rw-r--r--   0        0        0     2218 2024-05-28 17:06:44.773120 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/cen.csv
+-rw-r--r--   0        0        0      613 2024-05-28 17:06:44.773190 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/hya.csv
+-rw-r--r--   0        0        0     2178 2024-05-28 17:06:44.773377 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/ieo.csv
+-rw-r--r--   0        0        0     2243 2024-05-28 17:06:44.773469 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/imb.csv
+-rw-r--r--   0        0        0     2197 2024-05-28 17:06:44.773536 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/mba.csv
+-rw-r--r--   0        0        0     2219 2024-05-28 17:06:44.773696 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/mca.csv
+-rw-r--r--   0        0        0     2211 2024-05-28 17:06:44.773778 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/omb.csv
+-rw-r--r--   0        0        0     2226 2024-05-28 17:06:44.773869 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/tjn.csv
+-rw-r--r--   0        0        0     2161 2024-05-28 17:06:44.773946 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/tno.csv
+-rw-r--r--   0        0        0    10048 2024-05-28 17:06:44.774074 adam_core-0.2.0a1/src/adam_core/orbits/variants.py
+-rw-r--r--   0        0        0      226 2024-05-28 17:06:44.774231 adam_core-0.2.0a1/src/adam_core/propagator/__init__.py
+-rw-r--r--   0        0        0    15904 2024-05-28 17:06:44.774376 adam_core-0.2.0a1/src/adam_core/propagator/propagator.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:06:44.774411 adam_core-0.2.0a1/src/adam_core/propagator/tests/__init__.py
+-rw-r--r--   0        0        0     3663 2024-05-28 17:06:44.774551 adam_core-0.2.0a1/src/adam_core/propagator/tests/test_propagator.py
+-rw-r--r--   0        0        0     1523 2024-05-28 17:06:44.774620 adam_core-0.2.0a1/src/adam_core/propagator/tests/test_utils.py
+-rw-r--r--   0        0        0     1899 2024-05-28 17:06:44.774927 adam_core-0.2.0a1/src/adam_core/propagator/utils.py
+-rw-r--r--   0        0        0     1556 2024-05-28 17:06:44.775025 adam_core-0.2.0a1/src/adam_core/ray_cluster.py
+-rw-r--r--   0        0        0      933 2024-05-28 17:06:44.775357 adam_core-0.2.0a1/src/adam_core/tests/test_imports.py
+-rw-r--r--   0        0        0     1276 2024-05-28 17:06:44.775455 adam_core-0.2.0a1/src/adam_core/tests/test_ray_cluster.py
+-rw-r--r--   0        0        0       60 2024-05-28 17:06:44.775645 adam_core-0.2.0a1/src/adam_core/time/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:06:44.775689 adam_core-0.2.0a1/src/adam_core/time/tests/__init__.py
+-rw-r--r--   0        0        0    21981 2024-05-28 17:06:44.775853 adam_core-0.2.0a1/src/adam_core/time/tests/test_time.py
+-rw-r--r--   0        0        0    19352 2024-05-28 17:06:44.776037 adam_core-0.2.0a1/src/adam_core/time/time.py
+-rw-r--r--   0        0        0      123 2024-05-28 17:06:44.776124 adam_core-0.2.0a1/src/adam_core/utils/__init__.py
+-rw-r--r--   0        0        0      212 2024-05-28 17:06:44.776209 adam_core-0.2.0a1/src/adam_core/utils/helpers/__init__.py
+-rw-r--r--   0        0        0     1245 2024-05-28 17:06:44.776453 adam_core-0.2.0a1/src/adam_core/utils/helpers/data/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 17:06:44.776489 adam_core-0.2.0a1/src/adam_core/utils/helpers/data/__init__.py
+-rw-r--r--   0        0        0    10395 2024-05-28 17:06:44.776652 adam_core-0.2.0a1/src/adam_core/utils/helpers/data/elements_ssb_ec.csv
+-rw-r--r--   0        0        0    10398 2024-05-28 17:06:44.776772 adam_core-0.2.0a1/src/adam_core/utils/helpers/data/elements_ssb_eq.csv
+-rw-r--r--   0        0        0    10402 2024-05-28 17:06:44.776892 adam_core-0.2.0a1/src/adam_core/utils/helpers/data/elements_sun_ec.csv
+-rw-r--r--   0        0        0    10385 2024-05-28 17:06:44.776997 adam_core-0.2.0a1/src/adam_core/utils/helpers/data/elements_sun_eq.csv
+-rw-r--r--   0        0        0  1797474 2024-05-28 17:06:44.780662 adam_core-0.2.0a1/src/adam_core/utils/helpers/data/ephemeris.csv
+-rw-r--r--   0        0        0     6919 2024-05-28 17:06:44.780870 adam_core-0.2.0a1/src/adam_core/utils/helpers/data/get_test_data.py
+-rw-r--r--   0        0        0      504 2024-05-28 17:06:44.780949 adam_core-0.2.0a1/src/adam_core/utils/helpers/data/objects.csv
+-rw-r--r--   0        0        0    15438 2024-05-28 17:06:44.781091 adam_core-0.2.0a1/src/adam_core/utils/helpers/data/orbits.parquet
+-rw-r--r--   0        0        0   156180 2024-05-28 17:06:44.781753 adam_core-0.2.0a1/src/adam_core/utils/helpers/data/propagated_orbits.parquet
+-rw-r--r--   0        0        0     5273 2024-05-28 17:06:44.781932 adam_core-0.2.0a1/src/adam_core/utils/helpers/observations.py
+-rw-r--r--   0        0        0     2836 2024-05-28 17:06:44.782022 adam_core-0.2.0a1/src/adam_core/utils/helpers/orbits.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:06:44.782055 adam_core-0.2.0a1/src/adam_core/utils/helpers/tests/__init__.py
+-rw-r--r--   0        0        0     2096 2024-05-28 17:06:44.782161 adam_core-0.2.0a1/src/adam_core/utils/helpers/tests/test_observations.py
+-rw-r--r--   0        0        0      698 2024-05-28 17:06:44.782222 adam_core-0.2.0a1/src/adam_core/utils/helpers/tests/test_orbits.py
+-rw-r--r--   0        0        0    13599 2024-05-28 17:06:44.782348 adam_core-0.2.0a1/src/adam_core/utils/mpc.py
+-rw-r--r--   0        0        0     5263 2024-05-28 17:06:44.782462 adam_core-0.2.0a1/src/adam_core/utils/spice.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:06:44.782504 adam_core-0.2.0a1/src/adam_core/utils/tests/__init__.py
+-rw-r--r--   0        0        0     1455 2024-05-28 17:06:44.782631 adam_core-0.2.0a1/src/adam_core/utils/tests/test_benchmarks.py
+-rw-r--r--   0        0        0     7211 2024-05-28 17:06:44.782845 adam_core-0.2.0a1/src/adam_core/utils/tests/test_mpc.py
+-rw-r--r--   0        0        0      550 2024-05-28 17:06:44.782919 adam_core-0.2.0a1/src/adam_core/utils/tests/test_spice.py
+-rw-r--r--   0        0        0    18170 1970-01-01 00:00:00.000000 adam_core-0.2.0a1/PKG-INFO
```

### Comparing `adam_core-0.2.0/LICENSE.md` & `adam_core-0.2.0a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/README.md` & `adam_core-0.2.0a1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 # adam_core: ADAM Core Utilities
 #### A Python package by the Asteroid Institute, a program of the B612 Foundation
 [![Python 3.9+](https://img.shields.io/badge/Python-3.9%2B-blue)](https://img.shields.io/badge/Python-3.9%2B-blue)
 [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)  
-[![pip - Build, Lint, Test, and Coverage](https://github.com/B612-Asteroid-Institute/adam_core/actions/workflows/pip-build-lint-test-coverage.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/adam_core/actions/workflows/pip-build-lint-test-coverage.yml)
+[![docker - Build, Lint, and Test](https://github.com/B612-Asteroid-Institute/adam_core/actions/workflows/docker-build-lint-test.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/adam_core/actions/workflows/docker-build-lint-test.yml)
+[![pip - Build, Lint, Test, and Coverage](https://github.com/B612-Asteroid-Institute/adam_core/actions/workflows/pip-build-lint-test-coverage.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/adam_core/actions/workflows/pip-build-lint-test-coverage.yml)  
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 
 `adam_core` is used by a variety of library and services at the Asteroid Institute. Sharing these common classes, types, and conversions amongst our tools ensures consistency and accuracy.
 
-## Installation
-
-ADAM Core is available on PyPI
-
-```bash
-pip install adam_core
-```
-
 ## Usage
 
 ### Orbits
 
 To define an orbit:
 ```python
 from adam_core.coordinates import KeplerianCoordinates
@@ -154,35 +148,34 @@
 keplerian_elements = orbits.coordinates.to_keplerian()
 spherical_elements = orbits.coordinates.to_spherical()
 ```
 
 ### Propagator
 The propagator class in `adam_core` provides a generalized interface to the supported orbit integrators and ephemeris generators. The propagator class is designed to be used with the `Orbits` class and can handle multiple orbits and times. 
 
-You will need to install either adam_core[assist], or another compatible propagator in order to use propagation, ephemeris generation, or impact analysis.
+You will need to install either adam_core[pyoorb] or adam_core[assist], or another compatible propagator in order to use propagation, ephemeris generation, or impact analysis.
 
 #### Propagation
-To propagate orbits with ASSIST (here we grab some orbits from Horizons first):
+To propagate orbits with PYOORB (here we grab some orbits from Horizons first):
 
 ```python
 import numpy as np
 from astropy import units as u
 
 from adam_core.orbits.query import query_horizons
-from adam_core.propagator.adam_assist import ASSISTPropagator, download_jpl_ephemeris_files
+from adam_core.propagator import PYOORBPropagator
 from adam_core.time import Timestamp
 
 # Get orbits to propagate
 initial_time = Timestamp.from_mjd([60000.0], scale="tdb")
 object_ids = ["Duende", "Eros", "Ceres"]
 orbits = query_horizons(object_ids, initial_time)
 
-# Download ephemeris files used by propagator and initialize
-download_jpl_ephemeris_files()
-propagator = ASSISTPropagator()
+# Make sure PYOORB is ready
+propagator = PYOORBPropagator()
 
 # Define propagation times
 times = initial_time.from_mjd(initial_time.mjd() + np.arange(0, 100))
 
 # Propagate orbits! This function supports multiprocessing for large
 # propagation jobs.
 propagated_orbits = propagator.propagate_orbits(
@@ -192,27 +185,27 @@
     max_processes=1,
 )
 ```
 
 #### Ephemeris Generation
 Ephemeris generation requires a propagator that implements the EphemerisMixin interface. This is currently only implemented by the PYOORB propagator. The ephemeris generator will automatically map the propagated covariance matrices to the sky-plane.
 
-You will need to install adam-pyoorb in order to use the ephemeris generator, which is currently only available on GitHub.
+You will need to install adam-pyoorb in order to use the ephemeris generator.
 
 ```sh
-pip install git+https://github.com/B612-Asteroid-Institute/adam-pyoorb.git
+pip install adam-core[pyoorb]
 ```
 
 
 ```python
 import numpy as np
 from astropy import units as u
 
 from adam_core.orbits.query import query_horizons
-from adam_core.propagator.adam_pyoorb import PYOORBPropagator
+from adam_core.propagator import PYOORBPropagator
 from adam_core.observers import Observers
 from adam_core.time import Timestamp
 
 # Get orbits to propagate
 initial_time = Timestamp.from_mjd([60000.0], scale="tdb")
 object_ids = ["Duende", "Eros", "Ceres"]
 orbits = query_horizons(object_ids, initial_time)
@@ -289,15 +282,15 @@
 then automatically map the propagated covariance matrices to the sky-plane.
 
 ```python
 import numpy as np
 from astropy import units as u
 
 from adam_core.orbits.query import query_sbdb
-from adam_core.propagator.adam_pyoorb import PYOORBPropagator
+from adam_core.propagator import PYOORBPropagator
 from adam_core.observers import Observers
 from adam_core.dynamics import generate_ephemeris_2body
 from adam_core.time import Timestamp
 
 # Get orbits to propagate
 object_ids = ["Duende", "Eros", "Ceres"]
 orbits = query_sbdb(object_ids)
@@ -348,8 +341,29 @@
 ├── constants.py  # Shared constants
 ├── coordinates   # Coordinate classes and transformations
 ├── dynamics      # Numerical solutions
 ├── orbits        # Orbits class and query utilities
 └── utils         # Utility classes like Indexable or conversions like times_from_df
 ```
 
+## Installation
 
+ADAM Core is available on PyPI
+
+```bash
+pip install adam_core
+```
+
+## Development
+
+Development is made easy with our Docker container environment.
+
+```bash
+# Build the container
+docker compose build
+
+# Run tests in the container
+docker compose run adam_core pytest .
+
+# Run a shell in the container
+docker compose run adam_core bash
+```
```

### Comparing `adam_core-0.2.0/pyproject.toml` & `adam_core-0.2.0a1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -43,28 +43,25 @@
     "naif-de440",
     "naif-leapseconds",
     "naif-eop-high-prec",
     "naif-eop-predict",
     "naif-eop-historical",
     "naif-earth-itrf93",
 ]
-version = "0.2.0"
+version = "0.2.0a1"
 
 [project.license]
 file = "LICENSE.md"
 
 [project.urls]
 Documentation = "https://github.com/B612-Asteroid-Institute/adam_core#README.md"
 Issues = "https://github.com/B612-Asteroid-Institute/adam_core/issues"
 Source = "https://github.com/B612-Asteroid-Institute/adam_core"
 
 [project.optional-dependencies]
-assist = [
-    "adam-assist>=0.1.1a1",
-]
 dev = [
     "black",
     "ipython",
     "isort",
     "mypy",
     "pdm",
     "pytest-benchmark",
```

### Comparing `adam_core-0.2.0/src/adam_core/constants.py` & `adam_core-0.2.0a1/src/adam_core/constants.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/cartesian.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/cartesian.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/cometary.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/cometary.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/conversions.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/conversions.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/covariances.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/covariances.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/jacobian.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/jacobian.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/keplerian.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/keplerian.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/origin.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/origin.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/residuals.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/residuals.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/spherical.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/spherical.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/tests/conftest.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/tests/test_benchmarks.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/tests/test_cartesian.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_cartesian.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/tests/test_cometary.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_cometary.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/tests/test_covariances.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_covariances.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/tests/test_keplerian.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_keplerian.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/tests/test_origin.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_origin.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/tests/test_residuals.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_residuals.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/tests/test_spherical.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_spherical.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/tests/test_transforms_cometary.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_transforms_cometary.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/tests/test_transforms_keplerian.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_transforms_keplerian.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/tests/test_transforms_rotation.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_transforms_rotation.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/tests/test_transforms_spherical.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_transforms_spherical.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/tests/test_transforms_spice.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_transforms_spice.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/tests/test_transforms_translation.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_transforms_translation.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/transform.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/transform.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/types.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/types.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/coordinates/variants.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/variants.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/__pycache__/aberrations.add_light_time-15.py310.1.nbc` & `adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/aberrations.add_light_time-15.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/__pycache__/aberrations.add_light_time-15.py310.nbi` & `adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/aberrations.add_light_time-15.py310.nbi`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/__pycache__/aberrations.add_stellar_aberration-86.py310.1.nbc` & `adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/aberrations.add_stellar_aberration-86.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/__pycache__/aberrations.add_stellar_aberration-86.py310.nbi` & `adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/aberrations.add_stellar_aberration-86.py310.nbi`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/__pycache__/chi.calc_chi-13.py310.1.nbc` & `adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/chi.calc_chi-13.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/__pycache__/chi.calc_chi-13.py310.nbi` & `adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/chi.calc_chi-13.py310.nbi`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/__pycache__/lagrange.apply_lagrange_coefficients-92.py310.1.nbc` & `adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/lagrange.apply_lagrange_coefficients-92.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/__pycache__/lagrange.apply_lagrange_coefficients-92.py310.nbi` & `adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/lagrange.apply_lagrange_coefficients-92.py310.nbi`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/__pycache__/lagrange.calc_lagrange_coefficients-14.py310.1.nbc` & `adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/lagrange.calc_lagrange_coefficients-14.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/__pycache__/lagrange.calc_lagrange_coefficients-14.py310.nbi` & `adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/lagrange.calc_lagrange_coefficients-14.py310.nbi`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/__pycache__/state_transition._calc_M_matrix-15.py310.1.nbc` & `adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/state_transition._calc_M_matrix-15.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/__pycache__/state_transition._calc_M_matrix-15.py310.nbi` & `adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/state_transition._calc_M_matrix-15.py310.nbi`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/__pycache__/state_transition.calc_state_transition_matrix-112.py310.1.nbc` & `adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/state_transition.calc_state_transition_matrix-112.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/__pycache__/state_transition.calc_state_transition_matrix-112.py310.nbi` & `adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/state_transition.calc_state_transition_matrix-112.py310.nbi`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/__pycache__/stumpff.calc_stumpff-8.py310.1.nbc` & `adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/stumpff.calc_stumpff-8.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/__pycache__/stumpff.calc_stumpff-8.py310.nbi` & `adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/stumpff.calc_stumpff-8.py310.nbi`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/__pycache__/universal_propagate.propagate_universal-14.py310.1.nbc` & `adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/universal_propagate.propagate_universal-14.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/__pycache__/universal_propagate.propagate_universal-14.py310.nbi` & `adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/universal_propagate.propagate_universal-14.py310.nbi`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/aberrations.py` & `adam_core-0.2.0a1/src/adam_core/dynamics/aberrations.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/barker.py` & `adam_core-0.2.0a1/src/adam_core/dynamics/barker.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/chi.py` & `adam_core-0.2.0a1/src/adam_core/dynamics/chi.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/ephemeris.py` & `adam_core-0.2.0a1/src/adam_core/dynamics/ephemeris.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/impacts.py` & `adam_core-0.2.0a1/src/adam_core/dynamics/impacts.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/kepler.py` & `adam_core-0.2.0a1/src/adam_core/dynamics/kepler.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/lagrange.py` & `adam_core-0.2.0a1/src/adam_core/dynamics/lagrange.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/moid.py` & `adam_core-0.2.0a1/src/adam_core/dynamics/moid.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/propagation.py` & `adam_core-0.2.0a1/src/adam_core/dynamics/propagation.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/stumpff.py` & `adam_core-0.2.0a1/src/adam_core/dynamics/stumpff.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/tests/conftest.py` & `adam_core-0.2.0a1/src/adam_core/dynamics/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/tests/test_ephemeris.py` & `adam_core-0.2.0a1/src/adam_core/dynamics/tests/test_ephemeris.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/tests/test_impacts.py` & `adam_core-0.2.0a1/src/adam_core/dynamics/tests/test_impacts.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/tests/test_kepler.py` & `adam_core-0.2.0a1/src/adam_core/dynamics/tests/test_kepler.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/tests/test_moid.py` & `adam_core-0.2.0a1/src/adam_core/dynamics/tests/test_moid.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/tests/test_propagation.py` & `adam_core-0.2.0a1/src/adam_core/dynamics/tests/test_propagation.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/tests/test_tisserand.py` & `adam_core-0.2.0a1/src/adam_core/dynamics/tests/test_tisserand.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/dynamics/tisserand.py` & `adam_core-0.2.0a1/src/adam_core/dynamics/tisserand.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/observations/associations.py` & `adam_core-0.2.0a1/src/adam_core/observations/associations.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/observations/detections.py` & `adam_core-0.2.0a1/src/adam_core/observations/detections.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/observations/exposures.py` & `adam_core-0.2.0a1/src/adam_core/observations/exposures.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/observations/tests/test_associations.py` & `adam_core-0.2.0a1/src/adam_core/observations/tests/test_associations.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/observations/tests/test_detections.py` & `adam_core-0.2.0a1/src/adam_core/observations/tests/test_detections.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/observations/tests/test_exposures.py` & `adam_core-0.2.0a1/src/adam_core/observations/tests/test_exposures.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/observers/observers.py` & `adam_core-0.2.0a1/src/adam_core/observers/observers.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/observers/state.py` & `adam_core-0.2.0a1/src/adam_core/observers/state.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/observers/tests/test_benchmarks.py` & `adam_core-0.2.0a1/src/adam_core/observers/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/observers/tests/test_state.py` & `adam_core-0.2.0a1/src/adam_core/observers/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/observers/tests/testdata/000_ssb.parquet` & `adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/000_ssb.parquet`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/observers/tests/testdata/000_sun.parquet` & `adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/000_sun.parquet`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/observers/tests/testdata/500_ssb.parquet` & `adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/500_ssb.parquet`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/observers/tests/testdata/500_sun.parquet` & `adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/500_sun.parquet`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/observers/tests/testdata/F51_ssb.parquet` & `adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/F51_ssb.parquet`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/observers/tests/testdata/F51_sun.parquet` & `adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/F51_sun.parquet`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/observers/tests/testdata/I41_ssb.parquet` & `adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/I41_ssb.parquet`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/observers/tests/testdata/I41_sun.parquet` & `adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/I41_sun.parquet`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/observers/tests/testdata/README.md` & `adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/README.md`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/observers/tests/testdata/W84_ssb.parquet` & `adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/W84_ssb.parquet`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/observers/tests/testdata/W84_sun.parquet` & `adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/W84_sun.parquet`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/observers/tests/testdata/X05_ssb.parquet` & `adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/X05_ssb.parquet`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/observers/tests/testdata/X05_sun.parquet` & `adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/X05_sun.parquet`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/observers/tests/testdata/get_states.py` & `adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/get_states.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbit_determination/differential_correction.py` & `adam_core-0.2.0a1/src/adam_core/orbit_determination/differential_correction.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbit_determination/evaluate.py` & `adam_core-0.2.0a1/src/adam_core/orbit_determination/evaluate.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbit_determination/fitted_orbits.py` & `adam_core-0.2.0a1/src/adam_core/orbit_determination/fitted_orbits.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbit_determination/outliers.py` & `adam_core-0.2.0a1/src/adam_core/orbit_determination/outliers.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbit_determination/tests/conftest.py` & `adam_core-0.2.0a1/src/adam_core/orbit_determination/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbit_determination/tests/data/pure_iod_orbit.parquet` & `adam_core-0.2.0a1/src/adam_core/orbit_determination/tests/data/pure_iod_orbit.parquet`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbit_determination/tests/data/pure_iod_orbit_members.parquet` & `adam_core-0.2.0a1/src/adam_core/orbit_determination/tests/data/pure_iod_orbit_members.parquet`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbit_determination/tests/data/pure_iod_orbit_observations.parquet` & `adam_core-0.2.0a1/src/adam_core/orbit_determination/tests/data/pure_iod_orbit_observations.parquet`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbit_determination/tests/test_differential_correction.py` & `adam_core-0.2.0a1/src/adam_core/orbit_determination/tests/test_differential_correction.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 import os
 
 import pytest
 
-try:
-    from adam_core.propagator.adam_pyoorb import PYOORBPropagator
-except ImportError:
-    PYOORBPropagator = None
+from adam_core.propagator.adam_pyoorb import PYOORBPropagator
 
 from ..differential_correction import fit_least_squares
 
 
 @pytest.mark.skipif(
     os.environ.get("OORB_DATA") is None, reason="OORB_DATA environment variable not set"
 )
-@pytest.mark.skipif(PYOORBPropagator is None, reason="PYOORBPropagator not available")
 def test_fit_least_squares_pure_iod_orbit(pure_iod_orbit):
     # Test that fit_least_squares can fit and improve a pure orbit from an IOD
     # process using least squares
 
     orbit, orbit_members, observations = pure_iod_orbit
     propagator = PYOORBPropagator()
```

### Comparing `adam_core-0.2.0/src/adam_core/orbit_determination/tests/test_evaluate.py` & `adam_core-0.2.0a1/src/adam_core/orbit_determination/tests/test_evaluate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import os
 
 import numpy as np
 import pyarrow as pa
 import pytest
 import quivr as qv
 
-try:
-    from adam_core.propagator.adam_pyoorb import PYOORBPropagator
-except ImportError:
-    PYOORBPropagator = None
+from adam_core.propagator.adam_pyoorb import PYOORBPropagator
 
 from ..evaluate import evaluate_orbits
 
 
 @pytest.mark.skipif(
     os.environ.get("OORB_DATA") is None, reason="OORB_DATA environment variable not set"
 )
-@pytest.mark.skipif(PYOORBPropagator is None, reason="PYOORBPropagator not available")
 def test_evaluate_orbits(pure_iod_orbit):
     # Test that evaluate_orbit correctly calculates residuals and other
     # parameters for an input orbit
     orbit, orbit_members, observations = pure_iod_orbit
     propagator = PYOORBPropagator()
 
     # Concatenate the orbit three times to test we can handle multiple orbits
@@ -60,15 +56,14 @@
             orbit_members.residuals.to_array(),
         )
 
 
 @pytest.mark.skipif(
     os.environ.get("OORB_DATA") is None, reason="OORB_DATA environment variable not set"
 )
-@pytest.mark.skipif(PYOORBPropagator is None, reason="PYOORBPropagator not available")
 def test_evaluate_orbits_outliers(pure_iod_orbit):
     # Test that evaluate_orbit correctly calculates residuals and other
     # parameters for an input orbit with outliers defined
     orbit, orbit_members, observations = pure_iod_orbit
     propagator = PYOORBPropagator()
 
     # Lets remove the last two observations
```

### Comparing `adam_core-0.2.0/src/adam_core/orbit_determination/tests/test_outliers.py` & `adam_core-0.2.0a1/src/adam_core/orbit_determination/tests/test_outliers.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/classification.py` & `adam_core-0.2.0a1/src/adam_core/orbits/classification.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/ephemeris.py` & `adam_core-0.2.0a1/src/adam_core/orbits/ephemeris.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/orbits.py` & `adam_core-0.2.0a1/src/adam_core/orbits/orbits.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/query/horizons.py` & `adam_core-0.2.0a1/src/adam_core/orbits/query/horizons.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/query/sbdb.py` & `adam_core-0.2.0a1/src/adam_core/orbits/query/sbdb.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/query/tests/__init__.py` & `adam_core-0.2.0a1/src/adam_core/orbits/query/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/query/tests/test_sbdb.py` & `adam_core-0.2.0a1/src/adam_core/orbits/query/tests/test_sbdb.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/query/tests/testdata/sbdb/2001VB.json` & `adam_core-0.2.0a1/src/adam_core/orbits/query/tests/testdata/sbdb/2001VB.json`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/query/tests/testdata/sbdb/54509.json` & `adam_core-0.2.0a1/src/adam_core/orbits/query/tests/testdata/sbdb/54509.json`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/query/tests/testdata/sbdb/Ceres.json` & `adam_core-0.2.0a1/src/adam_core/orbits/query/tests/testdata/sbdb/Ceres.json`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/tests/test_classification.py` & `adam_core-0.2.0a1/src/adam_core/orbits/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/tests/test_ephemeris.py` & `adam_core-0.2.0a1/src/adam_core/orbits/tests/test_ephemeris.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/tests/test_orbits.py` & `adam_core-0.2.0a1/src/adam_core/orbits/tests/test_orbits.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/tests/test_variants.py` & `adam_core-0.2.0a1/src/adam_core/orbits/tests/test_variants.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/tests/testdata/amo.csv` & `adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/amo.csv`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/tests/testdata/apo.csv` & `adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/apo.csv`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/tests/testdata/ast.csv` & `adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/ast.csv`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/tests/testdata/ate.csv` & `adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/ate.csv`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/tests/testdata/cen.csv` & `adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/cen.csv`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/tests/testdata/hya.csv` & `adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/hya.csv`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/tests/testdata/ieo.csv` & `adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/ieo.csv`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/tests/testdata/imb.csv` & `adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/imb.csv`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/tests/testdata/mba.csv` & `adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/mba.csv`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/tests/testdata/mca.csv` & `adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/mca.csv`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/tests/testdata/omb.csv` & `adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/omb.csv`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/tests/testdata/tjn.csv` & `adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/tjn.csv`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/tests/testdata/tno.csv` & `adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/tno.csv`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/orbits/variants.py` & `adam_core-0.2.0a1/src/adam_core/orbits/variants.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/propagator/propagator.py` & `adam_core-0.2.0a1/src/adam_core/propagator/propagator.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/propagator/tests/test_propagator.py` & `adam_core-0.2.0a1/src/adam_core/propagator/tests/test_propagator.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/propagator/tests/test_utils.py` & `adam_core-0.2.0a1/src/adam_core/propagator/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/propagator/utils.py` & `adam_core-0.2.0a1/src/adam_core/propagator/utils.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/ray_cluster.py` & `adam_core-0.2.0a1/src/adam_core/ray_cluster.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/tests/test_imports.py` & `adam_core-0.2.0a1/src/adam_core/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/tests/test_ray_cluster.py` & `adam_core-0.2.0a1/src/adam_core/tests/test_ray_cluster.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/time/tests/test_time.py` & `adam_core-0.2.0a1/src/adam_core/time/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/time/time.py` & `adam_core-0.2.0a1/src/adam_core/time/time.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/utils/helpers/data/README.md` & `adam_core-0.2.0a1/src/adam_core/utils/helpers/data/README.md`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/utils/helpers/data/elements_ssb_ec.csv` & `adam_core-0.2.0a1/src/adam_core/utils/helpers/data/elements_ssb_ec.csv`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/utils/helpers/data/elements_ssb_eq.csv` & `adam_core-0.2.0a1/src/adam_core/utils/helpers/data/elements_ssb_eq.csv`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/utils/helpers/data/elements_sun_ec.csv` & `adam_core-0.2.0a1/src/adam_core/utils/helpers/data/elements_sun_ec.csv`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/utils/helpers/data/elements_sun_eq.csv` & `adam_core-0.2.0a1/src/adam_core/utils/helpers/data/elements_sun_eq.csv`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/utils/helpers/data/ephemeris.csv` & `adam_core-0.2.0a1/src/adam_core/utils/helpers/data/ephemeris.csv`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/utils/helpers/data/get_test_data.py` & `adam_core-0.2.0a1/src/adam_core/utils/helpers/data/get_test_data.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/utils/helpers/data/orbits.parquet` & `adam_core-0.2.0a1/src/adam_core/utils/helpers/data/orbits.parquet`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/utils/helpers/data/propagated_orbits.parquet` & `adam_core-0.2.0a1/src/adam_core/utils/helpers/data/propagated_orbits.parquet`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/utils/helpers/observations.py` & `adam_core-0.2.0a1/src/adam_core/utils/helpers/observations.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/utils/helpers/orbits.py` & `adam_core-0.2.0a1/src/adam_core/utils/helpers/orbits.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/utils/helpers/tests/test_observations.py` & `adam_core-0.2.0a1/src/adam_core/utils/helpers/tests/test_observations.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/utils/helpers/tests/test_orbits.py` & `adam_core-0.2.0a1/src/adam_core/utils/helpers/tests/test_orbits.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/utils/mpc.py` & `adam_core-0.2.0a1/src/adam_core/utils/mpc.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/utils/spice.py` & `adam_core-0.2.0a1/src/adam_core/utils/spice.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/utils/tests/test_benchmarks.py` & `adam_core-0.2.0a1/src/adam_core/utils/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/utils/tests/test_mpc.py` & `adam_core-0.2.0a1/src/adam_core/utils/tests/test_mpc.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/src/adam_core/utils/tests/test_spice.py` & `adam_core-0.2.0a1/src/adam_core/utils/tests/test_spice.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.2.0/PKG-INFO` & `adam_core-0.2.0a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adam_core
-Version: 0.2.0
+Version: 0.2.0a1
 Summary: Core libraries for the ADAM platform
 Keywords: astronomy,orbital mechanics,propagation
 Author-Email: Kathleen Kiker <kathleen@b612foundation.org>, Alec Koumjian <alec@b612foundation.org>, Joachim Moeyens <moeyensj@uw.edu>, Spencer Nelson <spencer@b612foundation.org>, Nate Tellis <nate@b612foundation.org>
 License: The MIT License (MIT)
         
         Copyright (c) 2022-2023, Asteroid Institute
         
@@ -91,46 +91,38 @@
 Requires-Dist: mpc-obscodes
 Requires-Dist: naif-de440
 Requires-Dist: naif-leapseconds
 Requires-Dist: naif-eop-high-prec
 Requires-Dist: naif-eop-predict
 Requires-Dist: naif-eop-historical
 Requires-Dist: naif-earth-itrf93
-Requires-Dist: adam-assist>=0.1.1a1; extra == "assist"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pdm; extra == "dev"
 Requires-Dist: pytest-benchmark; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-doctestplus; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
-Provides-Extra: assist
 Provides-Extra: dev
 Description-Content-Type: text/markdown
 
 # adam_core: ADAM Core Utilities
 #### A Python package by the Asteroid Institute, a program of the B612 Foundation
 [![Python 3.9+](https://img.shields.io/badge/Python-3.9%2B-blue)](https://img.shields.io/badge/Python-3.9%2B-blue)
 [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)  
-[![pip - Build, Lint, Test, and Coverage](https://github.com/B612-Asteroid-Institute/adam_core/actions/workflows/pip-build-lint-test-coverage.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/adam_core/actions/workflows/pip-build-lint-test-coverage.yml)
+[![docker - Build, Lint, and Test](https://github.com/B612-Asteroid-Institute/adam_core/actions/workflows/docker-build-lint-test.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/adam_core/actions/workflows/docker-build-lint-test.yml)
+[![pip - Build, Lint, Test, and Coverage](https://github.com/B612-Asteroid-Institute/adam_core/actions/workflows/pip-build-lint-test-coverage.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/adam_core/actions/workflows/pip-build-lint-test-coverage.yml)  
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 
 `adam_core` is used by a variety of library and services at the Asteroid Institute. Sharing these common classes, types, and conversions amongst our tools ensures consistency and accuracy.
 
-## Installation
-
-ADAM Core is available on PyPI
-
-```bash
-pip install adam_core
-```
-
 ## Usage
 
 ### Orbits
 
 To define an orbit:
 ```python
 from adam_core.coordinates import KeplerianCoordinates
@@ -267,35 +259,34 @@
 keplerian_elements = orbits.coordinates.to_keplerian()
 spherical_elements = orbits.coordinates.to_spherical()
 ```
 
 ### Propagator
 The propagator class in `adam_core` provides a generalized interface to the supported orbit integrators and ephemeris generators. The propagator class is designed to be used with the `Orbits` class and can handle multiple orbits and times. 
 
-You will need to install either adam_core[assist], or another compatible propagator in order to use propagation, ephemeris generation, or impact analysis.
+You will need to install either adam_core[pyoorb] or adam_core[assist], or another compatible propagator in order to use propagation, ephemeris generation, or impact analysis.
 
 #### Propagation
-To propagate orbits with ASSIST (here we grab some orbits from Horizons first):
+To propagate orbits with PYOORB (here we grab some orbits from Horizons first):
 
 ```python
 import numpy as np
 from astropy import units as u
 
 from adam_core.orbits.query import query_horizons
-from adam_core.propagator.adam_assist import ASSISTPropagator, download_jpl_ephemeris_files
+from adam_core.propagator import PYOORBPropagator
 from adam_core.time import Timestamp
 
 # Get orbits to propagate
 initial_time = Timestamp.from_mjd([60000.0], scale="tdb")
 object_ids = ["Duende", "Eros", "Ceres"]
 orbits = query_horizons(object_ids, initial_time)
 
-# Download ephemeris files used by propagator and initialize
-download_jpl_ephemeris_files()
-propagator = ASSISTPropagator()
+# Make sure PYOORB is ready
+propagator = PYOORBPropagator()
 
 # Define propagation times
 times = initial_time.from_mjd(initial_time.mjd() + np.arange(0, 100))
 
 # Propagate orbits! This function supports multiprocessing for large
 # propagation jobs.
 propagated_orbits = propagator.propagate_orbits(
@@ -305,27 +296,27 @@
     max_processes=1,
 )
 ```
 
 #### Ephemeris Generation
 Ephemeris generation requires a propagator that implements the EphemerisMixin interface. This is currently only implemented by the PYOORB propagator. The ephemeris generator will automatically map the propagated covariance matrices to the sky-plane.
 
-You will need to install adam-pyoorb in order to use the ephemeris generator, which is currently only available on GitHub.
+You will need to install adam-pyoorb in order to use the ephemeris generator.
 
 ```sh
-pip install git+https://github.com/B612-Asteroid-Institute/adam-pyoorb.git
+pip install adam-core[pyoorb]
 ```
 
 
 ```python
 import numpy as np
 from astropy import units as u
 
 from adam_core.orbits.query import query_horizons
-from adam_core.propagator.adam_pyoorb import PYOORBPropagator
+from adam_core.propagator import PYOORBPropagator
 from adam_core.observers import Observers
 from adam_core.time import Timestamp
 
 # Get orbits to propagate
 initial_time = Timestamp.from_mjd([60000.0], scale="tdb")
 object_ids = ["Duende", "Eros", "Ceres"]
 orbits = query_horizons(object_ids, initial_time)
@@ -402,15 +393,15 @@
 then automatically map the propagated covariance matrices to the sky-plane.
 
 ```python
 import numpy as np
 from astropy import units as u
 
 from adam_core.orbits.query import query_sbdb
-from adam_core.propagator.adam_pyoorb import PYOORBPropagator
+from adam_core.propagator import PYOORBPropagator
 from adam_core.observers import Observers
 from adam_core.dynamics import generate_ephemeris_2body
 from adam_core.time import Timestamp
 
 # Get orbits to propagate
 object_ids = ["Duende", "Eros", "Ceres"]
 orbits = query_sbdb(object_ids)
@@ -461,8 +452,29 @@
 ├── constants.py  # Shared constants
 ├── coordinates   # Coordinate classes and transformations
 ├── dynamics      # Numerical solutions
 ├── orbits        # Orbits class and query utilities
 └── utils         # Utility classes like Indexable or conversions like times_from_df
 ```
 
+## Installation
 
+ADAM Core is available on PyPI
+
+```bash
+pip install adam_core
+```
+
+## Development
+
+Development is made easy with our Docker container environment.
+
+```bash
+# Build the container
+docker compose build
+
+# Run tests in the container
+docker compose run adam_core pytest .
+
+# Run a shell in the container
+docker compose run adam_core bash
+```
```

