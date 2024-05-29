# Comparing `tmp/Navix-0.4.0.tar.gz` & `tmp/navix-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Navix-0.4.0.tar", last modified: Fri Mar  8 16:22:49 2024, max compression
+gzip compressed data, was "navix-0.5.0.tar", last modified: Wed May 29 10:00:46 2024, max compression
```

## Comparing `Navix-0.4.0.tar` & `navix-0.5.0.tar`

### file list

```diff
@@ -1,113 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 16:22:49.662503 Navix-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 16:22:49.646503 Navix-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 16:22:49.650503 Navix-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-08 16:22:43.000000 Navix-0.4.0/.github/workflows/CD.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-03-08 16:22:43.000000 Navix-0.4.0/.github/workflows/CI.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-03-08 16:22:43.000000 Navix-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-08 16:22:43.000000 Navix-0.4.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-08 16:22:43.000000 Navix-0.4.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-08 16:22:43.000000 Navix-0.4.0/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-03-08 16:22:43.000000 Navix-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-08 16:22:43.000000 Navix-0.4.0/NOTICE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 16:22:49.662503 Navix-0.4.0/Navix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20222 2024-03-08 16:22:49.000000 Navix-0.4.0/Navix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-03-08 16:22:49.000000 Navix-0.4.0/Navix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 16:22:49.000000 Navix-0.4.0/Navix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-08 16:22:49.000000 Navix-0.4.0/Navix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-08 16:22:49.000000 Navix-0.4.0/Navix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20222 2024-03-08 16:22:49.662503 Navix-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-03-08 16:22:43.000000 Navix-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 16:22:49.650503 Navix-0.4.0/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 16:22:49.658503 Navix-0.4.0/assets/sprites/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/ball_blue.png
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/ball_green.png
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/ball_grey.png
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/ball_purple.png
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/ball_red.png
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/ball_yellow.png
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/box_blue.png
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/box_green.png
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/box_grey.png
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/box_purple.png
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/box_red.png
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/box_yellow.png
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/door_closed_blue.png
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/door_closed_green.png
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/door_closed_grey.png
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/door_closed_purple.png
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/door_closed_red.png
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/door_closed_yellow.png
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/door_locked_blue.png
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/door_locked_green.png
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/door_locked_grey.png
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/door_locked_purple.png
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/door_locked_red.png
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/door_locked_yellow.png
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/door_open_blue.png
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/door_open_green.png
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/door_open_grey.png
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/door_open_purple.png
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/door_open_red.png
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/door_open_yellow.png
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/floor.png
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/goal.png
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/key_blue.png
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/key_green.png
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/key_grey.png
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/key_purple.png
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/key_red.png
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/key_yellow.png
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/lava.png
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/player_east.png
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/player_north.png
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/player_south.png
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/player_west.png
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-08 16:22:43.000000 Navix-0.4.0/assets/sprites/wall.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 16:22:49.658503 Navix-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-03-08 16:22:43.000000 Navix-0.4.0/docs/design_notes.md
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-03-08 16:22:43.000000 Navix-0.4.0/docs/performance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 16:22:49.658503 Navix-0.4.0/navix/
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-08 16:22:43.000000 Navix-0.4.0/navix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-03-08 16:22:43.000000 Navix-0.4.0/navix/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-03-08 16:22:43.000000 Navix-0.4.0/navix/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-03-08 16:22:43.000000 Navix-0.4.0/navix/components.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-08 16:22:43.000000 Navix-0.4.0/navix/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-03-08 16:22:43.000000 Navix-0.4.0/navix/entities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 16:22:49.658503 Navix-0.4.0/navix/environments/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-08 16:22:43.000000 Navix-0.4.0/navix/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-03-08 16:22:43.000000 Navix-0.4.0/navix/environments/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-03-08 16:22:43.000000 Navix-0.4.0/navix/environments/keydoor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-03-08 16:22:43.000000 Navix-0.4.0/navix/environments/room.py
--rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-03-08 16:22:43.000000 Navix-0.4.0/navix/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-03-08 16:22:43.000000 Navix-0.4.0/navix/observations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 16:22:49.658503 Navix-0.4.0/navix/rendering/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-08 16:22:43.000000 Navix-0.4.0/navix/rendering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-03-08 16:22:43.000000 Navix-0.4.0/navix/rendering/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-03-08 16:22:43.000000 Navix-0.4.0/navix/rendering/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-03-08 16:22:43.000000 Navix-0.4.0/navix/spaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-03-08 16:22:43.000000 Navix-0.4.0/navix/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-08 16:22:43.000000 Navix-0.4.0/navix/terminations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-03-08 16:22:43.000000 Navix-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-08 16:22:43.000000 Navix-0.4.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 16:22:49.662503 Navix-0.4.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      808 2024-03-08 16:22:43.000000 Navix-0.4.0/scripts/release.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 16:22:49.662503 Navix-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 16:22:49.662503 Navix-0.4.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 16:22:49.662503 Navix-0.4.0/tests/performance/
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-03-08 16:22:43.000000 Navix-0.4.0/tests/performance/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-03-08 16:22:43.000000 Navix-0.4.0/tests/performance/minigrid.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-08 16:22:43.000000 Navix-0.4.0/tests/performance/minigrid_report.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-03-08 16:22:43.000000 Navix-0.4.0/tests/performance/observations.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-08 16:22:43.000000 Navix-0.4.0/tests/performance/observations_keydoor_report.txt
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-08 16:22:43.000000 Navix-0.4.0/tests/performance/observations_room_report.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-08 16:22:43.000000 Navix-0.4.0/tests/performance/profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-03-08 16:22:43.000000 Navix-0.4.0/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-08 16:22:43.000000 Navix-0.4.0/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-03-08 16:22:43.000000 Navix-0.4.0/tests/test_environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-03-08 16:22:43.000000 Navix-0.4.0/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-03-08 16:22:43.000000 Navix-0.4.0/tests/test_observations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-08 16:22:43.000000 Navix-0.4.0/tests/test_spaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-03-08 16:22:43.000000 Navix-0.4.0/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-03-08 16:22:43.000000 Navix-0.4.0/tests/test_terminations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:00:46.619430 navix-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:00:46.595430 navix-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:00:46.599430 navix-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-29 10:00:40.000000 navix-0.5.0/.github/workflows/CD.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-29 10:00:40.000000 navix-0.5.0/.github/workflows/CI.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-29 10:00:40.000000 navix-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 10:00:40.000000 navix-0.5.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-29 10:00:40.000000 navix-0.5.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-29 10:00:40.000000 navix-0.5.0/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-05-29 10:00:40.000000 navix-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-29 10:00:40.000000 navix-0.5.0/NOTICE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:00:46.619430 navix-0.5.0/Navix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20222 2024-05-29 10:00:46.000000 navix-0.5.0/Navix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-29 10:00:46.000000 navix-0.5.0/Navix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:00:46.000000 navix-0.5.0/Navix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-29 10:00:46.000000 navix-0.5.0/Navix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-29 10:00:46.000000 navix-0.5.0/Navix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20222 2024-05-29 10:00:46.619430 navix-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-05-29 10:00:40.000000 navix-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:00:46.599430 navix-0.5.0/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-29 10:00:40.000000 navix-0.5.0/assets/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-29 10:00:40.000000 navix-0.5.0/assets/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:00:46.607430 navix-0.5.0/assets/sprites/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/ball_blue.png
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/ball_green.png
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/ball_grey.png
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/ball_purple.png
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/ball_red.png
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/ball_yellow.png
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/box_blue.png
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/box_green.png
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/box_grey.png
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/box_purple.png
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/box_red.png
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/box_yellow.png
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/door_closed_blue.png
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/door_closed_green.png
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/door_closed_grey.png
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/door_closed_purple.png
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/door_closed_red.png
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/door_closed_yellow.png
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/door_locked_blue.png
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/door_locked_green.png
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/door_locked_grey.png
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/door_locked_purple.png
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/door_locked_red.png
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/door_locked_yellow.png
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/door_open_blue.png
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/door_open_green.png
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/door_open_grey.png
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/door_open_purple.png
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/door_open_red.png
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/door_open_yellow.png
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/floor.png
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/goal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/key_blue.png
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/key_green.png
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/key_grey.png
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/key_purple.png
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/key_red.png
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/key_yellow.png
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/lava.png
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/player_east.png
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/player_north.png
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/player_south.png
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/player_west.png
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-29 10:00:40.000000 navix-0.5.0/assets/sprites/wall.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:00:46.607430 navix-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-29 10:00:40.000000 navix-0.5.0/docs/design_notes.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-29 10:00:40.000000 navix-0.5.0/docs/performance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:00:46.611430 navix-0.5.0/navix/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-29 10:00:40.000000 navix-0.5.0/navix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-29 10:00:40.000000 navix-0.5.0/navix/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-29 10:00:40.000000 navix-0.5.0/navix/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-29 10:00:40.000000 navix-0.5.0/navix/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-29 10:00:40.000000 navix-0.5.0/navix/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-05-29 10:00:40.000000 navix-0.5.0/navix/entities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:00:46.615430 navix-0.5.0/navix/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-29 10:00:40.000000 navix-0.5.0/navix/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-29 10:00:40.000000 navix-0.5.0/navix/environments/crossings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-29 10:00:40.000000 navix-0.5.0/navix/environments/dist_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-29 10:00:40.000000 navix-0.5.0/navix/environments/dynamic_obstacles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-29 10:00:40.000000 navix-0.5.0/navix/environments/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-29 10:00:40.000000 navix-0.5.0/navix/environments/four_rooms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-05-29 10:00:40.000000 navix-0.5.0/navix/environments/go_to_door.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-05-29 10:00:40.000000 navix-0.5.0/navix/environments/key_corridor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-29 10:00:40.000000 navix-0.5.0/navix/environments/key_door.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-29 10:00:40.000000 navix-0.5.0/navix/environments/lava_gap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-29 10:00:40.000000 navix-0.5.0/navix/environments/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-29 10:00:40.000000 navix-0.5.0/navix/environments/room.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-29 10:00:40.000000 navix-0.5.0/navix/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11519 2024-05-29 10:00:40.000000 navix-0.5.0/navix/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-29 10:00:40.000000 navix-0.5.0/navix/observations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:00:46.615430 navix-0.5.0/navix/rendering/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-29 10:00:40.000000 navix-0.5.0/navix/rendering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-05-29 10:00:40.000000 navix-0.5.0/navix/rendering/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-29 10:00:40.000000 navix-0.5.0/navix/rendering/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-29 10:00:40.000000 navix-0.5.0/navix/rewards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-29 10:00:40.000000 navix-0.5.0/navix/spaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-29 10:00:40.000000 navix-0.5.0/navix/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-29 10:00:40.000000 navix-0.5.0/navix/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-29 10:00:40.000000 navix-0.5.0/navix/terminations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-29 10:00:40.000000 navix-0.5.0/navix/transitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-29 10:00:40.000000 navix-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-29 10:00:40.000000 navix-0.5.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:00:46.615430 navix-0.5.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      808 2024-05-29 10:00:40.000000 navix-0.5.0/scripts/release.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 10:00:46.619430 navix-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:00:46.615430 navix-0.5.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:00:46.619430 navix-0.5.0/tests/performance/
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-29 10:00:40.000000 navix-0.5.0/tests/performance/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-29 10:00:40.000000 navix-0.5.0/tests/performance/minigrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-29 10:00:40.000000 navix-0.5.0/tests/performance/minigrid_report.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-29 10:00:40.000000 navix-0.5.0/tests/performance/observations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-29 10:00:40.000000 navix-0.5.0/tests/performance/observations_keydoor_report.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-29 10:00:40.000000 navix-0.5.0/tests/performance/observations_room_report.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-29 10:00:40.000000 navix-0.5.0/tests/performance/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13695 2024-05-29 10:00:40.000000 navix-0.5.0/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-29 10:00:40.000000 navix-0.5.0/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-29 10:00:40.000000 navix-0.5.0/tests/test_environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-29 10:00:40.000000 navix-0.5.0/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-05-29 10:00:40.000000 navix-0.5.0/tests/test_observations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-29 10:00:40.000000 navix-0.5.0/tests/test_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-29 10:00:40.000000 navix-0.5.0/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-29 10:00:40.000000 navix-0.5.0/tests/test_terminations.py
```

### Comparing `Navix-0.4.0/.github/workflows/CD.yml` & `navix-0.5.0/.github/workflows/CD.yml`

 * *Files identical despite different names*

### Comparing `Navix-0.4.0/.github/workflows/CI.yml` & `navix-0.5.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `Navix-0.4.0/.gitignore` & `navix-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `Navix-0.4.0/COPYRIGHT` & `navix-0.5.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `Navix-0.4.0/LICENSE` & `navix-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Navix-0.4.0/Navix.egg-info/PKG-INFO` & `navix-0.5.0/Navix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Navix
-Version: 0.4.0
+Version: 0.5.0
 Summary: Accelerated gridworld navigation with JAX for deep reinforcement learning
 Author-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 Maintainer-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `Navix-0.4.0/Navix.egg-info/SOURCES.txt` & `navix-0.5.0/Navix.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -65,22 +65,34 @@
 docs/performance.py
 navix/__init__.py
 navix/_version.py
 navix/actions.py
 navix/components.py
 navix/config.py
 navix/entities.py
+navix/events.py
 navix/grid.py
 navix/observations.py
+navix/rewards.py
 navix/spaces.py
+navix/states.py
 navix/tasks.py
 navix/terminations.py
+navix/transitions.py
 navix/environments/__init__.py
+navix/environments/crossings.py
+navix/environments/dist_shift.py
+navix/environments/dynamic_obstacles.py
 navix/environments/environment.py
-navix/environments/keydoor.py
+navix/environments/four_rooms.py
+navix/environments/go_to_door.py
+navix/environments/key_corridor.py
+navix/environments/key_door.py
+navix/environments/lava_gap.py
+navix/environments/registry.py
 navix/environments/room.py
 navix/rendering/__init__.py
 navix/rendering/cache.py
 navix/rendering/registry.py
 scripts/release.sh
 tests/test_actions.py
 tests/test_entities.py
```

### Comparing `Navix-0.4.0/PKG-INFO` & `navix-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Navix
-Version: 0.4.0
+Version: 0.5.0
 Summary: Accelerated gridworld navigation with JAX for deep reinforcement learning
 Author-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 Maintainer-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `Navix-0.4.0/README.md` & `navix-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `Navix-0.4.0/assets/LICENSE` & `navix-0.5.0/assets/LICENSE`

 * *Files identical despite different names*

### Comparing `Navix-0.4.0/docs/design_notes.md` & `navix-0.5.0/docs/design_notes.md`

 * *Files identical despite different names*

### Comparing `Navix-0.4.0/docs/performance.py` & `navix-0.5.0/docs/performance.py`

 * *Files identical despite different names*

### Comparing `Navix-0.4.0/navix/__init__.py` & `navix-0.5.0/navix/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 
 from . import (
     actions,
     components,
     entities,
     grid,
     observations,
-    tasks,
+    rewards,
     environments,
     terminations,
     config,
     spaces,
-    rendering
+    rendering,
+    transitions,
+    events,
 )
```

### Comparing `Navix-0.4.0/navix/_version.py` & `navix-0.5.0/navix/rendering/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,9 +14,8 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
-__version__ = "0.4.0"
-__version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
+from . import cache, registry
```

### Comparing `Navix-0.4.0/navix/actions.py` & `navix-0.5.0/navix/actions.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,31 +12,33 @@
 
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-
 from __future__ import annotations
+from typing import Tuple
 
 import jax
-import jax.numpy as jnp
 from jax import Array
+import jax.numpy as jnp
+import jax.tree_util as jtu
 
-from .entities import Entities, State
+from .entities import Entities
+from .states import EventsManager, State
 from .components import DISCARD_PILE_COORDS
 from .grid import translate, rotate, positions_equal
 
 
 class Directions:
-    EAST = 0
-    SOUTH = 1
-    WEST = 2
-    NORTH = 3
+    EAST = jnp.asarray(0)
+    SOUTH = jnp.asarray(1)
+    WEST = jnp.asarray(2)
+    NORTH = jnp.asarray(3)
 
 
 def _rotate(state: State, spin: int) -> State:
     if Entities.PLAYER not in state.entities:
         return state
 
     player = state.get_player(idx=0)
@@ -48,49 +50,50 @@
     player = player.replace(direction=direction)
 
     state = state.set_player(player)
 
     return state
 
 
-def _walkable(state: State, position: Array) -> Array:
+def _can_walk_there(state: State, position: Array) -> Tuple[Array, EventsManager]:
     # according to the grid
     walkable = jnp.equal(state.grid[tuple(position)], 0)
+    events = jax.lax.cond(
+        walkable,
+        lambda: state.events,
+        lambda: state.events.record_grid_hit(position),
+    )
 
     for k in state.entities:
+        same_position = positions_equal(state.entities[k].position, position)
+        events = jax.lax.cond(
+            jnp.any(same_position),
+            lambda x: x.record_walk_into(state.entities[k], position),
+            lambda x: x,
+            events,
+        )
         obstructs = jnp.logical_and(
-            jnp.logical_not(state.entities[k].walkable),
-            positions_equal(state.entities[k].position, position),
+            jnp.logical_not(state.entities[k].walkable), same_position
         )
         walkable = jnp.logical_and(walkable, jnp.any(jnp.logical_not(obstructs)))
-    return jnp.asarray(walkable, dtype=jnp.bool_)
+    return jnp.asarray(walkable, dtype=jnp.bool_), events
 
 
 def _move(state: State, direction: Array) -> State:
     if Entities.PLAYER not in state.entities:
         return state
 
     player = state.get_player(idx=0)
     new_position = translate(player.position, direction)
-    can_move = _walkable(state, new_position)
+    can_move, events = _can_walk_there(state, new_position)
     new_position = jnp.where(can_move, new_position, player.position)
+    # update structs
     player = player.replace(position=new_position)
     state = state.set_player(player)
-    return state
-
-
-def undefined(state: State) -> State:
-    # this is problematic because jax.lax.switch evaluates
-    # all *python* branches (no XLA computation is performed)
-    # even though only one is selected
-    # one option is the following, but this breaks type checking
-    # def raise_error(state: State) -> State:
-    #     raise ValueError("Undefined action")
-    # jax.debug.callback(raise_error)
-    raise ValueError("Undefined action")
+    return state.replace(events=events)
 
 
 def noop(state: State) -> State:
     return state
 
 
 def rotate_cw(state: State) -> State:
@@ -138,19 +141,35 @@
 
     # update player's pocket, if the pocket has something else, we overwrite it
     key = jnp.sum(keys.id * key_found, dtype=jnp.int32)
     player = jax.lax.cond(
         jnp.any(key_found), lambda: player.replace(pocket=key), lambda: player
     )
 
+    # update events
+    events = jax.lax.cond(
+        jnp.any(key_found),
+        lambda: state.events.record_key_pickup(keys, position_in_front),
+        lambda: state.events,
+    )
+
     state = state.set_player(player)
     state = state.set_keys(keys)
+    state = state.set_events(events)
     return state
 
 
+def drop(state: State) -> State:
+    raise NotImplementedError()
+
+
+def toggle(state: State) -> State:
+    raise NotImplementedError()
+
+
 def open(state: State) -> State:
     """Unlocks and opens an openable object (like a door) if possible"""
 
     if Entities.DOOR not in state.entities:
         return state
 
     # get the tile in front of the player
@@ -175,26 +194,53 @@
 
     # remove key from player's pocket
     pocket = jnp.asarray(player.pocket * jnp.any(can_open), dtype=jnp.int32)
     player = jax.lax.cond(
         jnp.any(can_open), lambda: player.replace(pocket=pocket), lambda: player
     )
 
+    # update events
+    events = jax.lax.cond(
+        jnp.any(do_open),
+        lambda: state.events.record_door_opening(doors, position_in_front),
+        lambda: state.events,
+    )
+
     state = state.set_player(player)
     state = state.set_doors(doors)
+    state = state.set_events(events)
 
     return state
 
 
-# TODO(epignatelli): a mutable dictionary here is dangerous
-ACTIONS = {
-    # -1: undefined,
-    0: noop,
-    1: rotate_cw,
-    2: rotate_ccw,
-    3: forward,
-    4: right,
-    5: backward,
-    6: left,
-    7: pickup,
-    8: open,
-}
+def done(state: State) -> State:
+    return state
+
+
+# DEFAULT_ACTION_SET = (
+#     rotate_ccw,
+#     rotate_cw,
+#     forward,
+#     pickup,
+#     drop,
+#     toggle,
+#     done
+# )
+"""Default action set from Minigrid. See
+https://github.com/Farama-Foundation/Minigrid/blob/master/minigrid/core/actions.py"""
+
+
+COMPLETE_ACTION_SET = (
+    noop,
+    rotate_cw,
+    rotate_ccw,
+    forward,
+    right,
+    backward,
+    left,
+    pickup,
+    open,
+    done,
+)
+
+
+DEFAULT_ACTION_SET = COMPLETE_ACTION_SET
```

### Comparing `Navix-0.4.0/navix/components.py` & `navix-0.5.0/navix/components.py`

 * *Files identical despite different names*

### Comparing `Navix-0.4.0/navix/entities.py` & `navix-0.5.0/navix/entities.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
-import dataclasses
-from typing import Dict, Tuple, TypeVar
+from typing import Tuple, TypeVar
 
 import jax
 from jax import Array
 import jax.numpy as jnp
 from flax import struct
 
 
@@ -15,57 +14,58 @@
     HasTag,
     Stochastic,
     Openable,
     Pickable,
     Holder,
     HasSprite,
 )
-from .rendering.cache import RenderingCache
-from .rendering.registry import PALETTE, SPRITES_REGISTRY
-from .config import config
+from .rendering.registry import SPRITES_REGISTRY
 
 T = TypeVar("T", bound="Entity")
 
 
 class Entities(struct.PyTreeNode):
     WALL: str = struct.field(pytree_node=False, default="wall")
     FLOOR: str = struct.field(pytree_node=False, default="floor")
     PLAYER: str = struct.field(pytree_node=False, default="player")
     GOAL: str = struct.field(pytree_node=False, default="goal")
     KEY: str = struct.field(pytree_node=False, default="key")
     DOOR: str = struct.field(pytree_node=False, default="door")
+    LAVA: str = struct.field(pytree_node=False, default="lava")
+    BALL: str = struct.field(pytree_node=False, default="ball")
+    BOX: str = struct.field(pytree_node=False, default="box")
 
 
 class Entity(Positionable, HasTag, HasSprite):
     """Entities are components that can be placed in the environment"""
 
-    def __post_init__(self) -> None:
-        if not config.ARRAY_CHECKS_ENABLED:
-            return
-        # Check that all fields have the same batch size
-        fields = self.__dataclass_fields__
-        batch_size = self.shape[0:]
-        for path, leaf in jax.tree_util.tree_leaves_with_path(self):
-            name = path[0].name
-            default_ndim = len(fields[name].metadata["shape"])
-            prefix = int(default_ndim != leaf.ndim)
-            leaf_batch_size = leaf.shape[:prefix]
-            assert (
-                leaf_batch_size == batch_size
-            ), f"Expected {name} to have batch size {batch_size}, got {leaf_batch_size} instead"
-
-    def check_ndim(self, batched: bool = False) -> None:
-        if not config.ARRAY_CHECKS_ENABLED:
-            return
-        for field in dataclasses.fields(self):
-            value = getattr(self, field.name)
-            default_ndim = len(field.metadata["shape"])
-            assert (
-                value.ndim == default_ndim + batched
-            ), f"Expected {field.name} to have ndim {default_ndim - batched}, got {value.ndim} instead"
+    # def __post_init__(self) -> None:
+    #     if not config.ARRAY_CHECKS_ENABLED:
+    #         return
+    #     # Check that all fields have the same batch size
+    #     fields = self.__dataclass_fields__
+    #     batch_size = self.shape[0:]
+    #     for path, leaf in jax.tree_util.tree_leaves_with_path(self):
+    #         name = path[0].name
+    #         default_ndim = len(fields[name].metadata["shape"])
+    #         prefix = int(default_ndim != leaf.ndim)
+    #         leaf_batch_size = leaf.shape[:prefix]
+    #         assert (
+    #             leaf_batch_size == batch_size
+    #         ), f"Expected {name} to have batch size {batch_size}, got {leaf_batch_size} instead"
+
+    # def check_ndim(self, batched: bool = False) -> None:
+    #     if not config.ARRAY_CHECKS_ENABLED:
+    #         return
+    #     for field in dataclasses.fields(self):
+    #         value = getattr(self, field.name)
+    #         default_ndim = len(field.metadata["shape"])
+    #         assert (
+    #             value.ndim == default_ndim + batched
+    #         ), f"Expected {field.name} to have ndim {default_ndim - batched}, got {value.ndim} instead"
 
     def __getitem__(self: T, idx) -> T:
         return jax.tree_util.tree_map(lambda x: x[idx], self)
 
     @property
     def name(self) -> str:
         return self.__class__.__name__
@@ -272,74 +272,111 @@
         return jnp.broadcast_to(jnp.asarray(5), self.shape)
 
     @property
     def locked(self) -> Array:
         return self.requires != jnp.asarray(-1)
 
 
-class State(struct.PyTreeNode):
-    """The Markovian state of the environment"""
+class Lava(Entity):
+    """Goals are entities that can be reached by the player"""
 
-    key: Array
-    """The random number generator state"""
-    grid: Array
-    """The base map of the environment that remains constant throughout the training"""
-    cache: RenderingCache
-    """The rendering cache to speed up rendering"""
-    entities: Dict[str, Entity] = struct.field(default_factory=dict)
-    """The entities in the environment, indexed via entity type string representation.
-    Batched over the number of entities for each type"""
+    @classmethod
+    def create(
+        cls,
+        position: Array,
+    ) -> Lava:
+        return cls(position=position)
 
-    def get_entity(self, entity_enum: str) -> Entity:
-        return self.entities[entity_enum]
+    @property
+    def walkable(self) -> Array:
+        return jnp.broadcast_to(jnp.asarray(True), self.shape)
 
-    def set_entity(self, entity_enum: str, entity: Entity) -> State:
-        self.entities[entity_enum] = entity
-        return self
+    @property
+    def transparent(self) -> Array:
+        return jnp.broadcast_to(jnp.asarray(True), self.shape)
 
-    def get_walls(self) -> Wall:
-        return self.entities.get(Entities.WALL, Wall())  # type: ignore
+    @property
+    def sprite(self) -> Array:
+        sprite = SPRITES_REGISTRY[Entities.LAVA]
+        if sprite.ndim == 3:
+            # batch it
+            sprite = sprite[None]
+        # ensure same batch size
+        if sprite.shape[0] != self.position.shape[0]:
+            sprite = jnp.broadcast_to(sprite, (*self.shape, *sprite.shape[1:]))
+        return sprite
 
-    def set_walls(self, walls: Wall) -> State:
-        self.entities[Entities.WALL] = walls
-        return self
+    @property
+    def tag(self) -> Array:
+        return jnp.broadcast_to(jnp.asarray(6), self.shape)
 
-    def get_player(self, idx: int = 0) -> Player:
-        return self.entities[Entities.PLAYER][idx]  # type: ignore
 
-    def set_player(self, player: Player, idx: int = 0) -> State:
-        # TODO(epignatelli): this is a hack and won't work in multi-agent settings
-        self.entities[Entities.PLAYER] = player[None]
-        return self
+class Ball(Entity, HasColour, Stochastic):
+    """Goals are entities that can be reached by the player"""
 
-    def get_goals(self) -> Goal:
-        return self.entities[Entities.GOAL]  # type: ignore
+    @classmethod
+    def create(
+        cls,
+        position: Array,
+        colour: Array,
+        probability: Array,
+    ) -> Ball:
+        return cls(position=position, colour=colour, probability=probability)
 
-    def set_goals(self, goals: Goal) -> State:
-        self.entities[Entities.GOAL] = goals
-        return self
+    @property
+    def walkable(self) -> Array:
+        return jnp.broadcast_to(jnp.asarray(False), self.shape)
 
-    def get_keys(self) -> Key:
-        return self.entities[Entities.KEY]  # type: ignore
+    @property
+    def transparent(self) -> Array:
+        return jnp.broadcast_to(jnp.asarray(True), self.shape)
 
-    def set_keys(self, keys: Key) -> State:
-        self.entities[Entities.KEY] = keys
-        return self
+    @property
+    def sprite(self) -> Array:
+        sprite = SPRITES_REGISTRY[Entities.BALL][self.colour]
+        if sprite.ndim == 3:
+            # batch it
+            sprite = sprite[None]
+        # ensure same batch size
+        if sprite.shape[0] != self.position.shape[0]:
+            sprite = jnp.broadcast_to(sprite, (*self.shape, *sprite.shape[1:]))
+        return sprite
+
+    @property
+    def tag(self) -> Array:
+        return jnp.broadcast_to(jnp.asarray(7), self.shape)
 
-    def get_doors(self) -> Door:
-        return self.entities[Entities.DOOR]  # type: ignore
 
-    def set_doors(self, doors: Door) -> State:
-        self.entities[Entities.DOOR] = doors
-        return self
+class Box(Entity, HasColour, Holder):
+    """Goals are entities that can be reached by the player"""
+
+    @classmethod
+    def create(
+        cls,
+        position: Array,
+        colour: Array,
+        pocket: Array,
+    ) -> Box:
+        return cls(position=position, colour=colour, pocket=pocket)
 
-    def get_positions(self) -> Array:
-        return jnp.concatenate([self.entities[k].position for k in self.entities])
+    @property
+    def walkable(self) -> Array:
+        return jnp.broadcast_to(jnp.asarray(False), self.shape)
 
-    def get_tags(self) -> Array:
-        return jnp.concatenate([self.entities[k].tag for k in self.entities])
+    @property
+    def transparent(self) -> Array:
+        return jnp.broadcast_to(jnp.asarray(True), self.shape)
 
-    def get_sprites(self) -> Array:
-        return jnp.concatenate([self.entities[k].sprite for k in self.entities])
+    @property
+    def sprite(self) -> Array:
+        sprite = SPRITES_REGISTRY[Entities.BOX][self.colour]
+        if sprite.ndim == 3:
+            # batch it
+            sprite = sprite[None]
+        # ensure same batch size
+        if sprite.shape[0] != self.position.shape[0]:
+            sprite = jnp.broadcast_to(sprite, (*self.shape, *sprite.shape[1:]))
+        return sprite
 
-    def get_transparency(self) -> Array:
-        return jnp.concatenate([self.entities[k].transparent for k in self.entities])
+    @property
+    def tag(self) -> Array:
+        return jnp.broadcast_to(jnp.asarray(8), self.shape)
```

### Comparing `Navix-0.4.0/navix/environments/__init__.py` & `navix-0.5.0/navix/_version.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,13 +14,9 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
-from __future__ import annotations
-
-
-from .environment import Environment, Timestep
-from .room import Room
-from .keydoor import KeyDoor
+__version__ = "0.5.0"
+__version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
```

### Comparing `Navix-0.4.0/navix/environments/environment.py` & `navix-0.5.0/navix/environments/environment.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import abc
-from typing import Any, Callable, Dict
+from typing import Any, Callable, Dict, Tuple
 import jax
 import jax.numpy as jnp
 from jax import Array
 from flax import struct
 
 
-from .. import tasks, terminations, observations
+from .. import rewards, terminations, observations, transitions
 from ..rendering.cache import RenderingCache, TILE_SIZE
-from ..entities import State
-from ..actions import ACTIONS
+from ..states import State
+from ..actions import DEFAULT_ACTION_SET
 from ..spaces import Space, Discrete, Continuous
 
 
 class StepType(struct.PyTreeNode):
     TRANSITION = jnp.asarray(0)
     """Standard timestep transition: the episode continues"""
     TRUNCATION = jnp.asarray(1)
@@ -61,23 +61,30 @@
     """Additional information about the environment. Useful for accumulations (e.g. returns)"""
 
 
 class Environment(struct.PyTreeNode):
     height: int = struct.field(pytree_node=False)
     width: int = struct.field(pytree_node=False)
     max_steps: int = struct.field(pytree_node=False)
-    gamma: float = struct.field(pytree_node=False, default=1.0)
+    gamma: float = struct.field(pytree_node=False, default=0.99)
+    penality_coeff: float = struct.field(pytree_node=False, default=0.9)
     observation_fn: Callable[[State], Array] = struct.field(
         pytree_node=False, default=observations.none
     )
     reward_fn: Callable[[State, Array, State], Array] = struct.field(
-        pytree_node=False, default=tasks.navigation
+        pytree_node=False, default=rewards.DEFAULT_TASK
     )
     termination_fn: Callable[[State, Array, State], Array] = struct.field(
-        pytree_node=False, default=terminations.on_navigation_completion
+        pytree_node=False, default=terminations.DEFAULT_TERMINATION
+    )
+    transitions_fn: Callable[
+        [State, Array, Tuple[Callable[[State], State], ...]], State
+    ] = struct.field(pytree_node=False, default=transitions.DEFAULT_TRANSITION)
+    action_set: Tuple[Callable[[State], State], ...] = struct.field(
+        pytree_node=False, default=DEFAULT_ACTION_SET
     )
 
     @property
     def observation_space(self) -> Space:
         if self.observation_fn == observations.none:
             return Continuous(shape=())
         elif self.observation_fn == observations.categorical:
@@ -103,44 +110,69 @@
                 "Unknown observation space for observation function {}".format(
                     self.observation_fn
                 )
             )
 
     @property
     def action_space(self) -> Space:
-        return Discrete(len(ACTIONS))
+        return Discrete(len(self.action_set))
 
     @abc.abstractmethod
     def reset(self, key: Array, cache: RenderingCache | None = None) -> Timestep:
         raise NotImplementedError()
 
-    def _step(self, timestep: Timestep, action: Array, actions_set=ACTIONS) -> Timestep:
+    def step(self, timestep: Timestep, action: Array) -> Timestep:
+        # autoreset if necessary: 0 = transition, 1 = truncation, 2 = termination
+        should_reset = timestep.step_type > 0
+        return jax.lax.cond(
+            should_reset,
+            lambda timestep: self._reset(timestep.state.key, timestep.state.cache),
+            lambda timestep: self._step(timestep, action),
+            timestep,
+        )
+
+    def _reset(self, key: Array, cache: RenderingCache | None = None) -> Timestep:
+        k1, k2 = jax.random.split(key)
+        timestep = self.reset(k1, cache)
+        return timestep.replace(state=timestep.state.replace(key=k2))
+
+    def _step(self, timestep: Timestep, action: Array) -> Timestep:
+        """
+        Args:
+            timestep (Timestep): The timestep at time $t$.
+            action (Array): The action $a_t \\sim \\pi(A_t | s_t)$
+        Returns:
+            (Timestep): The timestep at time $t + 1$
+        """
         # update agents
-        state = jax.lax.switch(action, actions_set.values(), timestep.state)
+        state = self.transitions_fn(timestep.state, action, self.action_set)
+        t = timestep.t + 1
+
+        # calculate termination
+        step_type = self.termination(timestep.state, action, state, timestep.t + 1)
+
+        # calculate reward
+        reward = self.reward(timestep.state, action, state)
+        reward = jax.lax.cond(
+            step_type == StepType.TERMINATION,
+            lambda reward: reward - self.penality_coeff * (t / self.max_steps),
+            lambda reward: reward,
+            reward,
+        )
 
         # build timestep
         return Timestep(
-            t=timestep.t + 1,
+            t=t,
             state=state,
             action=jnp.asarray(action),
-            reward=self.reward(timestep.state, action, state),
-            step_type=self.termination(timestep.state, action, state, timestep.t + 1),
+            reward=reward,
+            step_type=step_type,
             observation=self.observation(state),
         )
 
-    def step(self, timestep: Timestep, action: Array, actions_set=ACTIONS) -> Timestep:
-        # autoreset if necessary: 0 = transition, 1 = truncation, 2 = termination
-        should_reset = timestep.step_type > 0
-        return jax.lax.cond(
-            should_reset,
-            lambda timestep: self.reset(timestep.state.key, timestep.state.cache),
-            lambda timestep: self._step(timestep, action, actions_set),
-            timestep,
-        )
-
     def observation(self, state: State):
         return self.observation_fn(state)
 
     def reward(self, state: State, action: Array, new_state: State):
         return self.reward_fn(state, action, new_state)
 
     def termination(
```

### Comparing `Navix-0.4.0/navix/environments/keydoor.py` & `navix-0.5.0/navix/environments/four_rooms.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,103 +1,109 @@
+# Copyright 2023 The Navix Authors.
+
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+
+
+from __future__ import annotations
+from typing import Union
+
 import jax
 import jax.numpy as jnp
 from jax import Array
-from typing import Union
 
 from ..components import EMPTY_POCKET_ID
+from ..entities import Entities, Goal, Player, Wall
+from ..states import State
+from ..grid import (
+    random_positions,
+    random_directions,
+    room,
+    horizontal_wall,
+    vertical_wall,
+)
 from ..rendering.cache import RenderingCache
-from ..rendering.registry import PALETTE
-from ..environments import Environment
-from ..entities import State, Player, Key, Door, Goal, Wall
-from ..environments import Timestep
-from ..grid import mask_by_coordinates, room, random_positions, random_directions
-
-
-class KeyDoor(Environment):
-    def reset(self, key: Array, cache: Union[RenderingCache, None] = None) -> Timestep:  # type: ignore
-        # check minimum height and width
-        assert (
-            self.height > 3
-        ), f"Room height must be greater than 3, got {self.height} instead"
-        assert (
-            self.width > 4
-        ), f"Room width must be greater than 5, got {self.width} instead"
+from .environment import Environment, Timestep
+from .registry import register_env
 
-        key, k1, k2, k3, k4 = jax.random.split(key, 5)
 
-        grid = room(height=self.height, width=self.width)
+class FourRooms(Environment):
+    def reset(self, key: Array, cache: Union[RenderingCache, None] = None) -> Timestep:
+        assert self.height > 4, f"Insufficient height for room {self.height} < 4"
+        assert self.width > 4, f"Insufficient width for room {self.width} < 4"
+        key, k1, k2 = jax.random.split(key, 3)
 
-        # door positions
-        # col can be between 1 and height - 2
-        door_col = jax.random.randint(k4, (), 2, self.width - 2)  # col
-        # row can be between 1 and height - 2
-        door_row = jax.random.randint(k3, (), 1, self.height - 1)  # row
-        door_pos = jnp.asarray((door_row, door_col))
-        doors = Door(
-            position=door_pos,
-            requires=jnp.asarray(3),
-            open=jnp.asarray(False),
-            colour=PALETTE.YELLOW,
-        )
-
-        # wall positions
-        wall_rows = jnp.arange(1, self.height - 1)
-        wall_cols = jnp.asarray([door_col] * (self.height - 2))
-        wall_pos = jnp.stack((wall_rows, wall_cols), axis=1)
-        # remove wall where the door is
-        wall_pos = jnp.delete(
-            wall_pos, door_row - 1, axis=0, assume_unique_indices=True
-        )
-        walls = Wall(position=wall_pos)
-
-        # get rooms
-        first_room_mask = mask_by_coordinates(
-            grid, (jnp.asarray(self.height), door_col), jnp.less
-        )
-        first_room = jnp.where(first_room_mask, grid, -1)  # put walls where not mask
-        second_room_mask = mask_by_coordinates(
-            grid, (jnp.asarray(0), door_col), jnp.greater
-        )
-        second_room = jnp.where(second_room_mask, grid, -1)  # put walls where not mask
+        # map
+        grid = room(height=self.height, width=self.width)
 
-        # spawn player
-        player_pos = random_positions(k1, first_room)
-        player_dir = random_directions(k2)
+        # vertical partition
+        opening_1 = jax.random.randint(k1, shape=(), minval=1, maxval=self.height // 2)
+        opening_2 = jax.random.randint(
+            k1, shape=(), minval=self.height // 2 + 2, maxval=self.height
+        )
+        openings = jnp.stack([opening_1, opening_2])
+        wall_pos_vert = vertical_wall(grid, 9, openings)
+
+        # horizontal partition
+        opening_1 = jax.random.randint(k2, shape=(), minval=1, maxval=self.width // 2)
+        opening_2 = jax.random.randint(
+            k1, shape=(), minval=self.width // 2 + 2, maxval=self.width
+        )
+        openings = jnp.stack([opening_1, opening_2])
+        wall_pos_hor = horizontal_wall(grid, 9, openings)
+
+        walls_pos = jnp.concatenate([wall_pos_vert, wall_pos_hor])
+        walls = Wall(position=walls_pos)
+
+        # player
+        player_pos, goal_pos = random_positions(k1, grid, n=2, exclude=walls_pos)
+        direction = random_directions(k2, n=1)
         player = Player(
-            position=player_pos, direction=player_dir, pocket=EMPTY_POCKET_ID
+            position=player_pos,
+            direction=direction,
+            pocket=EMPTY_POCKET_ID,
         )
-
-        # spawn key
-        key_pos = random_positions(k2, first_room, exclude=player_pos)
-        keys = Key(position=key_pos, id=jnp.asarray(3), colour=PALETTE.YELLOW)
-
-        # mask the second room
-
-        # spawn goal
-        goal_pos = random_positions(k2, second_room)
-        goals = Goal(position=goal_pos, probability=jnp.asarray(1.0))
-
-        # remove the wall beneath the door
-        grid = grid.at[tuple(door_pos)].set(0)
+        # goal
+        goal = Goal(position=goal_pos, probability=jnp.asarray(1.0))
 
         entities = {
-            "player": player[None],
-            "key": keys[None],
-            "door": doors[None],
-            "goal": goals[None],
-            "wall": walls,
+            Entities.PLAYER: player[None],
+            Entities.GOAL: goal[None],
+            Entities.WALL: walls,
         }
 
+        # systems
         state = State(
             key=key,
             grid=grid,
             cache=cache or RenderingCache.init(grid),
             entities=entities,
         )
+
         return Timestep(
             t=jnp.asarray(0, dtype=jnp.int32),
             observation=self.observation(state),
-            action=jnp.asarray(-1, dtype=jnp.int32),
+            action=jnp.asarray(0, dtype=jnp.int32),
             reward=jnp.asarray(0.0, dtype=jnp.float32),
             step_type=jnp.asarray(0, dtype=jnp.int32),
             state=state,
         )
+
+
+register_env(
+    "Navix-FourRooms-v0",
+    lambda *args, **kwargs: FourRooms(*args, **kwargs, height=19, width=19),
+)
```

### Comparing `Navix-0.4.0/navix/observations.py` & `navix-0.5.0/navix/observations.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import jax
 
 import jax.numpy as jnp
 from jax import Array
 
 from .rendering.cache import TILE_SIZE, unflatten_patches
 from .components import DISCARD_PILE_IDX
-from .entities import State
+from .states import State
 from .grid import align, idx_from_coordinates, crop, view_cone
 
 
 RADIUS = 3
 
 
 def none(
```

### Comparing `Navix-0.4.0/navix/rendering/cache.py` & `navix-0.5.0/navix/rendering/cache.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,37 @@
+# Copyright 2023 The Navix Authors.
+
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+
+
 from __future__ import annotations
 
 from typing import Dict, Tuple
 
 import jax
 from jax import Array
 import jax.numpy as jnp
 from flax import struct
 
-from .registry import SpritesRegistry, TILE_SIZE, SPRITES_REGISTRY
+from .registry import TILE_SIZE, SPRITES_REGISTRY
 
 
 class RenderingCache(struct.PyTreeNode):
     patches: Array
     """A flat set of patches representing the RGB values of each tile in the base map"""
 
     @classmethod
```

### Comparing `Navix-0.4.0/navix/rendering/registry.py` & `navix-0.5.0/navix/rendering/registry.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,56 @@
+# Copyright 2023 The Navix Authors.
+
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+
+
 from __future__ import annotations
 
 import os
-from typing import Dict, Tuple
 from PIL import Image
 
 import jax
 from jax import Array
 import jax.numpy as jnp
 
 
 SPRITES_DIR = os.path.normpath(
     os.path.join(__file__, "..", "..", "..", "assets", "sprites")
 )
 MIN_TILE__SIZE = 8
-TILE_SIZE = 32
+TILE_SIZE = 16
 
 
 def load_sprite(name: str) -> Array:
     """Loads an image from disk in RGB space.
     Args:
         path(str): the filepath of the image on disk
 
     Returns:
         (Array): a jax.Array of shape (H, W, C)"""
     path = os.path.join(SPRITES_DIR, f"{name}.png")
     image = Image.open(path)
     array = jnp.asarray(image)
-    resized = jax.image.resize(array, (TILE_SIZE, TILE_SIZE, 3), method="nearest")
-    return resized
+    resized = jax.image.resize(array, (TILE_SIZE, TILE_SIZE, 3), method="cubic")
+    return jnp.asarray(resized, dtype=jnp.uint8)
 
 
 class PALETTE:
     RED: Array = jnp.asarray(0)
     GREEN: Array = jnp.asarray(1)
     BLUE: Array = jnp.asarray(2)
     PURPLE: Array = jnp.asarray(3)
@@ -56,14 +75,17 @@
         """Populates the sprites registry for all entities."""
         self.set_wall_sprite()
         self.set_floor_sprite()
         self.set_goal_sprite()
         self.set_key_sprite()
         self.set_player_sprite()
         self.set_door_sprite()
+        self.set_lava_sprite()
+        self.set_ball_sprite()
+        self.set_box_sprite()
 
     def set_wall_sprite(self):
         self.registry["wall"] = load_sprite("wall")
 
     def set_floor_sprite(self):
         self.registry["floor"] = load_sprite("floor")
 
@@ -92,10 +114,25 @@
         )
         for c_idx, colour in enumerate(PALETTE.as_string()):
             for s_idx, state in enumerate(["closed", "open", "locked"]):
                 sprite = load_sprite("door" + f"_{state}" + f"_{colour}")
                 door = door.at[c_idx, s_idx].set(sprite)
         self.registry["door"] = door
 
+    def set_lava_sprite(self):
+        self.registry["lava"] = load_sprite("lava")
+
+    def set_ball_sprite(self):
+        ball_coloured = [
+            load_sprite("ball" + f"_{colour}") for colour in PALETTE.as_string()
+        ]
+        self.registry["ball"] = jnp.stack(ball_coloured, axis=0)
+
+    def set_box_sprite(self):
+        box_coloured = [
+            load_sprite("box" + f"_{colour}") for colour in PALETTE.as_string()
+        ]
+        self.registry["box"] = jnp.stack(box_coloured, axis=0)
+
 
 # initialise sprites registry
 SPRITES_REGISTRY = SpritesRegistry().registry
```

### Comparing `Navix-0.4.0/navix/spaces.py` & `navix-0.5.0/navix/spaces.py`

 * *Files identical despite different names*

### Comparing `Navix-0.4.0/navix/tasks.py` & `navix-0.5.0/navix/terminations.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,79 +12,50 @@
 
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-
-
 from __future__ import annotations
+
 from typing import Callable
+from jax import Array
+import jax.numpy as jnp
 
+from . import events
+from .states import State
+from .grid import translate
+from .entities import Entities, Player
 
-import jax
-import jax.numpy as jnp
-from jax import Array
 
-from .entities import State
+def compose(
+    *term_functions: Callable[[State, Array, State], Array],
+    operator: Callable = jnp.any,
+) -> Callable:
+    return lambda prev_state, action, state: operator(
+        jnp.asarray([term_f(prev_state, action, state) for term_f in term_functions])
+    )
 
 
-def compose(*fns: Callable[[State, Array, State], Array]):
-    def composed(prev_state: State, action: Array, state: State) -> Array:
-        reward = jnp.asarray(0.0)
-        for fn in fns:
-            reward += fn(prev_state, action, state)
-        return reward
+def check_truncation(terminated: Array, truncated: Array) -> Array:
+    result = jnp.asarray(truncated + 2 * terminated, dtype=jnp.int32)
+    return jnp.clip(result, 0, 2)
 
-    return composed
 
+def on_goal_reached(prev_state: State, action: Array, state: State) -> Array:
+    return jnp.asarray(events.on_goal_reached(state), dtype=jnp.bool_)
 
-def free(state: State) -> Array:
-    return jnp.asarray(0.0)
 
+def on_lava_fall(prev_state: State, action: Array, state: State) -> Array:
+    return jnp.asarray(events.on_lava_fall(state), dtype=jnp.bool_)
 
-def navigation(prev_state: State, action: Array, state: State) -> Array:
-    player = state.get_player()
-    goals = state.get_goals()
 
-    reached = jax.vmap(jnp.array_equal, in_axes=(None, 0))(
-        player.position, goals.position
-    )
+def on_ball_hit(prev_state: State, action: Array, state: State) -> Array:
+    return jnp.asarray(events.on_ball_hit(state), dtype=jnp.bool_)
+
+
+def on_door_done(prev_state: State, action: Array, state: State) -> Array:
+    return jnp.asarray(events.on_door_done(state), dtype=jnp.bool_)
+
 
-    # exoxgenous reward noise
-    draws = jax.random.uniform(state.key, (len(goals.probability),))
-    # if there is a reward and the player reached the goal, then reward
-    reward = reached * jnp.less_equal(draws, goals.probability)
-    # if two goals are at the same position, we sum them
-    reward = jnp.sum(reward, dtype=jnp.float32).squeeze()
-
-    # ensure scalar reward
-    assert reward.shape == (), f"Reward must be a scalar but got shape {reward.shape}"
-    return reward
-
-
-def action_cost(
-    prev_state: State, action: Array, new_state: State, cost: float = 0.01
-) -> Array:
-    # noops are free
-    return -jnp.asarray(action > 0, dtype=jnp.float32) * cost
-
-
-def time_cost(
-    prev_state: State, action: Array, new_state: State, cost: float = 0.01
-) -> Array:
-    # time always has a cost
-    return -jnp.asarray(cost)
-
-
-def wall_hit_cost(
-    prev_state: State, action: Array, state: State, cost: float = 0.01
-) -> Array:
-    prev_player = prev_state.get_player()
-    player = state.get_player()
-
-    # if state is unchanged, maybe the wall was hit
-    didnt_move = jnp.array_equal(prev_player.position, player.position)
-    but_wanted_to = jnp.less_equal(3, action) * jnp.less_equal(action, 6)
-    hit = jnp.logical_and(didnt_move, but_wanted_to)
-    return -jnp.asarray(cost) * hit
+DEFAULT_TERMINATION = compose(on_goal_reached, on_lava_fall, on_ball_hit)
```

### Comparing `Navix-0.4.0/navix/terminations.py` & `navix-0.5.0/navix/environments/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,24 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
 from __future__ import annotations
 
-from jax import Array
-import jax.numpy as jnp
-from .entities import State
-from .grid import positions_equal
 
-
-def check_truncation(terminated: Array, truncated: Array) -> Array:
-    result = jnp.asarray(truncated + 2 * terminated, dtype=jnp.int32)
-    return jnp.clip(result, 0, 2)
-
-
-def on_navigation_completion(prev_state: State, action: Array, state: State) -> Array:
-    player = state.get_player()
-    goals = state.get_goals()
-
-    reached = positions_equal(player.position, goals.position)
-    return jnp.any(reached)
+from .environment import Environment, Timestep
+from .room import Room
+from .key_door import KeyDoor
+from .four_rooms import FourRooms
+from .key_corridor import KeyCorridor
+from .lava_gap import LavaGap
+from .crossings import Crossings
+from .dynamic_obstacles import DynamicObstacles
+from .dist_shift import DistShift
+from .go_to_door import GoToDoor
```

### Comparing `Navix-0.4.0/pyproject.toml` & `navix-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Navix-0.4.0/scripts/release.sh` & `navix-0.5.0/scripts/release.sh`

 * *Files identical despite different names*

### Comparing `Navix-0.4.0/tests/performance/grid.py` & `navix-0.5.0/tests/performance/grid.py`

 * *Files identical despite different names*

### Comparing `Navix-0.4.0/tests/performance/minigrid.py` & `navix-0.5.0/tests/performance/minigrid.py`

 * *Files identical despite different names*

### Comparing `Navix-0.4.0/tests/performance/observations.py` & `navix-0.5.0/tests/performance/observations.py`

 * *Files identical despite different names*

### Comparing `Navix-0.4.0/tests/performance/observations_keydoor_report.txt` & `navix-0.5.0/tests/performance/observations_keydoor_report.txt`

 * *Files identical despite different names*

### Comparing `Navix-0.4.0/tests/performance/observations_room_report.txt` & `navix-0.5.0/tests/performance/observations_room_report.txt`

 * *Files identical despite different names*

### Comparing `Navix-0.4.0/tests/performance/profiling.py` & `navix-0.5.0/tests/performance/profiling.py`

 * *Files identical despite different names*

### Comparing `Navix-0.4.0/tests/test_actions.py` & `navix-0.5.0/tests/test_actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import Dict
 import jax
 import jax.numpy as jnp
 
 import navix as nx
+from navix.actions import Directions
 from navix.components import EMPTY_POCKET_ID, DISCARD_PILE_COORDS
-from navix.entities import Entities, Entity, State
+from navix.entities import Entities, Entity
+from navix.states import State
 from navix.rendering.registry import PALETTE
 
 
 def test_rotation():
     direction = jnp.asarray(0)
 
     key = jax.random.PRNGKey(0)
@@ -20,15 +22,15 @@
 
     entities: Dict[str, Entity] = {
         Entities.PLAYER: player,
     }
 
     player.check_ndim(batched=True)
 
-    state = nx.entities.State(
+    state = State(
         grid=grid,
         entities=entities,
         cache=cache,
         key=key,
     )
 
     msg = "Expected direction to be {}, got {}"
@@ -88,15 +90,15 @@
     """
     entities = {
         Entities.PLAYER: player[None],
         Entities.GOAL: goals[None],
         Entities.KEY: keys[None],
         Entities.DOOR: doors[None],
     }
-    state = nx.entities.State(
+    state = State(
         key=key,
         grid=grid,
         entities=entities,
         cache=cache,
     )
 
     # check forward
@@ -151,20 +153,19 @@
     expected_position = jnp.asarray((1, 2))
     player = state.get_player()
     player.check_ndim(batched=False)
     assert jnp.array_equal(player.position, expected_position)
 
 
 def test_walkable():
-    heigh, width = 5, 5
-    grid = jnp.zeros((heigh - 2, width - 2), dtype=jnp.int32)
-    grid = jnp.pad(grid, pad_width=1, mode="constant", constant_values=1)
+    height, width = 5, 5
+    grid = nx.grid.room(height, width)
     key = jax.random.PRNGKey(0)
     player = nx.entities.Player(
-        position=jnp.asarray((1, 1)), direction=jnp.asarray(0), pocket=EMPTY_POCKET_ID
+        position=jnp.asarray((1, 1)), direction=Directions.EAST, pocket=EMPTY_POCKET_ID
     )
     goals = nx.entities.Goal(position=jnp.asarray((3, 3)), probability=jnp.asarray(1.0))
     keys = nx.entities.Key(
         position=jnp.asarray((3, 1)), id=jnp.asarray(1), colour=PALETTE.YELLOW
     )
     doors = nx.entities.Door(
         position=jnp.asarray((1, 3)),
@@ -183,15 +184,15 @@
     """
     #  #  #  #  #
     #  P  .  D #
     #  .  .  . #
     #  K  .  G #
     #  #  #  #  #
     """
-    state = nx.entities.State(
+    state = State(
         key=key,
         grid=grid,
         cache=cache,
         entities={
             Entities.PLAYER: player[None],
             Entities.GOAL: goals[None],
             Entities.KEY: keys[None],
@@ -200,16 +201,17 @@
     )
 
     def check_forward_position(state: State):
         player = state.get_player()
         player.check_ndim(batched=False)
         prev_pos = player.position
         pos = nx.grid.translate_forward(prev_pos, player.direction, jnp.asarray(1))
-        assert not nx.actions._walkable(
-            state, pos
+        walkable, _ = nx.actions._can_walk_there(state, pos)
+        assert (
+            not walkable
         ), "Expected position {} to be not walkable, since it is a {}".format(
             pos, state.grid[tuple(pos)]
         )
 
     # should not be able to walk on/through a closed door
     state = nx.actions.forward(state)
     check_forward_position(state)
@@ -271,15 +273,15 @@
     """
     entities = {
         Entities.PLAYER: player[None],
         Entities.GOAL: goals[None],
         Entities.KEY: keys[None],
         Entities.DOOR: doors[None],
     }
-    state = nx.entities.State(
+    state = State(
         key=key,
         grid=grid,
         cache=cache,
         entities=entities,
     )
 
     # check that the player has no keys
@@ -321,15 +323,15 @@
     keys = nx.entities.Key(
         position=jnp.asarray((3, 1)), id=jnp.asarray(1), colour=PALETTE.YELLOW
     )
     doors = nx.entities.Door(
         position=jnp.asarray((1, 3)),
         requires=jnp.asarray(1),
         open=jnp.asarray(False),
-        colour=PALETTE.YELLOW
+        colour=PALETTE.YELLOW,
     )
     cache = nx.rendering.cache.RenderingCache.init(grid)
 
     player.check_ndim(batched=False)
     goals.check_ndim(batched=False)
     keys.check_ndim(batched=False)
     doors.check_ndim(batched=False)
@@ -343,15 +345,15 @@
     entities = {
         Entities.PLAYER: player[None],
         Entities.GOAL: goals[None],
         Entities.KEY: keys[None],
         Entities.DOOR: doors[None],
     }
 
-    state = nx.entities.State(
+    state = State(
         key=key,
         grid=grid,
         cache=cache,
         entities=entities,
     )
 
     # check that the player has no keys
@@ -424,12 +426,12 @@
         player.position, expected_position
     ), "Expected player position to be {}, got {}".format(
         expected_position, player.position
     )
 
 
 if __name__ == "__main__":
-    test_rotation()
-    test_move()
+    # test_rotation()
+    # test_move()
     test_walkable()
     test_pickup()
-    test_open()
+    # test_open()
```

### Comparing `Navix-0.4.0/tests/test_entities.py` & `navix-0.5.0/tests/test_entities.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import jax
 import jax.numpy as jnp
 
-import navix as nx
 from navix.entities import Goal, Player
 from navix.rendering.registry import TILE_SIZE
 
 
 def test_indexing():
     # batched entity with batch size 1
     entity = Player(
```

### Comparing `Navix-0.4.0/tests/test_environments.py` & `navix-0.5.0/tests/test_environments.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             3,  # forward
         )
         print(timestep)
         print()
         for action in actions:
             timestep = step(timestep, jnp.asarray(action))
             print()
-            print(nx.actions.ACTIONS[action])
+            print(nx.actions.DEFAULT_ACTION_SET[action])
             print(timestep)
         return timestep
 
     f()
     timestep = jax.jit(f)()
     print(timestep)
 
@@ -59,15 +59,15 @@
             3,  # forward
             3,  # forward
         )
         print(timestep)
         for action in actions:
             timestep = step(timestep, jnp.asarray(action))
             print()
-            print(nx.actions.ACTIONS[action])
+            print(nx.actions.DEFAULT_ACTION_SET[action])
             print(timestep)
         return timestep
 
     f()
     jax.jit(f)()
 
 
@@ -78,9 +78,9 @@
     timestep = env.reset(key)
     return
 
 
 if __name__ == "__main__":
     # test_room()
     # jax.jit(test_room)()
-    # test_keydoor()
-    test_keydoor2()
+    test_keydoor()
+    # test_keydoor2()
```

### Comparing `Navix-0.4.0/tests/test_grid.py` & `navix-0.5.0/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `Navix-0.4.0/tests/test_observations.py` & `navix-0.5.0/tests/test_observations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import jax
 import jax.numpy as jnp
 
 import navix as nx
+from navix.states import State
 from navix.entities import Entities, Player, Goal, Key, Door
 from navix.components import EMPTY_POCKET_ID
 from navix.rendering.cache import RenderingCache, TILE_SIZE
 from navix.rendering.registry import SPRITES_REGISTRY, PALETTE
 
 
 def test_rgb():
@@ -29,15 +30,15 @@
     entities = {
         Entities.PLAYER: players[None],
         Entities.GOAL: goals[None],
         Entities.KEY: keys[None],
         Entities.DOOR: doors,
     }
 
-    state = nx.entities.State(
+    state = State(
         key=jax.random.PRNGKey(0),
         grid=grid,
         cache=RenderingCache.init(grid),
         entities=entities,
     )
     sprites_registry = SPRITES_REGISTRY
 
@@ -69,17 +70,15 @@
     goals = state.get_goals()
     goal_tile = get_tile(goals.position[0])
     assert jnp.array_equal(goal_tile, sprites_registry[Entities.GOAL]), goal_tile
 
     keys = state.get_keys()
     key_tile = get_tile(keys.position[0])
     colour = keys.colour[0]
-    assert jnp.array_equal(
-        key_tile, sprites_registry[Entities.KEY][colour]
-    ), key_tile
+    assert jnp.array_equal(key_tile, sprites_registry[Entities.KEY][colour]), key_tile
 
     doors = state.get_doors()
     door = doors[0]
     door_tile = get_tile(door.position)
     colour = door.colour
     idx = jnp.asarray(door.open + 2 * door.locked, dtype=jnp.int32)
     assert jnp.array_equal(
@@ -117,15 +116,15 @@
     entities = {
         Entities.PLAYER: players[None],
         Entities.GOAL: goals[None],
         Entities.KEY: keys[None],
         Entities.DOOR: doors,
     }
 
-    state = nx.entities.State(
+    state = State(
         key=jax.random.PRNGKey(0),
         grid=grid,
         cache=RenderingCache.init(grid),
         entities=entities,
     )
 
     obs = nx.observations.categorical_first_person(state)
```

### Comparing `Navix-0.4.0/tests/test_spaces.py` & `navix-0.5.0/tests/test_spaces.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,19 +16,27 @@
                 print(sample)
                 assert jnp.all(jnp.logical_not(jnp.isnan(sample)))
 
 
 def test_continuous():
     key = jax.random.PRNGKey(42)
     shapes = ((), (0,), (0, 0), (1, 2), (5, 5))
-    min_max = [(0.0, 1.0), (0.0, 1), (0, 1), (1.0, -1.0), (MIN_INT, MAX_INT),]
+    min_max = [
+        (0.0, 1.0),
+        (0.0, 1),
+        (0, 1),
+        (1.0, -1.0),
+        (MIN_INT, MAX_INT),
+    ]
     for shape in shapes:
         for minimum, maximum in min_max:
-            space = Continuous(shape=shape, minimum=jnp.asarray(minimum), maximum=jnp.asarray(maximum))
+            space = Continuous(
+                shape=shape, minimum=jnp.asarray(minimum), maximum=jnp.asarray(maximum)
+            )
             sample = space.sample(key)
             print(sample)
             assert jnp.all(jnp.logical_not(jnp.isnan(sample)))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     test_discrete()
-    test_continuous()
+    test_continuous()
```

### Comparing `Navix-0.4.0/tests/test_tasks.py` & `navix-0.5.0/tests/test_tasks.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import jax
 import jax.numpy as jnp
 
 import navix as nx
+from navix.states import State
 from navix.entities import Entities, Player, Goal, Key, Door
 from navix.components import EMPTY_POCKET_ID
 from navix.rendering.registry import PALETTE
 
 
 def test_navigation():
     """Unittest for https://github.com/epignatelli/navix/pull/47"""
@@ -31,31 +32,31 @@
     entities = {
         Entities.PLAYER: players[None],
         Entities.GOAL: goals,
         Entities.KEY: keys[None],
         Entities.DOOR: doors,
     }
 
-    state = nx.entities.State(
+    state = State(
         key=jax.random.PRNGKey(0),
         grid=grid,
         cache=nx.rendering.cache.RenderingCache.init(grid),
         entities=entities,
     )
     action = jnp.asarray(0)
-    reward = nx.tasks.navigation(state, action, state)
+    reward = nx.rewards.on_goal_reached(state, action, state)
     assert jnp.array_equal(reward, jnp.asarray(0.0))
 
 
 def test_tasks_composition():
-    reward_fn = nx.tasks.compose(
-        nx.tasks.navigation,
-        nx.tasks.action_cost,
-        nx.tasks.time_cost,
-        nx.tasks.wall_hit_cost,
+    reward_fn = nx.rewards.compose(
+        nx.rewards.on_goal_reached,
+        nx.rewards.action_cost,
+        nx.rewards.time_cost,
+        nx.rewards.wall_hit_cost,
     )
 
     env = nx.environments.Room(height=3, width=3, max_steps=8, reward_fn=reward_fn)
     key = jax.random.PRNGKey(0)
 
     def _test():
         timestep = env.reset(key)
```

### Comparing `Navix-0.4.0/tests/test_terminations.py` & `navix-0.5.0/tests/test_terminations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 import jax
 import jax.numpy as jnp
 
 import navix as nx
+from navix.actions import Directions
+from navix.states import State
 from navix.components import EMPTY_POCKET_ID
 
 
 def test_on_navigation_completion():
     grid = jnp.zeros((5, 5), dtype=jnp.int32)
 
     players = nx.entities.Player(
-        position=jnp.asarray((1, 1)), direction=jnp.asarray(0), pocket=EMPTY_POCKET_ID
+        position=jnp.asarray((1, 1)), direction=Directions.EAST, pocket=EMPTY_POCKET_ID
     )
-    goals = nx.entities.Goal(position=jnp.asarray((3, 3)), probability=jnp.asarray(1))
+    goals = nx.entities.Goal(position=jnp.asarray((1, 2)), probability=jnp.asarray(1))
     entities = {
         nx.entities.Entities.PLAYER: players[None],
         nx.entities.Entities.GOAL: goals[None],
     }
 
-    state = nx.entities.State(
+    state = State(
         key=jax.random.PRNGKey(0),
         grid=grid,
-        cache=nx.entities.RenderingCache.init(grid),
+        cache=nx.rendering.cache.RenderingCache.init(grid),
         entities=entities,
     )
-    # shpuld not terminate
-    termination = nx.terminations.on_navigation_completion(state, jnp.asarray(0), state)
+    # should not terminate
+    termination = nx.terminations.on_goal_reached(state, jnp.asarray(0), state)
     assert not termination, f"Should not terminate, got {termination} instead"
 
-    # artificially put agent on goal
-    player = state.get_player()
-    goals = state.get_goals()
-    new_state = state.set_player(player.replace(position=goals.position[0]))
-    termination = nx.terminations.on_navigation_completion(
-        state, jnp.asarray(0), new_state
-    )
+    # move forward
+    new_state = nx.actions.forward(state)
+    termination = nx.terminations.on_goal_reached(state, jnp.asarray(0), new_state)
     assert termination, f"Should terminate, got {termination} instead"
 
 
 def test_check_truncation():
     terminated = jnp.asarray(False)
     truncated = jnp.asarray(False)
     assert nx.terminations.check_truncation(terminated, truncated) == jnp.asarray(
```

