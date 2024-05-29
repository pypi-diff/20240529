# Comparing `tmp/mapdata-3.7.1.tar.gz` & `tmp/mapdata-3.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapdata-3.7.1.tar", last modified: Tue May 28 15:17:52 2024, max compression
+gzip compressed data, was "mapdata-3.7.2.tar", last modified: Wed May 29 20:15:00 2024, max compression
```

## Comparing `mapdata-3.7.1.tar` & `mapdata-3.7.2.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-28 15:17:52.470894 mapdata-3.7.1/
--rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-3.7.1/LICENSE.txt
--rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-3.7.1/MANIFEST.in
--rw-r--r--   0 dreas     (1000) dreas     (1000)     7898 2024-05-28 15:17:52.470894 mapdata-3.7.1/PKG-INFO
--rw-r--r--   0 dreas     (1000) dreas     (1000)     6421 2024-05-04 17:16:18.000000 mapdata-3.7.1/README.md
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-28 15:17:52.398892 mapdata-3.7.1/mapdata/
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-28 15:17:52.398892 mapdata-3.7.1/mapdata/configfile/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     9002 2024-03-04 21:04:24.000000 mapdata-3.7.1/mapdata/configfile/mapdata.conf
--rwxrwxr-x   0 dreas     (1000) dreas     (1000)   691388 2024-05-28 15:12:44.000000 mapdata-3.7.1/mapdata/mapdata.py
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-28 15:17:52.394892 mapdata-3.7.1/mapdata/symbols/
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-28 15:17:52.470894 mapdata-3.7.1/mapdata/symbols/16x16/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:04:56.000000 mapdata-3.7.1/mapdata/symbols/16x16/0.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:16.000000 mapdata-3.7.1/mapdata/symbols/16x16/1.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:29.000000 mapdata-3.7.1/mapdata/symbols/16x16/2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:40.000000 mapdata-3.7.1/mapdata/symbols/16x16/3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:05:52.000000 mapdata-3.7.1/mapdata/symbols/16x16/4.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:06:03.000000 mapdata-3.7.1/mapdata/symbols/16x16/5.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2024-01-31 04:28:02.000000 mapdata-3.7.1/mapdata/symbols/16x16/6.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:06:27.000000 mapdata-3.7.1/mapdata/symbols/16x16/7.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:06:40.000000 mapdata-3.7.1/mapdata/symbols/16x16/8.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2024-01-31 04:26:59.000000 mapdata-3.7.1/mapdata/symbols/16x16/9.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-15 16:04:26.000000 mapdata-3.7.1/mapdata/symbols/16x16/A.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:07:30.000000 mapdata-3.7.1/mapdata/symbols/16x16/B.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:10:14.000000 mapdata-3.7.1/mapdata/symbols/16x16/C.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:13:27.000000 mapdata-3.7.1/mapdata/symbols/16x16/D.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:14:22.000000 mapdata-3.7.1/mapdata/symbols/16x16/E.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-15 16:15:26.000000 mapdata-3.7.1/mapdata/symbols/16x16/F.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 00:14:24.000000 mapdata-3.7.1/mapdata/symbols/16x16/G.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:15:07.000000 mapdata-3.7.1/mapdata/symbols/16x16/H.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:16:00.000000 mapdata-3.7.1/mapdata/symbols/16x16/I.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:18:38.000000 mapdata-3.7.1/mapdata/symbols/16x16/J.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:21:25.000000 mapdata-3.7.1/mapdata/symbols/16x16/K.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:22:10.000000 mapdata-3.7.1/mapdata/symbols/16x16/L.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:24:58.000000 mapdata-3.7.1/mapdata/symbols/16x16/M.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:27:42.000000 mapdata-3.7.1/mapdata/symbols/16x16/N.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 14:04:25.000000 mapdata-3.7.1/mapdata/symbols/16x16/O.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:28:05.000000 mapdata-3.7.1/mapdata/symbols/16x16/P.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:29:12.000000 mapdata-3.7.1/mapdata/symbols/16x16/Q.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:30:16.000000 mapdata-3.7.1/mapdata/symbols/16x16/R.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:34:31.000000 mapdata-3.7.1/mapdata/symbols/16x16/S.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:35:37.000000 mapdata-3.7.1/mapdata/symbols/16x16/T.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:37:27.000000 mapdata-3.7.1/mapdata/symbols/16x16/U.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:40:22.000000 mapdata-3.7.1/mapdata/symbols/16x16/V.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:44:48.000000 mapdata-3.7.1/mapdata/symbols/16x16/W.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:46:24.000000 mapdata-3.7.1/mapdata/symbols/16x16/X.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:47:50.000000 mapdata-3.7.1/mapdata/symbols/16x16/Y.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:49:43.000000 mapdata-3.7.1/mapdata/symbols/16x16/Z.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-21 14:55:41.000000 mapdata-3.7.1/mapdata/symbols/16x16/airplane.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-06-24 15:22:11.000000 mapdata-3.7.1/mapdata/symbols/16x16/anchor.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-07-04 17:00:25.000000 mapdata-3.7.1/mapdata/symbols/16x16/ball.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2024-01-24 20:44:54.000000 mapdata-3.7.1/mapdata/symbols/16x16/ball_small.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-05-16 13:39:00.000000 mapdata-3.7.1/mapdata/symbols/16x16/bar.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-07-04 17:04:48.000000 mapdata-3.7.1/mapdata/symbols/16x16/bars.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 14:43:55.000000 mapdata-3.7.1/mapdata/symbols/16x16/binoculars.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 22:29:19.000000 mapdata-3.7.1/mapdata/symbols/16x16/bird.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      288 2023-04-24 16:37:43.000000 mapdata-3.7.1/mapdata/symbols/16x16/block.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2024-01-26 04:36:33.000000 mapdata-3.7.1/mapdata/symbols/16x16/block_small.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-16 18:31:20.000000 mapdata-3.7.1/mapdata/symbols/16x16/bookmark.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-24 15:29:01.000000 mapdata-3.7.1/mapdata/symbols/16x16/box_stack.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-04-30 14:46:15.000000 mapdata-3.7.1/mapdata/symbols/16x16/camera.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-25 16:51:47.000000 mapdata-3.7.1/mapdata/symbols/16x16/cancel.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-05-21 15:05:05.000000 mapdata-3.7.1/mapdata/symbols/16x16/car.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-21 15:04:37.000000 mapdata-3.7.1/mapdata/symbols/16x16/car2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-24 01:00:13.000000 mapdata-3.7.1/mapdata/symbols/16x16/center8.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:35:37.000000 mapdata-3.7.1/mapdata/symbols/16x16/check.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-06-24 14:51:14.000000 mapdata-3.7.1/mapdata/symbols/16x16/check_circle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-16 14:20:03.000000 mapdata-3.7.1/mapdata/symbols/16x16/checkbox.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-04-28 13:31:04.000000 mapdata-3.7.1/mapdata/symbols/16x16/checkerboard.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 14:29:46.000000 mapdata-3.7.1/mapdata/symbols/16x16/chevrons.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-16 18:12:28.000000 mapdata-3.7.1/mapdata/symbols/16x16/circle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 14:22:20.000000 mapdata-3.7.1/mapdata/symbols/16x16/circle_bar.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-06-24 14:58:14.000000 mapdata-3.7.1/mapdata/symbols/16x16/circle_plus.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      314 2023-04-28 13:09:20.000000 mapdata-3.7.1/mapdata/symbols/16x16/circle_stipple.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      317 2023-06-24 14:29:15.000000 mapdata-3.7.1/mapdata/symbols/16x16/circle_triangle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-04-25 14:40:36.000000 mapdata-3.7.1/mapdata/symbols/16x16/circle_wedge.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-06-24 14:56:37.000000 mapdata-3.7.1/mapdata/symbols/16x16/circle_x.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-07-04 17:10:15.000000 mapdata-3.7.1/mapdata/symbols/16x16/clock.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 14:05:41.000000 mapdata-3.7.1/mapdata/symbols/16x16/columns.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-25 13:50:11.000000 mapdata-3.7.1/mapdata/symbols/16x16/contract.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-04-16 17:48:39.000000 mapdata-3.7.1/mapdata/symbols/16x16/cross.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-23 18:45:40.000000 mapdata-3.7.1/mapdata/symbols/16x16/darkeye.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:18:32.000000 mapdata-3.7.1/mapdata/symbols/16x16/decrease.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-06-30 12:46:46.000000 mapdata-3.7.1/mapdata/symbols/16x16/deposition.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:47.000000 mapdata-3.7.1/mapdata/symbols/16x16/diag_ll.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:26.000000 mapdata-3.7.1/mapdata/symbols/16x16/diag_lr.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:05.000000 mapdata-3.7.1/mapdata/symbols/16x16/diag_ul.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:17:04.000000 mapdata-3.7.1/mapdata/symbols/16x16/diag_ur.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-20 18:41:19.000000 mapdata-3.7.1/mapdata/symbols/16x16/dialog.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-16 17:38:10.000000 mapdata-3.7.1/mapdata/symbols/16x16/diamond.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 13:47:24.000000 mapdata-3.7.1/mapdata/symbols/16x16/donkey.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-04-30 16:45:55.000000 mapdata-3.7.1/mapdata/symbols/16x16/dot.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:00:44.000000 mapdata-3.7.1/mapdata/symbols/16x16/down.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:38:22.000000 mapdata-3.7.1/mapdata/symbols/16x16/drop.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-03 02:15:55.000000 mapdata-3.7.1/mapdata/symbols/16x16/elephant.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-25 14:33:40.000000 mapdata-3.7.1/mapdata/symbols/16x16/expand.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-04-30 15:03:32.000000 mapdata-3.7.1/mapdata/symbols/16x16/eye.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-06-24 13:59:48.000000 mapdata-3.7.1/mapdata/symbols/16x16/fire.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 22:13:54.000000 mapdata-3.7.1/mapdata/symbols/16x16/fish.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-30 14:36:11.000000 mapdata-3.7.1/mapdata/symbols/16x16/flag.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-30 15:04:58.000000 mapdata-3.7.1/mapdata/symbols/16x16/flag2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-06-24 15:06:07.000000 mapdata-3.7.1/mapdata/symbols/16x16/four_arrows.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 22:25:14.000000 mapdata-3.7.1/mapdata/symbols/16x16/graph.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-06-24 15:18:19.000000 mapdata-3.7.1/mapdata/symbols/16x16/hand.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:04:09.000000 mapdata-3.7.1/mapdata/symbols/16x16/hash.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-03 01:53:41.000000 mapdata-3.7.1/mapdata/symbols/16x16/heart.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2024-01-31 04:51:54.000000 mapdata-3.7.1/mapdata/symbols/16x16/hidden.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-24 15:40:09.000000 mapdata-3.7.1/mapdata/symbols/16x16/hourglass.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-24 22:31:53.000000 mapdata-3.7.1/mapdata/symbols/16x16/house.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:18:05.000000 mapdata-3.7.1/mapdata/symbols/16x16/increase.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-24 23:05:40.000000 mapdata-3.7.1/mapdata/symbols/16x16/info.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-30 14:51:36.000000 mapdata-3.7.1/mapdata/symbols/16x16/leaf.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:02:45.000000 mapdata-3.7.1/mapdata/symbols/16x16/left.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-23 13:36:40.000000 mapdata-3.7.1/mapdata/symbols/16x16/lightbulb.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 16:38:25.000000 mapdata-3.7.1/mapdata/symbols/16x16/lightning.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      314 2023-04-28 13:14:23.000000 mapdata-3.7.1/mapdata/symbols/16x16/lightning2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-07-04 16:58:13.000000 mapdata-3.7.1/mapdata/symbols/16x16/location_ptr.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-20 14:06:42.000000 mapdata-3.7.1/mapdata/symbols/16x16/mine.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-06-24 15:07:56.000000 mapdata-3.7.1/mapdata/symbols/16x16/nested_boxes.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 14:07:35.000000 mapdata-3.7.1/mapdata/symbols/16x16/pennant.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 13:16:09.000000 mapdata-3.7.1/mapdata/symbols/16x16/pennant2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-18 19:04:36.000000 mapdata-3.7.1/mapdata/symbols/16x16/people.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:26:34.000000 mapdata-3.7.1/mapdata/symbols/16x16/person.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:30:45.000000 mapdata-3.7.1/mapdata/symbols/16x16/person2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-20 18:43:50.000000 mapdata-3.7.1/mapdata/symbols/16x16/person3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-24 15:37:42.000000 mapdata-3.7.1/mapdata/symbols/16x16/phone.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:18:45.000000 mapdata-3.7.1/mapdata/symbols/16x16/photo.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-19 22:48:26.000000 mapdata-3.7.1/mapdata/symbols/16x16/picnic.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-19 03:57:15.000000 mapdata-3.7.1/mapdata/symbols/16x16/plus.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      358 2023-05-03 01:58:16.000000 mapdata-3.7.1/mapdata/symbols/16x16/point_down.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      356 2023-05-03 01:58:03.000000 mapdata-3.7.1/mapdata/symbols/16x16/point_left.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      362 2023-05-03 01:57:47.000000 mapdata-3.7.1/mapdata/symbols/16x16/point_right.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      347 2023-05-03 01:56:56.000000 mapdata-3.7.1/mapdata/symbols/16x16/point_up.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      357 2023-05-03 01:58:38.000000 mapdata-3.7.1/mapdata/symbols/16x16/pointer_ne.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      356 2023-05-03 01:59:20.000000 mapdata-3.7.1/mapdata/symbols/16x16/pointer_nw.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      358 2023-05-03 01:58:54.000000 mapdata-3.7.1/mapdata/symbols/16x16/pointer_se.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      357 2023-05-03 01:59:07.000000 mapdata-3.7.1/mapdata/symbols/16x16/pointer_sw.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-20 18:51:06.000000 mapdata-3.7.1/mapdata/symbols/16x16/puzzle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:52:56.000000 mapdata-3.7.1/mapdata/symbols/16x16/q1.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:57:59.000000 mapdata-3.7.1/mapdata/symbols/16x16/q1_notch.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:25.000000 mapdata-3.7.1/mapdata/symbols/16x16/q2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:55.000000 mapdata-3.7.1/mapdata/symbols/16x16/q2_notch.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:46.000000 mapdata-3.7.1/mapdata/symbols/16x16/q3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:28.000000 mapdata-3.7.1/mapdata/symbols/16x16/q3_notch.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:57.000000 mapdata-3.7.1/mapdata/symbols/16x16/q4.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:13.000000 mapdata-3.7.1/mapdata/symbols/16x16/q4_notch.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-05-20 18:36:19.000000 mapdata-3.7.1/mapdata/symbols/16x16/qmark_circle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      311 2023-05-20 18:37:52.000000 mapdata-3.7.1/mapdata/symbols/16x16/qmark_circle2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:43:45.000000 mapdata-3.7.1/mapdata/symbols/16x16/raincloud.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-24 16:39:34.000000 mapdata-3.7.1/mapdata/symbols/16x16/right.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-20 17:23:57.000000 mapdata-3.7.1/mapdata/symbols/16x16/rocket.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-20 17:25:43.000000 mapdata-3.7.1/mapdata/symbols/16x16/rocket2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-23 16:07:27.000000 mapdata-3.7.1/mapdata/symbols/16x16/rose.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-28 14:05:56.000000 mapdata-3.7.1/mapdata/symbols/16x16/rows.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-28 14:27:34.000000 mapdata-3.7.1/mapdata/symbols/16x16/scales.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-07-04 17:07:45.000000 mapdata-3.7.1/mapdata/symbols/16x16/search.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-07-04 17:08:06.000000 mapdata-3.7.1/mapdata/symbols/16x16/search2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-01 15:46:45.000000 mapdata-3.7.1/mapdata/symbols/16x16/skull.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-17 02:43:53.000000 mapdata-3.7.1/mapdata/symbols/16x16/square.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:26:56.000000 mapdata-3.7.1/mapdata/symbols/16x16/star.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 13:07:07.000000 mapdata-3.7.1/mapdata/symbols/16x16/stipple.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-03 02:10:57.000000 mapdata-3.7.1/mapdata/symbols/16x16/stop.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      317 2023-06-24 15:31:50.000000 mapdata-3.7.1/mapdata/symbols/16x16/surprise_circle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:22:10.000000 mapdata-3.7.1/mapdata/symbols/16x16/swamp.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-16 18:27:50.000000 mapdata-3.7.1/mapdata/symbols/16x16/target.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 04:37:09.000000 mapdata-3.7.1/mapdata/symbols/16x16/target2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-06-24 15:27:04.000000 mapdata-3.7.1/mapdata/symbols/16x16/ten.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-24 14:54:31.000000 mapdata-3.7.1/mapdata/symbols/16x16/trash.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-09 17:01:43.000000 mapdata-3.7.1/mapdata/symbols/16x16/tree.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 12:59:30.000000 mapdata-3.7.1/mapdata/symbols/16x16/tree2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:26:26.000000 mapdata-3.7.1/mapdata/symbols/16x16/tree3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-09 16:59:51.000000 mapdata-3.7.1/mapdata/symbols/16x16/triangle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      311 2023-05-09 17:08:13.000000 mapdata-3.7.1/mapdata/symbols/16x16/triangle_open.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-05-20 17:46:38.000000 mapdata-3.7.1/mapdata/symbols/16x16/triangle_sm.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-04-16 18:01:12.000000 mapdata-3.7.1/mapdata/symbols/16x16/up.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-30 12:50:50.000000 mapdata-3.7.1/mapdata/symbols/16x16/vapor.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 03:55:52.000000 mapdata-3.7.1/mapdata/symbols/16x16/warning.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 20:02:51.000000 mapdata-3.7.1/mapdata/symbols/16x16/wave.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:12:01.000000 mapdata-3.7.1/mapdata/symbols/16x16/wave2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:12:43.000000 mapdata-3.7.1/mapdata/symbols/16x16/wave3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-04-30 14:42:04.000000 mapdata-3.7.1/mapdata/symbols/16x16/weather.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 16:37:24.000000 mapdata-3.7.1/mapdata/symbols/16x16/wedge.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-25 13:53:34.000000 mapdata-3.7.1/mapdata/symbols/16x16/wedge_sm.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-29 15:40:02.000000 mapdata-3.7.1/mapdata/symbols/16x16/wedges_3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-20 14:23:44.000000 mapdata-3.7.1/mapdata/symbols/16x16/well.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 22:20:04.000000 mapdata-3.7.1/mapdata/symbols/16x16/whale.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-28 12:54:47.000000 mapdata-3.7.1/mapdata/symbols/16x16/whale2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-06-24 15:49:53.000000 mapdata-3.7.1/mapdata/symbols/16x16/wheelchair.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 04:04:57.000000 mapdata-3.7.1/mapdata/symbols/16x16/zigzags.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-19 04:39:05.000000 mapdata-3.7.1/mapdata/symbols/16x16/zigzags2.xbm
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-28 15:17:52.470894 mapdata-3.7.1/mapdata/symbols/20x20/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      464 2023-06-24 14:14:12.000000 mapdata-3.7.1/mapdata/symbols/20x20/ball20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      467 2023-06-24 14:24:29.000000 mapdata-3.7.1/mapdata/symbols/20x20/block20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      470 2023-06-24 14:13:06.000000 mapdata-3.7.1/mapdata/symbols/20x20/circle20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:11.000000 mapdata-3.7.1/mapdata/symbols/20x20/q1_20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:22.000000 mapdata-3.7.1/mapdata/symbols/20x20/q2_20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:35.000000 mapdata-3.7.1/mapdata/symbols/20x20/q3_20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:54.000000 mapdata-3.7.1/mapdata/symbols/20x20/q4_20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      470 2023-06-24 14:24:00.000000 mapdata-3.7.1/mapdata/symbols/20x20/square20.xbm
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-28 15:17:52.470894 mapdata-3.7.1/mapdata/symbols/24x24/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      539 2023-06-24 14:20:48.000000 mapdata-3.7.1/mapdata/symbols/24x24/ball24.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      542 2023-06-24 14:25:39.000000 mapdata-3.7.1/mapdata/symbols/24x24/block24.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      545 2023-06-24 14:20:00.000000 mapdata-3.7.1/mapdata/symbols/24x24/circle24.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      545 2023-06-24 14:22:10.000000 mapdata-3.7.1/mapdata/symbols/24x24/square24.xbm
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-28 15:17:52.470894 mapdata-3.7.1/mapdata/symbols/28x28/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      793 2023-06-24 14:41:23.000000 mapdata-3.7.1/mapdata/symbols/28x28/ball28.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      794 2023-06-24 14:42:33.000000 mapdata-3.7.1/mapdata/symbols/28x28/block28.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      797 2023-06-24 14:41:39.000000 mapdata-3.7.1/mapdata/symbols/28x28/circle28.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      797 2023-06-24 14:42:15.000000 mapdata-3.7.1/mapdata/symbols/28x28/square28.xbm
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-28 15:17:52.470894 mapdata-3.7.1/mapdata.egg-info/
--rw-r--r--   0 dreas     (1000) dreas     (1000)     7898 2024-05-28 15:17:52.000000 mapdata-3.7.1/mapdata.egg-info/PKG-INFO
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     6598 2024-05-28 15:17:52.000000 mapdata-3.7.1/mapdata.egg-info/SOURCES.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2024-05-28 15:17:52.000000 mapdata-3.7.1/mapdata.egg-info/dependency_links.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      143 2024-05-28 15:17:52.000000 mapdata-3.7.1/mapdata.egg-info/requires.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        8 2024-05-28 15:17:52.000000 mapdata-3.7.1/mapdata.egg-info/top_level.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2024-05-28 15:17:52.470894 mapdata-3.7.1/setup.cfg
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     1813 2024-05-28 15:10:40.000000 mapdata-3.7.1/setup.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-29 20:15:00.634091 mapdata-3.7.2/
+-rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-3.7.2/LICENSE.txt
+-rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-3.7.2/MANIFEST.in
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     7898 2024-05-29 20:15:00.630091 mapdata-3.7.2/PKG-INFO
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     6421 2024-05-04 17:16:18.000000 mapdata-3.7.2/README.md
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-29 20:15:00.574090 mapdata-3.7.2/mapdata/
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-29 20:15:00.578091 mapdata-3.7.2/mapdata/configfile/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     9002 2024-03-04 21:04:24.000000 mapdata-3.7.2/mapdata/configfile/mapdata.conf
+-rwxrwxr-x   0 dreas     (1000) dreas     (1000)   693471 2024-05-29 19:29:21.000000 mapdata-3.7.2/mapdata/mapdata.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-29 20:15:00.574090 mapdata-3.7.2/mapdata/symbols/
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-29 20:15:00.630091 mapdata-3.7.2/mapdata/symbols/16x16/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:04:56.000000 mapdata-3.7.2/mapdata/symbols/16x16/0.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:16.000000 mapdata-3.7.2/mapdata/symbols/16x16/1.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:29.000000 mapdata-3.7.2/mapdata/symbols/16x16/2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:40.000000 mapdata-3.7.2/mapdata/symbols/16x16/3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:05:52.000000 mapdata-3.7.2/mapdata/symbols/16x16/4.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:06:03.000000 mapdata-3.7.2/mapdata/symbols/16x16/5.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2024-01-31 04:28:02.000000 mapdata-3.7.2/mapdata/symbols/16x16/6.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:06:27.000000 mapdata-3.7.2/mapdata/symbols/16x16/7.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:06:40.000000 mapdata-3.7.2/mapdata/symbols/16x16/8.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2024-01-31 04:26:59.000000 mapdata-3.7.2/mapdata/symbols/16x16/9.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-15 16:04:26.000000 mapdata-3.7.2/mapdata/symbols/16x16/A.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:07:30.000000 mapdata-3.7.2/mapdata/symbols/16x16/B.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:10:14.000000 mapdata-3.7.2/mapdata/symbols/16x16/C.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:13:27.000000 mapdata-3.7.2/mapdata/symbols/16x16/D.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:14:22.000000 mapdata-3.7.2/mapdata/symbols/16x16/E.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-15 16:15:26.000000 mapdata-3.7.2/mapdata/symbols/16x16/F.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 00:14:24.000000 mapdata-3.7.2/mapdata/symbols/16x16/G.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:15:07.000000 mapdata-3.7.2/mapdata/symbols/16x16/H.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:16:00.000000 mapdata-3.7.2/mapdata/symbols/16x16/I.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:18:38.000000 mapdata-3.7.2/mapdata/symbols/16x16/J.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:21:25.000000 mapdata-3.7.2/mapdata/symbols/16x16/K.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:22:10.000000 mapdata-3.7.2/mapdata/symbols/16x16/L.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:24:58.000000 mapdata-3.7.2/mapdata/symbols/16x16/M.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:27:42.000000 mapdata-3.7.2/mapdata/symbols/16x16/N.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 14:04:25.000000 mapdata-3.7.2/mapdata/symbols/16x16/O.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:28:05.000000 mapdata-3.7.2/mapdata/symbols/16x16/P.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:29:12.000000 mapdata-3.7.2/mapdata/symbols/16x16/Q.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:30:16.000000 mapdata-3.7.2/mapdata/symbols/16x16/R.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:34:31.000000 mapdata-3.7.2/mapdata/symbols/16x16/S.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:35:37.000000 mapdata-3.7.2/mapdata/symbols/16x16/T.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:37:27.000000 mapdata-3.7.2/mapdata/symbols/16x16/U.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:40:22.000000 mapdata-3.7.2/mapdata/symbols/16x16/V.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:44:48.000000 mapdata-3.7.2/mapdata/symbols/16x16/W.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:46:24.000000 mapdata-3.7.2/mapdata/symbols/16x16/X.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:47:50.000000 mapdata-3.7.2/mapdata/symbols/16x16/Y.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:49:43.000000 mapdata-3.7.2/mapdata/symbols/16x16/Z.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-21 14:55:41.000000 mapdata-3.7.2/mapdata/symbols/16x16/airplane.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-06-24 15:22:11.000000 mapdata-3.7.2/mapdata/symbols/16x16/anchor.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-07-04 17:00:25.000000 mapdata-3.7.2/mapdata/symbols/16x16/ball.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2024-01-24 20:44:54.000000 mapdata-3.7.2/mapdata/symbols/16x16/ball_small.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-05-16 13:39:00.000000 mapdata-3.7.2/mapdata/symbols/16x16/bar.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-07-04 17:04:48.000000 mapdata-3.7.2/mapdata/symbols/16x16/bars.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 14:43:55.000000 mapdata-3.7.2/mapdata/symbols/16x16/binoculars.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 22:29:19.000000 mapdata-3.7.2/mapdata/symbols/16x16/bird.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      288 2023-04-24 16:37:43.000000 mapdata-3.7.2/mapdata/symbols/16x16/block.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2024-01-26 04:36:33.000000 mapdata-3.7.2/mapdata/symbols/16x16/block_small.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-16 18:31:20.000000 mapdata-3.7.2/mapdata/symbols/16x16/bookmark.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-24 15:29:01.000000 mapdata-3.7.2/mapdata/symbols/16x16/box_stack.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-04-30 14:46:15.000000 mapdata-3.7.2/mapdata/symbols/16x16/camera.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-25 16:51:47.000000 mapdata-3.7.2/mapdata/symbols/16x16/cancel.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-05-21 15:05:05.000000 mapdata-3.7.2/mapdata/symbols/16x16/car.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-21 15:04:37.000000 mapdata-3.7.2/mapdata/symbols/16x16/car2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-24 01:00:13.000000 mapdata-3.7.2/mapdata/symbols/16x16/center8.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:35:37.000000 mapdata-3.7.2/mapdata/symbols/16x16/check.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-06-24 14:51:14.000000 mapdata-3.7.2/mapdata/symbols/16x16/check_circle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-16 14:20:03.000000 mapdata-3.7.2/mapdata/symbols/16x16/checkbox.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-04-28 13:31:04.000000 mapdata-3.7.2/mapdata/symbols/16x16/checkerboard.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 14:29:46.000000 mapdata-3.7.2/mapdata/symbols/16x16/chevrons.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-16 18:12:28.000000 mapdata-3.7.2/mapdata/symbols/16x16/circle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 14:22:20.000000 mapdata-3.7.2/mapdata/symbols/16x16/circle_bar.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-06-24 14:58:14.000000 mapdata-3.7.2/mapdata/symbols/16x16/circle_plus.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      314 2023-04-28 13:09:20.000000 mapdata-3.7.2/mapdata/symbols/16x16/circle_stipple.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      317 2023-06-24 14:29:15.000000 mapdata-3.7.2/mapdata/symbols/16x16/circle_triangle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-04-25 14:40:36.000000 mapdata-3.7.2/mapdata/symbols/16x16/circle_wedge.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-06-24 14:56:37.000000 mapdata-3.7.2/mapdata/symbols/16x16/circle_x.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-07-04 17:10:15.000000 mapdata-3.7.2/mapdata/symbols/16x16/clock.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 14:05:41.000000 mapdata-3.7.2/mapdata/symbols/16x16/columns.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-25 13:50:11.000000 mapdata-3.7.2/mapdata/symbols/16x16/contract.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-04-16 17:48:39.000000 mapdata-3.7.2/mapdata/symbols/16x16/cross.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-23 18:45:40.000000 mapdata-3.7.2/mapdata/symbols/16x16/darkeye.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:18:32.000000 mapdata-3.7.2/mapdata/symbols/16x16/decrease.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-06-30 12:46:46.000000 mapdata-3.7.2/mapdata/symbols/16x16/deposition.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:47.000000 mapdata-3.7.2/mapdata/symbols/16x16/diag_ll.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:26.000000 mapdata-3.7.2/mapdata/symbols/16x16/diag_lr.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:05.000000 mapdata-3.7.2/mapdata/symbols/16x16/diag_ul.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:17:04.000000 mapdata-3.7.2/mapdata/symbols/16x16/diag_ur.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-20 18:41:19.000000 mapdata-3.7.2/mapdata/symbols/16x16/dialog.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-16 17:38:10.000000 mapdata-3.7.2/mapdata/symbols/16x16/diamond.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 13:47:24.000000 mapdata-3.7.2/mapdata/symbols/16x16/donkey.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-04-30 16:45:55.000000 mapdata-3.7.2/mapdata/symbols/16x16/dot.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:00:44.000000 mapdata-3.7.2/mapdata/symbols/16x16/down.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:38:22.000000 mapdata-3.7.2/mapdata/symbols/16x16/drop.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-03 02:15:55.000000 mapdata-3.7.2/mapdata/symbols/16x16/elephant.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-25 14:33:40.000000 mapdata-3.7.2/mapdata/symbols/16x16/expand.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-04-30 15:03:32.000000 mapdata-3.7.2/mapdata/symbols/16x16/eye.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-06-24 13:59:48.000000 mapdata-3.7.2/mapdata/symbols/16x16/fire.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 22:13:54.000000 mapdata-3.7.2/mapdata/symbols/16x16/fish.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-30 14:36:11.000000 mapdata-3.7.2/mapdata/symbols/16x16/flag.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-30 15:04:58.000000 mapdata-3.7.2/mapdata/symbols/16x16/flag2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-06-24 15:06:07.000000 mapdata-3.7.2/mapdata/symbols/16x16/four_arrows.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 22:25:14.000000 mapdata-3.7.2/mapdata/symbols/16x16/graph.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-06-24 15:18:19.000000 mapdata-3.7.2/mapdata/symbols/16x16/hand.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:04:09.000000 mapdata-3.7.2/mapdata/symbols/16x16/hash.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-03 01:53:41.000000 mapdata-3.7.2/mapdata/symbols/16x16/heart.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2024-01-31 04:51:54.000000 mapdata-3.7.2/mapdata/symbols/16x16/hidden.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-24 15:40:09.000000 mapdata-3.7.2/mapdata/symbols/16x16/hourglass.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-24 22:31:53.000000 mapdata-3.7.2/mapdata/symbols/16x16/house.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:18:05.000000 mapdata-3.7.2/mapdata/symbols/16x16/increase.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-24 23:05:40.000000 mapdata-3.7.2/mapdata/symbols/16x16/info.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-30 14:51:36.000000 mapdata-3.7.2/mapdata/symbols/16x16/leaf.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:02:45.000000 mapdata-3.7.2/mapdata/symbols/16x16/left.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-23 13:36:40.000000 mapdata-3.7.2/mapdata/symbols/16x16/lightbulb.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 16:38:25.000000 mapdata-3.7.2/mapdata/symbols/16x16/lightning.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      314 2023-04-28 13:14:23.000000 mapdata-3.7.2/mapdata/symbols/16x16/lightning2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-07-04 16:58:13.000000 mapdata-3.7.2/mapdata/symbols/16x16/location_ptr.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-20 14:06:42.000000 mapdata-3.7.2/mapdata/symbols/16x16/mine.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-06-24 15:07:56.000000 mapdata-3.7.2/mapdata/symbols/16x16/nested_boxes.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 14:07:35.000000 mapdata-3.7.2/mapdata/symbols/16x16/pennant.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 13:16:09.000000 mapdata-3.7.2/mapdata/symbols/16x16/pennant2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-18 19:04:36.000000 mapdata-3.7.2/mapdata/symbols/16x16/people.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:26:34.000000 mapdata-3.7.2/mapdata/symbols/16x16/person.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:30:45.000000 mapdata-3.7.2/mapdata/symbols/16x16/person2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-20 18:43:50.000000 mapdata-3.7.2/mapdata/symbols/16x16/person3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-24 15:37:42.000000 mapdata-3.7.2/mapdata/symbols/16x16/phone.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:18:45.000000 mapdata-3.7.2/mapdata/symbols/16x16/photo.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-19 22:48:26.000000 mapdata-3.7.2/mapdata/symbols/16x16/picnic.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-19 03:57:15.000000 mapdata-3.7.2/mapdata/symbols/16x16/plus.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      358 2023-05-03 01:58:16.000000 mapdata-3.7.2/mapdata/symbols/16x16/point_down.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      356 2023-05-03 01:58:03.000000 mapdata-3.7.2/mapdata/symbols/16x16/point_left.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      362 2023-05-03 01:57:47.000000 mapdata-3.7.2/mapdata/symbols/16x16/point_right.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      347 2023-05-03 01:56:56.000000 mapdata-3.7.2/mapdata/symbols/16x16/point_up.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      357 2023-05-03 01:58:38.000000 mapdata-3.7.2/mapdata/symbols/16x16/pointer_ne.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      356 2023-05-03 01:59:20.000000 mapdata-3.7.2/mapdata/symbols/16x16/pointer_nw.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      358 2023-05-03 01:58:54.000000 mapdata-3.7.2/mapdata/symbols/16x16/pointer_se.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      357 2023-05-03 01:59:07.000000 mapdata-3.7.2/mapdata/symbols/16x16/pointer_sw.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-20 18:51:06.000000 mapdata-3.7.2/mapdata/symbols/16x16/puzzle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:52:56.000000 mapdata-3.7.2/mapdata/symbols/16x16/q1.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:57:59.000000 mapdata-3.7.2/mapdata/symbols/16x16/q1_notch.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:25.000000 mapdata-3.7.2/mapdata/symbols/16x16/q2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:55.000000 mapdata-3.7.2/mapdata/symbols/16x16/q2_notch.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:46.000000 mapdata-3.7.2/mapdata/symbols/16x16/q3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:28.000000 mapdata-3.7.2/mapdata/symbols/16x16/q3_notch.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:57.000000 mapdata-3.7.2/mapdata/symbols/16x16/q4.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:13.000000 mapdata-3.7.2/mapdata/symbols/16x16/q4_notch.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-05-20 18:36:19.000000 mapdata-3.7.2/mapdata/symbols/16x16/qmark_circle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      311 2023-05-20 18:37:52.000000 mapdata-3.7.2/mapdata/symbols/16x16/qmark_circle2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:43:45.000000 mapdata-3.7.2/mapdata/symbols/16x16/raincloud.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-24 16:39:34.000000 mapdata-3.7.2/mapdata/symbols/16x16/right.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-20 17:23:57.000000 mapdata-3.7.2/mapdata/symbols/16x16/rocket.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-20 17:25:43.000000 mapdata-3.7.2/mapdata/symbols/16x16/rocket2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-23 16:07:27.000000 mapdata-3.7.2/mapdata/symbols/16x16/rose.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-28 14:05:56.000000 mapdata-3.7.2/mapdata/symbols/16x16/rows.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-28 14:27:34.000000 mapdata-3.7.2/mapdata/symbols/16x16/scales.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-07-04 17:07:45.000000 mapdata-3.7.2/mapdata/symbols/16x16/search.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-07-04 17:08:06.000000 mapdata-3.7.2/mapdata/symbols/16x16/search2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-01 15:46:45.000000 mapdata-3.7.2/mapdata/symbols/16x16/skull.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-17 02:43:53.000000 mapdata-3.7.2/mapdata/symbols/16x16/square.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:26:56.000000 mapdata-3.7.2/mapdata/symbols/16x16/star.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 13:07:07.000000 mapdata-3.7.2/mapdata/symbols/16x16/stipple.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-03 02:10:57.000000 mapdata-3.7.2/mapdata/symbols/16x16/stop.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      317 2023-06-24 15:31:50.000000 mapdata-3.7.2/mapdata/symbols/16x16/surprise_circle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:22:10.000000 mapdata-3.7.2/mapdata/symbols/16x16/swamp.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-16 18:27:50.000000 mapdata-3.7.2/mapdata/symbols/16x16/target.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 04:37:09.000000 mapdata-3.7.2/mapdata/symbols/16x16/target2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-06-24 15:27:04.000000 mapdata-3.7.2/mapdata/symbols/16x16/ten.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-24 14:54:31.000000 mapdata-3.7.2/mapdata/symbols/16x16/trash.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-09 17:01:43.000000 mapdata-3.7.2/mapdata/symbols/16x16/tree.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 12:59:30.000000 mapdata-3.7.2/mapdata/symbols/16x16/tree2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:26:26.000000 mapdata-3.7.2/mapdata/symbols/16x16/tree3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-09 16:59:51.000000 mapdata-3.7.2/mapdata/symbols/16x16/triangle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      311 2023-05-09 17:08:13.000000 mapdata-3.7.2/mapdata/symbols/16x16/triangle_open.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-05-20 17:46:38.000000 mapdata-3.7.2/mapdata/symbols/16x16/triangle_sm.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-04-16 18:01:12.000000 mapdata-3.7.2/mapdata/symbols/16x16/up.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-30 12:50:50.000000 mapdata-3.7.2/mapdata/symbols/16x16/vapor.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 03:55:52.000000 mapdata-3.7.2/mapdata/symbols/16x16/warning.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 20:02:51.000000 mapdata-3.7.2/mapdata/symbols/16x16/wave.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:12:01.000000 mapdata-3.7.2/mapdata/symbols/16x16/wave2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:12:43.000000 mapdata-3.7.2/mapdata/symbols/16x16/wave3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-04-30 14:42:04.000000 mapdata-3.7.2/mapdata/symbols/16x16/weather.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 16:37:24.000000 mapdata-3.7.2/mapdata/symbols/16x16/wedge.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-25 13:53:34.000000 mapdata-3.7.2/mapdata/symbols/16x16/wedge_sm.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-29 15:40:02.000000 mapdata-3.7.2/mapdata/symbols/16x16/wedges_3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-20 14:23:44.000000 mapdata-3.7.2/mapdata/symbols/16x16/well.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 22:20:04.000000 mapdata-3.7.2/mapdata/symbols/16x16/whale.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-28 12:54:47.000000 mapdata-3.7.2/mapdata/symbols/16x16/whale2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-06-24 15:49:53.000000 mapdata-3.7.2/mapdata/symbols/16x16/wheelchair.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 04:04:57.000000 mapdata-3.7.2/mapdata/symbols/16x16/zigzags.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-19 04:39:05.000000 mapdata-3.7.2/mapdata/symbols/16x16/zigzags2.xbm
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-29 20:15:00.630091 mapdata-3.7.2/mapdata/symbols/20x20/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      464 2023-06-24 14:14:12.000000 mapdata-3.7.2/mapdata/symbols/20x20/ball20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      467 2023-06-24 14:24:29.000000 mapdata-3.7.2/mapdata/symbols/20x20/block20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      470 2023-06-24 14:13:06.000000 mapdata-3.7.2/mapdata/symbols/20x20/circle20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:11.000000 mapdata-3.7.2/mapdata/symbols/20x20/q1_20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:22.000000 mapdata-3.7.2/mapdata/symbols/20x20/q2_20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:35.000000 mapdata-3.7.2/mapdata/symbols/20x20/q3_20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:54.000000 mapdata-3.7.2/mapdata/symbols/20x20/q4_20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      470 2023-06-24 14:24:00.000000 mapdata-3.7.2/mapdata/symbols/20x20/square20.xbm
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-29 20:15:00.630091 mapdata-3.7.2/mapdata/symbols/24x24/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      539 2023-06-24 14:20:48.000000 mapdata-3.7.2/mapdata/symbols/24x24/ball24.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      542 2023-06-24 14:25:39.000000 mapdata-3.7.2/mapdata/symbols/24x24/block24.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      545 2023-06-24 14:20:00.000000 mapdata-3.7.2/mapdata/symbols/24x24/circle24.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      545 2023-06-24 14:22:10.000000 mapdata-3.7.2/mapdata/symbols/24x24/square24.xbm
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-29 20:15:00.630091 mapdata-3.7.2/mapdata/symbols/28x28/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      793 2023-06-24 14:41:23.000000 mapdata-3.7.2/mapdata/symbols/28x28/ball28.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      794 2023-06-24 14:42:33.000000 mapdata-3.7.2/mapdata/symbols/28x28/block28.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      797 2023-06-24 14:41:39.000000 mapdata-3.7.2/mapdata/symbols/28x28/circle28.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      797 2023-06-24 14:42:15.000000 mapdata-3.7.2/mapdata/symbols/28x28/square28.xbm
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-29 20:15:00.630091 mapdata-3.7.2/mapdata.egg-info/
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     7898 2024-05-29 20:15:00.000000 mapdata-3.7.2/mapdata.egg-info/PKG-INFO
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     6598 2024-05-29 20:15:00.000000 mapdata-3.7.2/mapdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2024-05-29 20:15:00.000000 mapdata-3.7.2/mapdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      143 2024-05-29 20:15:00.000000 mapdata-3.7.2/mapdata.egg-info/requires.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        8 2024-05-29 20:15:00.000000 mapdata-3.7.2/mapdata.egg-info/top_level.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2024-05-29 20:15:00.634091 mapdata-3.7.2/setup.cfg
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     1813 2024-05-29 19:30:39.000000 mapdata-3.7.2/setup.py
```

### Comparing `mapdata-3.7.1/LICENSE.txt` & `mapdata-3.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapdata-3.7.1/PKG-INFO` & `mapdata-3.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 3.7.1
+Version: 3.7.2
 Summary: An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: cortice@tutanota.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,Spreadsheet,Database,PNG,JPG,Postscript
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mapdata-3.7.1/README.md` & `mapdata-3.7.2/README.md`

 * *Files identical despite different names*

### Comparing `mapdata-3.7.1/mapdata/configfile/mapdata.conf` & `mapdata-3.7.2/mapdata/configfile/mapdata.conf`

 * *Files identical despite different names*

### Comparing `mapdata-3.7.1/mapdata/mapdata.py` & `mapdata-3.7.2/mapdata/mapdata.py`

 * *Files identical despite different names*

```diff
@@ -20,16 +20,16 @@
 # 	The GNU General Public License is available at <http://www.gnu.org/licenses/>
 #
 # AUTHOR
 #	Dreas Nielsen (RDN)
 #
 # ==================================================================
 
-version = "3.7.1"
-vdate = "2024-05-25"
+version = "3.7.2"
+vdate = "2024-05-29"
 
 copyright = "2023-2024"
 
 
 import sys
 import os.path
 import io
@@ -293,14 +293,31 @@
 		return self.empty_tile_image
 
 tkmv.map_widget.TkinterMapView.request_image = alt_request_image
 
 
 #=====  Global constants and variables =====
 
+# SQL (SQLite) keywords
+sql_kw = ('add', 'all', 'alter', 'analyze', 'and', 'as', 'asc', 'autoincrement', 'before', 'begin',
+			'between', 'by', 'cascade', 'case', 'cast', 'check', 'column', 'commit', 'conflict', 'constraint',
+			'create', 'cross', 'current', 'current_date', 'current_time', 'current_timestamp', 'database',
+			'default', 'delete', 'desc', 'distinct', 'do', 'drop', 'each', 'else', 'end', 'except', 'exclude',
+			'exclusive', 'exists', 'explain', 'filter', 'first', 'for', 'foreign', 'from', 'full', 'glob',
+			'group', 'groups', 'having', 'if', 'immediate', 'in', 'index', 'indexed', 'initially', 'inner',
+			'insert', 'instead', 'intersect', 'into', 'is', 'isnull', 'join', 'key', 'last', 'left', 'like',
+			'limit', 'match', 'materialized', 'natural', 'no', 'not', 'nothing', 'notnull', 'null', 'nulls',
+			'of', 'offset', 'on', 'or', 'order', 'others', 'outer', 'over', 'partition', 'plan', 'pragma',
+			'preceding', 'primary', 'query', 'raise', 'range', 'recursive', 'references', 'reindex', 'release',
+			'rename', 'replace', 'restrict', 'returning', 'right', 'rollback', 'row', 'rows', 'savepoint',
+			'select', 'set', 'table', 'temp', 'temporary', 'then', 'ties', 'to', 'transaction', 'trigger',
+			'unbounded', 'union', 'unique', 'update', 'using', 'vacuum', 'values', 'view', 'virtual',
+			'when', 'where', 'window', 'with', 'without')
+
+
 # Tile servers for map basemap layers
 bm_servers = {"OpenStreetMap": "https://a.tile.openstreetmap.org/{z}/{x}/{y}.png",
 			"Google streets": "https://mt0.google.com/vt/lyrs=m&hl=en&x={x}&y={y}&z={z}&s=Ga",
 			"Google satellite": "https://mt0.google.com/vt/lyrs=s&hl=en&x={x}&y={y}&z={z}&s=Ga",
 			"Open topo map": "https://tile.opentopomap.org/{z}/{x}/{y}.png"
 			}
 
@@ -1496,14 +1513,16 @@
 	# with double-quoting of any name that is not all alphanumeric and starts with
 	# an alphabetic.
 	colnames = []
 	for hdr in tbl_hdrs:
 		h2 = re.subn(r'\W', '_', hdr)[0]
 		if not h2[0].isalnum() and h2[0] != '_':
 			h2 = '_' + h2
+		if h2.lower() in sql_kw:
+			h2 = h2 + '_'
 		colnames.append(h2)
 	return colnames
 
 def isint(v):
 	# Missing values match and will be handled by 'conv_int()'
 	if v is None or (type(v) is str and v.strip() == ''):
 		return True
@@ -2154,14 +2173,24 @@
 		if args.message is None:
 			self.win.title("Map of %s" % src_name)
 
 		# Source and possibly un-projected crs
 		self.src_crs = crs
 		self.crs = crs
 
+		# Check that the specified column names are valid.
+		if not (lat_col in headers and lon_col in headers):
+			fatal_error("The specified coordinate columns are not in the data table.", kwargs={"parent": self.win})
+		if label_col is not None and not (label_col in headers):
+			fatal_error("The label column is not in the data table.", kwargs={"parent": self.win})
+		if symbol_col is not None and not (symbol_col in headers):
+			fatal_error("The symbol type column is not in the data table.", kwargs={"parent": self.win})
+		if color_col is not None and not (color_col in headers):
+			fatal_error("The symbol color column is not in the data table.", kwargs={"parent": self.win})
+
 		# Populate the table frame
 		self.tblframe.rowconfigure(0, weight=1)
 		self.tblframe.columnconfigure(0, weight=1)
 		try:
 			self.tableframe, self.tbl = self.add_data(rows, headers, lat_col, lon_col, label_col, symbol_col, color_col)
 		except:
 			self.loading_dlg.hide_all()
@@ -2501,15 +2530,14 @@
 			except:
 				lon_val = None
 			if lon_val is not None and lat_val is not None:
 				has_latlon = True
 				break
 		if not has_latlon:
 			fatal_error("All data rows are missing latitude and longitude coordinates.", {'parent': self.win})
-	
 
 		# Determine data types for use in table statistics display and in column selection for plotting.
 		# This is done in a separate process for performance (on Linux).  After the data types are set,
 		# values in numeric columns in SQLite and the Treeview table are cast to the appropriate numeric type.
 		# This is done as early as possible in 'add_data()' to give its process as much time as possible
 		# before it is needed by the 'build_database' process.
 		self.launch_set_data_types(headers, rows)
```

### Comparing `mapdata-3.7.1/mapdata/symbols/24x24/ball24.xbm` & `mapdata-3.7.2/mapdata/symbols/24x24/ball24.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.7.1/mapdata/symbols/24x24/block24.xbm` & `mapdata-3.7.2/mapdata/symbols/24x24/block24.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.7.1/mapdata/symbols/24x24/circle24.xbm` & `mapdata-3.7.2/mapdata/symbols/24x24/circle24.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.7.1/mapdata/symbols/24x24/square24.xbm` & `mapdata-3.7.2/mapdata/symbols/24x24/square24.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.7.1/mapdata/symbols/28x28/ball28.xbm` & `mapdata-3.7.2/mapdata/symbols/28x28/ball28.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.7.1/mapdata/symbols/28x28/block28.xbm` & `mapdata-3.7.2/mapdata/symbols/28x28/block28.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.7.1/mapdata/symbols/28x28/circle28.xbm` & `mapdata-3.7.2/mapdata/symbols/28x28/circle28.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.7.1/mapdata/symbols/28x28/square28.xbm` & `mapdata-3.7.2/mapdata/symbols/28x28/square28.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.7.1/mapdata.egg-info/PKG-INFO` & `mapdata-3.7.2/mapdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 3.7.1
+Version: 3.7.2
 Summary: An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: cortice@tutanota.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,Spreadsheet,Database,PNG,JPG,Postscript
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mapdata-3.7.1/mapdata.egg-info/SOURCES.txt` & `mapdata-3.7.2/mapdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mapdata-3.7.1/setup.py` & `mapdata-3.7.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with io.open('README.md', encoding='utf-8') as f:
 	long_description = f.read()
 
 symbol_files = glob.glob("mapdata/symbols/16x16/*.xbm") + glob.glob("mapdata/symbols/20x20/*.xbm") + \
 			glob.glob("mapdata/symbols/24x24/*.xbm") + glob.glob("mapdata/symbols/28x28/*.xbm")
 
 setuptools.setup(name='mapdata',
-	version='3.7.1',
+	version='3.7.2',
 	description="An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database",
 	author='Dreas Nielsen',
 	author_email='cortice@tutanota.com',
     url='https://osdn.net/project/mapdata/',
     packages=['mapdata'],
 	scripts=['mapdata/mapdata.py'],
 	data_files=[('symbols', symbol_files), ('config', ['mapdata/configfile/mapdata.conf'])],
```

