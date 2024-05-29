# Comparing `tmp/uplogic-2.2.tar.gz` & `tmp/uplogic-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uplogic-2.2.tar", last modified: Tue Apr 23 18:17:52 2024, max compression
+gzip compressed data, was "uplogic-3.2.tar", last modified: Wed May 29 08:25:10 2024, max compression
```

## Comparing `uplogic-2.2.tar` & `uplogic-3.2.tar`

### file list

```diff
@@ -1,426 +1,1573 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.601885 uplogic-2.2/
--rw-rw-rw-   0        0        0      189 2022-01-15 11:35:38.000000 uplogic-2.2/LICENSE.md
--rw-rw-rw-   0        0        0     1045 2024-04-23 18:17:52.600888 uplogic-2.2/PKG-INFO
--rw-rw-rw-   0        0        0      262 2022-01-15 11:34:53.000000 uplogic-2.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 18:17:52.601885 uplogic-2.2/setup.cfg
--rw-rw-rw-   0        0        0     1739 2024-04-23 18:17:43.000000 uplogic-2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.442417 uplogic-2.2/uplogic/
--rw-rw-rw-   0        0        0     6474 2024-03-22 08:56:45.000000 uplogic-2.2/uplogic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.456371 uplogic-2.2/uplogic/animation/
--rw-rw-rw-   0        0        0      341 2023-12-07 08:59:05.000000 uplogic-2.2/uplogic/animation/__init__.py
--rw-rw-rw-   0        0        0    14151 2024-04-23 18:12:22.000000 uplogic-2.2/uplogic/animation/action.py
--rw-rw-rw-   0        0        0     4152 2024-02-18 10:41:26.000000 uplogic-2.2/uplogic/animation/actionsystem.py
--rw-rw-rw-   0        0        0     2419 2023-11-10 06:42:05.000000 uplogic-2.2/uplogic/animation/rig.py
--rw-rw-rw-   0        0        0     6893 2024-02-18 10:45:19.000000 uplogic-2.2/uplogic/animation/sequence.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.457368 uplogic-2.2/uplogic/audio/
--rw-rw-rw-   0        0        0      606 2023-12-15 10:12:29.000000 uplogic-2.2/uplogic/audio/__init__.py
--rw-rw-rw-   0        0        0     7747 2024-02-10 14:51:22.000000 uplogic-2.2/uplogic/audio/audiosystem.py
--rw-rw-rw-   0        0        0     6839 2023-05-14 08:47:09.000000 uplogic-2.2/uplogic/audio/music.py
--rw-rw-rw-   0        0        0    24557 2024-03-18 08:04:37.000000 uplogic-2.2/uplogic/audio/sound.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.458364 uplogic-2.2/uplogic/console/
--rw-rw-rw-   0        0        0    12943 2024-04-23 18:12:22.000000 uplogic-2.2/uplogic/console/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.459361 uplogic-2.2/uplogic/data/
--rw-rw-rw-   0        0        0     1861 2022-10-06 13:43:59.000000 uplogic-2.2/uplogic/data/__init__.py
--rw-rw-rw-   0        0        0     3161 2024-02-02 14:24:41.000000 uplogic-2.2/uplogic/data/file.py
--rw-rw-rw-   0        0        0     7457 2024-03-18 08:04:37.000000 uplogic-2.2/uplogic/data/globaldb.py
--rw-rw-rw-   0        0        0     2050 2021-12-21 09:41:07.000000 uplogic-2.2/uplogic/data/serializers.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.464345 uplogic-2.2/uplogic/decorators/
--rw-rw-rw-   0        0        0    18211 2024-02-18 10:35:16.000000 uplogic-2.2/uplogic/decorators/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.464345 uplogic-2.2/uplogic/events/
--rw-rw-rw-   0        0        0     8314 2024-02-18 10:46:49.000000 uplogic-2.2/uplogic/events/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.470324 uplogic-2.2/uplogic/input/
--rw-rw-rw-   0        0        0     1541 2023-09-30 18:00:52.000000 uplogic-2.2/uplogic/input/__init__.py
--rw-rw-rw-   0        0        0    15973 2024-04-23 18:12:22.000000 uplogic-2.2/uplogic/input/gamepad.py
--rw-rw-rw-   0        0        0    10967 2024-03-22 08:50:05.000000 uplogic-2.2/uplogic/input/keyboard.py
--rw-rw-rw-   0        0        0    15356 2024-03-18 14:27:09.000000 uplogic-2.2/uplogic/input/mouse.py
--rw-rw-rw-   0        0        0     9131 2023-05-14 08:49:48.000000 uplogic-2.2/uplogic/input/vr.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.471321 uplogic-2.2/uplogic/network/
--rw-rw-rw-   0        0        0       56 2023-06-05 09:06:00.000000 uplogic-2.2/uplogic/network/__init__.py
--rw-rw-rw-   0        0        0     2919 2024-03-22 08:56:49.000000 uplogic-2.2/uplogic/network/client.py
--rw-rw-rw-   0        0        0     4687 2024-03-22 08:56:53.000000 uplogic-2.2/uplogic/network/server.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.472318 uplogic-2.2/uplogic/nodes/
--rw-rw-rw-   0        0        0     4276 2024-02-19 13:51:02.000000 uplogic-2.2/uplogic/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.522151 uplogic-2.2/uplogic/nodes/actions/
--rw-rw-rw-   0        0        0     8317 2024-01-16 18:59:56.000000 uplogic-2.2/uplogic/nodes/actions/__init__.py
--rw-rw-rw-   0        0        0     4259 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/addfilter.py
--rw-rw-rw-   0        0        0     1049 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/addobject.py
--rw-rw-rw-   0        0        0     2180 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/addphysicsconstraint.py
--rw-rw-rw-   0        0        0      627 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/adduiwidget.py
--rw-rw-rw-   0        0        0      933 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/alignaxistovector.py
--rw-rw-rw-   0        0        0      820 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/appendlistitem.py
--rw-rw-rw-   0        0        0      684 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/applyforce.py
--rw-rw-rw-   0        0        0      799 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/applyimpulse.py
--rw-rw-rw-   0        0        0      728 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/applymovement.py
--rw-rw-rw-   0        0        0      891 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/applyrotation.py
--rw-rw-rw-   0        0        0      742 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/applytorque.py
--rw-rw-rw-   0        0        0     1501 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/applytransform.py
--rw-rw-rw-   0        0        0     1541 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/cameraraycast.py
--rw-rw-rw-   0        0        0      654 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/characterjump.py
--rw-rw-rw-   0        0        0     1174 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/clampedmodifyproperty.py
--rw-rw-rw-   0        0        0     1471 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/clearvariables.py
--rw-rw-rw-   0        0        0     1022 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/copyproperty.py
--rw-rw-rw-   0        0        0     3464 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/createuibutton.py
--rw-rw-rw-   0        0        0      734 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/createuicanvas.py
--rw-rw-rw-   0        0        0     1736 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/createuiimage.py
--rw-rw-rw-   0        0        0     2420 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/createuilabel.py
--rw-rw-rw-   0        0        0     2245 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/createuilayout.py
--rw-rw-rw-   0        0        0     4393 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/createuislider.py
--rw-rw-rw-   0        0        0     1618 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/createvehicle.py
--rw-rw-rw-   0        0        0     1287 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/cursorbehavior.py
--rw-rw-rw-   0        0        0      612 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/cursorvisibility.py
--rw-rw-rw-   0        0        0      775 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/dispatchevent.py
--rw-rw-rw-   0        0        0     2485 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/draw.py
--rw-rw-rw-   0        0        0     1123 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/drawbox.py
--rw-rw-rw-   0        0        0      979 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/drawcube.py
--rw-rw-rw-   0        0        0      922 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/drawline.py
--rw-rw-rw-   0        0        0     2993 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/editbone.py
--rw-rw-rw-   0        0        0      432 2023-10-13 21:24:56.000000 uplogic-2.2/uplogic/nodes/actions/endgame.py
--rw-rw-rw-   0        0        0      690 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/endobject.py
--rw-rw-rw-   0        0        0     1261 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/executesubnetwork.py
--rw-rw-rw-   0        0        0     4759 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/followpath.py
--rw-rw-rw-   0        0        0     2774 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/gamepadlook.py
--rw-rw-rw-   0        0        0     1146 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/gamepadvibration.py
--rw-rw-rw-   0        0        0     1973 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/getperformanceprofile.py
--rw-rw-rw-   0        0        0      963 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/installsubnetwork.py
--rw-rw-rw-   0        0        0     2005 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/instream.py
--rw-rw-rw-   0        0        0     1097 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/listglobalvalues.py
--rw-rw-rw-   0        0        0     1875 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/listvariables.py
--rw-rw-rw-   0        0        0      595 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/loadblendfile.py
--rw-rw-rw-   0        0        0     1510 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/loadfilecontent.py
--rw-rw-rw-   0        0        0     4039 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/loadgame.py
--rw-rw-rw-   0        0        0     1624 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/loadscene.py
--rw-rw-rw-   0        0        0     2437 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/localclient.py
--rw-rw-rw-   0        0        0     2313 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/localserver.py
--rw-rw-rw-   0        0        0      736 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/makeuniquelight.py
--rw-rw-rw-   0        0        0     1308 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/modifyproperty.py
--rw-rw-rw-   0        0        0     2711 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/mouselook.py
--rw-rw-rw-   0        0        0     1541 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/mouseraycast.py
--rw-rw-rw-   0        0        0      771 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/mousesetposition.py
--rw-rw-rw-   0        0        0     1117 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/moveto.py
--rw-rw-rw-   0        0        0     4608 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/movetowithnavmesh.py
--rw-rw-rw-   0        0        0      595 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/pausesound.py
--rw-rw-rw-   0        0        0     4347 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/playaction.py
--rw-rw-rw-   0        0        0     2237 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/playsequence.py
--rw-rw-rw-   0        0        0     1096 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/popdictkey.py
--rw-rw-rw-   0        0        0      623 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/printvalue.py
--rw-rw-rw-   0        0        0     2947 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/projectileraycast.py
--rw-rw-rw-   0        0        0     3025 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/raycast.py
--rw-rw-rw-   0        0        0      611 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/removefilter.py
--rw-rw-rw-   0        0        0      938 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/removelistindex.py
--rw-rw-rw-   0        0        0      971 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/removelistvalue.py
--rw-rw-rw-   0        0        0      633 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/removeoverlaycollection.py
--rw-rw-rw-   0        0        0      581 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/removeparent.py
--rw-rw-rw-   0        0        0      698 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/removephysicsconstraint.py
--rw-rw-rw-   0        0        0     1605 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/removevariable.py
--rw-rw-rw-   0        0        0     1025 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/replacemesh.py
--rw-rw-rw-   0        0        0      505 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/restartgame.py
--rw-rw-rw-   0        0        0      547 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/resumesound.py
--rw-rw-rw-   0        0        0      993 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/rotateto.py
--rw-rw-rw-   0        0        0      910 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/runactuator.py
--rw-rw-rw-   0        0        0     1855 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/runpython.py
--rw-rw-rw-   0        0        0     7749 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/savegame.py
--rw-rw-rw-   0        0        0     1773 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/savevariable.py
--rw-rw-rw-   0        0        0     1512 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/savevariabledict.py
--rw-rw-rw-   0        0        0     1016 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/sendmessage.py
--rw-rw-rw-   0        0        0      692 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/sendnetworkmessage.py
--rw-rw-rw-   0        0        0     2243 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setactionframe.py
--rw-rw-rw-   0        0        0      900 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setactuatorvalue.py
--rw-rw-rw-   0        0        0     1097 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setboneconstraintattr.py
--rw-rw-rw-   0        0        0      974 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setboneconstraintinfluence.py
--rw-rw-rw-   0        0        0      970 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setboneconstrainttarget.py
--rw-rw-rw-   0        0        0     1182 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setboneposition.py
--rw-rw-rw-   0        0        0      625 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setcamera.py
--rw-rw-rw-   0        0        0      617 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setcamerafov.py
--rw-rw-rw-   0        0        0      640 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setcameraorthoscale.py
--rw-rw-rw-   0        0        0      829 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setcharactergravity.py
--rw-rw-rw-   0        0        0      742 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setcharacterjumpspeed.py
--rw-rw-rw-   0        0        0      756 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setcharactermaxjumps.py
--rw-rw-rw-   0        0        0      871 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setcharactervelocity.py
--rw-rw-rw-   0        0        0     1450 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setcharacterwalkdir.py
--rw-rw-rw-   0        0        0      773 2024-04-04 13:01:22.000000 uplogic-2.2/uplogic/nodes/actions/setcollisiongroup.py
--rw-rw-rw-   0        0        0      661 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setcollisionmask.py
--rw-rw-rw-   0        0        0      851 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setconstraintattribute.py
--rw-rw-rw-   0        0        0     1137 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setcurvepoints.py
--rw-rw-rw-   0        0        0      964 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setcustomcursor.py
--rw-rw-rw-   0        0        0      860 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setdictkey.py
--rw-rw-rw-   0        0        0      820 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setdynamics.py
--rw-rw-rw-   0        0        0      659 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/seteeveeao.py
--rw-rw-rw-   0        0        0      663 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/seteeveebloom.py
--rw-rw-rw-   0        0        0      592 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/seteeveesmaa.py
--rw-rw-rw-   0        0        0      633 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/seteeveesmaaquality.py
--rw-rw-rw-   0        0        0      659 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/seteeveessr.py
--rw-rw-rw-   0        0        0      705 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/seteeveevolumetrics.py
--rw-rw-rw-   0        0        0      692 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setexposure.py
--rw-rw-rw-   0        0        0      697 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setfilterstate.py
--rw-rw-rw-   0        0        0      621 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setfullscreen.py
--rw-rw-rw-   0        0        0     1681 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setgameobjectattr.py
--rw-rw-rw-   0        0        0      686 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setgamma.py
--rw-rw-rw-   0        0        0      869 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setglobalvalue.py
--rw-rw-rw-   0        0        0      612 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setgravity.py
--rw-rw-rw-   0        0        0      778 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setlightcolor.py
--rw-rw-rw-   0        0        0      724 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setlightenergy.py
--rw-rw-rw-   0        0        0      744 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setlightshadow.py
--rw-rw-rw-   0        0        0      894 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setlistindex.py
--rw-rw-rw-   0        0        0      783 2024-01-22 11:02:02.000000 uplogic-2.2/uplogic/nodes/actions/setlogictreeproperty.py
--rw-rw-rw-   0        0        0     1052 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setmaterial.py
--rw-rw-rw-   0        0        0      989 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setmatnodesocket.py
--rw-rw-rw-   0        0        0     1182 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setmatnodevalue.py
--rw-rw-rw-   0        0        0      956 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setnodesocket.py
--rw-rw-rw-   0        0        0     1149 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setnodevalue.py
--rw-rw-rw-   0        0        0      803 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setoverlaycollection.py
--rw-rw-rw-   0        0        0      851 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setparent.py
--rw-rw-rw-   0        0        0      837 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setphysics.py
--rw-rw-rw-   0        0        0      604 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setprofile.py
--rw-rw-rw-   0        0        0      962 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setproperty.py
--rw-rw-rw-   0        0        0      715 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setpyinstanceattr.py
--rw-rw-rw-   0        0        0      663 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setresolution.py
--rw-rw-rw-   0        0        0      746 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setrigidbody.py
--rw-rw-rw-   0        0        0      633 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setscene.py
--rw-rw-rw-   0        0        0      965 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setsensorvalue.py
--rw-rw-rw-   0        0        0      624 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/settimescale.py
--rw-rw-rw-   0        0        0     2204 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setuiwidgetattr.py
--rw-rw-rw-   0        0        0     2327 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setvisibility.py
--rw-rw-rw-   0        0        0      546 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setvsync.py
--rw-rw-rw-   0        0        0      617 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/showframerate.py
--rw-rw-rw-   0        0        0     1208 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/slowfollow.py
--rw-rw-rw-   0        0        0     3973 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/spawnpool.py
--rw-rw-rw-   0        0        0     5315 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/startsound.py
--rw-rw-rw-   0        0        0     1856 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/startsound2d.py
--rw-rw-rw-   0        0        0     2950 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/startsound3d.py
--rw-rw-rw-   0        0        0     2464 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/startspeaker.py
--rw-rw-rw-   0        0        0     1192 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/startsubnetwork.py
--rw-rw-rw-   0        0        0     1161 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/stopaction.py
--rw-rw-rw-   0        0        0      592 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/stopallsounds.py
--rw-rw-rw-   0        0        0      543 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/stopsound.py
--rw-rw-rw-   0        0        0      886 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/stopsubnetwork.py
--rw-rw-rw-   0        0        0      611 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/togglefilter.py
--rw-rw-rw-   0        0        0      815 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/toggleproperty.py
--rw-rw-rw-   0        0        0      524 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/translate.py
--rw-rw-rw-   0        0        0      992 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/vectoranglecheck.py
--rw-rw-rw-   0        0        0     1044 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/vehicleapplybraking.py
--rw-rw-rw-   0        0        0     1037 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/vehicleapplyforce.py
--rw-rw-rw-   0        0        0     1045 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/vehicleapplysteering.py
--rw-rw-rw-   0        0        0     3133 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/vehiclesetattributes.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.534111 uplogic-2.2/uplogic/nodes/conditions/
--rw-rw-rw-   0        0        0     2026 2023-10-03 15:16:22.000000 uplogic-2.2/uplogic/nodes/conditions/__init__.py
--rw-rw-rw-   0        0        0      880 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/barrier.py
--rw-rw-rw-   0        0        0      826 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/checkdistance.py
--rw-rw-rw-   0        0        0     4178 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/collision.py
--rw-rw-rw-   0        0        0      823 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/compare.py
--rw-rw-rw-   0        0        0     1165 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/comparevectors.py
--rw-rw-rw-   0        0        0     2047 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/controllerstatus.py
--rw-rw-rw-   0        0        0      898 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/evaluateproperty.py
--rw-rw-rw-   0        0        0      739 2024-02-07 13:13:10.000000 uplogic-2.2/uplogic/nodes/conditions/gamepadactive.py
--rw-rw-rw-   0        0        0      708 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/gamepadbutton.py
--rw-rw-rw-   0        0        0     1252 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/gamepadbuttonup.py
--rw-rw-rw-   0        0        0      811 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/handleevent.py
--rw-rw-rw-   0        0        0      637 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/hasproperty.py
--rw-rw-rw-   0        0        0      311 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/keyboardactive.py
--rw-rw-rw-   0        0        0      615 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/keypressed.py
--rw-rw-rw-   0        0        0      610 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/keyreleased.py
--rw-rw-rw-   0        0        0      974 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/logicand.py
--rw-rw-rw-   0        0        0      416 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/logicandnot.py
--rw-rw-rw-   0        0        0     1722 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/logicgate.py
--rw-rw-rw-   0        0        0      907 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/logicgatelist.py
--rw-rw-rw-   0        0        0      314 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/logicnone.py
--rw-rw-rw-   0        0        0      332 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/logicnot.py
--rw-rw-rw-   0        0        0      323 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/logicnotnone.py
--rw-rw-rw-   0        0        0     1003 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/logicor.py
--rw-rw-rw-   0        0        0      962 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/logictreestatus.py
--rw-rw-rw-   0        0        0      389 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/mousemoved.py
--rw-rw-rw-   0        0        0     2881 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/mouseover.py
--rw-rw-rw-   0        0        0      631 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/mousepressed.py
--rw-rw-rw-   0        0        0      940 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/mousepressedon.py
--rw-rw-rw-   0        0        0      726 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/mousereleased.py
--rw-rw-rw-   0        0        0      665 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/mousescroll.py
--rw-rw-rw-   0        0        0      782 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/once.py
--rw-rw-rw-   0        0        0      268 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/oninit.py
--rw-rw-rw-   0        0        0      625 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/onnexttick.py
--rw-rw-rw-   0        0        0      243 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/onupdate.py
--rw-rw-rw-   0        0        0      974 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/onvaluechanged.py
--rw-rw-rw-   0        0        0      772 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/onvaluechangedto.py
--rw-rw-rw-   0        0        0      854 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/pulsify.py
--rw-rw-rw-   0        0        0      454 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/sensorpositive.py
--rw-rw-rw-   0        0        0      845 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/timedelay.py
--rw-rw-rw-   0        0        0      901 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/timer.py
--rw-rw-rw-   0        0        0      451 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/truefalse.py
--rw-rw-rw-   0        0        0      389 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/valuevalid.py
--rw-rw-rw-   0        0        0     1001 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/vectoranglecheck.py
--rw-rw-rw-   0        0        0     5388 2024-03-18 08:04:37.000000 uplogic-2.2/uplogic/nodes/logictree.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.563014 uplogic-2.2/uplogic/nodes/parameters/
--rw-rw-rw-   0        0        0     5254 2024-04-04 13:03:49.000000 uplogic-2.2/uplogic/nodes/parameters/__init__.py
--rw-rw-rw-   0        0        0      392 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/absolutevalue.py
--rw-rw-rw-   0        0        0     1392 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/actionstatus.py
--rw-rw-rw-   0        0        0      334 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/activecamera.py
--rw-rw-rw-   0        0        0      461 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/axisvector.py
--rw-rw-rw-   0        0        0     1694 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/bonestatus.py
--rw-rw-rw-   0        0        0     1521 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/characterinfo.py
--rw-rw-rw-   0        0        0      559 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/childbyindex.py
--rw-rw-rw-   0        0        0      553 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/childbyname.py
--rw-rw-rw-   0        0        0      834 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/clamp.py
--rw-rw-rw-   0        0        0      394 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/colorrgb.py
--rw-rw-rw-   0        0        0      395 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/colorrgba.py
--rw-rw-rw-   0        0        0      437 2024-02-18 16:30:58.000000 uplogic-2.2/uplogic/nodes/parameters/curveinterpolation.py
--rw-rw-rw-   0        0        0      565 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/dictvalue.py
--rw-rw-rw-   0        0        0      465 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/distance.py
--rw-rw-rw-   0        0        0      602 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/euler.py
--rw-rw-rw-   0        0        0      553 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/eulertomatrix.py
--rw-rw-rw-   0        0        0      732 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/formattedstring.py
--rw-rw-rw-   0        0        0     1919 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/formula.py
--rw-rw-rw-   0        0        0      324 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/fpsfactor.py
--rw-rw-rw-   0        0        0     1930 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/gamepadsticks.py
--rw-rw-rw-   0        0        0     1480 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/gamepadtrigger.py
--rw-rw-rw-   0        0        0      610 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getactuatorvalue.py
--rw-rw-rw-   0        0        0      323 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getcollection.py
--rw-rw-rw-   0        0        0      464 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getcollectionobjectnames.py
--rw-rw-rw-   0        0        0      529 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getcollectionobjects.py
--rw-rw-rw-   0        0        0      434 2024-04-04 13:03:32.000000 uplogic-2.2/uplogic/nodes/parameters/getcollisiongroup.py
--rw-rw-rw-   0        0        0      582 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getcurvepoints.py
--rw-rw-rw-   0        0        0      295 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getfont.py
--rw-rw-rw-   0        0        0      306 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getfullscreen.py
--rw-rw-rw-   0        0        0      562 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getglobalvalue.py
--rw-rw-rw-   0        0        0      337 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getgravity.py
--rw-rw-rw-   0        0        0      298 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getimage.py
--rw-rw-rw-   0        0        0      398 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getlightcolor.py
--rw-rw-rw-   0        0        0      404 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getlightenergy.py
--rw-rw-rw-   0        0        0      660 2024-01-22 11:02:02.000000 uplogic-2.2/uplogic/nodes/parameters/getlogictreeproperty.py
--rw-rw-rw-   0        0        0      805 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getnodeattribute.py
--rw-rw-rw-   0        0        0      659 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getnodesocket.py
--rw-rw-rw-   0        0        0      369 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getobject.py
--rw-rw-rw-   0        0        0      284 2024-01-22 11:02:02.000000 uplogic-2.2/uplogic/nodes/parameters/getowner.py
--rw-rw-rw-   0        0        0      322 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getparent.py
--rw-rw-rw-   0        0        0      837 2024-01-22 11:02:02.000000 uplogic-2.2/uplogic/nodes/parameters/getproperty.py
--rw-rw-rw-   0        0        0      429 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getpyinstanceattr.py
--rw-rw-rw-   0        0        0      661 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getresolution.py
--rw-rw-rw-   0        0        0      289 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getscene.py
--rw-rw-rw-   0        0        0      600 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getsensorvalue.py
--rw-rw-rw-   0        0        0      296 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getsound.py
--rw-rw-rw-   0        0        0      290 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/gettimescale.py
--rw-rw-rw-   0        0        0      825 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getuiwidgetattr.py
--rw-rw-rw-   0        0        0      286 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getvsync.py
--rw-rw-rw-   0        0        0      334 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/initemptydict.py
--rw-rw-rw-   0        0        0      414 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/initemptylist.py
--rw-rw-rw-   0        0        0      396 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/initnewdict.py
--rw-rw-rw-   0        0        0      856 2024-02-09 10:13:40.000000 uplogic-2.2/uplogic/nodes/parameters/instream.py
--rw-rw-rw-   0        0        0      478 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/interpolate.py
--rw-rw-rw-   0        0        0      404 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/invertvalue.py
--rw-rw-rw-   0        0        0      299 2024-04-23 18:12:22.000000 uplogic-2.2/uplogic/nodes/parameters/keycode.py
--rw-rw-rw-   0        0        0     1232 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/limitrange.py
--rw-rw-rw-   0        0        0      343 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/listduplicate.py
--rw-rw-rw-   0        0        0      527 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/listextend.py
--rw-rw-rw-   0        0        0      327 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/listfromitems.py
--rw-rw-rw-   0        0        0      461 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/listindex.py
--rw-rw-rw-   0        0        0      447 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/listindexrandom.py
--rw-rw-rw-   0        0        0     1466 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/loadvariable.py
--rw-rw-rw-   0        0        0     1175 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/loadvariabledict.py
--rw-rw-rw-   0        0        0      831 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/maprange.py
--rw-rw-rw-   0        0        0      853 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/materialgetattribute.py
--rw-rw-rw-   0        0        0      556 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/materialgetnode.py
--rw-rw-rw-   0        0        0      693 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/materialgetsocket.py
--rw-rw-rw-   0        0        0     1673 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/math.py
--rw-rw-rw-   0        0        0      568 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/matrixtoxyz.py
--rw-rw-rw-   0        0        0     1045 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/mousedata.py
--rw-rw-rw-   0        0        0      657 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/objectattr.py
--rw-rw-rw-   0        0        0      352 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/objectdataname.py
--rw-rw-rw-   0        0        0      584 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/objectdatavertices.py
--rw-rw-rw-   0        0        0      741 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/randomfloat.py
--rw-rw-rw-   0        0        0      690 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/randomint.py
--rw-rw-rw-   0        0        0     1722 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/randomvalue.py
--rw-rw-rw-   0        0        0      639 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/randomvect.py
--rw-rw-rw-   0        0        0      929 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/rangedthreshold.py
--rw-rw-rw-   0        0        0     1522 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/rebuilddata.py
--rw-rw-rw-   0        0        0      867 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/resizevector.py
--rw-rw-rw-   0        0        0     1930 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/rotatebypoint.py
--rw-rw-rw-   0        0        0      462 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/screenposition.py
--rw-rw-rw-   0        0        0      734 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/serializedata.py
--rw-rw-rw-   0        0        0      322 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/simplevalue.py
--rw-rw-rw-   0        0        0      930 2024-04-04 13:47:56.000000 uplogic-2.2/uplogic/nodes/parameters/storevalue.py
--rw-rw-rw-   0        0        0      758 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/threshold.py
--rw-rw-rw-   0        0        0      885 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/timedata.py
--rw-rw-rw-   0        0        0     3026 2024-02-19 17:25:02.000000 uplogic-2.2/uplogic/nodes/parameters/tweenvalue.py
--rw-rw-rw-   0        0        0      685 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/typecastvalue.py
--rw-rw-rw-   0        0        0     4193 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/valueswitch.py
--rw-rw-rw-   0        0        0      502 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/vectorabsolute.py
--rw-rw-rw-   0        0        0      587 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/vectorangle.py
--rw-rw-rw-   0        0        0       60 2023-09-30 12:04:19.000000 uplogic-2.2/uplogic/nodes/parameters/vectoranglecheck.py
--rw-rw-rw-   0        0        0      378 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/vectorlength.py
--rw-rw-rw-   0        0        0     4632 2024-04-23 15:15:14.000000 uplogic-2.2/uplogic/nodes/parameters/vectormath.py
--rw-rw-rw-   0        0        0      578 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/vectorsplitxy.py
--rw-rw-rw-   0        0        0      686 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/vectorsplitxyz.py
--rw-rw-rw-   0        0        0      439 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/vectorxy.py
--rw-rw-rw-   0        0        0      514 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/vectorxyz.py
--rw-rw-rw-   0        0        0      585 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/vectorxyzw.py
--rw-rw-rw-   0        0        0     1273 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/vrcontrollervalues.py
--rw-rw-rw-   0        0        0      486 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/vrheadsetvalues.py
--rw-rw-rw-   0        0        0      923 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/withinrange.py
--rw-rw-rw-   0        0        0      731 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/worldposition.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.565008 uplogic-2.2/uplogic/physics/
--rw-rw-rw-   0        0        0      540 2023-03-06 11:18:24.000000 uplogic-2.2/uplogic/physics/__init__.py
--rw-rw-rw-   0        0        0     4164 2024-03-18 08:04:37.000000 uplogic-2.2/uplogic/physics/buoyancy.py
--rw-rw-rw-   0        0        0     4060 2024-03-22 08:57:02.000000 uplogic-2.2/uplogic/physics/character.py
--rw-rw-rw-   0        0        0     3595 2023-11-06 03:14:00.000000 uplogic-2.2/uplogic/physics/collision.py
--rw-rw-rw-   0        0        0     8370 2024-02-06 12:40:32.000000 uplogic-2.2/uplogic/physics/constraints.py
--rw-rw-rw-   0        0        0    10164 2024-01-25 16:38:46.000000 uplogic-2.2/uplogic/physics/vehicle.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.565008 uplogic-2.2/uplogic/serialize/
--rw-rw-rw-   0        0        0     2965 2023-12-11 16:15:51.000000 uplogic-2.2/uplogic/serialize/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.584942 uplogic-2.2/uplogic/shaders/
--rw-rw-rw-   0        0        0      795 2024-04-23 15:16:36.000000 uplogic-2.2/uplogic/shaders/__init__.py
--rw-rw-rw-   0        0        0      872 2023-04-01 06:53:25.000000 uplogic-2.2/uplogic/shaders/adaptivetonemapping.py
--rw-rw-rw-   0        0        0     1633 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/shaders/blur.py
--rw-rw-rw-   0        0        0      685 2023-04-01 06:54:25.000000 uplogic-2.2/uplogic/shaders/brightness.py
--rw-rw-rw-   0        0        0     1182 2024-03-22 08:50:05.000000 uplogic-2.2/uplogic/shaders/buffer.py
--rw-rw-rw-   0        0        0     1070 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/shaders/chromaticaberration.py
--rw-rw-rw-   0        0        0     7049 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/shaders/distort.py
--rw-rw-rw-   0        0        0     9821 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/shaders/dof.py
--rw-rw-rw-   0        0        0     9068 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/shaders/droplets.py
--rw-rw-rw-   0        0        0       10 2024-02-21 19:10:36.000000 uplogic-2.2/uplogic/shaders/filtersystem.py
--rw-rw-rw-   0        0        0    33422 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/shaders/fxaa.py
--rw-rw-rw-   0        0        0      916 2023-04-01 06:54:25.000000 uplogic-2.2/uplogic/shaders/grayscale.py
--rw-rw-rw-   0        0        0     9683 2023-07-05 14:45:48.000000 uplogic-2.2/uplogic/shaders/hbao.py
--rw-rw-rw-   0        0        0     1035 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/shaders/lens.py
--rw-rw-rw-   0        0        0     1137 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/shaders/letterbox.py
--rw-rw-rw-   0        0        0     1027 2023-04-01 06:54:25.000000 uplogic-2.2/uplogic/shaders/levels.py
--rw-rw-rw-   0        0        0     4172 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/shaders/mist.py
--rw-rw-rw-   0        0        0     1779 2024-02-12 11:42:26.000000 uplogic-2.2/uplogic/shaders/rendertoscreen.py
--rw-rw-rw-   0        0        0     5818 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/shaders/shader.py
--rw-rw-rw-   0        0        0     2268 2023-04-01 06:54:25.000000 uplogic-2.2/uplogic/shaders/sharpen.py
--rw-rw-rw-   0        0        0     2898 2024-02-12 11:42:41.000000 uplogic-2.2/uplogic/shaders/splitscreen.py
--rw-rw-rw-   0        0        0     5754 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/shaders/ssao.py
--rw-rw-rw-   0        0        0     2373 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/shaders/texture.py
--rw-rw-rw-   0        0        0     1189 2024-02-12 15:10:32.000000 uplogic-2.2/uplogic/shaders/vignette.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.592914 uplogic-2.2/uplogic/ui/
--rw-rw-rw-   0        0        0      653 2024-03-22 08:50:05.000000 uplogic-2.2/uplogic/ui/__init__.py
--rw-rw-rw-   0        0        0     1712 2024-02-16 10:02:44.000000 uplogic-2.2/uplogic/ui/behaviors.py
--rw-rw-rw-   0        0        0    10061 2024-03-22 08:50:05.000000 uplogic-2.2/uplogic/ui/button.py
--rw-rw-rw-   0        0        0     1722 2024-03-22 08:50:05.000000 uplogic-2.2/uplogic/ui/camera.py
--rw-rw-rw-   0        0        0     3577 2024-03-22 08:50:05.000000 uplogic-2.2/uplogic/ui/canvas.py
--rw-rw-rw-   0        0        0     3765 2024-03-22 08:50:05.000000 uplogic-2.2/uplogic/ui/cursor.py
--rw-rw-rw-   0        0        0     7177 2024-04-04 12:19:18.000000 uplogic-2.2/uplogic/ui/image.py
--rw-rw-rw-   0        0        0     8118 2024-04-23 18:12:22.000000 uplogic-2.2/uplogic/ui/label.py
--rw-rw-rw-   0        0        0    13537 2024-04-04 03:21:32.000000 uplogic-2.2/uplogic/ui/layout.py
--rw-rw-rw-   0        0        0     5166 2024-03-22 08:50:05.000000 uplogic-2.2/uplogic/ui/path.py
--rw-rw-rw-   0        0        0     2041 2024-03-22 08:50:05.000000 uplogic-2.2/uplogic/ui/render.py
--rw-rw-rw-   0        0        0     8061 2024-03-22 08:50:05.000000 uplogic-2.2/uplogic/ui/slider.py
--rw-rw-rw-   0        0        0     8690 2024-04-23 18:12:22.000000 uplogic-2.2/uplogic/ui/textinput.py
--rw-rw-rw-   0        0        0    16519 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/ui/widget.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.600888 uplogic-2.2/uplogic/utils/
--rw-rw-rw-   0        0        0     7473 2024-04-04 03:20:50.000000 uplogic-2.2/uplogic/utils/__init__.py
--rw-rw-rw-   0        0        0     1642 2023-11-09 02:27:44.000000 uplogic-2.2/uplogic/utils/constants.py
--rw-rw-rw-   0        0        0     1089 2024-03-22 08:50:05.000000 uplogic-2.2/uplogic/utils/engine.py
--rw-rw-rw-   0        0        0      854 2022-09-08 15:54:10.000000 uplogic-2.2/uplogic/utils/errors.py
--rw-rw-rw-   0        0        0     4650 2023-11-22 09:34:56.000000 uplogic-2.2/uplogic/utils/lights.py
--rw-rw-rw-   0        0        0    11028 2024-04-04 03:23:58.000000 uplogic-2.2/uplogic/utils/math.py
--rw-rw-rw-   0        0        0     4801 2023-12-31 14:36:53.000000 uplogic-2.2/uplogic/utils/nodetrees.py
--rw-rw-rw-   0        0        0    17010 2024-03-18 08:04:37.000000 uplogic-2.2/uplogic/utils/objects.py
--rw-rw-rw-   0        0        0    10075 2023-11-09 14:18:13.000000 uplogic-2.2/uplogic/utils/pooling.py
--rw-rw-rw-   0        0        0    13778 2023-10-13 21:24:56.000000 uplogic-2.2/uplogic/utils/raycasting.py
--rw-rw-rw-   0        0        0     6451 2024-03-18 08:04:37.000000 uplogic-2.2/uplogic/utils/scene.py
--rw-rw-rw-   0        0        0     3528 2024-03-18 12:51:09.000000 uplogic-2.2/uplogic/utils/visualize.py
--rw-rw-rw-   0        0        0     2553 2024-03-22 08:50:05.000000 uplogic-2.2/uplogic/utils/visuals.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.454378 uplogic-2.2/uplogic.egg-info/
--rw-rw-rw-   0        0        0     1045 2024-04-23 18:17:52.000000 uplogic-2.2/uplogic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    14795 2024-04-23 18:17:52.000000 uplogic-2.2/uplogic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 18:17:52.000000 uplogic-2.2/uplogic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-23 18:17:52.000000 uplogic-2.2/uplogic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-23 18:17:52.000000 uplogic-2.2/uplogic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-03-17 18:28:53.000000 uplogic-2.2/uplogic.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:10.718306 uplogic-3.2/
+-rw-rw-rw-   0        0        0      189 2022-01-15 11:35:38.000000 uplogic-3.2/LICENSE.md
+-rw-rw-rw-   0        0        0     1045 2024-05-29 08:25:10.717311 uplogic-3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2022-01-15 11:34:53.000000 uplogic-3.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-29 08:25:10.718306 uplogic-3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1739 2024-05-29 08:24:51.000000 uplogic-3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.385203 uplogic-3.2/uplogic/
+-rw-rw-rw-   0        0        0     6499 2024-05-29 08:21:32.000000 uplogic-3.2/uplogic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.402147 uplogic-3.2/uplogic/__pycache__/
+-rw-rw-rw-   0        0        0     7457 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0    12349 2024-05-29 08:21:14.000000 uplogic-3.2/uplogic/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6704 2023-01-21 12:36:04.000000 uplogic-3.2/uplogic/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.403144 uplogic-3.2/uplogic/ai/
+-rw-rw-rw-   0        0        0       24 2024-02-19 17:27:15.000000 uplogic-3.2/uplogic/ai/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.404141 uplogic-3.2/uplogic/ai/__pycache__/
+-rw-rw-rw-   0        0        0      183 2024-02-19 17:27:16.000000 uplogic-3.2/uplogic/ai/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5487 2024-02-19 17:43:26.000000 uplogic-3.2/uplogic/ai/__pycache__/agent.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3525 2024-02-19 17:43:26.000000 uplogic-3.2/uplogic/ai/__pycache__/navigation.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5874 2024-05-04 07:36:26.000000 uplogic-3.2/uplogic/ai/agent.py
+-rw-rw-rw-   0        0        0     3024 2024-02-19 17:41:02.000000 uplogic-3.2/uplogic/ai/navigation.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.407131 uplogic-3.2/uplogic/animation/
+-rw-rw-rw-   0        0        0      341 2023-12-07 08:59:05.000000 uplogic-3.2/uplogic/animation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.416100 uplogic-3.2/uplogic/animation/__pycache__/
+-rw-rw-rw-   0        0        0      508 2023-12-07 08:59:08.000000 uplogic-3.2/uplogic/animation/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      624 2024-01-02 14:08:24.000000 uplogic-3.2/uplogic/animation/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      472 2022-10-05 12:11:16.000000 uplogic-3.2/uplogic/animation/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    11568 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/animation/__pycache__/action.cpython-310.pyc
+-rw-rw-rw-   0        0        0    17433 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/animation/__pycache__/action.cpython-311.pyc
+-rw-rw-rw-   0        0        0     8603 2023-01-21 12:36:25.000000 uplogic-3.2/uplogic/animation/__pycache__/action.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4681 2024-02-18 10:43:28.000000 uplogic-3.2/uplogic/animation/__pycache__/actionsystem.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7407 2024-05-04 07:45:28.000000 uplogic-3.2/uplogic/animation/__pycache__/actionsystem.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4536 2023-01-21 12:36:25.000000 uplogic-3.2/uplogic/animation/__pycache__/actionsystem.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3160 2023-11-10 06:42:35.000000 uplogic-3.2/uplogic/animation/__pycache__/rig.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4946 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/animation/__pycache__/sequence.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7882 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/animation/__pycache__/sequence.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3499 2023-01-21 12:36:25.000000 uplogic-3.2/uplogic/animation/__pycache__/sequence.cpython-39.pyc
+-rw-rw-rw-   0        0        0    14237 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/animation/action.py
+-rw-rw-rw-   0        0        0     4152 2024-05-04 07:36:26.000000 uplogic-3.2/uplogic/animation/actionsystem.py
+-rw-rw-rw-   0        0        0     2419 2024-05-04 07:36:26.000000 uplogic-3.2/uplogic/animation/rig.py
+-rw-rw-rw-   0        0        0     6950 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/animation/sequence.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.419090 uplogic-3.2/uplogic/audio/
+-rw-rw-rw-   0        0        0      606 2023-12-15 10:12:29.000000 uplogic-3.2/uplogic/audio/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.429057 uplogic-3.2/uplogic/audio/__pycache__/
+-rw-rw-rw-   0        0        0      715 2023-12-15 10:20:08.000000 uplogic-3.2/uplogic/audio/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      967 2024-01-02 14:08:24.000000 uplogic-3.2/uplogic/audio/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      559 2023-01-21 12:36:04.000000 uplogic-3.2/uplogic/audio/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6718 2024-02-10 14:51:33.000000 uplogic-3.2/uplogic/audio/__pycache__/audiosystem.cpython-310.pyc
+-rw-rw-rw-   0        0        0    11547 2024-05-08 17:40:49.000000 uplogic-3.2/uplogic/audio/__pycache__/audiosystem.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6621 2023-01-21 12:36:04.000000 uplogic-3.2/uplogic/audio/__pycache__/audiosystem.cpython-39.pyc
+-rw-rw-rw-   0        0        0    21589 2024-05-09 11:48:32.000000 uplogic-3.2/uplogic/audio/__pycache__/fmod.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7365 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/audio/__pycache__/music.cpython-310.pyc
+-rw-rw-rw-   0        0        0    11980 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/audio/__pycache__/music.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6966 2022-09-19 13:05:14.000000 uplogic-3.2/uplogic/audio/__pycache__/music.cpython-39.pyc
+-rw-rw-rw-   0        0        0    16845 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/audio/__pycache__/sound.cpython-310.pyc
+-rw-rw-rw-   0        0        0    31018 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/audio/__pycache__/sound.cpython-311.pyc
+-rw-rw-rw-   0        0        0    11167 2023-01-21 12:36:04.000000 uplogic-3.2/uplogic/audio/__pycache__/sound.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7747 2024-05-08 17:38:49.000000 uplogic-3.2/uplogic/audio/audiosystem.py
+-rw-rw-rw-   0        0        0    10578 2024-05-29 07:40:30.000000 uplogic-3.2/uplogic/audio/fmod.py
+-rw-rw-rw-   0        0        0     6894 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/audio/music.py
+-rw-rw-rw-   0        0        0    24586 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/audio/sound.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.430054 uplogic-3.2/uplogic/console/
+-rw-rw-rw-   0        0        0    16638 2024-05-16 15:40:59.000000 uplogic-3.2/uplogic/console/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.437031 uplogic-3.2/uplogic/console/__pycache__/
+-rw-rw-rw-   0        0        0    14667 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/console/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0    29182 2024-05-16 15:51:36.000000 uplogic-3.2/uplogic/console/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4228 2022-08-15 17:30:07.000000 uplogic-3.2/uplogic/console/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2485 2024-03-19 08:06:24.000000 uplogic-3.2/uplogic/console/__pycache__/commands.cpython-311.pyc
+-rw-rw-rw-   0        0        0      335 2022-07-21 09:01:11.000000 uplogic-3.2/uplogic/console/__pycache__/handlers.cpython-310.pyc
+-rw-rw-rw-   0        0        0      272 2022-07-21 08:49:55.000000 uplogic-3.2/uplogic/console/__pycache__/reset.cpython-310.pyc
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.439024 uplogic-3.2/uplogic/data/
+-rw-rw-rw-   0        0        0     1861 2022-10-06 13:43:59.000000 uplogic-3.2/uplogic/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.447994 uplogic-3.2/uplogic/data/__pycache__/
+-rw-rw-rw-   0        0        0     2058 2022-10-06 13:58:48.000000 uplogic-3.2/uplogic/data/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3474 2024-01-02 14:08:23.000000 uplogic-3.2/uplogic/data/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2050 2023-01-21 12:36:04.000000 uplogic-3.2/uplogic/data/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4034 2024-02-02 14:25:14.000000 uplogic-3.2/uplogic/data/__pycache__/file.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7032 2024-02-14 12:32:07.000000 uplogic-3.2/uplogic/data/__pycache__/file.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2019 2023-01-21 12:36:04.000000 uplogic-3.2/uplogic/data/__pycache__/file.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7727 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/data/__pycache__/globaldb.cpython-310.pyc
+-rw-rw-rw-   0        0        0    14348 2024-05-04 07:45:28.000000 uplogic-3.2/uplogic/data/__pycache__/globaldb.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7410 2022-09-19 13:05:14.000000 uplogic-3.2/uplogic/data/__pycache__/globaldb.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2815 2022-03-09 09:46:36.000000 uplogic-3.2/uplogic/data/__pycache__/serializers.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5179 2024-05-04 07:45:28.000000 uplogic-3.2/uplogic/data/__pycache__/serializers.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2961 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/data/__pycache__/serializers.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3161 2024-02-02 14:24:41.000000 uplogic-3.2/uplogic/data/file.py
+-rw-rw-rw-   0        0        0     7457 2024-05-04 07:36:26.000000 uplogic-3.2/uplogic/data/globaldb.py
+-rw-rw-rw-   0        0        0     2050 2024-05-04 07:36:26.000000 uplogic-3.2/uplogic/data/serializers.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.448990 uplogic-3.2/uplogic/decorators/
+-rw-rw-rw-   0        0        0    18211 2024-05-04 07:36:26.000000 uplogic-3.2/uplogic/decorators/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.450984 uplogic-3.2/uplogic/decorators/__pycache__/
+-rw-rw-rw-   0        0        0    15269 2024-02-23 15:45:47.000000 uplogic-3.2/uplogic/decorators/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0    26192 2024-05-16 09:54:50.000000 uplogic-3.2/uplogic/decorators/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6699 2022-09-19 13:05:15.000000 uplogic-3.2/uplogic/decorators/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.451981 uplogic-3.2/uplogic/events/
+-rw-rw-rw-   0        0        0     8666 2024-05-16 14:57:09.000000 uplogic-3.2/uplogic/events/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.454970 uplogic-3.2/uplogic/events/__pycache__/
+-rw-rw-rw-   0        0        0    10062 2024-02-18 16:31:23.000000 uplogic-3.2/uplogic/events/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0    16793 2024-05-16 14:57:13.000000 uplogic-3.2/uplogic/events/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9063 2023-01-21 12:36:04.000000 uplogic-3.2/uplogic/events/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.457960 uplogic-3.2/uplogic/input/
+-rw-rw-rw-   0        0        0     1541 2023-09-30 18:00:52.000000 uplogic-3.2/uplogic/input/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.471914 uplogic-3.2/uplogic/input/__pycache__/
+-rw-rw-rw-   0        0        0     1534 2023-09-30 18:43:32.000000 uplogic-3.2/uplogic/input/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2182 2024-01-02 14:08:23.000000 uplogic-3.2/uplogic/input/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1353 2023-01-21 12:36:04.000000 uplogic-3.2/uplogic/input/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    13484 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/input/__pycache__/gamepad.cpython-310.pyc
+-rw-rw-rw-   0        0        0    21886 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/input/__pycache__/gamepad.cpython-311.pyc
+-rw-rw-rw-   0        0        0    12115 2022-08-15 17:30:07.000000 uplogic-3.2/uplogic/input/__pycache__/gamepad.cpython-39.pyc
+-rw-rw-rw-   0        0        0    10071 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/input/__pycache__/keyboard.cpython-310.pyc
+-rw-rw-rw-   0        0        0    12237 2024-03-22 08:50:09.000000 uplogic-3.2/uplogic/input/__pycache__/keyboard.cpython-311.pyc
+-rw-rw-rw-   0        0        0     8631 2023-01-21 12:36:04.000000 uplogic-3.2/uplogic/input/__pycache__/keyboard.cpython-39.pyc
+-rw-rw-rw-   0        0        0    12653 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/input/__pycache__/mouse.cpython-310.pyc
+-rw-rw-rw-   0        0        0    21886 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/input/__pycache__/mouse.cpython-311.pyc
+-rw-rw-rw-   0        0        0    12026 2023-01-21 12:36:04.000000 uplogic-3.2/uplogic/input/__pycache__/mouse.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9725 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/input/__pycache__/vr.cpython-310.pyc
+-rw-rw-rw-   0        0        0    16665 2024-05-08 16:47:48.000000 uplogic-3.2/uplogic/input/__pycache__/vr.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9246 2023-01-21 12:36:04.000000 uplogic-3.2/uplogic/input/__pycache__/vr.cpython-39.pyc
+-rw-rw-rw-   0        0        0    16073 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/input/gamepad.py
+-rw-rw-rw-   0        0        0    10967 2024-03-22 08:50:05.000000 uplogic-3.2/uplogic/input/keyboard.py
+-rw-rw-rw-   0        0        0    15456 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/input/mouse.py
+-rw-rw-rw-   0        0        0     9441 2024-05-08 16:47:41.000000 uplogic-3.2/uplogic/input/vr.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.472910 uplogic-3.2/uplogic/network/
+-rw-rw-rw-   0        0        0       56 2023-06-05 09:06:00.000000 uplogic-3.2/uplogic/network/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.479887 uplogic-3.2/uplogic/network/__pycache__/
+-rw-rw-rw-   0        0        0      249 2023-06-05 09:28:04.000000 uplogic-3.2/uplogic/network/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      273 2024-01-02 14:08:24.000000 uplogic-3.2/uplogic/network/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2807 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/network/__pycache__/client.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5504 2024-05-04 07:45:29.000000 uplogic-3.2/uplogic/network/__pycache__/client.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2403 2023-05-14 17:50:19.000000 uplogic-3.2/uplogic/network/__pycache__/entity.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1076 2022-09-28 21:57:52.000000 uplogic-3.2/uplogic/network/__pycache__/network.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4126 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/network/__pycache__/server.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8725 2024-05-04 07:45:29.000000 uplogic-3.2/uplogic/network/__pycache__/server.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1601 2022-09-28 20:02:43.000000 uplogic-3.2/uplogic/network/__pycache__/server.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2919 2024-05-04 07:36:38.000000 uplogic-3.2/uplogic/network/client.py
+-rw-rw-rw-   0        0        0     4687 2024-05-04 07:36:26.000000 uplogic-3.2/uplogic/network/server.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.480884 uplogic-3.2/uplogic/nodes/
+-rw-rw-rw-   0        0        0     4304 2024-05-09 10:14:07.000000 uplogic-3.2/uplogic/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.484871 uplogic-3.2/uplogic/nodes/__pycache__/
+-rw-rw-rw-   0        0        0     5543 2024-02-19 13:52:59.000000 uplogic-3.2/uplogic/nodes/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7992 2024-05-09 10:14:34.000000 uplogic-3.2/uplogic/nodes/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6578 2023-01-21 12:36:04.000000 uplogic-3.2/uplogic/nodes/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4958 2024-02-28 12:12:59.000000 uplogic-3.2/uplogic/nodes/__pycache__/logictree.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8594 2024-03-18 08:07:31.000000 uplogic-3.2/uplogic/nodes/__pycache__/logictree.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6332 2023-01-21 12:36:04.000000 uplogic-3.2/uplogic/nodes/__pycache__/logictree.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.564604 uplogic-3.2/uplogic/nodes/actions/
+-rw-rw-rw-   0        0        0     8317 2024-01-16 18:59:56.000000 uplogic-3.2/uplogic/nodes/actions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.974234 uplogic-3.2/uplogic/nodes/actions/__pycache__/
+-rw-rw-rw-   0        0        0     8898 2024-01-17 08:08:50.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0    11456 2024-01-16 19:39:47.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7811 2023-01-21 12:36:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2416 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/addfilter.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6117 2024-05-04 07:45:29.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/addfilter.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2479 2023-01-21 12:36:26.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/addfilter.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1356 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/addobject.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2237 2024-05-04 07:45:29.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/addobject.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1515 2022-10-05 12:11:16.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/addobject.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1769 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/addphysicsconstraint.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3370 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/addphysicsconstraint.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1991 2022-04-24 16:11:10.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/addphysicsconstraint.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1022 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/adduiwidget.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1568 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/adduiwidget.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1238 2024-02-16 09:50:31.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/alignaxistovector.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2067 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/alignaxistovector.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1478 2023-01-21 12:36:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/alignaxistovector.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1222 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/appendlistitem.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1897 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/appendlistitem.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1362 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/appendlistitem.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1052 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/applyforce.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1620 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/applyforce.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1236 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/applyforce.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1113 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/applyimpulse.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1760 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/applyimpulse.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1340 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/applyimpulse.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1079 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/applymovement.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1653 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/applymovement.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1267 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/applymovement.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1152 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/applyrotation.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1882 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/applyrotation.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1340 2023-01-21 12:36:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/applyrotation.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1077 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/applytorque.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1664 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/applytorque.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1209 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/applytorque.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2019 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/applytransform.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3388 2024-04-22 11:18:39.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/applytransform.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1933 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/cameraraycast.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3180 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/cameraraycast.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2252 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/cameraraycast.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1077 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/characterjump.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1612 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/characterjump.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1271 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/characterjump.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1380 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/clampedmodifyproperty.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2272 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/clampedmodifyproperty.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1561 2022-04-24 16:11:10.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/clampedmodifyproperty.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1803 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/clearvariables.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3132 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/clearvariables.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1894 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/clearvariables.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1191 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/copyproperty.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1909 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/copyproperty.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1390 2022-04-24 16:11:10.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/copyproperty.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3153 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/createuibutton.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5373 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/createuibutton.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1214 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/createuicanvas.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1790 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/createuicanvas.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1774 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/createuiimage.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2971 2024-04-22 11:18:39.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/createuiimage.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2200 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/createuilabel.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3661 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/createuilabel.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2063 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/createuilayout.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3459 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/createuilayout.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3059 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/createuislider.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6256 2024-04-22 11:18:39.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/createuislider.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1730 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/createvehicle.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2924 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/createvehicle.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1874 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/createvehicle.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1402 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/cursorbehavior.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2342 2024-04-22 11:18:37.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/cursorbehavior.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1532 2022-10-05 12:11:16.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/cursorbehavior.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1066 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/cursorvisibility.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1535 2024-04-22 11:18:37.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/cursorvisibility.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1196 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/cursorvisibility.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1232 2023-03-02 21:03:47.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/customcursorvisibility.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1139 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/dispatchevent.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1778 2024-04-22 11:18:37.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/dispatchevent.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1393 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/dispatchevent.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2452 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/draw.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4979 2024-04-22 11:18:39.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/draw.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1323 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/drawbox.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2250 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/drawbox.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1239 2022-10-05 12:11:17.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/drawbox.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1251 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/drawcube.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2023 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/drawcube.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1162 2022-10-05 12:11:17.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/drawcube.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1140 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/drawline.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1804 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/drawline.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1075 2022-10-05 12:11:17.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/drawline.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2494 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/editbone.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4445 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/editbone.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2728 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/editbone.cpython-39.pyc
+-rw-rw-rw-   0        0        0      822 2023-10-13 21:24:59.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/endgame.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1232 2024-01-02 14:08:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/endgame.cpython-311.pyc
+-rw-rw-rw-   0        0        0      905 2022-10-05 12:11:16.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/endgame.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1051 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/endobject.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1597 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/endobject.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1235 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/endobject.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1447 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/executesubnetwork.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2230 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/executesubnetwork.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1449 2022-02-07 22:48:49.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/executesubnetwork.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3329 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/followpath.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6444 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/followpath.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3585 2022-10-05 12:11:17.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/followpath.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2212 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/gamepadlook.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4024 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/gamepadlook.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2818 2022-01-31 12:25:39.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/gamepadlook.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1426 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/gamepadvibration.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2413 2024-04-22 11:18:37.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/gamepadvibration.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1588 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/gamepadvibration.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1973 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/getperformanceprofile.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3293 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/getperformanceprofile.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2109 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/getperformanceprofile.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1307 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/installsubnetwork.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1992 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/installsubnetwork.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1503 2022-02-08 11:04:16.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/installsubnetwork.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2151 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/instream.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3408 2024-04-22 11:18:37.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/instream.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2030 2022-09-06 09:53:21.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/keylogger.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2038 2022-10-05 12:11:16.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/keylogger.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1479 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/listglobalvalues.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2395 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/listglobalvalues.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1615 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/listglobalvalues.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2087 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/listvariables.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3758 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/listvariables.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2247 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/listvariables.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1041 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/loadblendfile.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1530 2024-04-22 11:18:37.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/loadblendfile.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1057 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/loadblendfile.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1915 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/loadfilecontent.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3015 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/loadfilecontent.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1944 2022-10-05 12:11:17.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/loadfilecontent.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2752 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/loadgame.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5410 2024-04-22 11:18:37.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/loadgame.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2910 2022-02-10 19:17:03.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/loadgame.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1942 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/loadscene.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3133 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/loadscene.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1932 2022-10-05 12:11:17.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/loadscene.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2711 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/localclient.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4675 2024-04-22 11:18:39.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/localclient.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2619 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/localserver.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4509 2024-04-22 11:18:39.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/localserver.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1220 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/makeuniquelight.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1818 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/makeuniquelight.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1385 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/makeuniquelight.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1405 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/modifyproperty.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2370 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/modifyproperty.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1415 2022-04-24 16:11:10.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/modifyproperty.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2317 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/mouselook.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4217 2024-04-22 11:18:37.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/mouselook.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3356 2023-01-21 12:36:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/mouselook.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1906 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/mouseraycast.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3116 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/mouseraycast.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2049 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/mouseraycast.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1232 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/mousesetposition.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1837 2024-04-22 11:18:37.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/mousesetposition.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1364 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/mousesetposition.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1230 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/moveto.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2339 2024-05-09 09:30:49.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/moveto.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1212 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/moveto.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3590 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/movetowithnavmesh.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6527 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/movetowithnavmesh.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3794 2022-10-05 12:11:17.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/movetowithnavmesh.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1016 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/pausesound.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1516 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/pausesound.cpython-311.pyc
+-rw-rw-rw-   0        0        0      920 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/pausesound.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3443 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/playaction.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6284 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/playaction.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3847 2023-01-21 12:36:26.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/playaction.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2119 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/playsequence.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3752 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/playsequence.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2186 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/playsequence.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1491 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/popdictkey.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2387 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/popdictkey.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1624 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/popdictkey.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1050 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/printvalue.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1556 2024-05-16 15:29:17.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/printvalue.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1054 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/printvalue.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3033 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/projectileraycast.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5183 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/projectileraycast.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2979 2023-01-21 12:36:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/projectileraycast.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2967 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/raycast.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5187 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/raycast.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3174 2022-10-05 12:11:17.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/raycast.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1043 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/removefilter.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1522 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/removefilter.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1173 2022-10-05 12:11:17.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/removefilter.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1329 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/removelistindex.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2058 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/removelistindex.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1454 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/removelistindex.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1366 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/removelistvalue.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2151 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/removelistvalue.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1491 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/removelistvalue.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1105 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/removeoverlaycollection.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1652 2024-04-22 11:18:37.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/removeoverlaycollection.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1117 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/removeoverlaycollection.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1002 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/removeparent.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1481 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/removeparent.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1208 2022-02-01 19:49:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/removeparent.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1164 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/removephysicsconstraint.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1781 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/removephysicsconstraint.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1310 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/removephysicsconstraint.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1897 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/removevariable.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3358 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/removevariable.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1999 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/removevariable.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1289 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/replacemesh.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2089 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/replacemesh.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1335 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/replacemesh.cpython-39.pyc
+-rw-rw-rw-   0        0        0      986 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/restartgame.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1403 2024-04-22 11:18:37.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/restartgame.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1004 2022-02-10 19:19:26.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/restartgame.cpython-39.pyc
+-rw-rw-rw-   0        0        0      971 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/resumesound.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1455 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/resumesound.cpython-311.pyc
+-rw-rw-rw-   0        0        0      925 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/resumesound.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1236 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/rotateto.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2011 2024-05-04 07:19:57.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/rotateto.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1471 2022-10-05 12:11:17.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/rotateto.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1164 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/runactuator.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1864 2024-04-22 11:18:37.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/runactuator.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1296 2022-02-09 13:39:14.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/runactuator.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1880 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/runpython.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3421 2024-04-22 11:18:37.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/runpython.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1641 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/runpython.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3276 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/savegame.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6288 2024-04-22 11:18:37.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/savegame.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3404 2022-02-08 15:53:00.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/savegame.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1979 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/savevariable.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3599 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/savevariable.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2085 2023-01-21 12:36:26.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/savevariable.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1878 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/savevariabledict.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3287 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/savevariabledict.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1982 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/savevariabledict.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1236 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/sendmessage.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1990 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/sendmessage.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1170 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/sendmessage.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1073 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/sendnetworkmessage.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1705 2024-04-22 11:18:39.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/sendnetworkmessage.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2062 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setactionframe.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3541 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setactionframe.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2193 2022-10-05 12:11:17.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setactionframe.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1189 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setactuatorvalue.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1939 2024-04-22 11:18:37.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setactuatorvalue.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1321 2022-02-26 12:23:54.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setactuatorvalue.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1301 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setboneconstraintattr.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2122 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setboneconstraintattr.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1501 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setboneconstraintattr.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1250 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setboneconstraintinfluence.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1973 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setboneconstraintinfluence.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1444 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setboneconstraintinfluence.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1234 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setboneconstrainttarget.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1968 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setboneconstrainttarget.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1428 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setboneconstrainttarget.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1399 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setboneposition.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2234 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setboneposition.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1530 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setboneposition.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1052 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcamera.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1554 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcamera.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1236 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcamera.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1017 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcamerafov.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1530 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcamerafov.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1203 2022-01-24 10:48:44.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcamerafov.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1067 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcameraorthoscale.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1581 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcameraorthoscale.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1253 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcameraorthoscale.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1156 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcharactergravity.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1754 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcharactergravity.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1340 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcharactergravity.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1159 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcharacterjumpspeed.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1736 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcharacterjumpspeed.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1353 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcharacterjumpspeed.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1157 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcharactermaxjumps.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1734 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcharactermaxjumps.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1343 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcharactermaxjumps.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1232 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcharactervelocity.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1947 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcharactervelocity.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1416 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcharactervelocity.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1533 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcharacterwalkdir.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2541 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcharacterwalkdir.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1719 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcharacterwalkdir.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1120 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcollisiongroup.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1682 2024-04-04 13:14:21.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcollisiongroup.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1261 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcollisiongroup.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1059 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcollisionmask.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1575 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcollisionmask.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1255 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcollisionmask.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1206 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setconstraintattribute.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1916 2024-04-22 11:18:39.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setconstraintattribute.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1329 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcurvepoints.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2291 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcurvepoints.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1523 2022-02-16 14:34:14.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcurvepoints.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1404 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcustomcursor.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2162 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setcustomcursor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1228 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setdictkey.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1935 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setdictkey.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1370 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setdictkey.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1116 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setdynamics.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1796 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setdynamics.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1304 2022-10-05 12:11:17.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setdynamics.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1110 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/seteeveeao.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1683 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/seteeveeao.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1240 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/seteeveeao.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1126 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/seteeveebloom.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1699 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/seteeveebloom.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1256 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/seteeveebloom.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1085 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/seteeveesmaa.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1519 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/seteeveesmaa.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1256 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/seteeveesmaa.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1128 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/seteeveesmaaquality.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1557 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/seteeveesmaaquality.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1291 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/seteeveesmaaquality.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1114 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/seteeveessr.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1687 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/seteeveessr.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1244 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/seteeveessr.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1176 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/seteeveevolumetrics.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1749 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/seteeveevolumetrics.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1304 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/seteeveevolumetrics.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1131 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setexposure.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1703 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setexposure.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1259 2022-02-06 14:06:47.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setexposure.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1097 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setfilterstate.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1649 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setfilterstate.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1229 2022-10-05 12:11:17.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setfilterstate.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1051 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setfullscreen.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1543 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setfullscreen.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1181 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setfullscreen.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1619 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setgameobjectattr.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2880 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setgameobjectattr.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1742 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setgameobjectattr.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1113 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setgamma.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1685 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setgamma.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1241 2022-01-21 14:10:26.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setgamma.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1200 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setglobalvalue.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1955 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setglobalvalue.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1444 2022-01-21 14:10:26.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setglobalvalue.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1040 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setgravity.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1543 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setgravity.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1224 2022-01-21 14:10:26.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setgravity.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1145 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setlightcolor.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1757 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setlightcolor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1263 2022-01-21 14:10:26.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setlightcolor.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1108 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setlightenergy.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1662 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setlightenergy.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1226 2022-01-21 14:10:26.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setlightenergy.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1112 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setlightshadow.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1667 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setlightshadow.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1230 2022-01-21 14:10:26.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setlightshadow.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1239 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setlistindex.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1946 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setlistindex.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1381 2022-01-21 14:10:26.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setlistindex.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1180 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setlogictreeproperty.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1875 2024-02-21 10:59:09.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setlogictreeproperty.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1343 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setmaterial.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2116 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setmaterial.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1474 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setmaterial.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1245 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setmatnodesocket.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1975 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setmatnodesocket.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1445 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setmatnodesocket.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1340 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setmatnodevalue.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2233 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setmatnodevalue.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1527 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setmatnodevalue.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1212 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setnodesocket.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1931 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setnodesocket.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1420 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setnodesocket.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1307 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setnodevalue.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2191 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setnodevalue.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1506 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setnodevalue.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1235 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setoverlaycollection.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1874 2024-04-22 11:18:37.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setoverlaycollection.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1146 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setoverlaycollection.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1117 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setparent.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1817 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setparent.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1279 2022-01-21 14:10:26.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setparent.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1114 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setphysics.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1794 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setphysics.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1302 2022-01-21 14:10:26.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setphysics.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1031 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setprofile.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1523 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setprofile.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1161 2022-01-21 14:10:26.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setprofile.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1171 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setproperty.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1853 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setproperty.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1381 2022-10-05 13:36:58.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setproperty.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1084 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setpyinstanceattr.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1705 2024-04-22 11:18:37.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setpyinstanceattr.cpython-311.pyc
+-rw-rw-rw-   0        0        0      999 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setpyinstanceattr.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1083 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setresolution.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1646 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setresolution.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1215 2022-01-24 10:48:44.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setresolution.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1081 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setrigidbody.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1688 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setrigidbody.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1267 2022-01-21 14:10:26.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setrigidbody.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1078 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setscene.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1638 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setscene.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1161 2022-10-05 12:11:17.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setscene.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1176 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setsensorvalue.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1926 2024-04-22 11:18:37.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setsensorvalue.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1308 2022-02-04 18:03:40.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setsensorvalue.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1054 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/settimescale.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1557 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/settimescale.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1238 2022-01-21 14:10:26.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/settimescale.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2026 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setuiwidgetattr.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3106 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setuiwidgetattr.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2462 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setvisibility.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4241 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setvisibility.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2742 2022-02-06 12:51:49.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setvisibility.cpython-39.pyc
+-rw-rw-rw-   0        0        0      998 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setvsync.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1439 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setvsync.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1147 2022-01-21 14:10:26.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/setvsync.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1050 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/showframerate.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1542 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/showframerate.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1180 2022-01-21 14:10:26.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/showframerate.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1141 2023-03-02 16:40:30.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/showuiwidget.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1334 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/slowfollow.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2274 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/slowfollow.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1510 2023-01-21 12:36:26.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/slowfollow.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4166 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/spawnpool.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7393 2024-04-22 11:18:39.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/spawnpool.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4210 2024-01-24 16:53:31.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/startsound.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8346 2024-04-22 11:18:37.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/startsound.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2001 2023-01-21 12:36:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/startsound.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1962 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/startsound2d.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3316 2024-04-22 11:18:37.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/startsound2d.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2543 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/startsound3d.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4659 2024-04-22 11:18:37.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/startsound3d.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2499 2023-01-21 12:36:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/startsound3d.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2188 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/startspeaker.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3607 2024-04-22 11:18:37.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/startspeaker.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2267 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/startspeaker.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1418 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/startsubnetwork.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2169 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/startsubnetwork.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1547 2022-02-08 11:04:17.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/startsubnetwork.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1458 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/stopaction.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2365 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/stopaction.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1676 2023-01-21 12:36:26.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/stopaction.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1069 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/stopallsounds.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1604 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/stopallsounds.cpython-311.pyc
+-rw-rw-rw-   0        0        0      972 2022-01-21 14:10:26.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/stopallsounds.cpython-39.pyc
+-rw-rw-rw-   0        0        0      959 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/stopsound.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1443 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/stopsound.cpython-311.pyc
+-rw-rw-rw-   0        0        0      915 2022-01-21 14:10:26.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/stopsound.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1193 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/stopsubnetwork.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1851 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/stopsubnetwork.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1352 2022-02-08 11:04:17.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/stopsubnetwork.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1043 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/togglefilter.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1522 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/togglefilter.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1173 2022-10-05 12:11:17.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/togglefilter.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1133 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/toggleproperty.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1745 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/toggleproperty.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1343 2022-04-24 16:11:10.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/toggleproperty.cpython-39.pyc
+-rw-rw-rw-   0        0        0      981 2024-01-22 11:02:24.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/translate.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1366 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/translate.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1871 2022-01-21 14:10:26.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/translate.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1336 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/vehicleapplybraking.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2161 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/vehicleapplybraking.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1499 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/vehicleapplybraking.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1333 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/vehicleapplyforce.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2160 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/vehicleapplyforce.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1496 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/vehicleapplyforce.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1341 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/vehicleapplysteering.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2166 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/vehicleapplysteering.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1504 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/vehicleapplysteering.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2399 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/vehiclesetattributes.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4589 2024-04-22 11:18:38.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/vehiclesetattributes.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2562 2022-01-24 10:48:07.000000 uplogic-3.2/uplogic/nodes/actions/__pycache__/vehiclesetattributes.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4259 2024-05-04 07:36:26.000000 uplogic-3.2/uplogic/nodes/actions/addfilter.py
+-rw-rw-rw-   0        0        0     1049 2024-05-04 07:36:38.000000 uplogic-3.2/uplogic/nodes/actions/addobject.py
+-rw-rw-rw-   0        0        0     2180 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/addphysicsconstraint.py
+-rw-rw-rw-   0        0        0      627 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/adduiwidget.py
+-rw-rw-rw-   0        0        0      933 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/alignaxistovector.py
+-rw-rw-rw-   0        0        0      820 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/appendlistitem.py
+-rw-rw-rw-   0        0        0      684 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/applyforce.py
+-rw-rw-rw-   0        0        0      799 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/applyimpulse.py
+-rw-rw-rw-   0        0        0      728 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/applymovement.py
+-rw-rw-rw-   0        0        0      891 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/applyrotation.py
+-rw-rw-rw-   0        0        0      742 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/applytorque.py
+-rw-rw-rw-   0        0        0     1501 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/applytransform.py
+-rw-rw-rw-   0        0        0     1541 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/cameraraycast.py
+-rw-rw-rw-   0        0        0      654 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/characterjump.py
+-rw-rw-rw-   0        0        0     1174 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/clampedmodifyproperty.py
+-rw-rw-rw-   0        0        0     1471 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/clearvariables.py
+-rw-rw-rw-   0        0        0     1022 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/copyproperty.py
+-rw-rw-rw-   0        0        0     3464 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/createuibutton.py
+-rw-rw-rw-   0        0        0      734 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/createuicanvas.py
+-rw-rw-rw-   0        0        0     1736 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/createuiimage.py
+-rw-rw-rw-   0        0        0     2420 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/createuilabel.py
+-rw-rw-rw-   0        0        0     2245 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/createuilayout.py
+-rw-rw-rw-   0        0        0     4393 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/createuislider.py
+-rw-rw-rw-   0        0        0     1618 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/createvehicle.py
+-rw-rw-rw-   0        0        0     1287 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/cursorbehavior.py
+-rw-rw-rw-   0        0        0      612 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/cursorvisibility.py
+-rw-rw-rw-   0        0        0      775 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/dispatchevent.py
+-rw-rw-rw-   0        0        0     2485 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/draw.py
+-rw-rw-rw-   0        0        0     1123 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/drawbox.py
+-rw-rw-rw-   0        0        0      979 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/drawcube.py
+-rw-rw-rw-   0        0        0      922 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/drawline.py
+-rw-rw-rw-   0        0        0     2993 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/editbone.py
+-rw-rw-rw-   0        0        0      432 2023-10-13 21:24:56.000000 uplogic-3.2/uplogic/nodes/actions/endgame.py
+-rw-rw-rw-   0        0        0      690 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/endobject.py
+-rw-rw-rw-   0        0        0     1261 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/executesubnetwork.py
+-rw-rw-rw-   0        0        0     4759 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/followpath.py
+-rw-rw-rw-   0        0        0     2774 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/gamepadlook.py
+-rw-rw-rw-   0        0        0     1146 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/gamepadvibration.py
+-rw-rw-rw-   0        0        0     1973 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/getperformanceprofile.py
+-rw-rw-rw-   0        0        0      963 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/installsubnetwork.py
+-rw-rw-rw-   0        0        0     2005 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/instream.py
+-rw-rw-rw-   0        0        0     1097 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/listglobalvalues.py
+-rw-rw-rw-   0        0        0     1875 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/listvariables.py
+-rw-rw-rw-   0        0        0      595 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/loadblendfile.py
+-rw-rw-rw-   0        0        0     1510 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/loadfilecontent.py
+-rw-rw-rw-   0        0        0     4039 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/loadgame.py
+-rw-rw-rw-   0        0        0     1624 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/loadscene.py
+-rw-rw-rw-   0        0        0     2437 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/localclient.py
+-rw-rw-rw-   0        0        0     2313 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/localserver.py
+-rw-rw-rw-   0        0        0      736 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/makeuniquelight.py
+-rw-rw-rw-   0        0        0     1308 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/modifyproperty.py
+-rw-rw-rw-   0        0        0     2711 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/mouselook.py
+-rw-rw-rw-   0        0        0     1541 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/mouseraycast.py
+-rw-rw-rw-   0        0        0      771 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/mousesetposition.py
+-rw-rw-rw-   0        0        0     1282 2024-05-09 09:30:19.000000 uplogic-3.2/uplogic/nodes/actions/moveto.py
+-rw-rw-rw-   0        0        0     4608 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/movetowithnavmesh.py
+-rw-rw-rw-   0        0        0      595 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/pausesound.py
+-rw-rw-rw-   0        0        0     4347 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/playaction.py
+-rw-rw-rw-   0        0        0     2237 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/playsequence.py
+-rw-rw-rw-   0        0        0     1096 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/popdictkey.py
+-rw-rw-rw-   0        0        0      627 2024-05-16 15:29:16.000000 uplogic-3.2/uplogic/nodes/actions/printvalue.py
+-rw-rw-rw-   0        0        0     2947 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/projectileraycast.py
+-rw-rw-rw-   0        0        0     3025 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/raycast.py
+-rw-rw-rw-   0        0        0      611 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/removefilter.py
+-rw-rw-rw-   0        0        0      938 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/removelistindex.py
+-rw-rw-rw-   0        0        0      971 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/removelistvalue.py
+-rw-rw-rw-   0        0        0      633 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/removeoverlaycollection.py
+-rw-rw-rw-   0        0        0      581 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/removeparent.py
+-rw-rw-rw-   0        0        0      698 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/removephysicsconstraint.py
+-rw-rw-rw-   0        0        0     1605 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/removevariable.py
+-rw-rw-rw-   0        0        0     1025 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/replacemesh.py
+-rw-rw-rw-   0        0        0      505 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/restartgame.py
+-rw-rw-rw-   0        0        0      547 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/resumesound.py
+-rw-rw-rw-   0        0        0      993 2024-05-04 07:17:17.000000 uplogic-3.2/uplogic/nodes/actions/rotateto.py
+-rw-rw-rw-   0        0        0      910 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/runactuator.py
+-rw-rw-rw-   0        0        0     1855 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/runpython.py
+-rw-rw-rw-   0        0        0     7749 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/savegame.py
+-rw-rw-rw-   0        0        0     1773 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/savevariable.py
+-rw-rw-rw-   0        0        0     1512 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/savevariabledict.py
+-rw-rw-rw-   0        0        0     1016 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/sendmessage.py
+-rw-rw-rw-   0        0        0      692 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/sendnetworkmessage.py
+-rw-rw-rw-   0        0        0     2243 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setactionframe.py
+-rw-rw-rw-   0        0        0      900 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setactuatorvalue.py
+-rw-rw-rw-   0        0        0     1097 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setboneconstraintattr.py
+-rw-rw-rw-   0        0        0      974 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setboneconstraintinfluence.py
+-rw-rw-rw-   0        0        0      970 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setboneconstrainttarget.py
+-rw-rw-rw-   0        0        0     1182 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setboneposition.py
+-rw-rw-rw-   0        0        0      625 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setcamera.py
+-rw-rw-rw-   0        0        0      617 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setcamerafov.py
+-rw-rw-rw-   0        0        0      640 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setcameraorthoscale.py
+-rw-rw-rw-   0        0        0      829 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setcharactergravity.py
+-rw-rw-rw-   0        0        0      742 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setcharacterjumpspeed.py
+-rw-rw-rw-   0        0        0      756 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setcharactermaxjumps.py
+-rw-rw-rw-   0        0        0      871 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setcharactervelocity.py
+-rw-rw-rw-   0        0        0     1450 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setcharacterwalkdir.py
+-rw-rw-rw-   0        0        0      773 2024-04-04 13:01:22.000000 uplogic-3.2/uplogic/nodes/actions/setcollisiongroup.py
+-rw-rw-rw-   0        0        0      661 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setcollisionmask.py
+-rw-rw-rw-   0        0        0      851 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setconstraintattribute.py
+-rw-rw-rw-   0        0        0     1137 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setcurvepoints.py
+-rw-rw-rw-   0        0        0      964 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setcustomcursor.py
+-rw-rw-rw-   0        0        0      860 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setdictkey.py
+-rw-rw-rw-   0        0        0      820 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setdynamics.py
+-rw-rw-rw-   0        0        0      659 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/seteeveeao.py
+-rw-rw-rw-   0        0        0      663 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/seteeveebloom.py
+-rw-rw-rw-   0        0        0      592 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/seteeveesmaa.py
+-rw-rw-rw-   0        0        0      633 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/seteeveesmaaquality.py
+-rw-rw-rw-   0        0        0      659 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/seteeveessr.py
+-rw-rw-rw-   0        0        0      705 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/seteeveevolumetrics.py
+-rw-rw-rw-   0        0        0      692 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setexposure.py
+-rw-rw-rw-   0        0        0      697 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setfilterstate.py
+-rw-rw-rw-   0        0        0      621 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setfullscreen.py
+-rw-rw-rw-   0        0        0     1681 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setgameobjectattr.py
+-rw-rw-rw-   0        0        0      686 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setgamma.py
+-rw-rw-rw-   0        0        0      869 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setglobalvalue.py
+-rw-rw-rw-   0        0        0      612 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setgravity.py
+-rw-rw-rw-   0        0        0      778 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setlightcolor.py
+-rw-rw-rw-   0        0        0      724 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setlightenergy.py
+-rw-rw-rw-   0        0        0      744 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setlightshadow.py
+-rw-rw-rw-   0        0        0      894 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setlistindex.py
+-rw-rw-rw-   0        0        0      783 2024-01-22 11:02:02.000000 uplogic-3.2/uplogic/nodes/actions/setlogictreeproperty.py
+-rw-rw-rw-   0        0        0     1052 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setmaterial.py
+-rw-rw-rw-   0        0        0      989 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setmatnodesocket.py
+-rw-rw-rw-   0        0        0     1182 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setmatnodevalue.py
+-rw-rw-rw-   0        0        0      956 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setnodesocket.py
+-rw-rw-rw-   0        0        0     1149 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setnodevalue.py
+-rw-rw-rw-   0        0        0      803 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setoverlaycollection.py
+-rw-rw-rw-   0        0        0      851 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setparent.py
+-rw-rw-rw-   0        0        0      837 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setphysics.py
+-rw-rw-rw-   0        0        0      604 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setprofile.py
+-rw-rw-rw-   0        0        0      962 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setproperty.py
+-rw-rw-rw-   0        0        0      715 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setpyinstanceattr.py
+-rw-rw-rw-   0        0        0      663 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setresolution.py
+-rw-rw-rw-   0        0        0      746 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setrigidbody.py
+-rw-rw-rw-   0        0        0      633 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setscene.py
+-rw-rw-rw-   0        0        0      965 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setsensorvalue.py
+-rw-rw-rw-   0        0        0      624 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/settimescale.py
+-rw-rw-rw-   0        0        0     2204 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setuiwidgetattr.py
+-rw-rw-rw-   0        0        0     2327 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setvisibility.py
+-rw-rw-rw-   0        0        0      546 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/setvsync.py
+-rw-rw-rw-   0        0        0      617 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/showframerate.py
+-rw-rw-rw-   0        0        0     1208 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/slowfollow.py
+-rw-rw-rw-   0        0        0     3973 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/spawnpool.py
+-rw-rw-rw-   0        0        0     5315 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/startsound.py
+-rw-rw-rw-   0        0        0     1856 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/startsound2d.py
+-rw-rw-rw-   0        0        0     2950 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/startsound3d.py
+-rw-rw-rw-   0        0        0     2464 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/startspeaker.py
+-rw-rw-rw-   0        0        0     1192 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/startsubnetwork.py
+-rw-rw-rw-   0        0        0     1161 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/stopaction.py
+-rw-rw-rw-   0        0        0      592 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/stopallsounds.py
+-rw-rw-rw-   0        0        0      543 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/stopsound.py
+-rw-rw-rw-   0        0        0      886 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/stopsubnetwork.py
+-rw-rw-rw-   0        0        0      611 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/togglefilter.py
+-rw-rw-rw-   0        0        0      815 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/toggleproperty.py
+-rw-rw-rw-   0        0        0      524 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/translate.py
+-rw-rw-rw-   0        0        0      992 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/vectoranglecheck.py
+-rw-rw-rw-   0        0        0     1044 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/vehicleapplybraking.py
+-rw-rw-rw-   0        0        0     1037 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/vehicleapplyforce.py
+-rw-rw-rw-   0        0        0     1045 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/vehicleapplysteering.py
+-rw-rw-rw-   0        0        0     3133 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/actions/vehiclesetattributes.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.993171 uplogic-3.2/uplogic/nodes/conditions/
+-rw-rw-rw-   0        0        0     2026 2023-10-03 15:16:22.000000 uplogic-3.2/uplogic/nodes/conditions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:10.126725 uplogic-3.2/uplogic/nodes/conditions/__pycache__/
+-rw-rw-rw-   0        0        0     2235 2023-10-03 16:23:14.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2953 2024-01-02 14:11:12.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2135 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1113 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/barrier.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1732 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/barrier.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1084 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/barrier.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1342 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/checkdistance.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2108 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/checkdistance.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1951 2022-02-07 21:08:00.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/checkdistance.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3416 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/collision.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5884 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/collision.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3398 2023-01-21 12:36:26.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/collision.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1050 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/compare.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1680 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/compare.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1402 2022-01-27 17:43:14.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/compare.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1362 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/comparevectors.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2240 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/comparevectors.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1823 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/comparevectors.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2396 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/controllerstatus.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4228 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/controllerstatus.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2762 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/controllerstatus.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1323 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/evaluateproperty.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2058 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/evaluateproperty.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1600 2022-04-24 16:11:09.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/evaluateproperty.cpython-39.pyc
+-rw-rw-rw-   0        0        0      987 2024-02-09 10:52:27.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/gamepadactive.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1538 2024-02-21 10:59:05.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/gamepadactive.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1002 2022-01-28 16:50:55.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/gamepadactive.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1065 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/gamepadbutton.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1588 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/gamepadbutton.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1403 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/gamepadbutton.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1178 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/gamepadbuttonup.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1860 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/gamepadbuttonup.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1500 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/gamepadbuttonup.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1379 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/handleevent.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2092 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/handleevent.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1551 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/handleevent.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1081 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/hasproperty.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1644 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/hasproperty.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1430 2022-04-24 16:11:09.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/hasproperty.cpython-39.pyc
+-rw-rw-rw-   0        0        0      794 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/keyboardactive.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1099 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/keyboardactive.cpython-311.pyc
+-rw-rw-rw-   0        0        0      752 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/keyboardactive.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1001 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/keypressed.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1484 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/keypressed.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1093 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/keypressed.cpython-39.pyc
+-rw-rw-rw-   0        0        0      926 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/keyreleased.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1367 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/keyreleased.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1083 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/keyreleased.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1288 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logicand.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2326 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logicand.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1666 2022-02-04 11:40:27.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logicand.cpython-39.pyc
+-rw-rw-rw-   0        0        0      795 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logicandnot.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1179 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logicandnot.cpython-311.pyc
+-rw-rw-rw-   0        0        0      888 2022-02-04 11:47:46.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logicandnot.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2272 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logicgate.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3843 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logicgate.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1337 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logicgatelist.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1981 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logicgatelist.cpython-311.pyc
+-rw-rw-rw-   0        0        0      729 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logicnone.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1032 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logicnone.cpython-311.pyc
+-rw-rw-rw-   0        0        0      726 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logicnone.cpython-39.pyc
+-rw-rw-rw-   0        0        0      744 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logicnot.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1034 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logicnot.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1054 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logicnot.cpython-39.pyc
+-rw-rw-rw-   0        0        0      741 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logicnotnone.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1044 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logicnotnone.cpython-311.pyc
+-rw-rw-rw-   0        0        0      738 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logicnotnone.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1295 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logicor.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2329 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logicor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1489 2022-02-04 18:24:17.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logicor.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1306 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logictreestatus.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2021 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logictreestatus.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1647 2022-01-21 17:57:45.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/logictreestatus.cpython-39.pyc
+-rw-rw-rw-   0        0        0      800 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/mousemoved.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1137 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/mousemoved.cpython-311.pyc
+-rw-rw-rw-   0        0        0      832 2022-10-05 12:11:17.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/mousemoved.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2229 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/mouseover.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3602 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/mouseover.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2526 2022-10-05 12:11:17.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/mouseover.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1012 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/mousepressed.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1484 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/mousepressed.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1365 2022-10-05 12:11:17.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/mousepressed.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1245 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/mousepressedon.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1964 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/mousepressedon.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1618 2022-10-05 12:11:17.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/mousepressedon.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1095 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/mousereleased.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1564 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/mousereleased.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1431 2022-10-05 12:11:17.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/mousereleased.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1060 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/mousescroll.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1590 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/mousescroll.cpython-311.pyc
+-rw-rw-rw-   0        0        0      964 2022-10-05 12:11:17.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/mousescroll.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1034 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/once.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1574 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/once.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1114 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/once.cpython-39.pyc
+-rw-rw-rw-   0        0        0      710 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/oninit.cpython-310.pyc
+-rw-rw-rw-   0        0        0      963 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/oninit.cpython-311.pyc
+-rw-rw-rw-   0        0        0      837 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/oninit.cpython-39.pyc
+-rw-rw-rw-   0        0        0      875 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/onnexttick.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1285 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/onnexttick.cpython-311.pyc
+-rw-rw-rw-   0        0        0      861 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/onnexttick.cpython-39.pyc
+-rw-rw-rw-   0        0        0      703 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/onupdate.cpython-310.pyc
+-rw-rw-rw-   0        0        0      919 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/onupdate.cpython-311.pyc
+-rw-rw-rw-   0        0        0      848 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/onupdate.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1454 2024-01-22 11:37:06.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/onvaluechanged.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2216 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/onvaluechanged.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1676 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/onvaluechanged.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1078 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/onvaluechangedto.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1613 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/onvaluechangedto.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1277 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/onvaluechangedto.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1122 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/pulsify.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1781 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/pulsify.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1197 2022-10-05 12:11:17.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/pulsify.cpython-39.pyc
+-rw-rw-rw-   0        0        0      861 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/sensorpositive.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1255 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/sensorpositive.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1245 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/sensorpositive.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1137 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/timedelay.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1825 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/timedelay.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1129 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/timedelay.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1219 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/timer.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1847 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/timer.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1134 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/timer.cpython-39.pyc
+-rw-rw-rw-   0        0        0      933 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/truefalse.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1359 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/truefalse.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1061 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/truefalse.cpython-39.pyc
+-rw-rw-rw-   0        0        0      818 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/valuevalid.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1169 2024-04-22 11:19:22.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/valuevalid.cpython-311.pyc
+-rw-rw-rw-   0        0        0      800 2022-01-21 14:10:25.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/valuevalid.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1438 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/vectoranglecheck.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2281 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/conditions/__pycache__/vectoranglecheck.cpython-311.pyc
+-rw-rw-rw-   0        0        0      880 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/barrier.py
+-rw-rw-rw-   0        0        0      826 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/checkdistance.py
+-rw-rw-rw-   0        0        0     4178 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/collision.py
+-rw-rw-rw-   0        0        0      823 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/compare.py
+-rw-rw-rw-   0        0        0     1165 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/comparevectors.py
+-rw-rw-rw-   0        0        0     2047 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/controllerstatus.py
+-rw-rw-rw-   0        0        0      898 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/evaluateproperty.py
+-rw-rw-rw-   0        0        0      739 2024-02-07 13:13:10.000000 uplogic-3.2/uplogic/nodes/conditions/gamepadactive.py
+-rw-rw-rw-   0        0        0      708 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/gamepadbutton.py
+-rw-rw-rw-   0        0        0     1252 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/gamepadbuttonup.py
+-rw-rw-rw-   0        0        0      811 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/handleevent.py
+-rw-rw-rw-   0        0        0      637 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/hasproperty.py
+-rw-rw-rw-   0        0        0      311 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/keyboardactive.py
+-rw-rw-rw-   0        0        0      615 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/keypressed.py
+-rw-rw-rw-   0        0        0      610 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/keyreleased.py
+-rw-rw-rw-   0        0        0      974 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/logicand.py
+-rw-rw-rw-   0        0        0      416 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/logicandnot.py
+-rw-rw-rw-   0        0        0     1722 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/logicgate.py
+-rw-rw-rw-   0        0        0      907 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/logicgatelist.py
+-rw-rw-rw-   0        0        0      314 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/logicnone.py
+-rw-rw-rw-   0        0        0      332 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/logicnot.py
+-rw-rw-rw-   0        0        0      323 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/logicnotnone.py
+-rw-rw-rw-   0        0        0     1003 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/logicor.py
+-rw-rw-rw-   0        0        0      962 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/logictreestatus.py
+-rw-rw-rw-   0        0        0      389 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/mousemoved.py
+-rw-rw-rw-   0        0        0     2881 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/mouseover.py
+-rw-rw-rw-   0        0        0      631 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/mousepressed.py
+-rw-rw-rw-   0        0        0      940 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/mousepressedon.py
+-rw-rw-rw-   0        0        0      726 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/mousereleased.py
+-rw-rw-rw-   0        0        0      665 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/mousescroll.py
+-rw-rw-rw-   0        0        0      782 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/once.py
+-rw-rw-rw-   0        0        0      268 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/oninit.py
+-rw-rw-rw-   0        0        0      625 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/onnexttick.py
+-rw-rw-rw-   0        0        0      243 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/onupdate.py
+-rw-rw-rw-   0        0        0      974 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/onvaluechanged.py
+-rw-rw-rw-   0        0        0      772 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/onvaluechangedto.py
+-rw-rw-rw-   0        0        0      854 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/pulsify.py
+-rw-rw-rw-   0        0        0      454 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/sensorpositive.py
+-rw-rw-rw-   0        0        0      845 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/timedelay.py
+-rw-rw-rw-   0        0        0      901 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/timer.py
+-rw-rw-rw-   0        0        0      451 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/truefalse.py
+-rw-rw-rw-   0        0        0      389 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/valuevalid.py
+-rw-rw-rw-   0        0        0     1001 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/conditions/vectoranglecheck.py
+-rw-rw-rw-   0        0        0     5388 2024-03-18 08:04:37.000000 uplogic-3.2/uplogic/nodes/logictree.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:10.203467 uplogic-3.2/uplogic/nodes/parameters/
+-rw-rw-rw-   0        0        0     5340 2024-05-09 08:47:54.000000 uplogic-3.2/uplogic/nodes/parameters/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:10.546339 uplogic-3.2/uplogic/nodes/parameters/__pycache__/
+-rw-rw-rw-   0        0        0     5547 2024-02-19 13:06:22.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7472 2024-05-09 08:49:09.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4830 2022-10-05 12:11:17.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      838 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/absolutevalue.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1187 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/absolutevalue.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1083 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/absolutevalue.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1842 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/actionstatus.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2987 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/actionstatus.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1909 2022-01-24 10:48:07.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/actionstatus.cpython-39.pyc
+-rw-rw-rw-   0        0        0      814 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/activecamera.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1101 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/activecamera.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1056 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/activecamera.cpython-39.pyc
+-rw-rw-rw-   0        0        0      888 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/axisvector.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1275 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/axisvector.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1182 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/axisvector.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1847 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/bonestatus.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3043 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/bonestatus.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1985 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/bonestatus.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2070 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/characterinfo.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3213 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/characterinfo.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2253 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/characterinfo.cpython-39.pyc
+-rw-rw-rw-   0        0        0      925 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/childbyindex.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1384 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/childbyindex.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1296 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/childbyindex.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1030 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/childbyname.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1489 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/childbyname.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1178 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/childbyname.cpython-39.pyc
+-rw-rw-rw-   0        0        0      990 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/clamp.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1656 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/clamp.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1216 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/clamp.cpython-39.pyc
+-rw-rw-rw-   0        0        0      816 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/colorrgb.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1203 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/colorrgb.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1131 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/colorrgb.cpython-39.pyc
+-rw-rw-rw-   0        0        0      820 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/colorrgba.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1207 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/colorrgba.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1090 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/colorrgba.cpython-39.pyc
+-rw-rw-rw-   0        0        0      850 2024-02-18 16:31:25.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/curveinterpolation.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1281 2024-02-21 10:59:07.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/curveinterpolation.cpython-311.pyc
+-rw-rw-rw-   0        0        0      871 2024-01-26 09:06:20.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/dictvalue.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1350 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/dictvalue.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1131 2022-02-17 16:48:37.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/dictvalue.cpython-39.pyc
+-rw-rw-rw-   0        0        0      859 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/distance.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1266 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/distance.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1166 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/distance.cpython-39.pyc
+-rw-rw-rw-   0        0        0      954 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/euler.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1498 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/euler.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1145 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/euler.cpython-39.pyc
+-rw-rw-rw-   0        0        0      986 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/eulertomatrix.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1521 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/eulertomatrix.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1191 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/eulertomatrix.cpython-39.pyc
+-rw-rw-rw-   0        0        0      987 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/formattedstring.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1616 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/formattedstring.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1363 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/formattedstring.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1948 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/formula.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3384 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/formula.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2041 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/formula.cpython-39.pyc
+-rw-rw-rw-   0        0        0      798 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/fpsfactor.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1073 2024-04-23 08:21:49.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/fpsfactor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2044 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/gamepadsticks.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3543 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/gamepadsticks.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1797 2022-01-31 12:25:39.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/gamepadsticks.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1713 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/gamepadtrigger.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2915 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/gamepadtrigger.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1533 2022-01-28 16:40:38.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/gamepadtrigger.cpython-39.pyc
+-rw-rw-rw-   0        0        0      928 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getactuatorvalue.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1438 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getactuatorvalue.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1261 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getactuatorvalue.cpython-39.pyc
+-rw-rw-rw-   0        0        0      779 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getcollection.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1064 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getcollection.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1035 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getcollection.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1080 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getcollectionobjectnames.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1465 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getcollectionobjectnames.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1332 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getcollectionobjectnames.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1134 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getcollectionobjects.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1626 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getcollectionobjects.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1326 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getcollectionobjects.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1228 2024-04-04 13:14:21.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getcollisiongroup.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1271 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getcurvepoints.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1967 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getcurvepoints.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1562 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getcurvepoints.cpython-39.pyc
+-rw-rw-rw-   0        0        0      737 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getfont.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1021 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getfont.cpython-311.pyc
+-rw-rw-rw-   0        0        0      793 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getfullscreen.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1066 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getfullscreen.cpython-311.pyc
+-rw-rw-rw-   0        0        0      913 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getfullscreen.cpython-39.pyc
+-rw-rw-rw-   0        0        0      946 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getglobalvalue.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1483 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getglobalvalue.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1323 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getglobalvalue.cpython-39.pyc
+-rw-rw-rw-   0        0        0      807 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getgravity.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1104 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getgravity.cpython-311.pyc
+-rw-rw-rw-   0        0        0      936 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getgravity.cpython-39.pyc
+-rw-rw-rw-   0        0        0      742 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getimage.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1026 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getimage.cpython-311.pyc
+-rw-rw-rw-   0        0        0      993 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getimage.cpython-39.pyc
+-rw-rw-rw-   0        0        0      841 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getlightcolor.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1178 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getlightcolor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1084 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getlightcolor.cpython-39.pyc
+-rw-rw-rw-   0        0        0      849 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getlightenergy.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1186 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getlightenergy.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1093 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getlightenergy.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1051 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getlogictreeproperty.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1666 2024-02-21 10:59:07.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getlogictreeproperty.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1031 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getnodeattribute.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1654 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getnodeattribute.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1418 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getnodeattribute.cpython-39.pyc
+-rw-rw-rw-   0        0        0      965 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getnodesocket.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1466 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getnodesocket.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1345 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getnodesocket.cpython-39.pyc
+-rw-rw-rw-   0        0        0      815 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getobject.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1185 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getobject.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1002 2022-10-05 12:11:18.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getobject.cpython-39.pyc
+-rw-rw-rw-   0        0        0      715 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getowner.cpython-310.pyc
+-rw-rw-rw-   0        0        0      998 2024-02-21 10:59:06.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getowner.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1009 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getowner.cpython-39.pyc
+-rw-rw-rw-   0        0        0      766 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getparent.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1063 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getparent.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1018 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getparent.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1159 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getproperty.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1870 2024-02-21 10:59:06.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getproperty.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1383 2022-10-05 12:11:18.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getproperty.cpython-39.pyc
+-rw-rw-rw-   0        0        0      849 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getpyinstanceattr.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1242 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getpyinstanceattr.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1128 2022-02-04 12:00:46.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getpyinstanceattr.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1216 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getresolution.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1813 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getresolution.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1358 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getresolution.cpython-39.pyc
+-rw-rw-rw-   0        0        0      762 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getscene.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1034 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getscene.cpython-311.pyc
+-rw-rw-rw-   0        0        0      889 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getscene.cpython-39.pyc
+-rw-rw-rw-   0        0        0      957 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getsensorvalue.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1459 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getsensorvalue.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1223 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getsensorvalue.cpython-39.pyc
+-rw-rw-rw-   0        0        0      742 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getsound.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1026 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getsound.cpython-311.pyc
+-rw-rw-rw-   0        0        0      993 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getsound.cpython-39.pyc
+-rw-rw-rw-   0        0        0      775 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/gettimescale.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1047 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/gettimescale.cpython-311.pyc
+-rw-rw-rw-   0        0        0      906 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/gettimescale.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1012 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getuiwidgetattr.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1895 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getuiwidgetattr.cpython-311.pyc
+-rw-rw-rw-   0        0        0      758 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getvsync.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1029 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getvsync.cpython-311.pyc
+-rw-rw-rw-   0        0        0      883 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/getvsync.cpython-39.pyc
+-rw-rw-rw-   0        0        0      774 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/initemptydict.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1029 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/initemptydict.cpython-311.pyc
+-rw-rw-rw-   0        0        0      906 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/initemptydict.cpython-39.pyc
+-rw-rw-rw-   0        0        0      979 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/initemptylist.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1369 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/initemptylist.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1178 2022-01-26 18:16:26.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/initemptylist.cpython-39.pyc
+-rw-rw-rw-   0        0        0      818 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/initnewdict.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1210 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/initnewdict.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1061 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/initnewdict.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1476 2024-02-09 10:52:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/instream.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2337 2024-02-21 10:59:07.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/instream.cpython-311.pyc
+-rw-rw-rw-   0        0        0      890 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/interpolate.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1368 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/interpolate.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1198 2022-02-10 13:44:11.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/interpolate.cpython-39.pyc
+-rw-rw-rw-   0        0        0      828 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/invertvalue.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1186 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/invertvalue.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1043 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/invertvalue.cpython-39.pyc
+-rw-rw-rw-   0        0        0      727 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/keycode.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1023 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/keycode.cpython-311.pyc
+-rw-rw-rw-   0        0        0      722 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/keycode.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1386 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/limitrange.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2434 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/limitrange.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1605 2022-10-05 12:11:18.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/limitrange.cpython-39.pyc
+-rw-rw-rw-   0        0        0      795 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/listduplicate.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1136 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/listduplicate.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1054 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/listduplicate.cpython-39.pyc
+-rw-rw-rw-   0        0        0      967 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/listextend.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1452 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/listextend.cpython-311.pyc
+-rw-rw-rw-   0        0        0      924 2024-01-24 16:53:31.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/listfromitems.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1272 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/listfromitems.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1384 2022-02-17 08:21:55.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/listfromitems.cpython-39.pyc
+-rw-rw-rw-   0        0        0      835 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/listindex.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1256 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/listindex.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1128 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/listindex.cpython-39.pyc
+-rw-rw-rw-   0        0        0      870 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/listindexrandom.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1254 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/listindexrandom.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1186 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/listindexrandom.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1686 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/loadvariable.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3019 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/loadvariable.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1996 2022-03-05 16:11:37.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/loadvariable.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1582 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/loadvariabledict.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2691 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/loadvariabledict.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1783 2022-02-06 14:17:54.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/loadvariabledict.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1061 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/maprange.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1775 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/maprange.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1081 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/materialgetattribute.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1720 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/materialgetattribute.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1445 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/materialgetattribute.cpython-39.pyc
+-rw-rw-rw-   0        0        0      925 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/materialgetnode.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1338 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/materialgetnode.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1153 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/materialgetnode.cpython-39.pyc
+-rw-rw-rw-   0        0        0      999 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/materialgetsocket.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1511 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/materialgetsocket.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1371 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/materialgetsocket.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1457 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/math.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3065 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/math.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1918 2022-10-05 12:11:18.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/math.cpython-39.pyc
+-rw-rw-rw-   0        0        0      935 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/matrixtoxyz.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1453 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/matrixtoxyz.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1086 2022-01-30 15:01:27.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/matrixtoxyz.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1719 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/mousedata.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2765 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/mousedata.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2103 2022-10-05 12:11:18.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/mousedata.cpython-39.pyc
+-rw-rw-rw-   0        0        0      985 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/objectattr.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1563 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/objectattr.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1267 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/objectattr.cpython-39.pyc
+-rw-rw-rw-   0        0        0      810 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/objectdataname.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1122 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/objectdataname.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1054 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/objectdataname.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1114 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/objectdatavertices.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1630 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/objectdatavertices.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1433 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/objectdatavertices.cpython-39.pyc
+-rw-rw-rw-   0        0        0      968 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/randomfloat.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1502 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/randomfloat.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1291 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/randomfloat.cpython-39.pyc
+-rw-rw-rw-   0        0        0      933 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/randomint.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1430 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/randomint.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1254 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/randomint.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2030 2024-02-16 09:49:00.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/randomvalue.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3598 2024-04-23 08:21:49.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/randomvalue.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1012 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/randomvect.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1609 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/randomvect.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1286 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/randomvect.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1273 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/rangedthreshold.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2066 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/rangedthreshold.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1413 2022-10-05 12:11:18.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/rangedthreshold.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1513 2024-01-26 09:20:16.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/rebuilddata.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2592 2024-04-23 08:21:49.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/rebuilddata.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1528 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/resizevector.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2336 2024-04-23 08:21:49.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/resizevector.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2011 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/rotatebypoint.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3948 2024-04-23 08:21:49.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/rotatebypoint.cpython-311.pyc
+-rw-rw-rw-   0        0        0      874 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/screenposition.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1236 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/screenposition.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1210 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/screenposition.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1051 2024-01-26 09:15:05.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/serializedata.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1572 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/serializedata.cpython-311.pyc
+-rw-rw-rw-   0        0        0      767 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/simplevalue.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1054 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/simplevalue.cpython-311.pyc
+-rw-rw-rw-   0        0        0      897 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/simplevalue.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1039 2024-02-16 09:47:28.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/storevalue.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1806 2024-04-04 13:48:41.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/storevalue.cpython-311.pyc
+-rw-rw-rw-   0        0        0      990 2022-10-05 12:11:18.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/storevalue.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1134 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/threshold.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1741 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/threshold.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1401 2022-10-05 12:11:18.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/threshold.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1538 2024-01-22 11:37:06.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/timedata.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2174 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/timedata.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1661 2022-10-05 12:11:18.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/timedata.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2475 2024-02-19 17:56:52.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/tweenvalue.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5077 2024-05-08 11:17:25.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/tweenvalue.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1078 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/typecastvalue.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1626 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/typecastvalue.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1340 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/typecastvalue.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3325 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/valueswitch.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6935 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/valueswitch.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4058 2022-01-27 17:43:14.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/valueswitch.cpython-39.pyc
+-rw-rw-rw-   0        0        0      921 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectorabsolute.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1459 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectorabsolute.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1153 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectorabsolute.cpython-39.pyc
+-rw-rw-rw-   0        0        0      935 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectorangle.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1414 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectorangle.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1184 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectorangle.cpython-39.pyc
+-rw-rw-rw-   0        0        0      240 2023-09-30 13:39:07.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectoranglecheck.cpython-310.pyc
+-rw-rw-rw-   0        0        0      270 2024-01-02 14:42:14.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectoranglecheck.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1601 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectoranglecheck.cpython-39.pyc
+-rw-rw-rw-   0        0        0      838 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectorlength.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1188 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectorlength.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1081 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectorlength.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4942 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectormath.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8094 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectormath.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1604 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectormath.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1157 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectorsplitxy.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1652 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectorsplitxy.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1229 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectorsplitxy.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1306 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectorsplitxyz.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1900 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectorsplitxyz.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1497 2022-01-30 15:01:27.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectorsplitxyz.cpython-39.pyc
+-rw-rw-rw-   0        0        0      836 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectorxy.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1242 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectorxy.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1106 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectorxy.cpython-39.pyc
+-rw-rw-rw-   0        0        0      874 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectorxyz.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1348 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectorxyz.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1173 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectorxyz.cpython-39.pyc
+-rw-rw-rw-   0        0        0      912 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectorxyzw.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1454 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectorxyzw.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1245 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vectorxyzw.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2054 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vrcontrollervalues.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3194 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vrcontrollervalues.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2240 2022-10-05 12:11:18.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vrcontrollervalues.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1019 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vrheadsetvalues.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1460 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vrheadsetvalues.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1158 2022-10-05 12:11:18.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/vrheadsetvalues.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1238 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/withinrange.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2029 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/withinrange.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1374 2022-10-05 12:11:18.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/withinrange.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1004 2024-01-22 11:02:23.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/worldposition.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1594 2024-04-23 08:21:48.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/worldposition.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1344 2022-01-21 15:13:29.000000 uplogic-3.2/uplogic/nodes/parameters/__pycache__/worldposition.cpython-39.pyc
+-rw-rw-rw-   0        0        0      392 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/absolutevalue.py
+-rw-rw-rw-   0        0        0     1392 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/actionstatus.py
+-rw-rw-rw-   0        0        0      334 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/activecamera.py
+-rw-rw-rw-   0        0        0      461 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/axisvector.py
+-rw-rw-rw-   0        0        0     1694 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/bonestatus.py
+-rw-rw-rw-   0        0        0     1521 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/characterinfo.py
+-rw-rw-rw-   0        0        0      559 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/childbyindex.py
+-rw-rw-rw-   0        0        0      553 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/childbyname.py
+-rw-rw-rw-   0        0        0      834 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/clamp.py
+-rw-rw-rw-   0        0        0      394 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/colorrgb.py
+-rw-rw-rw-   0        0        0      395 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/colorrgba.py
+-rw-rw-rw-   0        0        0      437 2024-02-18 16:30:58.000000 uplogic-3.2/uplogic/nodes/parameters/curveinterpolation.py
+-rw-rw-rw-   0        0        0      565 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/dictvalue.py
+-rw-rw-rw-   0        0        0      465 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/distance.py
+-rw-rw-rw-   0        0        0      602 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/euler.py
+-rw-rw-rw-   0        0        0      553 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/eulertomatrix.py
+-rw-rw-rw-   0        0        0      732 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/formattedstring.py
+-rw-rw-rw-   0        0        0     1919 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/formula.py
+-rw-rw-rw-   0        0        0      324 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/fpsfactor.py
+-rw-rw-rw-   0        0        0     1930 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/gamepadsticks.py
+-rw-rw-rw-   0        0        0     1480 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/gamepadtrigger.py
+-rw-rw-rw-   0        0        0      610 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/getactuatorvalue.py
+-rw-rw-rw-   0        0        0      323 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/getcollection.py
+-rw-rw-rw-   0        0        0      464 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/getcollectionobjectnames.py
+-rw-rw-rw-   0        0        0      529 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/getcollectionobjects.py
+-rw-rw-rw-   0        0        0      434 2024-04-04 13:03:32.000000 uplogic-3.2/uplogic/nodes/parameters/getcollisiongroup.py
+-rw-rw-rw-   0        0        0      582 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/getcurvepoints.py
+-rw-rw-rw-   0        0        0      295 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/getfont.py
+-rw-rw-rw-   0        0        0      306 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/getfullscreen.py
+-rw-rw-rw-   0        0        0      562 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/getglobalvalue.py
+-rw-rw-rw-   0        0        0      337 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/getgravity.py
+-rw-rw-rw-   0        0        0      298 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/getimage.py
+-rw-rw-rw-   0        0        0      398 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/getlightcolor.py
+-rw-rw-rw-   0        0        0      404 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/getlightenergy.py
+-rw-rw-rw-   0        0        0      660 2024-01-22 11:02:02.000000 uplogic-3.2/uplogic/nodes/parameters/getlogictreeproperty.py
+-rw-rw-rw-   0        0        0      725 2024-05-09 09:06:13.000000 uplogic-3.2/uplogic/nodes/parameters/getmasterfolder.py
+-rw-rw-rw-   0        0        0      805 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/getnodeattribute.py
+-rw-rw-rw-   0        0        0      659 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/getnodesocket.py
+-rw-rw-rw-   0        0        0      369 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/getobject.py
+-rw-rw-rw-   0        0        0      284 2024-01-22 11:02:02.000000 uplogic-3.2/uplogic/nodes/parameters/getowner.py
+-rw-rw-rw-   0        0        0      322 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/getparent.py
+-rw-rw-rw-   0        0        0      837 2024-01-22 11:02:02.000000 uplogic-3.2/uplogic/nodes/parameters/getproperty.py
+-rw-rw-rw-   0        0        0      429 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/getpyinstanceattr.py
+-rw-rw-rw-   0        0        0      661 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/getresolution.py
+-rw-rw-rw-   0        0        0      289 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/getscene.py
+-rw-rw-rw-   0        0        0      600 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/getsensorvalue.py
+-rw-rw-rw-   0        0        0      296 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/getsound.py
+-rw-rw-rw-   0        0        0      290 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/gettimescale.py
+-rw-rw-rw-   0        0        0      825 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/getuiwidgetattr.py
+-rw-rw-rw-   0        0        0      286 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/getvsync.py
+-rw-rw-rw-   0        0        0      334 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/initemptydict.py
+-rw-rw-rw-   0        0        0      414 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/initemptylist.py
+-rw-rw-rw-   0        0        0      396 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/initnewdict.py
+-rw-rw-rw-   0        0        0      856 2024-02-09 10:13:40.000000 uplogic-3.2/uplogic/nodes/parameters/instream.py
+-rw-rw-rw-   0        0        0      478 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/interpolate.py
+-rw-rw-rw-   0        0        0      404 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/invertvalue.py
+-rw-rw-rw-   0        0        0      490 2024-05-09 08:59:29.000000 uplogic-3.2/uplogic/nodes/parameters/joinpath.py
+-rw-rw-rw-   0        0        0      299 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/nodes/parameters/keycode.py
+-rw-rw-rw-   0        0        0     1232 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/limitrange.py
+-rw-rw-rw-   0        0        0      343 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/listduplicate.py
+-rw-rw-rw-   0        0        0      527 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/listextend.py
+-rw-rw-rw-   0        0        0      327 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/listfromitems.py
+-rw-rw-rw-   0        0        0      461 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/listindex.py
+-rw-rw-rw-   0        0        0      447 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/listindexrandom.py
+-rw-rw-rw-   0        0        0     1466 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/loadvariable.py
+-rw-rw-rw-   0        0        0     1175 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/loadvariabledict.py
+-rw-rw-rw-   0        0        0      831 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/maprange.py
+-rw-rw-rw-   0        0        0      853 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/materialgetattribute.py
+-rw-rw-rw-   0        0        0      556 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/materialgetnode.py
+-rw-rw-rw-   0        0        0      693 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/materialgetsocket.py
+-rw-rw-rw-   0        0        0     1673 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/math.py
+-rw-rw-rw-   0        0        0      568 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/matrixtoxyz.py
+-rw-rw-rw-   0        0        0     1045 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/mousedata.py
+-rw-rw-rw-   0        0        0      657 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/objectattr.py
+-rw-rw-rw-   0        0        0      352 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/objectdataname.py
+-rw-rw-rw-   0        0        0      584 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/objectdatavertices.py
+-rw-rw-rw-   0        0        0      741 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/randomfloat.py
+-rw-rw-rw-   0        0        0      690 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/randomint.py
+-rw-rw-rw-   0        0        0     1722 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/randomvalue.py
+-rw-rw-rw-   0        0        0      639 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/randomvect.py
+-rw-rw-rw-   0        0        0      929 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/rangedthreshold.py
+-rw-rw-rw-   0        0        0     1522 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/rebuilddata.py
+-rw-rw-rw-   0        0        0      867 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/resizevector.py
+-rw-rw-rw-   0        0        0     1930 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/rotatebypoint.py
+-rw-rw-rw-   0        0        0      462 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/screenposition.py
+-rw-rw-rw-   0        0        0      734 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/serializedata.py
+-rw-rw-rw-   0        0        0      322 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/simplevalue.py
+-rw-rw-rw-   0        0        0      930 2024-04-04 13:47:56.000000 uplogic-3.2/uplogic/nodes/parameters/storevalue.py
+-rw-rw-rw-   0        0        0      758 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/threshold.py
+-rw-rw-rw-   0        0        0      885 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/timedata.py
+-rw-rw-rw-   0        0        0     3224 2024-05-08 11:16:31.000000 uplogic-3.2/uplogic/nodes/parameters/tweenvalue.py
+-rw-rw-rw-   0        0        0      685 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/typecastvalue.py
+-rw-rw-rw-   0        0        0     4193 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/valueswitch.py
+-rw-rw-rw-   0        0        0      502 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/vectorabsolute.py
+-rw-rw-rw-   0        0        0      587 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/vectorangle.py
+-rw-rw-rw-   0        0        0       60 2023-09-30 12:04:19.000000 uplogic-3.2/uplogic/nodes/parameters/vectoranglecheck.py
+-rw-rw-rw-   0        0        0      378 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/vectorlength.py
+-rw-rw-rw-   0        0        0     4632 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/nodes/parameters/vectormath.py
+-rw-rw-rw-   0        0        0      578 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/vectorsplitxy.py
+-rw-rw-rw-   0        0        0      686 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/vectorsplitxyz.py
+-rw-rw-rw-   0        0        0      439 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/vectorxy.py
+-rw-rw-rw-   0        0        0      514 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/vectorxyz.py
+-rw-rw-rw-   0        0        0      585 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/vectorxyzw.py
+-rw-rw-rw-   0        0        0     1273 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/vrcontrollervalues.py
+-rw-rw-rw-   0        0        0      486 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/vrheadsetvalues.py
+-rw-rw-rw-   0        0        0      923 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/withinrange.py
+-rw-rw-rw-   0        0        0      731 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/nodes/parameters/worldposition.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:10.550325 uplogic-3.2/uplogic/physics/
+-rw-rw-rw-   0        0        0      540 2023-03-06 11:18:24.000000 uplogic-3.2/uplogic/physics/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:10.565276 uplogic-3.2/uplogic/physics/__pycache__/
+-rw-rw-rw-   0        0        0      770 2023-03-06 11:22:36.000000 uplogic-3.2/uplogic/physics/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      941 2024-01-02 14:08:23.000000 uplogic-3.2/uplogic/physics/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      592 2022-04-24 08:20:18.000000 uplogic-3.2/uplogic/physics/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4412 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/physics/__pycache__/buoyancy.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7308 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/physics/__pycache__/buoyancy.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3966 2023-01-21 12:36:04.000000 uplogic-3.2/uplogic/physics/__pycache__/buoyancy.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4795 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/physics/__pycache__/character.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8233 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/physics/__pycache__/character.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4224 2023-01-21 12:36:04.000000 uplogic-3.2/uplogic/physics/__pycache__/character.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3542 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/physics/__pycache__/collision.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5658 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/physics/__pycache__/collision.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3094 2022-10-05 12:11:16.000000 uplogic-3.2/uplogic/physics/__pycache__/collision.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7894 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/physics/__pycache__/constraints.cpython-310.pyc
+-rw-rw-rw-   0        0        0    12855 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/physics/__pycache__/constraints.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7293 2022-08-15 17:30:07.000000 uplogic-3.2/uplogic/physics/__pycache__/constraints.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8453 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/physics/__pycache__/vehicle.cpython-310.pyc
+-rw-rw-rw-   0        0        0    16529 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/physics/__pycache__/vehicle.cpython-311.pyc
+-rw-rw-rw-   0        0        0     8456 2023-01-21 12:36:04.000000 uplogic-3.2/uplogic/physics/__pycache__/vehicle.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4160 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/physics/buoyancy.py
+-rw-rw-rw-   0        0        0     4109 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/physics/character.py
+-rw-rw-rw-   0        0        0     3644 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/physics/collision.py
+-rw-rw-rw-   0        0        0     8366 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/physics/constraints.py
+-rw-rw-rw-   0        0        0    10213 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/physics/vehicle.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:10.567270 uplogic-3.2/uplogic/serialize/
+-rw-rw-rw-   0        0        0     2965 2023-12-11 16:15:51.000000 uplogic-3.2/uplogic/serialize/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:10.568266 uplogic-3.2/uplogic/serialize/__pycache__/
+-rw-rw-rw-   0        0        0     2847 2023-12-11 16:16:10.000000 uplogic-3.2/uplogic/serialize/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5988 2024-01-02 14:08:24.000000 uplogic-3.2/uplogic/serialize/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:10.580227 uplogic-3.2/uplogic/shaders/
+-rw-rw-rw-   0        0        0      795 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/shaders/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:10.635042 uplogic-3.2/uplogic/shaders/__pycache__/
+-rw-rw-rw-   0        0        0     1141 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/shaders/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1555 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/shaders/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      757 2023-01-21 12:36:26.000000 uplogic-3.2/uplogic/shaders/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1393 2023-04-01 08:39:44.000000 uplogic-3.2/uplogic/shaders/__pycache__/adaptivetonemapping.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1952 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/shaders/__pycache__/adaptivetonemapping.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1367 2023-01-21 12:36:26.000000 uplogic-3.2/uplogic/shaders/__pycache__/adaptivetonemapping.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2098 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/shaders/__pycache__/blur.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2871 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/shaders/__pycache__/blur.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1160 2023-04-01 08:39:44.000000 uplogic-3.2/uplogic/shaders/__pycache__/brightness.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1674 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/shaders/__pycache__/brightness.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1134 2023-01-21 12:36:26.000000 uplogic-3.2/uplogic/shaders/__pycache__/brightness.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1757 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/shaders/__pycache__/buffer.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2762 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/shaders/__pycache__/buffer.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1581 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/shaders/__pycache__/chromaticaberration.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2087 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/shaders/__pycache__/chromaticaberration.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1557 2022-09-19 13:05:15.000000 uplogic-3.2/uplogic/shaders/__pycache__/chromaticaberration.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7382 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/shaders/__pycache__/distort.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8701 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/shaders/__pycache__/distort.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7729 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/shaders/__pycache__/dof.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9509 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/shaders/__pycache__/dof.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9463 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/shaders/__pycache__/droplets.cpython-310.pyc
+-rw-rw-rw-   0        0        0    11602 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/shaders/__pycache__/droplets.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3042 2024-05-02 18:01:29.000000 uplogic-3.2/uplogic/shaders/__pycache__/eyelids.cpython-311.pyc
+-rw-rw-rw-   0        0        0      191 2024-02-21 19:15:33.000000 uplogic-3.2/uplogic/shaders/__pycache__/filtersystem.cpython-311.pyc
+-rw-rw-rw-   0        0        0    33106 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/shaders/__pycache__/fxaa.cpython-310.pyc
+-rw-rw-rw-   0        0        0    33374 2024-04-16 09:41:39.000000 uplogic-3.2/uplogic/shaders/__pycache__/fxaa.cpython-311.pyc
+-rw-rw-rw-   0        0        0    33102 2022-09-19 13:05:14.000000 uplogic-3.2/uplogic/shaders/__pycache__/fxaa.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1414 2023-04-01 08:39:44.000000 uplogic-3.2/uplogic/shaders/__pycache__/grayscale.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1867 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/shaders/__pycache__/grayscale.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1386 2022-09-19 13:05:14.000000 uplogic-3.2/uplogic/shaders/__pycache__/grayscale.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9732 2023-07-05 15:03:20.000000 uplogic-3.2/uplogic/shaders/__pycache__/hbao.cpython-310.pyc
+-rw-rw-rw-   0        0        0    10620 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/shaders/__pycache__/hbao.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9729 2023-01-21 12:36:26.000000 uplogic-3.2/uplogic/shaders/__pycache__/hbao.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2140 2022-07-30 17:30:55.000000 uplogic-3.2/uplogic/shaders/__pycache__/hdr.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1499 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/shaders/__pycache__/lens.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2011 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/shaders/__pycache__/lens.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1627 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/shaders/__pycache__/letterbox.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2425 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/shaders/__pycache__/letterbox.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1541 2023-04-01 08:39:44.000000 uplogic-3.2/uplogic/shaders/__pycache__/levels.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2086 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/shaders/__pycache__/levels.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1515 2023-01-21 12:36:26.000000 uplogic-3.2/uplogic/shaders/__pycache__/levels.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4387 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/shaders/__pycache__/mist.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6221 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/shaders/__pycache__/mist.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4258 2022-10-05 13:36:58.000000 uplogic-3.2/uplogic/shaders/__pycache__/mist.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2026 2023-11-11 15:08:08.000000 uplogic-3.2/uplogic/shaders/__pycache__/offscreen.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1529 2022-07-30 16:46:29.000000 uplogic-3.2/uplogic/shaders/__pycache__/radialblur.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1902 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/shaders/__pycache__/rendertoscreen.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3436 2024-04-23 15:16:37.000000 uplogic-3.2/uplogic/shaders/__pycache__/rendertoscreen.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6241 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/shaders/__pycache__/shader.cpython-310.pyc
+-rw-rw-rw-   0        0        0    12549 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/shaders/__pycache__/shader.cpython-311.pyc
+-rw-rw-rw-   0        0        0     5110 2022-09-19 13:05:14.000000 uplogic-3.2/uplogic/shaders/__pycache__/shader.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2699 2023-04-01 08:39:44.000000 uplogic-3.2/uplogic/shaders/__pycache__/sharpen.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3199 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/shaders/__pycache__/sharpen.cpython-311.pyc
+-rw-rw-rw-   0        0        0    55031 2024-01-26 11:26:24.000000 uplogic-3.2/uplogic/shaders/__pycache__/smaa.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2408 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/shaders/__pycache__/splitscreen.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4341 2024-04-23 15:16:37.000000 uplogic-3.2/uplogic/shaders/__pycache__/splitscreen.cpython-311.pyc
+-rw-rw-rw-   0        0        0     5995 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/shaders/__pycache__/ssao.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6833 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/shaders/__pycache__/ssao.cpython-311.pyc
+-rw-rw-rw-   0        0        0     5975 2023-01-21 12:36:26.000000 uplogic-3.2/uplogic/shaders/__pycache__/ssao.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4247 2023-02-19 13:56:26.000000 uplogic-3.2/uplogic/shaders/__pycache__/ssgi.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2935 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/shaders/__pycache__/texture.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4802 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/shaders/__pycache__/texture.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1696 2024-02-12 15:23:12.000000 uplogic-3.2/uplogic/shaders/__pycache__/vignette.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2487 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/shaders/__pycache__/vignette.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1703 2022-09-19 13:05:14.000000 uplogic-3.2/uplogic/shaders/__pycache__/vignette.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9718 2023-02-12 16:47:36.000000 uplogic-3.2/uplogic/shaders/__pycache__/water.cpython-310.pyc
+-rw-rw-rw-   0        0        0      872 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/shaders/adaptivetonemapping.py
+-rw-rw-rw-   0        0        0     1656 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/shaders/blur.py
+-rw-rw-rw-   0        0        0      685 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/shaders/brightness.py
+-rw-rw-rw-   0        0        0     1182 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/shaders/buffer.py
+-rw-rw-rw-   0        0        0     1070 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/shaders/chromaticaberration.py
+-rw-rw-rw-   0        0        0     7049 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/shaders/distort.py
+-rw-rw-rw-   0        0        0     9821 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/shaders/dof.py
+-rw-rw-rw-   0        0        0     9064 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/shaders/droplets.py
+-rw-rw-rw-   0        0        0     1780 2024-05-02 18:01:21.000000 uplogic-3.2/uplogic/shaders/eyelids.py
+-rw-rw-rw-   0        0        0       10 2024-02-21 19:10:36.000000 uplogic-3.2/uplogic/shaders/filtersystem.py
+-rw-rw-rw-   0        0        0    33422 2024-04-16 09:39:46.000000 uplogic-3.2/uplogic/shaders/fxaa.py
+-rw-rw-rw-   0        0        0      892 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/shaders/grayscale.py
+-rw-rw-rw-   0        0        0     9683 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/shaders/hbao.py
+-rw-rw-rw-   0        0        0     1035 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/shaders/lens.py
+-rw-rw-rw-   0        0        0     1137 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/shaders/letterbox.py
+-rw-rw-rw-   0        0        0     1027 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/shaders/levels.py
+-rw-rw-rw-   0        0        0     4172 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/shaders/mist.py
+-rw-rw-rw-   0        0        0     1779 2024-02-12 11:42:26.000000 uplogic-3.2/uplogic/shaders/rendertoscreen.py
+-rw-rw-rw-   0        0        0     6157 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/shaders/shader.py
+-rw-rw-rw-   0        0        0     2268 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/shaders/sharpen.py
+-rw-rw-rw-   0        0        0     2898 2024-02-12 11:42:41.000000 uplogic-3.2/uplogic/shaders/splitscreen.py
+-rw-rw-rw-   0        0        0     5754 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/shaders/ssao.py
+-rw-rw-rw-   0        0        0     2507 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/shaders/texture.py
+-rw-rw-rw-   0        0        0     1189 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/shaders/vignette.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:10.654520 uplogic-3.2/uplogic/ui/
+-rw-rw-rw-   0        0        0      653 2024-05-06 10:41:48.000000 uplogic-3.2/uplogic/ui/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:10.686412 uplogic-3.2/uplogic/ui/__pycache__/
+-rw-rw-rw-   0        0        0      917 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/ui/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1249 2024-05-06 10:42:26.000000 uplogic-3.2/uplogic/ui/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2217 2024-02-16 10:05:54.000000 uplogic-3.2/uplogic/ui/__pycache__/behaviors.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3754 2024-05-16 15:16:41.000000 uplogic-3.2/uplogic/ui/__pycache__/behaviors.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9526 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/ui/__pycache__/button.cpython-310.pyc
+-rw-rw-rw-   0        0        0    16676 2024-05-16 15:31:20.000000 uplogic-3.2/uplogic/ui/__pycache__/button.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2104 2023-11-11 20:36:47.000000 uplogic-3.2/uplogic/ui/__pycache__/camera.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4157 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/ui/__pycache__/canvas.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7481 2024-05-16 15:20:11.000000 uplogic-3.2/uplogic/ui/__pycache__/canvas.cpython-311.pyc
+-rw-rw-rw-   0        0        0     8951 2024-03-22 08:49:59.000000 uplogic-3.2/uplogic/ui/__pycache__/compass.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3658 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/ui/__pycache__/cursor.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7253 2024-05-16 15:13:49.000000 uplogic-3.2/uplogic/ui/__pycache__/cursor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6277 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/ui/__pycache__/image.cpython-310.pyc
+-rw-rw-rw-   0        0        0    11421 2024-05-16 15:13:49.000000 uplogic-3.2/uplogic/ui/__pycache__/image.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6006 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/ui/__pycache__/label.cpython-310.pyc
+-rw-rw-rw-   0        0        0    11610 2024-05-16 15:13:49.000000 uplogic-3.2/uplogic/ui/__pycache__/label.cpython-311.pyc
+-rw-rw-rw-   0        0        0    12879 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/ui/__pycache__/layout.cpython-310.pyc
+-rw-rw-rw-   0        0        0    19336 2024-05-16 15:13:49.000000 uplogic-3.2/uplogic/ui/__pycache__/layout.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4902 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/ui/__pycache__/path.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8874 2024-05-16 15:13:49.000000 uplogic-3.2/uplogic/ui/__pycache__/path.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2229 2024-02-16 10:05:54.000000 uplogic-3.2/uplogic/ui/__pycache__/render.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8002 2024-02-14 16:59:36.000000 uplogic-3.2/uplogic/ui/__pycache__/render.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6361 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/ui/__pycache__/slider.cpython-310.pyc
+-rw-rw-rw-   0        0        0    12077 2024-05-16 15:13:49.000000 uplogic-3.2/uplogic/ui/__pycache__/slider.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1366 2023-02-14 11:39:44.000000 uplogic-3.2/uplogic/ui/__pycache__/system.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7106 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/ui/__pycache__/textinput.cpython-310.pyc
+-rw-rw-rw-   0        0        0    13138 2024-05-16 15:54:34.000000 uplogic-3.2/uplogic/ui/__pycache__/textinput.cpython-311.pyc
+-rw-rw-rw-   0        0        0    15120 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/ui/__pycache__/widget.cpython-310.pyc
+-rw-rw-rw-   0        0        0    25191 2024-05-17 19:51:25.000000 uplogic-3.2/uplogic/ui/__pycache__/widget.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1731 2023-02-27 08:15:13.000000 uplogic-3.2/uplogic/ui/__pycache__/window.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1846 2024-05-29 08:22:45.000000 uplogic-3.2/uplogic/ui/behaviors.py
+-rw-rw-rw-   0        0        0    10171 2024-05-16 15:31:17.000000 uplogic-3.2/uplogic/ui/button.py
+-rw-rw-rw-   0        0        0     1744 2024-05-16 15:11:26.000000 uplogic-3.2/uplogic/ui/camera.py
+-rw-rw-rw-   0        0        0     3637 2024-05-16 15:19:46.000000 uplogic-3.2/uplogic/ui/canvas.py
+-rw-rw-rw-   0        0        0     2616 2024-05-16 15:11:38.000000 uplogic-3.2/uplogic/ui/circle.py
+-rw-rw-rw-   0        0        0     3710 2024-05-16 15:11:56.000000 uplogic-3.2/uplogic/ui/cursor.py
+-rw-rw-rw-   0        0        0     7199 2024-05-16 15:12:05.000000 uplogic-3.2/uplogic/ui/image.py
+-rw-rw-rw-   0        0        0     8193 2024-05-16 15:12:11.000000 uplogic-3.2/uplogic/ui/label.py
+-rw-rw-rw-   0        0        0    13625 2024-05-16 15:12:54.000000 uplogic-3.2/uplogic/ui/layout.py
+-rw-rw-rw-   0        0        0     5232 2024-05-16 15:13:46.000000 uplogic-3.2/uplogic/ui/path.py
+-rw-rw-rw-   0        0        0     2063 2024-05-16 15:13:46.000000 uplogic-3.2/uplogic/ui/render.py
+-rw-rw-rw-   0        0        0     8127 2024-05-16 15:13:46.000000 uplogic-3.2/uplogic/ui/slider.py
+-rw-rw-rw-   0        0        0     9047 2024-05-16 15:54:32.000000 uplogic-3.2/uplogic/ui/textinput.py
+-rw-rw-rw-   0        0        0    16624 2024-05-29 08:22:04.000000 uplogic-3.2/uplogic/ui/widget.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:10.697376 uplogic-3.2/uplogic/utils/
+-rw-rw-rw-   0        0        0     7723 2024-05-04 10:43:34.000000 uplogic-3.2/uplogic/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:10.717311 uplogic-3.2/uplogic/utils/__pycache__/
+-rw-rw-rw-   0        0        0     6812 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/utils/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0    11044 2024-05-04 10:44:39.000000 uplogic-3.2/uplogic/utils/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1921 2023-11-09 02:27:46.000000 uplogic-3.2/uplogic/utils/__pycache__/constants.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2874 2024-05-08 14:04:14.000000 uplogic-3.2/uplogic/utils/__pycache__/constants.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1628 2023-05-14 12:11:03.000000 uplogic-3.2/uplogic/utils/__pycache__/errors.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2645 2024-01-02 14:08:23.000000 uplogic-3.2/uplogic/utils/__pycache__/errors.cpython-311.pyc
+-rw-rw-rw-   0        0        0     5009 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/utils/__pycache__/lights.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8721 2024-05-04 08:41:27.000000 uplogic-3.2/uplogic/utils/__pycache__/lights.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9104 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/utils/__pycache__/math.cpython-310.pyc
+-rw-rw-rw-   0        0        0    17041 2024-05-04 10:27:45.000000 uplogic-3.2/uplogic/utils/__pycache__/math.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3248 2023-12-31 14:40:59.000000 uplogic-3.2/uplogic/utils/__pycache__/nodetrees.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6404 2024-01-02 14:08:23.000000 uplogic-3.2/uplogic/utils/__pycache__/nodetrees.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16945 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/utils/__pycache__/objects.cpython-310.pyc
+-rw-rw-rw-   0        0        0    30406 2024-05-09 07:54:24.000000 uplogic-3.2/uplogic/utils/__pycache__/objects.cpython-311.pyc
+-rw-rw-rw-   0        0        0     8705 2023-11-10 06:33:13.000000 uplogic-3.2/uplogic/utils/__pycache__/pooling.cpython-310.pyc
+-rw-rw-rw-   0        0        0    15824 2024-01-02 14:08:23.000000 uplogic-3.2/uplogic/utils/__pycache__/pooling.cpython-311.pyc
+-rw-rw-rw-   0        0        0    12112 2023-10-13 21:24:59.000000 uplogic-3.2/uplogic/utils/__pycache__/raycasting.cpython-310.pyc
+-rw-rw-rw-   0        0        0    18633 2024-01-02 14:08:23.000000 uplogic-3.2/uplogic/utils/__pycache__/raycasting.cpython-311.pyc
+-rw-rw-rw-   0        0        0     5760 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/utils/__pycache__/scene.cpython-310.pyc
+-rw-rw-rw-   0        0        0    12982 2024-03-18 08:06:47.000000 uplogic-3.2/uplogic/utils/__pycache__/scene.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3127 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/utils/__pycache__/visualize.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6696 2024-03-18 13:15:32.000000 uplogic-3.2/uplogic/utils/__pycache__/visualize.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2235 2024-04-29 08:03:33.000000 uplogic-3.2/uplogic/utils/__pycache__/visuals.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4668 2024-03-22 08:50:09.000000 uplogic-3.2/uplogic/utils/__pycache__/visuals.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1642 2024-05-08 14:03:32.000000 uplogic-3.2/uplogic/utils/constants.py
+-rw-rw-rw-   0        0        0     1089 2024-03-22 08:50:05.000000 uplogic-3.2/uplogic/utils/engine.py
+-rw-rw-rw-   0        0        0      854 2022-09-08 15:54:10.000000 uplogic-3.2/uplogic/utils/errors.py
+-rw-rw-rw-   0        0        0     4648 2024-05-04 08:41:23.000000 uplogic-3.2/uplogic/utils/lights.py
+-rw-rw-rw-   0        0        0    11028 2024-05-04 10:27:32.000000 uplogic-3.2/uplogic/utils/math.py
+-rw-rw-rw-   0        0        0     4801 2023-12-31 14:36:53.000000 uplogic-3.2/uplogic/utils/nodetrees.py
+-rw-rw-rw-   0        0        0    16963 2024-05-09 07:54:22.000000 uplogic-3.2/uplogic/utils/objects.py
+-rw-rw-rw-   0        0        0    10075 2023-11-09 14:18:13.000000 uplogic-3.2/uplogic/utils/pooling.py
+-rw-rw-rw-   0        0        0    13778 2023-10-13 21:24:56.000000 uplogic-3.2/uplogic/utils/raycasting.py
+-rw-rw-rw-   0        0        0     6451 2024-03-18 08:04:37.000000 uplogic-3.2/uplogic/utils/scene.py
+-rw-rw-rw-   0        0        0     3528 2024-03-18 12:51:09.000000 uplogic-3.2/uplogic/utils/visualize.py
+-rw-rw-rw-   0        0        0     2553 2024-03-22 08:50:05.000000 uplogic-3.2/uplogic/utils/visuals.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:25:09.400154 uplogic-3.2/uplogic.egg-info/
+-rw-rw-rw-   0        0        0     1045 2024-05-29 08:25:09.000000 uplogic-3.2/uplogic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    84206 2024-05-29 08:25:09.000000 uplogic-3.2/uplogic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 08:25:09.000000 uplogic-3.2/uplogic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-29 08:25:09.000000 uplogic-3.2/uplogic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-29 08:25:09.000000 uplogic-3.2/uplogic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-03-17 18:28:53.000000 uplogic-3.2/uplogic.egg-info/zip-safe
```

### Comparing `uplogic-2.2/PKG-INFO` & `uplogic-3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: uplogic
-Version: 2.2
+Version: 3.2
 Summary: Uplogic utility for UPBGE.
 Home-page: https://github.com/UPBGE/uplogic
 Author: Leopold Auersperg-Castell
 Author-email: lauersperg@gmx.at
 License: GPLv2
-Download-URL: https://github.com/UPBGE/uplogic/archive/refs/tags/v2.2.tar.gz
+Download-URL: https://github.com/UPBGE/uplogic/archive/refs/tags/v3.2.tar.gz
 Keywords: Blender UPBGE logic
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python
 License-File: LICENSE.md
```

### Comparing `uplogic-2.2/setup.py` & `uplogic-3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def read_file(name):
     with open(os.path.join(os.path.dirname(__file__), name)) as f:
         return f.read()
 
 
-version = 'v2.2'
+version = 'v3.2'
 shortdesc = "Uplogic utility for UPBGE."
 longdesc = '\n\n'.join([read_file(name) for name in [
     'README.md',
     'LICENSE.md'
 ]])
 
 
@@ -27,15 +27,15 @@
         'Topic :: Multimedia :: Graphics',
         'Programming Language :: Python',
     ],
     keywords='Blender UPBGE logic',
     author='Leopold Auersperg-Castell',
     author_email='lauersperg@gmx.at',
     url='https://github.com/UPBGE/uplogic',
-    download_url='https://github.com/UPBGE/uplogic/archive/refs/tags/v2.2.tar.gz',
+    download_url='https://github.com/UPBGE/uplogic/archive/refs/tags/v3.2.tar.gz',
     license='GPLv2',
     packages=[
         'uplogic',
         'uplogic.animation',
         'uplogic.audio',
         'uplogic.data',
         'uplogic.decorators',
```

### Comparing `uplogic-2.2/uplogic/__init__.py` & `uplogic-3.2/uplogic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,17 @@
 import bge
 import bpy
 import signal
 import time
 import os, sys
 
 
+__version__ = '3.2'
+
+
 class MainLoop:
     _handles = {}
 
     def __init__(self, max_fps=60, tick_idle=.001):
         self.max_fps = max_fps
         self.tick_idle = tick_idle
         self.time_per_tick = 0.0
```

### Comparing `uplogic-2.2/uplogic/animation/action.py` & `uplogic-3.2/uplogic/animation/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from bge import logic
 from bge.types import KX_GameObject as GameObject
 from random import randint
 from random import random
 from uplogic.animation import ActionSystem
 from uplogic.animation.actionsystem import get_action_system
 from uplogic.events import schedule
+from uplogic.console import warning
 import bpy
 from uplogic.utils.math import clamp
 
 
 PLAY_MODES = {
     'play': logic.KX_ACTION_MODE_PLAY,
     'pingpong': logic.KX_ACTION_MODE_PING_PONG,
@@ -79,15 +80,15 @@
         play_mode: str = 'play',
         speed: float = 1,
         intensity: float = 1,
         blend_mode: str = 'blend',
         keep: bool = False
     ):
         if self._deprecated:
-            print('Warning: ULAction class will be renamed to "Action" in future releases!')
+            warning('Warning: ULAction class will be renamed to "Action" in future releases!')
         self._fps_factor = bpy.context.scene.render.fps / 60
         self._locked = False
         self._speed = speed
         self._frozen_speed = -1
         self.stopped = False
         '''Finish state of the animation.'''
         self.keep = keep
@@ -102,15 +103,16 @@
         '''Starting Frame of the animation.'''
         self.end_frame = end_frame
         '''End Frame of the animation.'''
         self.priority = priority
         '''Priority of this animation; This is only relevant if multiple
         animations are playing on the same layer.'''
         if priority != 0:
-            print("'uplogic.animation.Action' attribute 'priority' is disabled.")
+            from uplogic.console import debug
+            debug("'uplogic.animation.Action' attribute 'priority' is disabled.")
         self.blendin = blendin
         '''The amount of blending frames when starting the animation.'''
         self.layer = layer
         '''The layer the animation is playing on.'''
         self.play_mode = play_mode = PLAY_MODES.get(play_mode, play_mode)
         '''Playback mode of the animation.'''
         self.blend_mode = blend_mode = BLEND_MODES.get(blend_mode, blend_mode)
```

### Comparing `uplogic-2.2/uplogic/animation/actionsystem.py` & `uplogic-3.2/uplogic/animation/actionsystem.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/animation/rig.py` & `uplogic-3.2/uplogic/animation/rig.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/animation/sequence.py` & `uplogic-3.2/uplogic/animation/sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,29 +3,28 @@
 import bpy
 import time
 from bpy.types import ShaderNodeSpritesAnimation
 from bpy.types import ShaderNodeTexImage
 from bpy.types import Material
 
 
-class ULSequence():
-    '''[DEPRECATED] Use `uplogic.animation.Sequence` instead
-
+class Sequence():
+    '''
     Play an image animation through a material node.
 
     :param `material`: Name of the material to play the animation on.
     Each Object with this material applied will play the animation.
     :param `node`: Name of the node the image animation is loaded on.
     :param `start_frame`: Starting frame of the animation.
     :param `end_frame`: End frame of the animation.
     :param `fps`: Frames per second.
     :param `mode`: Animation mode, `str` of [`play`, `loop`, `pingpong`]
     '''
 
-    _deprecated = True
+    _deprecated = False
 
     @property
     def frame(self):
         if self._node_type:
             return self._player.frame_offset
         return round(self._player.inputs[0].default_value)
 
@@ -43,15 +42,16 @@
         node: str,
         start_frame: int,
         end_frame: int,
         fps: int = 60,
         mode: str = 'play'
     ) -> None:
         if self._deprecated:
-            print('Warning: ULSequence class will be renamed to "ULSequence" in future releases!')
+            from uplogic.console import warning
+            warning('Warning: ULSequence class will be renamed to "ULSequence" in future releases!')
 
         self.material = bpy.data.materials[material]
         """The material this sequence is played on."""
         self.node = node
         """Name of the node the image animation is loaded on."""
         self.start_frame = start_frame
         """Starting frame of the animation."""
@@ -179,19 +179,22 @@
             self.frame = end_frame if inverted else start_frame
         elif play_mode == 2:
             self._reverse = not self._reverse
         else:
             self.stop()
 
 
-class Sequence(ULSequence):
-    '''Play an image animation through a material node.
+class ULSequence(Sequence):
+
+    '''[DEPRECATED] Use `uplogic.animation.Sequence` instead
+
+    Play an image animation through a material node.
 
     :param `material`: Name of the material to play the animation on.
     Each Object with this material applied will play the animation.
     :param `node`: Name of the node the image animation is loaded on.
     :param `start_frame`: Starting frame of the animation.
     :param `end_frame`: End frame of the animation.
     :param `fps`: Frames per second.
     :param `mode`: Animation mode, `str` of [`play`, `loop`, `pingpong`]
     '''
-    _deprecated = False
+    _deprecated = True
```

### Comparing `uplogic-2.2/uplogic/audio/__init__.py` & `uplogic-3.2/uplogic/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/audio/audiosystem.py` & `uplogic-3.2/uplogic/audio/audiosystem.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/audio/music.py` & `uplogic-3.2/uplogic/audio/music.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,29 +42,29 @@
         if self._fade_event:
             self._fade_event.cancel()
             self._fade_event = None
         if self.volume < 1:
             self._fade_event = schedule_callback(self.fade_in, arg=factor)
 
 
-class ULMusic(ULMusicEffect):
-    '''[DEPRECATED] Use `uplogic.audio.Music` instead
-
+class Music(ULMusicEffect):
+    '''
     Management class for controlling multiple music tracks.
 
     :param `name`: Name of this music.'''
-    _deprecated = True
+    _deprecated = False
 
     def __init__(
         self,
         name: str = '',
         audio_system: str = 'music'
     ):
         if self._deprecated:
-            print('Warning: ULMusic class will be renamed to "Music" in future releases!')
+            from uplogic.console import warning
+            warning('Warning: ULMusic class will be renamed to "Music" in future releases!')
         super().__init__()
         self.name = name if name else uuid4()
         self.audio_system = get_audio_system(audio_system, '2D')
         self.tracks: list[ULMusicTrack] = []
 
     @property
     def position(self):
@@ -160,36 +160,38 @@
     def stop(self):
         '''Stop this music (all tracks).'''
         for track in self.tracks:
             track.sound.stop()
         self.position = 0.0
 
 
-class Music(ULMusic):
-    _deprecated = False
+class ULMusic(Music):
+    """[DEPRECATED] Use `uplogic.audio.Music` instead"""
 
+    _deprecated = True
 
-class ULMusicTrack(ULMusicEffect):
-    '''[DEPRECATED] Use `uplogic.audio.MusicTrack` instead
 
-    Track to be played on a `ULMusic` instance.
+class MusicTrack(ULMusicEffect):
+    '''
+    Track to be played on a `Music` instance.
     
     :param `music`: The music object this track will be played on.
     :param `sound`: Path to the soundfile of this track.
     :param `name`: Name of this track (e.g. "Drums).'''
-    _deprecated = True
+    _deprecated = False
 
     def __init__(
         self,
         music: Music,
         sound: str or Sound2D,
         name: str
     ):
         if self._deprecated:
-            print('Warning: ULMusic class will be renamed to "Music" in future releases!')
+            from uplogic.console import warning
+            warning('Warning: ULMusic class will be renamed to "Music" in future releases!')
         super().__init__()
         self.music = music
         self.name = name
         sound = Sound2D(
             sound,
             aud_sys=self.music.audio_system
         ) if isinstance(sound, str) else sound
@@ -230,9 +232,9 @@
 
     def remove(self):
         '''Stop and remove this track from its `ULMusic` object.'''
         self.sound.stop()
         self.music.tracks.remove(self)
 
 
-class MusicTrack(ULMusicTrack):
-    _deprecated = False
+class ULMusicTrack(MusicTrack):
+    _deprecated = True
```

### Comparing `uplogic-2.2/uplogic/audio/sound.py` & `uplogic-3.2/uplogic/audio/sound.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from bge import logic
 from bge.types import KX_GameObject as GameObject
 from mathutils import Vector
 from uplogic.audio import ULAudioSystem
 from uplogic.audio import get_audio_system
 from uplogic.events import schedule_callback
 from uplogic.utils.math import interpolate
+from uplogic.console import warning
 from uplogic.utils import DELTA_TIME
 import bpy
 import aud
 
 
 class ULReverb():
     """Reverb sound added by `Sound3D` on demand.
@@ -142,41 +143,40 @@
     def resume(self):
         self.sound.resume()
     
     def on_finish(self):
         pass
 
 
-class ULSound2D(ULSound):
-    '''[DEPRECATED] Use `uplogic.audio.Sound2D` instead
-    
+class Sound2D(ULSound):
+    '''
     Non-spacial sound, e.g. Music or Voice-Overs.\n
     This class allows for modification of pitch and volume while playing.
 
     :param `file`: Path to the sound file.
     :param `volume`: Initial volume.
     :param `pitch`: Initial pitch.
     :param `loop_count`: Plays the sound this many times (0 for once, -1 for endless).
     :param `aud_sys`: Audiosystem to play this sound on.
     '''
 
-    _deprecated = True
+    _deprecated = False
 
     def __init__(
         self,
         file: str = '',
         volume: float = 1,
         pitch: float = 1,
         loop_count: int = 0,
         lowpass = False,
         ignore_timescale = True,
         aud_sys: str = 'default'
     ):
         if self._deprecated:
-            print('Warning: ULSound2D class will be renamed to "Sound2D" in future releases!')
+            warning('Warning: ULSound2D class will be renamed to "Sound2D" in future releases!')
         self.file = file
         self._volume = 1
         self.finished = False
         if not (file):
             return
         self.aud_system = get_audio_system(aud_sys)
         soundfile = logic.expandPath(file)
@@ -251,27 +251,28 @@
         if not handle.status:
             self.finished = True
             self.on_finish()
             self.aud_system.remove(self)
             return
 
 
-class Sound2D(ULSound2D):
-    '''
+class ULSound2D(Sound2D):
+    '''[DEPRECATED] Use `uplogic.audio.Sound2D` instead
+
     Non-spacial sound, e.g. Music or Voice-Overs.\n
     This class allows for modification of pitch and volume while playing.
 
     :param `file`: Path to the sound file.
     :param `volume`: Initial volume.
     :param `pitch`: Initial pitch.
     :param `loop_count`: Plays the sound this many times (0 for once, -1 for endless).
     :param `aud_sys`: Audiosystem to play this sound on.
     '''
 
-    _deprecated = False
+    _deprecated = True
 
 
 class Sample2D(Sound2D):
     '''Non-spacial sample, e.g. Music or Voice-Overs.\n
     This class allows for modification of pitch and volume while playing.
     The played audio file can be limited to a start and end time.
 
@@ -321,20 +322,20 @@
         self.aud_system.add(self)
         self.volume = volume
         self.pitch = pitch
         self._lowpass = False
         self.lowpass = self.aud_system.lowpass
 
 
-class ULSound3D(ULSound):
+class Sound3D(ULSound):
     '''Spacial sound, e.g. World Effects or Voices.\n
     This class allows for modification of pitch and volume as well as other attributes while playing.
     '''
 
-    _deprecated = True
+    _deprecated = False
 
     @property
     def position(self):
         if self.handles:
             return self.handles[1][0].position
 
     @position.setter
@@ -357,15 +358,15 @@
         distance_ref: float = 1,
         cone_angle: list[float] = [360, 360],
         cone_outer_volume: float = 0,
         ignore_timescale: bool = False,
         aud_sys: str = 'default'
     ):
         if self._deprecated:
-            print('Warning: ULSound3D class will be renamed to "Sound3D" in future releases!')
+            warning('Warning: ULSound3D class will be renamed to "Sound3D" in future releases!')
         self._is_vector = isinstance(speaker, Vector)
         self.file = file
         self.finished = False
         if not (file and speaker):
             return
         self._clear_sound = 0 if occlusion else 1
         self._sustained = 1
@@ -552,16 +553,16 @@
         '''TODO: Documentation
         '''
         self.on_finish = dummy
         for sound in self.handles[1]:
             sound.stop()
 
 
-class Sound3D(ULSound3D):
-    _deprecated = False
+class ULSound3D(Sound3D):
+    _deprecated = True
 
 
 class Sample3D(Sound3D):
     '''Spacial sound, e.g. World Effects or Voices.\n
     This class allows for modification of pitch and volume as well as other attributes while playing.
     '''
 
@@ -649,62 +650,62 @@
                 sound,
                 self.handles[1][0]
             )
         self.aud_system.add(self)
         self.update(True)
 
 
-class ULSpeaker2D(ULSound2D):
+class Speaker2D(Sound2D):
 
-    _deprecated = True
+    _deprecated = False
 
     def __init__(
         self,
         speaker: GameObject,
         loop_count: int = 0,
         lowpass=False,
         ignore_timescale: bool = False,
         aud_sys: str = 'default'
     ):
         if self._deprecated:
-            print('Warning: ULSpeaker2D class will be renamed to "Speaker2D" in future releases!')
+            warning('Warning: ULSpeaker2D class will be renamed to "Speaker2D" in future releases!')
         speaker_data = speaker.blenderObject.data
         # ULSound2D()
         super().__init__(
             speaker_data.sound.filepath,
             speaker_data.volume,
             speaker_data.pitch,
             loop_count,
             lowpass,
             ignore_timescale=
             aud_sys
         )
 
 
-class Speaker2D(ULSpeaker2D):
-    _deprecated = False
+class ULSpeaker2D(Speaker2D):
+    _deprecated = True
 
 
-class ULSpeaker3D(ULSound3D):
+class Speaker3D(Sound3D):
 
-    _deprecated = True
+    _deprecated = False
 
     def __init__(
         self,
         speaker: GameObject,
         occlusion: bool = False,
         transition_speed: float = 0.1,
         cutoff_frequency: float = 0.1,
         loop_count: int = 0,
         reverb=False,
         ignore_timescale: bool = False,
         aud_sys: str = 'default'
     ):
         if self._deprecated:
-            print('Warning: ULSpeaker3D class will be renamed to "Speaker3D" in future releases!')
+            warning('Warning: ULSpeaker3D class will be renamed to "Speaker3D" in future releases!')
         speaker_data = speaker.blenderObject.data
         super().__init__(
             speaker,
             speaker_data.sound.filepath,
             occlusion,
             transition_speed,
             cutoff_frequency,
@@ -717,9 +718,9 @@
             [speaker_data.cone_angle_inner, speaker_data.cone_angle_outer],
             speaker_data.cone_volume_outer,
             ignore_timescale,
             aud_sys
         )
 
 
-class Speaker3D(ULSpeaker3D):
-    _deprecated = False
+class ULSpeaker3D(Speaker3D):
+    _deprecated = True
```

### Comparing `uplogic-2.2/uplogic/console/__init__.py` & `uplogic-3.2/uplogic/console/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,41 +4,41 @@
 from uplogic.ui.layout import RelativeLayout
 from uplogic.ui.label import Label
 from uplogic.ui.textinput import TextInput
 from uplogic.data import GlobalDB
 from uplogic.utils.raycasting import raycast_mouse
 from uplogic.utils.math import world_to_screen
 from uplogic.utils.math import cycle
+from uplogic.utils.math import clamp
 from uplogic.input import key_down, mouse_down, key_pulse, mouse_wheel
-import bpy
-import sys
+import bpy, blf
+import sys, os
 from datetime import datetime
 from mathutils import Vector
+import uplogic
 
 
 GLOBALS = {}
 
 
-def set_depth(depth):
-    ConsoleLayout.max_msg = depth
-
-
 def set_global(key, val):
     global GLOBALS
     GLOBALS[key] = val
 
 
 def _get_globals():
     scene = logic.getCurrentScene()
     global GLOBALS
     GLOBALS['scene'] = scene
     GLOBALS['bpy'] = bpy
     GLOBALS['bge'] = bge
+    GLOBALS['uplogic'] = uplogic
     GLOBALS['logic'] = logic
     GLOBALS['render'] = render
+    GLOBALS['console'] = get_console()
     for obj in scene.objects:
         GLOBALS[obj.blenderObject.name] = obj
     return GLOBALS
 
 
 def enable(toggle_key='F12', visible=False):
     get_console(True, toggle_key=toggle_key, visible=visible)
@@ -52,216 +52,322 @@
     console = get_console()
     if console:
         console.stop()
 
 
 class Console(StringIO):
 
-    # def writelines(self, __lines: Iterable[str]) -> None:
-    #     log(__lines, newline=False)
-
     def write(self, __s: str) -> int:
         log(__s)
-        sys.__stdout__.write(__s)
+        # sys.__stdout__.write(__s)
 
 
 class ErrorConsole(StringIO):
     def write(self, __s: str) -> int:
         error(__s)
-        # sys.__stderr__.write(__s)
 
+COLORS = {
+    'INFO': [1, 1, 1, 1],
+    'DEBUG': [1, 1, .6, 1],
+    'WARNING': [1, .8, .2, 1],
+    'ERROR': [1, .3, .3, 1],
+    'SUCCESS': [.3, 1, .3, 1]
+}
 
 class ConsoleLayout(Canvas):
-    colors = {
-        'INFO': [1, 1, 1, 1],
-        'DEBUG': [1, 1, .6, 1],
-        'WARNING': [1, 1, .3, 1],
-        'ERROR': [1, .3, .3, 1],
-        'SUCCESS': [.3, 1, .3, 1]
-    }
-    max_msg = 50
     opacity = 1
     padding = [5, 10]
     toggle_key = 'F12'
 
     def __init__(self, toggle_key='F12', visible=False):
         scene = logic.getCurrentScene()
         self.toggle_key = toggle_key
+        self._mouse_visible = False
+        self.issued_commands = []
         self._mouse_down = False
-        self._goback_index = 1
+        self._goback_index = -1
         super().__init__()
         if not getattr(bpy.context.scene, 'screen_console_open', False) and not visible:
             self.show = False
         self.input = TextInput(text='', shadow=True, valign='center')
         self.input.on_enter = self.on_enter
         self.input.edit = True
-        self.layout = RelativeLayout(relative={'size': True, 'pos': True}, pos=[0, 0], size=(1, .4), bg_color=[0, 0, 0, .3])
+        self.layout = RelativeLayout(relative={'size': True, 'pos': True}, pos=[0, 0], size=(1, .4), bg_color=[0, 0, 0, .4])
         self.layout.use_clipping = True
         self.add_widget(self.layout)
         self.layout.add_widget(self.input)
         self.fade_event = None
         self._toggle_key = False
         self._prev_msg = None
         if disable not in scene.onRemove:
             scene.onRemove.append(disable)
         if self.update not in scene.pre_draw:
             scene.pre_draw.append(self.update)
         self.nameplate = Label(text='', shadow=True, relative={'pos': True}, halign='center', font_size=13)
         self.nameplate.update = self.update_nameplate
         self.canvas.add_widget(self.nameplate)
+        self.font_size = 14
+        self.position = 'bottom'
+
+    @property
+    def position(self):
+        return self._position
+
+    @position.setter
+    def position(self, val):
+        if val == 'center':
+            self.layout.valign = val
+            self.layout.halign = val
+            self.layout.pos = (.5, .5)
+            self.layout.size = (.4, .4)
+            self._position = val
+        elif val == 'left':
+            self.layout.valign = 'bottom'
+            self.layout.halign = val
+            self.layout.size = (.4, 1)
+            self.layout.pos = (0, 0)
+            self._position = val
+        elif val == 'right':
+            self.layout.valign = 'bottom'
+            self.layout.halign = val
+            self.layout.pos = (1, 0)
+            self.layout.size = (.4, 1)
+            self._position = val
+        elif val == 'top':
+            self.layout.valign = 'top'
+            self.layout.halign = 'left'
+            self.layout.pos = (0, 1)
+            self.layout.size = (1, .4)
+            self._position = val
+        elif val == 'bottom':
+            self.layout.valign = 'bottom'
+            self.layout.halign = 'left'
+            self.layout.pos = (0, 0)
+            self.layout.size = (1, .4)
+            self._position = val
+        else:
+            error(f'"{val}" not recognized.')
+        self.arrange()
+
+    @property
+    def font_size(self):
+        return self._font_size
+
+    @font_size.setter
+    def font_size(self, val):
+        val = clamp(val, 5, 30)
+        self._font_size = int(val)
+        for c in self.layout.children:
+            c.font_size = int(val)
+        self.nameplate.font_size = int(val)
+        self.arrange()
 
     def on_enter(self):
+        self.issued_commands.append(self.input.text)
+        sys.__stdout__.write(f'{self.input.text}\n')
         self.add_message(self.input.text)
         command_name = self.input.text.split(' ')[0]
         command = Commands.commands.get(command_name)
         if command:
             command.invoke(self.input.text)
         else:
             try:
                 exec(self.input.text, _get_globals())
             except Exception as e:
-                error(f'Error occured when executing command "{command_name}":')
-                error(e)
-        self._goback_index = 0
+                error(f'Error occured when executing command "{command_name}":\n{e}')
+        self._goback_index = -1
         self.input.text = ''
+        self.input.edit = True
 
     def update_nameplate(self):
         ray = raycast_mouse()
         mdown = mouse_down()
         if ray.obj:
             self.nameplate.pos = world_to_screen(ray.point) + Vector((0, .01))
             self.nameplate.text = ray.obj.blenderObject.name
             if mdown and not self._mouse_down:
                 self.input.write(self.nameplate.text)
         else:
             self.nameplate.text = ''
         self._mouse_down = mdown
 
     def update(self):
-        if key_pulse('DOWNARROW'):
-            self.input.text = ''
-        if key_pulse('UPARROW'):
-            if not self._toggle_key:
-                line = self.layout.children[self._goback_index]
-                self.input.text = line.text[13:] if line is not self.input else ''
-                self._goback_index = cycle(self._goback_index + 1, 0, len(self.layout.children) - 1)
-            self._toggle_key = True
-        elif key_down(self.toggle_key):
+        if self.input.edit != self.show:
+            self.input.edit = self.show
+        move_goback = key_pulse('UPARROW') - key_pulse('DOWNARROW')
+        if key_down(self.toggle_key):
+            if not self.show:
+                self._mouse_visible = logic.mouse.visible
             if not self._toggle_key:
                 self.show = not self.show
                 self.opacity = 1
             self._toggle_key = True
+        elif not self.show:
+            self._toggle_key = False
+            return
+        elif move_goback:
+            if not self.issued_commands:
+                pass
+            elif not self._toggle_key:
+                self._goback_index = clamp(self._goback_index + move_goback, -1, len(self.issued_commands) - 1)
+                if self._goback_index < 0:
+                    self.input.text = ''
+                else:
+                    self.input.text = list(self.issued_commands.__reversed__())[self._goback_index]
+                self.input.move_cursor_to_end()
+            self._toggle_key = True
         else:
             self._toggle_key = False
-        logic.mouse.visible = self.show
+        logic.mouse.visible = self.show or self._mouse_visible
 
     def stop(self):
         self.clear()
         scene = logic.getCurrentScene()
         if self.toggle in scene.pre_draw:
             scene.pre_draw.remove(self.toggle)
 
     def add_message(self, msg, type='INFO', time=True):
         if (msg == ' ' or self._prev_msg == ' ') and len(self.layout.children):
             self.layout.children[-1].text += msg
             self._prev_msg = msg
             return
-        if len(self.layout.children) > self.max_msg -1:
-            self.layout.remove_widget(self.layout.children[0])
         now = datetime.now()
-        current_time = f'[{now.strftime("%H:%M:%S")}]' if time else "\t\t\t\t\t\t".replace('\t', '    ')
-        self.layout.add_widget(Label(text=f'>{current_time}  {msg}', pos=[5, 10], font_color=self.colors[type], shadow=True))
-        dim = self.layout.children[0].dimensions[1]
+        current_time = f'[{now.strftime("%H:%M:%S")}]' if time else "\t\t\t\t  ".replace('\t', '    ')
+        self.layout.add_widget(Label(text=f'{current_time}  {msg}', pos=[5, 10], font_color=COLORS[type], shadow=True, font_size=self.font_size))
+        self._prev_msg = msg
+        self.arrange()
+
+    def arrange(self):
+        blf.size(0, self.font_size)
+        dim = blf.dimensions(0, 'A')
+        cheight = dim[1]
+        cwidth = dim[0]
         lheight = self.layout._draw_size[1]
-        amount = lheight / dim
-        y = 40
+        amount = lheight / cheight
+        y = cheight * 2.4 * 1.5
         for i, child in enumerate(self.layout._children_reversed):
             if child is self.input:
                 continue
             child.pos[1] = y
-            y+=15
-            if child.pos[1] > lheight - dim:
+            y += cheight * 1.5
+            if child.pos[1] > lheight - cheight:
                 self.layout.remove_widget(child)
             child.opacity = 1 - (i * (1/amount))
             child.shadow_color[3] = child.font_color[3]
-        self.input.pos[1] = 20
-        self.input.pos[0] = 5
-        self._prev_msg = msg
+        self.input.pos[1] = self.font_size + 3
+        self.input.pos[0] = cwidth
 
 
 def get_console(create=False, toggle_key='F12', visible=False) -> ConsoleLayout:
     consoles = GlobalDB.retrieve('uplogic.consoles')
     console = consoles.get('default')
     if console is None and create:
         console = ConsoleLayout(toggle_key=toggle_key, visible=visible)
         consoles.put('default', console)
     return console
 
 
+class ansicol:
+    RED = '\033[31m\033[1m'
+    GREEN = '\033[32m\033[1m'
+    YELLOW = '\033[33m'
+    BYELLOW = '\033[93m'
+    BBLUE = '\033[36m'
+    END = '\033[0m'
+
+
+def write(msg, type):
+    _f = {
+        'INFO': log,
+        'DEBUG': debug,
+        'WARNING': warning,
+        'ERROR': error,
+        'SUCCESS': success
+    }
+
+    _f[type](msg)
+
+
 def log(msg, type='INFO'):
     console = get_console()
+
     if console is None:
         print(msg)
         return
     show_time = True
     for msg in str(msg).split('\n'):
         if msg:
             msg = msg.replace('  ', '    ')
             console.add_message(f'{msg}', type, time=show_time)
             show_time = False
+            sys.__stdout__.write(f'{msg}\n')
 
 
 def warning(msg):
     console = get_console()
+    sysmsg = f'{ansicol.YELLOW}Warning{ansicol.END}: {msg}'
     if console is None:
-        print(msg)
+        print(sysmsg)
         return
+    show_time = True
     for msg in str(msg).split('\n'):
         if msg:
             msg.replace('  ', '    ')
-            console.add_message(f'WARNING:\t{msg}', 'WARNING')
+            console.add_message(f'{msg}', 'WARNING', time=show_time)
+            show_time = False
+            sys.__stdout__.write(f'{sysmsg}\n')
 
 
 def error(msg):
     console = get_console()
+    sysmsg = f'{ansicol.RED}Error{ansicol.END}: {msg}'
     if console is None:
-        print(msg)
+        print(sysmsg)
+        # print(msg)
         return
+    show_time = True
     for msg in str(msg).split('\n'):
         if msg:
             msg.replace('  ', '    ')
-            console.add_message(f'{msg}', 'ERROR')
-            sys.__stdout__.write(f'{msg}\n')
+            console.add_message(f'{msg}', 'ERROR', time=show_time)
+            sys.__stdout__.write(f'{sysmsg}\n')
+            show_time = False
 
 
 def success(msg):
     console = get_console()
+    sysmsg = f'{ansicol.GREEN}Success{ansicol.END}: {msg}'
     if console is None:
-        print(msg)
+        print(sysmsg)
         return
+    show_time = True
     for msg in str(msg).split('\n'):
         if msg:
             msg.replace('  ', '    ')
-            console.add_message(f'{msg}', 'SUCCESS')
-            sys.__stdout__.write(f'{msg}\n')
+            console.add_message(f'{msg}', 'SUCCESS', time=show_time)
+            sys.__stdout__.write(f'{sysmsg}\n')
+            show_time = False
 
 
 def debug(msg):
     console = get_console()
+    sysmsg = f'{ansicol.BYELLOW}Debug{ansicol.END}: {msg}'
     if console is None:
-        print(msg)
+        print(sysmsg)
         return
+    show_time = True
     for msg in str(msg).split('\n'):
         if msg:
             msg.replace('  ', '    ')
-            console.add_message(f'{msg}', 'DEBUG')
-            sys.__stdout__.write(f'{msg}\n')
+            console.add_message(f'{msg}', 'DEBUG', time=show_time)
+            sys.__stdout__.write(f'{sysmsg}\n')
+            show_time = False
 
 nodeprefs = bpy.context.preferences.addons.get('bge_netlogic', None)
-if nodeprefs and getattr(bpy.context.scene, 'use_screen_console', False):
+if nodeprefs and getattr(bpy.context.scene, 'use_screen_console', True):
     enable(toggle_key='F12')
 
 
 import bpy
 import bge
 
 
@@ -433,16 +539,30 @@
 @console_command
 class HelpCommand(Command):
     command = 'help'
     description = 'Print out all available commands.'
 
     @classmethod
     def execute(cls, args):
-        print('Available Commands:')
         mode = None
+        msg = 'Available Commands:'
         if len(args) > 0:
             mode = args[0]
         for command in Commands.commands.values():
             if mode == '-d':
-                print(f' -  "{command.command} {command.usage}"    -    {command.description}')
+                msg += f'\n -  "{command.command} {command.usage}"    -    {command.description}'
             else:
-                print(f' -  "{command.command} {command.usage}"')
+                msg += f'\n -  "{command.command} {command.usage}"'
+        print(msg)
+
+
+@console_command
+class FontSizeCommand(Command):
+    command = 'fontsize'
+    arg_count = 1
+    usage = 'PX_SIZE'
+    description = 'Modify the font size of the console.'
+
+    @classmethod
+    def execute(cls, args):
+        size = args[0]
+        get_console().font_size = int(size)
```

### Comparing `uplogic-2.2/uplogic/data/__init__.py` & `uplogic-3.2/uplogic/data/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/data/file.py` & `uplogic-3.2/uplogic/data/file.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/data/globaldb.py` & `uplogic-3.2/uplogic/data/globaldb.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/data/serializers.py` & `uplogic-3.2/uplogic/data/serializers.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/decorators/__init__.py` & `uplogic-3.2/uplogic/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/events/__init__.py` & `uplogic-3.2/uplogic/events/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,29 @@
     EventManager.update_on.append(callback)
 
 
 def on_post_draw(callback):
     EventManager.update_on.append(callback)
 
 
+class _DeferredCallback():
+
+    def __init__(self, callback) -> None:
+        self.callback = callback
+        logic.getCurrentScene().post_draw.append(self._call)
+
+    def _call(self):
+        self.callback()
+        logic.getCurrentScene().post_draw.remove(self._call)
+
+
+def later(callback):
+    _DeferredCallback(callback)
+
+
 def get_event_manager():
     update = EventManager.update_on
     if update is None:
         update = logic.getCurrentScene().post_draw
     if EventManager.update not in update:
         update.append(EventManager.update)
     return EventManager
@@ -172,15 +187,15 @@
 def bind(id: int, callback) -> None:
     '''Bind a callback to an event.
 
     :param `id`: Name of the event; can be anything, not just `str`.
     :param `callback`: This callback will be called every time the event is
     triggered.
     '''
-    class BoundCallback():
+    class _BoundCallback():
         def __init__(self, id, cb) -> None:
             self.id = id
             self.callback = cb
             EventManager.bind(self._check_evt)
 
         def _check_evt(self):
             evt = receive(self.id)
@@ -189,18 +204,18 @@
 
         def unbind(self):
             EventManager.unbind(self._check_evt)
 
         def release(self):
             EventManager.unbind(self._check_evt)
 
-    return BoundCallback(id, callback)
+    return _BoundCallback(id, callback)
 
 
-class ScheduledEvent():
+class _ScheduledEvent():
     '''Event generated by `uplogic.events.schedule()`.
 
     :param `delay`: Delay with which to send the event in seconds.
     :param `id`: Identifier of the event; can be anything, not just `str`
     :param `content`: This can be used to store data in an event.
     :param `messenger`: Can be used to store an object.
     '''
@@ -225,28 +240,28 @@
         if self._consumed:
             return
         self._consumed = True
         EventManager.cancel(self._send_scheduled)
         ULEvent(self.id, self.content, self.messenger)
 
 
-def schedule(id: str, delay=0.0, content=None, messenger=None) -> ScheduledEvent:
+def schedule(id: str, delay=0.0, content=None, messenger=None) -> _ScheduledEvent:
     '''Send an event that can be reacted to with a delay.
 
     :param `id`: Name of the event; can be anything, not just `str`. If `id` is callable, `content` can be used as argument.
     :param `content`: This can be used to store data in an event.
     :param `messenger`: Can be used to store an object.
     :param `delay`: Delay with which to send the event in seconds.
     '''
     if callable(id):
-        return ScheduledCallback(id, delay, content)
-    return ScheduledEvent(delay, id, content, messenger)
+        return _ScheduledCallback(id, delay, content)
+    return _ScheduledEvent(delay, id, content, messenger)
 
 
-class ScheduledCallback():
+class _ScheduledCallback():
     '''Event generated by `uplogic.events.schedule_callback()`.
 
     **Not intended for manual use.**
 
     :param `cb`: Callback to be evaluated.
     :param `delay`: Delay with which to call the function in seconds.
     :param `arg`: If this is defined, callback will be called with this
@@ -275,19 +290,19 @@
         else:
             self.callback()
 
     def cancel(self):
         EventManager.cancel(self._call_scheduled)
 
 
-def schedule_callback(cb, delay=0.0, arg=None) -> ScheduledCallback:
+def schedule_callback(cb, delay=0.0, arg=None) -> _ScheduledCallback:
     '''Call a function with a delay. The function can have an argument when
     defined as a keyword.
 
     Callback cannot return anything.
 
     :param `cb`: Callback to be evaluated.
     :param `delay`: Delay with which to call the function in seconds.
     :param `arg`: If this is defined, callback will be called with this
     argument.
     '''
-    return ScheduledCallback(cb, delay, arg)
+    return _ScheduledCallback(cb, delay, arg)
```

### Comparing `uplogic-2.2/uplogic/input/__init__.py` & `uplogic-3.2/uplogic/input/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/input/gamepad.py` & `uplogic-3.2/uplogic/input/gamepad.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,15 +273,16 @@
 
     def __init__(
         self,
         idx: int = 0,
         layout: dict = XBOX
     ) -> None:
         if self._deprecated:
-            print('Warning: ULGamePad class will be renamed to "Gamepad" in future releases!')
+            from uplogic.console import warning
+            warning('Warning: ULGamePad class will be renamed to "Gamepad" in future releases!')
         self.idx = idx
         self.layout = layout
         if not logic.joysticks[idx]:
             print(f'No Joystick found at index: {idx}')
         self.device = logic.joysticks[idx]
 
     def button_down(self, button: str):
@@ -310,15 +311,15 @@
         self.rumble(strength, time)
 
 
 class ULGamePad(Gamepad):
     _deprecated = True
 
 
-class ULGamepadLook():
+class GamepadLook():
     """Automatically track the mouse movement and translate it to a rotate a
     body and optionally a head.
 
     This component can be activated/deactivated at any time to keep performance
     up.
     
     :param `obj`: Main object to rotate around the object's Z axis.
@@ -333,15 +334,15 @@
     :param `invert`: Whether to use inverted values for mous X/Y movement.
     :param `smoothing`: Amount of movement smoothing.
     :param `local`: Whether to use local transform for the body object.
     :param `front`: Front axis (traditionally in blender, Y is front).
     :param `active`: Whether to start this component in active or inactive mode
     (can be changed later).
     """
-    _deprecated = True
+    _deprecated = False
     def __init__(
         self,
         obj: GameObject,
         head: GameObject = None,
         sensitivity: float = .05,
         use_cap_x: bool = False,
         cap_x: tuple = (0, 0),
@@ -354,15 +355,16 @@
         idx: int = 0,
         stick: int = 'RS',
         threshold: float = 0.07,
         exponent: float = 2.3,
         active=True
     ) -> None:
         if self._deprecated:
-            print('Warning: ULGamepadLook class will be renamed to "GamepadLook" in future releases!')
+            from uplogic.console import warning
+            warning('Warning: ULGamepadLook class will be renamed to "GamepadLook" in future releases!')
         self.obj = obj
         self.head = head if head else obj
         self._defaults = [
             obj.localOrientation.copy(),
             head.localOrientation.copy()
             if head else
             obj.localOrientation.copy()]
@@ -508,16 +510,16 @@
 
         rot = [0, 0, 0]
         rot[1-self.front] = y
         game_object_y.applyRotation((*rot, ), True)
         self.done = True
 
 
-class GamepadLook(ULGamepadLook):
-    _deprecated = False
+class ULGamepadLook(GamepadLook):
+    _deprecated = True
 
 
 def gamepad_active(idx) -> bool:
     if logic.joysticks[idx]:
         joystick = logic.joysticks[idx]
     else:
         return False
```

### Comparing `uplogic-2.2/uplogic/input/keyboard.py` & `uplogic-3.2/uplogic/input/keyboard.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/input/mouse.py` & `uplogic-3.2/uplogic/input/mouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,22 +146,23 @@
             ) - (
                 MOUSE_EVENTS[events.WHEELDOWNMOUSE].activated or
                 MOUSE_EVENTS[events.WHEELDOWNMOUSE].active
             )
         )
 
 
-class ULMouse():
+class Mouse():
     """Mouse Wrapper for accessing mouse data."""
 
-    _deprecated = True
+    _deprecated = False
 
     def __init__(self) -> None:
         if self._deprecated:
-            print('Warning: ULMouse class will be renamed to "Mouse" in future releases!')
+            from uplogic.console import warning
+            warning('Warning: ULMouse class will be renamed to "Mouse" in future releases!')
         self._position = get_mouse_position()
         """Staggered updated mouse position for pos difference calculation."""
         self.movement = (0, 0)
         """Movement of the mouse as a tuple `(x, y)`."""
         self.active = True
 
     @property
@@ -239,21 +240,22 @@
         """Check if a button on the mouse is pressed once.
         
         :param `button`: The button to check for; `str` of [`'LMB'`, `'MMB'`,
         `'RMB'`]"""
         return mouse_tap(MOUSE_BUTTONS[button])
 
 
-class Mouse(ULMouse):
-    _deprecated = False
+class ULMouse(Mouse):
+    _deprecated = True
+
 
 MOUSE = Mouse()
 
 
-class ULMouseLook():
+class MouseLook():
     """Automatically track the mouse movement and translate it to a rotate a
     body and optionally a head.
 
     This component can be activated/deactivated at any time to keep performance
     up.
 
     :param `obj`: Main object to rotate around the object's Z axis.
@@ -269,15 +271,15 @@
     :param `smoothing`: Amount of movement smoothing.
     :param `local`: Whether to use local transform for the body object.
     :param `front`: Front axis (traditionally in blender, Y is front).
     :param `active`: Whether to start this component in active or inactive mode
     (can be changed later).
     """
 
-    _deprecated = True
+    _deprecated = False
 
     def __init__(
         self,
         obj: GameObject,
         head: GameObject = None,
         sensitivity: float = 1.0,
         use_cap_x: bool = False,
@@ -288,15 +290,16 @@
         smoothing: float = 0.0,
         local: bool = True,
         front: int = 1,
         center_mouse: bool = True,
         active: bool = True,
     ) -> None:
         if self._deprecated:
-            print('Warning: ULMouseLook class will be renamed to "MouseLook" in future releases!')
+            from uplogic.console import warning
+            warning('Warning: ULMouseLook class will be renamed to "MouseLook" in future releases!')
         self.obj = obj
         self.head = head if head else obj
         self._defaults = [
             obj.localOrientation.copy(),
             head.localOrientation.copy()
             if head else
             obj.localOrientation.copy()
@@ -467,9 +470,9 @@
             game_object_y.applyRotation((*rot, ), True)
         if self.center_mouse and (Vector(self.mouse.position) - Vector(self.screen_center)).length > .00001:
             self.mouse.position = self.screen_center
         self._old_mouse_pos = self.mouse.position
         self.done = True
 
 
-class MouseLook(ULMouseLook):
-    _deprecated = False
+class ULMouseLook(MouseLook):
+    _deprecated = True
```

### Comparing `uplogic-2.2/uplogic/input/vr.py` & `uplogic-3.2/uplogic/input/vr.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,93 +14,94 @@
     """
     session = bpy.context.window_manager.xr_session_state
     if not session:
         raise NoXRSessionError
     return (Vector(session.viewer_pose_location), Quaternion(session.viewer_pose_rotation).to_matrix())
 
 
-class ULControllerVR():
+class VRController():
     """Wrapper class for VR Controllers.
 
     This wrapper provides `position`, `position_aim`, `orientation`,
     `orientation_aim`, `trigger` and `thumbstick` attributes.
 
     :param `idx`: Controller index; 0 for left, 1 for right controller.
     """
 
-    _deprecated = True
+    _deprecated = False
 
     def __init__(self, idx: int=0) -> None:
         if self._deprecated:
-            print('Warning: ULControllerVR class will be renamed to "VRController" in future releases!')
+            from uplogic.console import warning
+            warning('Warning: ULControllerVR class will be renamed to "VRController" in future releases!')
         self.idx = idx
         self.stick_threshold = 0.0
         self.session = bpy.context.window_manager.xr_session_state
         if not self.session:
             raise NoXRSessionError
 
     @property
     def position(self) -> Vector:
         """The global position of the controller."""
         return Vector(self.session.controller_grip_location_get(bpy.context, self.idx))
 
     @position.setter
     def position(self, val):
-        print("Attribute 'position' of 'ULControllerVR' is read-only!")
+        print("Attribute 'position' of 'VRController' is read-only!")
 
     @property
     def orientation(self) -> Matrix:
         """The global orientation of the controller."""
         return Quaternion(self.session.controller_grip_rotation_get(bpy.context, self.idx)).to_matrix()
 
     @orientation.setter
     def orientation(self, val):
-        print("Attribute 'orientation' of 'ULControllerVR' is read-only!")
+        print("Attribute 'orientation' of 'VRController' is read-only!")
 
     @property
     def position_aim(self) -> Vector:
         """The global position of the tip of the controller."""
         return Vector(self.session.controller_aim_location_get(bpy.context, self.idx))
 
     @position_aim.setter
     def position_aim(self, val):
-        print("Attribute 'position_aim' of 'ULControllerVR' is read-only!")
+        print("Attribute 'position_aim' of 'VRController' is read-only!")
 
     @property
     def orientation_aim(self) -> Matrix:
         """The global orientation of the tip of the controller."""
         return Quaternion(self.session.controller_aim_rotation_get(bpy.context, self.idx)).to_matrix()
 
     @orientation_aim.setter
     def orientation_aim(self, val):
-        print("Attribute 'orientation_aim' of 'ULControllerVR' is read-only!")
+        print("Attribute 'orientation_aim' of 'VRController' is read-only!")
 
     @property
     def aim(self) -> Vector:
         """Targeting vector of the controller."""
         aim = self.position_aim - self.position
         return aim.normalized()
 
     @aim.setter
     def aim(self, val):
-        print("Attribute 'aim' of 'ULControllerVR' is read-only!")
+        print("Attribute 'aim' of 'VRController' is read-only!")
 
     @property
     def trigger(self) -> float:
         """The intensity with which the trigger on the controller is pressed."""
         return self.session.action_state_get(
             bpy.context,
             'blender_default',
             'teleport',
             f"/user/hand/{'left' if self.idx == 0 else 'right'}"
         )[0]
 
     @trigger.setter
     def trigger(self, val):
-        print("Attribute 'trigger' of 'ULControllerVR' is read-only!")
+        print("Attribute 'trigger' of 'VRController' is read-only!")
 
     @property
     def thumbstick(self) -> Vector:
         """Stick values for the controller."""
         if self.idx == 0:
             x = self.session.action_state_get(
                 bpy.context,
@@ -128,33 +129,31 @@
                 'fly_up',
                 '/user/hand/right'
             )[0]
             return Vector((x, y))
 
     @thumbstick.setter
     def thumbstick(self, val):
-        print("Attribute 'thumbstick' of 'ULControllerVR' is read-only!")
+        print("Attribute 'thumbstick' of 'VRController' is read-only!")
 
 
-class VRController(ULControllerVR):
-    _deprecated = False
+class ULControllerVR(VRController):
+    _deprecated = True
 
 
-class ULHeadsetVR():
+class VRHeadset():
     """Wrapper class for a VR Headset.
-
-    This wrapper provides a `position` and an `orientation`
-    attribute.
     """
 
-    _deprecated = True
+    _deprecated = False
 
     def __init__(self) -> None:
         if self._deprecated:
-            print('Warning: ULHeadsetVR class will be renamed to "VRHeadset" in future releases!')
+            from uplogic.console import warning
+            warning('Warning: ULHeadsetVR class will be renamed to "VRHeadset" in future releases!')
         self.session = bpy.context.window_manager.xr_session_state
         if not self.session:
             raise NoXRSessionError
 
     @property
     def position(self) -> Vector:
         return Vector(self.session.viewer_pose_location)
@@ -167,16 +166,19 @@
     def orientation(self) -> Matrix:
         return Quaternion(self.session.viewer_pose_rotation).to_matrix()
 
     @orientation.setter
     def orientation(self, val):
         print("Attribute 'orientation' of 'ULHeadsetVR' is read-only!")
 
+    def getAxisVect(self, vector):
+        return self.orientation @ vector
+
 
-class ULHeadsetVRWrapper(ULHeadsetVR):
+class ULHeadsetVRWrapper(VRHeadset):
     """Wrapper class for a VR Headset to be used for audio calculations.
 
     Not intended for manual use.
     """
     @property
     def worldPosition(self) -> Vector:
         return Vector(self.session.viewer_pose_location)
@@ -199,35 +201,35 @@
         obj_from,
         distance,
         xray
     ):
         return logic.getCurrentScene().active_camera.rayCast(obj_to, obj_from, distance, xray=xray)
 
 
-class VRHeadset(ULHeadsetVR):
-    _deprecated = False
+class ULHeadsetVR(VRHeadset):
+    _deprecated = True
 
 
-class ULCharacterVR():
+class VRCharacter():
     """Wrapper class for all VR Devices. This wrapper contains 2 `ULControllerVR` objects as well as one
     `ULHeadsetVR` object.
 
     Optionally, `KX_GameObjects` can be defined for both left and right controller. These objects will by
     automatically synched with their respective controller's position and orientation.
-
-    This class provides a `position` an `orientation` and a `scale` attribute.
     """
-    _deprecated = True
+    _deprecated = False
+
     def __init__(
         self,
         left_hand_object: GameObject = None,
         right_hand_object: GameObject = None
     ) -> None:
         if self._deprecated:
-            print('Warning: ULCharacterVR class will be renamed to "VRCharacter" in future releases!')
+            from uplogic.console import warning
+            warning('Warning: ULCharacterVR class will be renamed to "VRCharacter" in future releases!')
         self.session = bpy.context.window_manager.xr_session_state
         if not self.session:
             raise NoXRSessionError
         self.hand_left = ULControllerVR(0)
         self.hand_right = ULControllerVR(1)
         self.head = ULHeadsetVR()
         self.hand_left_object = left_hand_object
@@ -264,9 +266,17 @@
         return self.session.navigation_scale
 
     @scale.setter
     def scale(self, val):
         print("Attribute 'scale' of 'ULHeadsetVR' is read-only!")
 
 
-class VRCharacter(ULCharacterVR):
-    _deprecated = False
+class ULCharacterVR(VRCharacter):
+    _deprecated = True
+
+
+from uplogic.utils import check_vr_session_status
+
+
+VR_STATE = check_vr_session_status()
+VR_AUDIO = getattr(bpy.data.scenes[logic.getCurrentScene().name], 'use_vr_audio_space', False)
+VR_HEADSET = VRHeadset() if check_vr_session_status() else None
```

### Comparing `uplogic-2.2/uplogic/network/client.py` & `uplogic-3.2/uplogic/network/client.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/network/server.py` & `uplogic-3.2/uplogic/network/server.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/__init__.py` & `uplogic-3.2/uplogic/nodes/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
 class ULLogicContainer(ULLogicBase):
 
     def __init__(self):
         self._uid = None
         self._value = None
         self._children = []
+        self._done = False
         self.network = None
 
     def get_value(self):
         return self._value
 
     def _set_value(self, value):
         self._value = value
```

### Comparing `uplogic-2.2/uplogic/nodes/actions/__init__.py` & `uplogic-3.2/uplogic/nodes/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/addfilter.py` & `uplogic-3.2/uplogic/nodes/actions/addfilter.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/addobject.py` & `uplogic-3.2/uplogic/nodes/actions/addobject.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/addphysicsconstraint.py` & `uplogic-3.2/uplogic/nodes/actions/addphysicsconstraint.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/adduiwidget.py` & `uplogic-3.2/uplogic/nodes/actions/adduiwidget.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/alignaxistovector.py` & `uplogic-3.2/uplogic/nodes/actions/alignaxistovector.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/appendlistitem.py` & `uplogic-3.2/uplogic/nodes/actions/appendlistitem.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/applyforce.py` & `uplogic-3.2/uplogic/nodes/actions/applyforce.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/applyimpulse.py` & `uplogic-3.2/uplogic/nodes/actions/applyimpulse.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/applymovement.py` & `uplogic-3.2/uplogic/nodes/actions/applymovement.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/applyrotation.py` & `uplogic-3.2/uplogic/nodes/actions/applyrotation.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/applytorque.py` & `uplogic-3.2/uplogic/nodes/actions/applytorque.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/applytransform.py` & `uplogic-3.2/uplogic/nodes/actions/applytransform.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/cameraraycast.py` & `uplogic-3.2/uplogic/nodes/actions/cameraraycast.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/characterjump.py` & `uplogic-3.2/uplogic/nodes/actions/characterjump.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/clampedmodifyproperty.py` & `uplogic-3.2/uplogic/nodes/actions/clampedmodifyproperty.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/clearvariables.py` & `uplogic-3.2/uplogic/nodes/actions/clearvariables.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/copyproperty.py` & `uplogic-3.2/uplogic/nodes/actions/copyproperty.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/createuibutton.py` & `uplogic-3.2/uplogic/nodes/actions/createuibutton.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/createuicanvas.py` & `uplogic-3.2/uplogic/nodes/actions/createuicanvas.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/createuiimage.py` & `uplogic-3.2/uplogic/nodes/actions/createuiimage.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/createuilabel.py` & `uplogic-3.2/uplogic/nodes/actions/createuilabel.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/createuilayout.py` & `uplogic-3.2/uplogic/nodes/actions/createuilayout.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/createuislider.py` & `uplogic-3.2/uplogic/nodes/actions/createuislider.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/createvehicle.py` & `uplogic-3.2/uplogic/nodes/actions/createvehicle.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/cursorbehavior.py` & `uplogic-3.2/uplogic/nodes/actions/cursorbehavior.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/cursorvisibility.py` & `uplogic-3.2/uplogic/nodes/actions/cursorvisibility.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/dispatchevent.py` & `uplogic-3.2/uplogic/nodes/actions/dispatchevent.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/draw.py` & `uplogic-3.2/uplogic/nodes/actions/draw.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/drawbox.py` & `uplogic-3.2/uplogic/nodes/actions/drawbox.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/drawcube.py` & `uplogic-3.2/uplogic/nodes/actions/drawcube.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/drawline.py` & `uplogic-3.2/uplogic/nodes/actions/drawline.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/editbone.py` & `uplogic-3.2/uplogic/nodes/actions/editbone.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/endobject.py` & `uplogic-3.2/uplogic/nodes/actions/endobject.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/executesubnetwork.py` & `uplogic-3.2/uplogic/nodes/actions/executesubnetwork.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/followpath.py` & `uplogic-3.2/uplogic/nodes/actions/followpath.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/gamepadlook.py` & `uplogic-3.2/uplogic/nodes/actions/gamepadlook.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/gamepadvibration.py` & `uplogic-3.2/uplogic/nodes/actions/gamepadvibration.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/getperformanceprofile.py` & `uplogic-3.2/uplogic/nodes/actions/getperformanceprofile.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/installsubnetwork.py` & `uplogic-3.2/uplogic/nodes/actions/installsubnetwork.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/instream.py` & `uplogic-3.2/uplogic/nodes/actions/instream.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/listglobalvalues.py` & `uplogic-3.2/uplogic/nodes/actions/listglobalvalues.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/listvariables.py` & `uplogic-3.2/uplogic/nodes/actions/listvariables.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/loadblendfile.py` & `uplogic-3.2/uplogic/nodes/actions/loadblendfile.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/loadfilecontent.py` & `uplogic-3.2/uplogic/nodes/actions/loadfilecontent.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/loadgame.py` & `uplogic-3.2/uplogic/nodes/actions/loadgame.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/loadscene.py` & `uplogic-3.2/uplogic/nodes/actions/loadscene.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/localclient.py` & `uplogic-3.2/uplogic/nodes/actions/localclient.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/localserver.py` & `uplogic-3.2/uplogic/nodes/actions/localserver.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/makeuniquelight.py` & `uplogic-3.2/uplogic/nodes/actions/makeuniquelight.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/modifyproperty.py` & `uplogic-3.2/uplogic/nodes/actions/modifyproperty.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/mouselook.py` & `uplogic-3.2/uplogic/nodes/actions/mouselook.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/mouseraycast.py` & `uplogic-3.2/uplogic/nodes/actions/mouseraycast.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/mousesetposition.py` & `uplogic-3.2/uplogic/nodes/actions/mousesetposition.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/moveto.py` & `uplogic-3.2/uplogic/nodes/actions/moveto.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,29 +9,34 @@
         self.condition = None
         self.moving_object = None
         self.destination_point = None
         self.speed = None
         self.dynamic = None
         self.distance = None
         self.done = False
+        self._reached = False
         self.OUT = self.add_output(self.get_done)
+        self.REACHED = self.add_output(self.get_reached)
 
     def get_done(self):
         return self.done
 
+    def get_reached(self):
+        return self._reached
+
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
         moving_object = self.get_input(self.moving_object)
         destination_point = self.get_input(self.destination_point)
         speed = self.get_input(self.speed)
         distance = self.get_input(self.distance)
         dynamic = self.get_input(self.dynamic)
-        move_to(
+        self._reached = move_to(
             moving_object,
             destination_point,
             speed,
             self.network.time_per_frame,
             dynamic,
             distance
         )
```

### Comparing `uplogic-2.2/uplogic/nodes/actions/movetowithnavmesh.py` & `uplogic-3.2/uplogic/nodes/actions/movetowithnavmesh.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/pausesound.py` & `uplogic-3.2/uplogic/nodes/actions/pausesound.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/playaction.py` & `uplogic-3.2/uplogic/nodes/actions/playaction.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/playsequence.py` & `uplogic-3.2/uplogic/nodes/actions/playsequence.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/popdictkey.py` & `uplogic-3.2/uplogic/nodes/actions/popdictkey.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/printvalue.py` & `uplogic-3.2/uplogic/nodes/actions/printvalue.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from uplogic.nodes import ULActionNode
-from uplogic.console import log
+from uplogic.console import write
 
 
 class ULPrintValue(ULActionNode):
 
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
@@ -16,9 +16,9 @@
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
         value = self.get_input(self.value)
-        log(value, self.msg_type)
+        write(value, self.msg_type)
         self.done = True
```

### Comparing `uplogic-2.2/uplogic/nodes/actions/projectileraycast.py` & `uplogic-3.2/uplogic/nodes/actions/projectileraycast.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/raycast.py` & `uplogic-3.2/uplogic/nodes/actions/raycast.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/removefilter.py` & `uplogic-3.2/uplogic/nodes/actions/removefilter.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/removelistindex.py` & `uplogic-3.2/uplogic/nodes/actions/removelistindex.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/removelistvalue.py` & `uplogic-3.2/uplogic/nodes/actions/removelistvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/removeoverlaycollection.py` & `uplogic-3.2/uplogic/nodes/actions/removeoverlaycollection.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/removeparent.py` & `uplogic-3.2/uplogic/nodes/actions/removeparent.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/removephysicsconstraint.py` & `uplogic-3.2/uplogic/nodes/actions/removephysicsconstraint.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/removevariable.py` & `uplogic-3.2/uplogic/nodes/actions/removevariable.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/replacemesh.py` & `uplogic-3.2/uplogic/nodes/actions/replacemesh.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/resumesound.py` & `uplogic-3.2/uplogic/nodes/actions/resumesound.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/rotateto.py` & `uplogic-3.2/uplogic/nodes/actions/rotateto.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/runactuator.py` & `uplogic-3.2/uplogic/nodes/actions/runactuator.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/runpython.py` & `uplogic-3.2/uplogic/nodes/actions/runpython.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/savegame.py` & `uplogic-3.2/uplogic/nodes/actions/savegame.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/savevariable.py` & `uplogic-3.2/uplogic/nodes/actions/savevariable.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/savevariabledict.py` & `uplogic-3.2/uplogic/nodes/actions/savevariabledict.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/sendmessage.py` & `uplogic-3.2/uplogic/nodes/actions/sendmessage.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/sendnetworkmessage.py` & `uplogic-3.2/uplogic/nodes/actions/sendnetworkmessage.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setactionframe.py` & `uplogic-3.2/uplogic/nodes/actions/setactionframe.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setactuatorvalue.py` & `uplogic-3.2/uplogic/nodes/actions/setactuatorvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setboneconstraintattr.py` & `uplogic-3.2/uplogic/nodes/actions/setboneconstraintattr.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setboneconstraintinfluence.py` & `uplogic-3.2/uplogic/nodes/actions/setboneconstraintinfluence.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setboneconstrainttarget.py` & `uplogic-3.2/uplogic/nodes/actions/setboneconstrainttarget.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setboneposition.py` & `uplogic-3.2/uplogic/nodes/actions/setboneposition.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setcamera.py` & `uplogic-3.2/uplogic/nodes/actions/setcamera.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setcamerafov.py` & `uplogic-3.2/uplogic/nodes/actions/setcamerafov.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setcameraorthoscale.py` & `uplogic-3.2/uplogic/nodes/actions/setcameraorthoscale.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setcharactergravity.py` & `uplogic-3.2/uplogic/nodes/actions/setcharactergravity.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setcharacterjumpspeed.py` & `uplogic-3.2/uplogic/nodes/actions/setcharacterjumpspeed.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setcharactermaxjumps.py` & `uplogic-3.2/uplogic/nodes/actions/setcharactermaxjumps.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setcharactervelocity.py` & `uplogic-3.2/uplogic/nodes/actions/setcharactervelocity.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setcharacterwalkdir.py` & `uplogic-3.2/uplogic/nodes/actions/setcharacterwalkdir.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setcollisiongroup.py` & `uplogic-3.2/uplogic/nodes/actions/setcollisiongroup.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setcollisionmask.py` & `uplogic-3.2/uplogic/nodes/actions/setcollisionmask.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setconstraintattribute.py` & `uplogic-3.2/uplogic/nodes/actions/setconstraintattribute.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setcurvepoints.py` & `uplogic-3.2/uplogic/nodes/actions/setcurvepoints.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setcustomcursor.py` & `uplogic-3.2/uplogic/nodes/actions/setcustomcursor.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setdictkey.py` & `uplogic-3.2/uplogic/nodes/actions/setdictkey.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setdynamics.py` & `uplogic-3.2/uplogic/nodes/actions/setdynamics.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/seteeveeao.py` & `uplogic-3.2/uplogic/nodes/actions/seteeveeao.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/seteeveebloom.py` & `uplogic-3.2/uplogic/nodes/actions/seteeveebloom.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/seteeveesmaa.py` & `uplogic-3.2/uplogic/nodes/actions/seteeveesmaa.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/seteeveesmaaquality.py` & `uplogic-3.2/uplogic/nodes/actions/seteeveesmaaquality.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/seteeveessr.py` & `uplogic-3.2/uplogic/nodes/actions/seteeveessr.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/seteeveevolumetrics.py` & `uplogic-3.2/uplogic/nodes/actions/seteeveevolumetrics.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setexposure.py` & `uplogic-3.2/uplogic/nodes/actions/setexposure.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setfilterstate.py` & `uplogic-3.2/uplogic/nodes/actions/setfilterstate.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setfullscreen.py` & `uplogic-3.2/uplogic/nodes/actions/setfullscreen.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setgameobjectattr.py` & `uplogic-3.2/uplogic/nodes/actions/setgameobjectattr.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setgamma.py` & `uplogic-3.2/uplogic/nodes/actions/setgamma.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setglobalvalue.py` & `uplogic-3.2/uplogic/nodes/actions/setglobalvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setgravity.py` & `uplogic-3.2/uplogic/nodes/actions/setgravity.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setlightcolor.py` & `uplogic-3.2/uplogic/nodes/actions/setlightcolor.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setlightenergy.py` & `uplogic-3.2/uplogic/nodes/actions/setlightenergy.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setlightshadow.py` & `uplogic-3.2/uplogic/nodes/actions/setlightshadow.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setlistindex.py` & `uplogic-3.2/uplogic/nodes/actions/setlistindex.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setlogictreeproperty.py` & `uplogic-3.2/uplogic/nodes/actions/setlogictreeproperty.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setmaterial.py` & `uplogic-3.2/uplogic/nodes/actions/setmaterial.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setmatnodesocket.py` & `uplogic-3.2/uplogic/nodes/actions/setmatnodesocket.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setmatnodevalue.py` & `uplogic-3.2/uplogic/nodes/actions/setmatnodevalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setnodesocket.py` & `uplogic-3.2/uplogic/nodes/actions/setnodesocket.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setnodevalue.py` & `uplogic-3.2/uplogic/nodes/actions/setnodevalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setoverlaycollection.py` & `uplogic-3.2/uplogic/nodes/actions/setoverlaycollection.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setparent.py` & `uplogic-3.2/uplogic/nodes/actions/setparent.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setphysics.py` & `uplogic-3.2/uplogic/nodes/actions/setphysics.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setprofile.py` & `uplogic-3.2/uplogic/nodes/actions/setprofile.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setproperty.py` & `uplogic-3.2/uplogic/nodes/actions/setproperty.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setpyinstanceattr.py` & `uplogic-3.2/uplogic/nodes/actions/setpyinstanceattr.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setresolution.py` & `uplogic-3.2/uplogic/nodes/actions/setresolution.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setrigidbody.py` & `uplogic-3.2/uplogic/nodes/actions/setrigidbody.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setscene.py` & `uplogic-3.2/uplogic/nodes/actions/setscene.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setsensorvalue.py` & `uplogic-3.2/uplogic/nodes/actions/setsensorvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/settimescale.py` & `uplogic-3.2/uplogic/nodes/actions/settimescale.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setuiwidgetattr.py` & `uplogic-3.2/uplogic/nodes/actions/setuiwidgetattr.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setvisibility.py` & `uplogic-3.2/uplogic/nodes/actions/setvisibility.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/setvsync.py` & `uplogic-3.2/uplogic/nodes/actions/setvsync.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/showframerate.py` & `uplogic-3.2/uplogic/nodes/actions/showframerate.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/slowfollow.py` & `uplogic-3.2/uplogic/nodes/actions/slowfollow.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/spawnpool.py` & `uplogic-3.2/uplogic/nodes/actions/spawnpool.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/startsound.py` & `uplogic-3.2/uplogic/nodes/actions/startsound.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/startsound2d.py` & `uplogic-3.2/uplogic/nodes/actions/startsound2d.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/startsound3d.py` & `uplogic-3.2/uplogic/nodes/actions/startsound3d.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/startspeaker.py` & `uplogic-3.2/uplogic/nodes/actions/startspeaker.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/startsubnetwork.py` & `uplogic-3.2/uplogic/nodes/actions/startsubnetwork.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/stopaction.py` & `uplogic-3.2/uplogic/nodes/actions/stopaction.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/stopallsounds.py` & `uplogic-3.2/uplogic/nodes/actions/stopallsounds.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/stopsound.py` & `uplogic-3.2/uplogic/nodes/actions/stopsound.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/stopsubnetwork.py` & `uplogic-3.2/uplogic/nodes/actions/stopsubnetwork.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/togglefilter.py` & `uplogic-3.2/uplogic/nodes/actions/togglefilter.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/toggleproperty.py` & `uplogic-3.2/uplogic/nodes/actions/toggleproperty.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/translate.py` & `uplogic-3.2/uplogic/nodes/actions/translate.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/vectoranglecheck.py` & `uplogic-3.2/uplogic/nodes/actions/vectoranglecheck.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/vehicleapplybraking.py` & `uplogic-3.2/uplogic/nodes/actions/vehicleapplybraking.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/vehicleapplyforce.py` & `uplogic-3.2/uplogic/nodes/actions/vehicleapplyforce.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/vehicleapplysteering.py` & `uplogic-3.2/uplogic/nodes/actions/vehicleapplysteering.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/actions/vehiclesetattributes.py` & `uplogic-3.2/uplogic/nodes/actions/vehiclesetattributes.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/__init__.py` & `uplogic-3.2/uplogic/nodes/conditions/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/barrier.py` & `uplogic-3.2/uplogic/nodes/conditions/barrier.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/checkdistance.py` & `uplogic-3.2/uplogic/nodes/conditions/checkdistance.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/collision.py` & `uplogic-3.2/uplogic/nodes/conditions/collision.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/compare.py` & `uplogic-3.2/uplogic/nodes/conditions/compare.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/comparevectors.py` & `uplogic-3.2/uplogic/nodes/conditions/comparevectors.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/controllerstatus.py` & `uplogic-3.2/uplogic/nodes/conditions/controllerstatus.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/evaluateproperty.py` & `uplogic-3.2/uplogic/nodes/conditions/evaluateproperty.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/gamepadactive.py` & `uplogic-3.2/uplogic/nodes/conditions/gamepadactive.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/gamepadbutton.py` & `uplogic-3.2/uplogic/nodes/conditions/gamepadbutton.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/gamepadbuttonup.py` & `uplogic-3.2/uplogic/nodes/conditions/gamepadbuttonup.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/handleevent.py` & `uplogic-3.2/uplogic/nodes/conditions/handleevent.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/hasproperty.py` & `uplogic-3.2/uplogic/nodes/conditions/hasproperty.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/keypressed.py` & `uplogic-3.2/uplogic/nodes/conditions/keypressed.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/keyreleased.py` & `uplogic-3.2/uplogic/nodes/conditions/keyreleased.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/logicand.py` & `uplogic-3.2/uplogic/nodes/conditions/logicand.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/logicgate.py` & `uplogic-3.2/uplogic/nodes/conditions/logicgate.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/logicgatelist.py` & `uplogic-3.2/uplogic/nodes/conditions/logicgatelist.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/logicor.py` & `uplogic-3.2/uplogic/nodes/conditions/logicor.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/logictreestatus.py` & `uplogic-3.2/uplogic/nodes/conditions/logictreestatus.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/mouseover.py` & `uplogic-3.2/uplogic/nodes/conditions/mouseover.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/mousepressed.py` & `uplogic-3.2/uplogic/nodes/conditions/mousepressed.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/mousepressedon.py` & `uplogic-3.2/uplogic/nodes/conditions/mousepressedon.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/mousereleased.py` & `uplogic-3.2/uplogic/nodes/conditions/mousereleased.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/mousescroll.py` & `uplogic-3.2/uplogic/nodes/conditions/mousescroll.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/once.py` & `uplogic-3.2/uplogic/nodes/conditions/once.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/onnexttick.py` & `uplogic-3.2/uplogic/nodes/conditions/onnexttick.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/onvaluechanged.py` & `uplogic-3.2/uplogic/nodes/conditions/onvaluechanged.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/onvaluechangedto.py` & `uplogic-3.2/uplogic/nodes/conditions/onvaluechangedto.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/pulsify.py` & `uplogic-3.2/uplogic/nodes/conditions/pulsify.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/timedelay.py` & `uplogic-3.2/uplogic/nodes/conditions/timedelay.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/timer.py` & `uplogic-3.2/uplogic/nodes/conditions/timer.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/conditions/vectoranglecheck.py` & `uplogic-3.2/uplogic/nodes/conditions/vectoranglecheck.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/logictree.py` & `uplogic-3.2/uplogic/nodes/logictree.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/__init__.py` & `uplogic-3.2/uplogic/nodes/parameters/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,9 +100,11 @@
 from .instream import ULKeyLogger
 from .rotatebypoint import ULRotateByPoint
 from .getlogictreeproperty import ULGetLogicTreeProperty
 from .resizevector import ResizeVectorNode
 from .curveinterpolation import CurveInterpolationNode
 from .tweenvalue import TweenValueNode
 from .getcollisiongroup import GetCollisionGroupNode
+from .getmasterfolder import GetMasterFolderNode
+from .joinpath import JoinPathNode
 
 from .randomvalue import ULRandomValue
```

### Comparing `uplogic-2.2/uplogic/nodes/parameters/actionstatus.py` & `uplogic-3.2/uplogic/nodes/parameters/actionstatus.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/bonestatus.py` & `uplogic-3.2/uplogic/nodes/parameters/bonestatus.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/characterinfo.py` & `uplogic-3.2/uplogic/nodes/parameters/characterinfo.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/childbyindex.py` & `uplogic-3.2/uplogic/nodes/parameters/childbyindex.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/childbyname.py` & `uplogic-3.2/uplogic/nodes/parameters/childbyname.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/clamp.py` & `uplogic-3.2/uplogic/nodes/parameters/clamp.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/dictvalue.py` & `uplogic-3.2/uplogic/nodes/parameters/dictvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/euler.py` & `uplogic-3.2/uplogic/nodes/parameters/euler.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/eulertomatrix.py` & `uplogic-3.2/uplogic/nodes/parameters/eulertomatrix.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/formattedstring.py` & `uplogic-3.2/uplogic/nodes/parameters/formattedstring.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/formula.py` & `uplogic-3.2/uplogic/nodes/parameters/formula.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/gamepadsticks.py` & `uplogic-3.2/uplogic/nodes/parameters/gamepadsticks.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/gamepadtrigger.py` & `uplogic-3.2/uplogic/nodes/parameters/gamepadtrigger.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/getactuatorvalue.py` & `uplogic-3.2/uplogic/nodes/parameters/getactuatorvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/getcollectionobjects.py` & `uplogic-3.2/uplogic/nodes/parameters/getcollectionobjects.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/getcurvepoints.py` & `uplogic-3.2/uplogic/nodes/parameters/getcurvepoints.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/getglobalvalue.py` & `uplogic-3.2/uplogic/nodes/parameters/getglobalvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/getlogictreeproperty.py` & `uplogic-3.2/uplogic/nodes/parameters/getlogictreeproperty.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/getnodeattribute.py` & `uplogic-3.2/uplogic/nodes/parameters/getnodeattribute.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/getnodesocket.py` & `uplogic-3.2/uplogic/nodes/parameters/getnodesocket.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/getproperty.py` & `uplogic-3.2/uplogic/nodes/parameters/getproperty.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/getresolution.py` & `uplogic-3.2/uplogic/nodes/parameters/getresolution.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/getsensorvalue.py` & `uplogic-3.2/uplogic/nodes/parameters/getsensorvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/getuiwidgetattr.py` & `uplogic-3.2/uplogic/nodes/parameters/getuiwidgetattr.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/instream.py` & `uplogic-3.2/uplogic/nodes/parameters/instream.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/limitrange.py` & `uplogic-3.2/uplogic/nodes/parameters/limitrange.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/listextend.py` & `uplogic-3.2/uplogic/nodes/parameters/listextend.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/loadvariable.py` & `uplogic-3.2/uplogic/nodes/parameters/loadvariable.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/loadvariabledict.py` & `uplogic-3.2/uplogic/nodes/parameters/loadvariabledict.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/maprange.py` & `uplogic-3.2/uplogic/nodes/parameters/maprange.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/materialgetattribute.py` & `uplogic-3.2/uplogic/nodes/parameters/materialgetattribute.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/materialgetnode.py` & `uplogic-3.2/uplogic/nodes/parameters/materialgetnode.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/materialgetsocket.py` & `uplogic-3.2/uplogic/nodes/parameters/materialgetsocket.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/math.py` & `uplogic-3.2/uplogic/nodes/parameters/math.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/matrixtoxyz.py` & `uplogic-3.2/uplogic/nodes/parameters/matrixtoxyz.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/mousedata.py` & `uplogic-3.2/uplogic/nodes/parameters/mousedata.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/objectattr.py` & `uplogic-3.2/uplogic/nodes/parameters/objectattr.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/objectdatavertices.py` & `uplogic-3.2/uplogic/nodes/parameters/objectdatavertices.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/randomfloat.py` & `uplogic-3.2/uplogic/nodes/parameters/randomfloat.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/randomint.py` & `uplogic-3.2/uplogic/nodes/parameters/randomint.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/randomvalue.py` & `uplogic-3.2/uplogic/nodes/parameters/randomvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/randomvect.py` & `uplogic-3.2/uplogic/nodes/parameters/randomvect.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/rangedthreshold.py` & `uplogic-3.2/uplogic/nodes/parameters/rangedthreshold.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/rebuilddata.py` & `uplogic-3.2/uplogic/nodes/parameters/rebuilddata.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/resizevector.py` & `uplogic-3.2/uplogic/nodes/parameters/resizevector.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/rotatebypoint.py` & `uplogic-3.2/uplogic/nodes/parameters/rotatebypoint.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/serializedata.py` & `uplogic-3.2/uplogic/nodes/parameters/serializedata.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/storevalue.py` & `uplogic-3.2/uplogic/nodes/parameters/storevalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/threshold.py` & `uplogic-3.2/uplogic/nodes/parameters/threshold.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/timedata.py` & `uplogic-3.2/uplogic/nodes/parameters/timedata.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/tweenvalue.py` & `uplogic-3.2/uplogic/nodes/parameters/tweenvalue.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,33 +12,38 @@
         self.from_float = 0.0
         self.to_float = 1.0
         self.from_vec = Vector((0, 0, 0))
         self.to_vec = Vector((1, 1, 1))
         self.duration = 1.0
 
         self._time = 0.0
+        self._done = False
 
         self.mapping = None
         self.active = False
 
         self.on_demand = True
         self.value_type = 0  # 0 -> float, 1 -> Vector
         
         self._result = 0.0
         self._factor = 0.
         self._eval = 0.
 
         self._direction = 1
 
         self.DONE = self.add_output(self.get_done)
+        self.REACHED = self.add_output(self.get_reached)
         self.RESULT_FLOAT = self.add_output(self.get_float)
         self.RESULT_VEC = self.add_output(self.get_vec)
         self.FAC = self.add_output(self.get_fac)
 
     def get_done(self):
+        return self._done
+
+    def get_reached(self):
         return self._factor == self._direction
 
     def get_fac(self):
         return self._factor
 
     def get_vec(self):
         self.active = True
@@ -53,14 +58,15 @@
         if self.on_demand:
             self.forward = True
             self.back = False
         self._result = interpolate(self.get_input(self.from_float), self.get_input(self.to_float), self._eval)
         return self._result
 
     def evaluate(self):
+        self._done = False
         forward = self.get_input(self.forward)
         back = self.get_input(self.back)
         if forward or back:
             self.active = True
         if not self.active and not self.on_demand:
             return
         duration = self.get_input(self.duration)
@@ -87,7 +93,8 @@
                 ))
             else:
                 self._factor = 0
         self.active = False
         if self.on_demand:
             self.forward = False
             self.back = True
+        self._done = True
```

### Comparing `uplogic-2.2/uplogic/nodes/parameters/typecastvalue.py` & `uplogic-3.2/uplogic/nodes/parameters/typecastvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/valueswitch.py` & `uplogic-3.2/uplogic/nodes/parameters/valueswitch.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/vectorangle.py` & `uplogic-3.2/uplogic/nodes/parameters/vectorangle.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/vectormath.py` & `uplogic-3.2/uplogic/nodes/parameters/vectormath.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/vectorsplitxy.py` & `uplogic-3.2/uplogic/nodes/parameters/vectorsplitxy.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/vectorsplitxyz.py` & `uplogic-3.2/uplogic/nodes/parameters/vectorsplitxyz.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/vectorxyz.py` & `uplogic-3.2/uplogic/nodes/parameters/vectorxyz.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/vectorxyzw.py` & `uplogic-3.2/uplogic/nodes/parameters/vectorxyzw.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/vrcontrollervalues.py` & `uplogic-3.2/uplogic/nodes/parameters/vrcontrollervalues.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/withinrange.py` & `uplogic-3.2/uplogic/nodes/parameters/withinrange.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/nodes/parameters/worldposition.py` & `uplogic-3.2/uplogic/nodes/parameters/worldposition.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/physics/__init__.py` & `uplogic-3.2/uplogic/physics/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/physics/buoyancy.py` & `uplogic-3.2/uplogic/physics/buoyancy.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     def enable(self):
         self._active = True
 
     def destroy(self):
         raise NotImplementedError
 
 
-class ULFlotsam(ULBuoy):
-    _deprecated = True
+class Flotsam(ULBuoy):
+    _deprecated = False
 
     def __init__(self, game_object, buoyancy=1, height=200, align=True) -> None:
         if self._deprecated:
             print('ULFlotsam class will be renamed to "Flotsam" in future releases!')
         super().__init__()
         self.game_object = game_object
         game_object[FLOTSAM] = self
@@ -66,20 +66,20 @@
         flotsam.linearDamping = lindamp
         flotsam.angularDamping = lindamp * .8
 
     def destroy(self):
         logic.getCurrentScene().pre_draw.remove(self.update)
 
 
-class Flotsam(ULFlotsam):
-    _deprecated = False
+class ULFlotsam(Flotsam):
+    _deprecated = True
 
 
-class ULShip(ULBuoy):
-    _deprecated = True
+class Ship(ULBuoy):
+    _deprecated = False
 
     def __init__(self, game_object, buoyancy=1, height=200, water=None) -> None:
         if self._deprecated:
             print('ULShip class will be renamed to "Ship" in future releases!')
         super().__init__()
         self.game_object = game_object
         self.linear_damping = game_object.linearDamping
@@ -127,9 +127,9 @@
         ship.linearDamping = self.linear_damping + lin_dampen_factor
         ship.angularDamping = self.angular_damping + ang_dampen_factor
 
     def destroy(self):
         logic.getCurrentScene().pre_draw.remove(self.update)
 
 
-class Ship(ULShip):
-    _deprecated = False
+class ULShip(Ship):
+    _deprecated = True
```

### Comparing `uplogic-2.2/uplogic/physics/character.py` & `uplogic-3.2/uplogic/physics/character.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 from bge.constraints import getCharacter
 from bge.types import KX_GameObject as GameObject
 from uplogic.utils.constants import FRAMETIME_COMPARE
 from mathutils import Vector
 import bpy
 
 
-class ULCharacter():
-    _deprecated = True
+class Character():
+    _deprecated = False
 
     def __init__(self, owner: GameObject) -> None:
         if self._deprecated:
-            print('Warning: ULCharacter class will be renamed to "Character" in future releases!')
+            from uplogic.console import warning
+            warning('Warning: ULCharacter class will be renamed to "Character" in future releases!')
         self.owner = owner
         self.wrapper = getCharacter(owner)
         self._old_position = owner.worldPosition.copy()
         self.velocity = Vector((0, 0, 0))
         self.is_walking = False
         self._on_ground = self.wrapper.onGround
         self.landed = False
@@ -122,9 +123,9 @@
         self.is_walking = True
         self.wrapper.walkDirection = self.owner.worldOrientation @ direction * self.speed if local else direction * self.speed
 
     def jump(self):
         self.wrapper.jump()
 
 
-class Character(ULCharacter):
-    _deprecated = False
+class ULCharacter(Character):
+    _deprecated = True
```

### Comparing `uplogic-2.2/uplogic/physics/collision.py` & `uplogic-3.2/uplogic/physics/collision.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 from typing import Callable
 from bge import logic
 from bge.types import KX_GameObject as GameObject
 
 
-class ULCollision():
+class Collision():
     """Collision Handler.
 
     Not intended for manual use."""
     target = None
     point = None
     normal = None
     tap = False
     consumed = False
     active = False
     _objects = []
     _old_objs = []
     done_objs = []
 
-    _deprecated = True
+    _deprecated = False
 
     def __init__(
         self,
         game_object: GameObject,
         callback: Callable,
         prop: str = '',
         mat: str = '',
         tap: bool = False,
         post_call: bool = False
     ):
         if self._deprecated:
-            print('Warning: ULCollision class will be renamed to "Collision" in future releases!')
+            from uplogic.console import warning
+            warning('Warning: ULCollision class will be renamed to "Collision" in future releases!')
         self.callback: Callable = callback
         self.prop: str = prop
         self.mat: str = mat
         self.tap: bool = tap
         self.post_call = post_call
         self.game_object: GameObject = game_object
         self.register()
@@ -82,16 +83,16 @@
         logic.getCurrentScene().pre_draw.append(self.reset)
 
     def remove(self):
         self.game_object.collisionCallbacks.remove(self.collision)
         logic.getCurrentScene().pre_draw.remove(self.reset)
 
 
-class Collision(ULCollision):
-    _deprecated = False
+class ULCollision(Collision):
+    _deprecated = True
 
 
 def on_collision(
     obj: GameObject,
     callback: Callable,
     prop: str = '',
     material: str = '',
```

### Comparing `uplogic-2.2/uplogic/physics/constraints.py` & `uplogic-3.2/uplogic/physics/constraints.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,17 +61,17 @@
     """Wrapper function for `bge.constraints.removeConstraint()`. Creates a constraint
 
     :param `constraint`: The constraint to remove.
     """
     constraints.removeConstraint(constraint.getConstraintId())
 
 
-class ULTrackTo():
+class TrackTo():
 
-    _deprecated = True
+    _deprecated = False
 
     def __init__(
         self,
         game_object: GameObject,
         target: GameObject or Vector,
         axis: int = 2,
         front: int = 1,
@@ -121,19 +121,19 @@
         logic.getCurrentScene().pre_draw.remove(self.update)
 
     def update(self):
         if self.rotate_func:
             self.rotate_func(self.game_object, self.target, self.front, self.speed)
 
 
-class TrackTo(ULTrackTo):
-    _deprecated = False
+class ULTrackTo(TrackTo):
+    _deprecated = True
 
 
-class ULSpring():
+class Spring():
     """Spring Physics Constraint. The two objects connected by the string will
     be pulled towards each other if the string is streched, optionally they will
     be pushed apart when the spring is being compacted.
 
     :param `origin`: First connection point of the spring.
     :param `target`: Second connection point of the spring.
     :param `rigid_body_origin`: Object to be influenced by the spring (optional).
@@ -143,15 +143,15 @@
     :param `use_push`: Push the objects apart when spring is compressed.
     :param `use_breaking`: Remove the constraint when spring is pulled too much.
     :param `break_threshold`: Amount of strain the spring will endure.
     :param `curve`: Set a curve object to fit the spring.
     :param `visualize`: Enable a visual representation of the spring.
     """
 
-    _deprecated = True
+    _deprecated = False
 
     def __init__(
         self,
         origin: GameObject,
         target: GameObject,
         rigid_body_origin: GameObject = None,
         rigid_body_target: GameObject = None,
@@ -236,9 +236,9 @@
         rbt = self.rigid_body_target
         if hasattr(rbo, 'blenderObject') and rbo.blenderObject.data:
             rbo.applyImpulse(o.worldPosition, get_direction(o, t) * force)
         if hasattr(rbt, 'blenderObject') and rbt.blenderObject.data:
             rbt.applyImpulse(o.worldPosition, get_direction(t, o) * force)
 
 
-class Spring(ULSpring):
-    _deprecated = False
+class ULSpring(Spring):
+    _deprecated = True
```

### Comparing `uplogic-2.2/uplogic/physics/vehicle.py` & `uplogic-3.2/uplogic/physics/vehicle.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,30 +14,31 @@
 This will adress wheel indices starting in the back."""
 
 FOURWD = 'ALL'
 """Four Wheel Drive\n
 This will adress all wheels on the vehicle."""
 
 
-class ULVehicle():
-    _deprecated = True
+class Vehicle():
+    _deprecated = False
 
     def __init__(
         self,
         body: KX_GameObject,
         suspension: float = 0.06,
         stiffness: float = 50.0,
         damping: float = 5.0,
         friction: float = 2.0,
         wheel_size: float = 1.0,
         drive: str = FWD,
         steer_axle: str = FWD
     ) -> None:
         if self._deprecated:
-            print('Warning: ULVehicle class will be renamed to "Vehicle" in future releases!')
+            from uplogic.console import warning
+            warning('Warning: ULVehicle class will be renamed to "Vehicle" in future releases!')
         orig_ori = body.localOrientation.copy()
         body.localOrientation = Euler((0, 0, 0), 'XYZ')
         ph_id = body.getPhysicsId()
         car = createVehicle(ph_id)
         down = Vector((0, 0, -1))
         axle_dir = body.getAxisVect(Vector((-1, 0, 0)))
         wheels = []
@@ -308,9 +309,9 @@
         if steer_axle != self.steer_axle and steer_axle:
             self.steer_axle = steer_axle
         if wheelcount and wheelcount != self.steer_wheels:
             self.steer_wheels = wheelcount
         self.steering = power
 
 
-class Vehicle(ULVehicle):
-    _deprecated = False
+class ULVehicle(Vehicle):
+    _deprecated = True
```

### Comparing `uplogic-2.2/uplogic/serialize/__init__.py` & `uplogic-3.2/uplogic/serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/shaders/__init__.py` & `uplogic-3.2/uplogic/shaders/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/shaders/adaptivetonemapping.py` & `uplogic-3.2/uplogic/shaders/adaptivetonemapping.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     fragColor = (value/contrast) - brightness;
 }"""
 
 
 class AdaptiveToneMapping(Filter2D):
 
     def __init__(self, power=1.0, avgL=2.0, idx: int = None) -> None:
-        self.settings = {'power': float(power), 'avgL': float(avgL)}
-        super().__init__(glsl, idx, {'power': self.settings, 'avgL': self.settings})
+        self.uniforms = {'power': float(power), 'avgL': float(avgL)}
+        super().__init__(glsl, idx, {'power': self.uniforms, 'avgL': self.uniforms})
 
     @property
     def power(self):
-        return self.settings['power']
+        return self.uniforms['power']
 
     @power.setter
     def power(self, val):
-        self.settings['power'] = float(val)
+        self.uniforms['power'] = float(val)
```

### Comparing `uplogic-2.2/uplogic/shaders/blur.py` & `uplogic-3.2/uplogic/shaders/blur.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,47 +21,47 @@
 
 void main()
 {
     float Pi = 6.28318530718;
 
     float quality = 3.0;
    
-    vec2 radius = power/resolution.xy;
+    vec2 radius = power / resolution.xy;
     
     vec2 uv = texcoord;
 
     vec4 color = texture(bgl_RenderedTexture, uv);
     
     // Blur calculations
-    for( float d=0.0; d<Pi; d+=Pi/samples)
+    for (float d = 0.0; d < Pi; d += Pi / samples)
     {
-		for(float i=1.0/quality; i<=1.0; i+=1.0/quality)
+		for(float i = 1.0 / quality; i <= 1.0; i += 1.0 / quality)
         {
-			color += texture(bgl_RenderedTexture, uv+vec2(cos(d),sin(d)) * radius * i);
+			color += texture(bgl_RenderedTexture, uv + vec2(cos(d), sin(d)) * radius * i);
         }
     }
     color /= quality * samples - 15.0;
     fragColor = color;
 }"""
 
 
 class Blur(Filter2D):
 
     def __init__(self, power=1.0, samples=16, idx: int = None) -> None:
-       self.settings = {'samples': float(samples), 'power': float(power)}
-       super().__init__(glsl, idx, {'samples': self.settings, 'power': self.settings})
+       self.uniforms = {'samples': float(samples), 'power': float(power)}
+       super().__init__(glsl, idx, {'samples': self.uniforms, 'power': self.uniforms})
 
     @property
     def samples(self):
-        return self.settings['samples']
+        return self.uniforms['samples']
 
     @samples.setter
     def samples(self, val):
-        self.settings['samples'] = float(val)
+        self.uniforms['samples'] = float(val)
 
     @property
     def power(self):
-        return self.settings['power']
+        return self.uniforms['power']
 
     @power.setter
     def power(self, val):
-        self.settings['power'] = float(val)
+        self.uniforms['power'] = float(val)
```

### Comparing `uplogic-2.2/uplogic/shaders/brightness.py` & `uplogic-3.2/uplogic/shaders/brightness.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 }
 """
 
 
 class Brightness(Filter2D):
 
     def __init__(self, brightness=1.0, idx: int = None) -> None:
-        self.settings = {'brightness': float(brightness)}
-        super().__init__(glsl, idx, {'brightness': self.settings})
+        self.uniforms = {'brightness': float(brightness)}
+        super().__init__(glsl, idx, {'brightness': self.uniforms})
 
     @property
     def brightness(self):
-        return self.settings['brightness']
+        return self.uniforms['brightness']
 
     @brightness.setter
     def brightness(self, val):
-        self.settings['brightness'] = float(val)
+        self.uniforms['brightness'] = float(val)
```

### Comparing `uplogic-2.2/uplogic/shaders/buffer.py` & `uplogic-3.2/uplogic/shaders/buffer.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 }
 """
 
 
 class Buffer(Filter2D):
 
     def __init__(self, gamma=1, idx: int = None) -> None:
-        self.settings = {'gamma': float(gamma)}
-        super().__init__(glsl, idx, {'gamma': self.settings})
+        self.uniforms = {'gamma': float(gamma)}
+        super().__init__(glsl, idx, {'gamma': self.uniforms})
         self._filter.addOffScreen(0)
 
     @property
     def bindcode(self):
         return self._filter.offScreen.colorBindCodes[0]
 
     @property
@@ -44,11 +44,11 @@
 }
 """
 
 
 class DepthBuffer(Buffer):
 
     def __init__(self, gamma=1, idx: int = None) -> None:
-        self.settings = {'gamma': float(gamma)}
-        super().__init__(depth_glsl, idx, {'gamma': self.settings})
+        self.uniforms = {'gamma': float(gamma)}
+        super().__init__(depth_glsl, idx, {'gamma': self.uniforms})
         self._filter.addOffScreen(0)
```

### Comparing `uplogic-2.2/uplogic/shaders/chromaticaberration.py` & `uplogic-3.2/uplogic/shaders/chromaticaberration.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 }
 """
 
 
 class ChromaticAberration(Filter2D):
 
     def __init__(self, power: float = 2.0, idx: int = None) -> None:
-        self.settings = {'power': float(power)}
-        super().__init__(glsl, idx, {'power': self.settings})
+        self.uniforms = {'power': float(power)}
+        super().__init__(glsl, idx, {'power': self.uniforms})
 
     @property
     def power(self):
-        return self.settings['power']
+        return self.uniforms['power']
 
     @power.setter
     def power(self, val):
-        self.settings['power'] = val
+        self.uniforms['power'] = val
```

### Comparing `uplogic-2.2/uplogic/shaders/distort.py` & `uplogic-3.2/uplogic/shaders/distort.py`

 * *Files 6% similar despite different names*

```diff
@@ -166,41 +166,41 @@
 
 
 class Distort(Filter2D):
 
     def __init__(self, power=1.0, speed=1.0, idx: int = None) -> None:
         now = logic.getRealTime()
         self.speed = speed
-        self.settings = {'power': float(power), 'timer': now, 'resettimer': 0.0}
+        self.uniforms = {'power': float(power), 'timer': now, 'resettimer': 0.0}
         self._last_time = now
-        super().__init__(glsl, idx, {'power': self.settings, 'timer': self.settings, 'resettimer': self.settings})
+        super().__init__(glsl, idx, {'power': self.uniforms, 'timer': self.uniforms, 'resettimer': self.uniforms})
 
     def update(self):
         now = logic.getRealTime()
         self.timer += (now - self._last_time) * self.speed
         self._last_time = now
         self.resettimer += (now - self._last_time) * self.speed
         super().update()
 
     @property
     def timer(self):
-        return self.settings['timer']
+        return self.uniforms['timer']
 
     @timer.setter
     def timer(self, val):
-        self.settings['timer'] = float(val)
+        self.uniforms['timer'] = float(val)
 
     @property
     def resettimer(self):
-        return self.settings['resettimer']
+        return self.uniforms['resettimer']
 
     @resettimer.setter
     def resettimer(self, val):
-        self.settings['resettimer'] = float(val)
+        self.uniforms['resettimer'] = float(val)
 
     @property
     def power(self):
-        return self.settings['power']
+        return self.uniforms['power']
 
     @power.setter
     def power(self, val):
-        self.settings['power'] = float(val)
+        self.uniforms['power'] = float(val)
```

### Comparing `uplogic-2.2/uplogic/shaders/dof.py` & `uplogic-3.2/uplogic/shaders/dof.py`

 * *Files 20% similar despite different names*

```diff
@@ -288,71 +288,71 @@
 
 
 class DoF(Filter2D):
 
         
     def __init__(self, distance=1.0, autofocus=False, power=1.0, fstop=1, samples=16, idx: int = None) -> None:
         cam = logic.getCurrentScene().active_camera
-        self.settings = {
+        self.uniforms = {
             'distance': float(distance),
             'power': float(power),
             'fstop': float(fstop),
             'samples': int(samples),
             'autofocus': bool(autofocus)
             # 'znear': cam.near,
             # 'zfar': cam.far
         }
         super().__init__(glsl, idx, {
-            'distance': self.settings,
-            'power': self.settings,
-            'fstop': self.settings,
-            'samples': self.settings,
-            'autofocus': self.settings
-            # 'znear': self.settings,
-            # 'zfar': self.settings
+            'distance': self.uniforms,
+            'power': self.uniforms,
+            'fstop': self.uniforms,
+            'samples': self.uniforms,
+            'autofocus': self.uniforms
+            # 'znear': self.uniforms,
+            # 'zfar': self.uniforms
         })
 
     def update(self):
         super().update()
         cam = logic.getCurrentScene().active_camera
-        self.settings['znear'] = cam.near
-        self.settings['zfar'] = cam.far
+        self.uniforms['znear'] = cam.near
+        self.uniforms['zfar'] = cam.far
 
     @property
     def distance(self):
-        return self.settings['distance']
+        return self.uniforms['distance']
 
     @distance.setter
     def distance(self, val):
-        self.settings['distance'] = float(val)
+        self.uniforms['distance'] = float(val)
 
     @property
     def autofocus(self):
-        return self.settings['autofocus']
+        return self.uniforms['autofocus']
 
     @autofocus.setter
     def autofocus(self, val):
-        self.settings['autofocus'] = bool(val)
+        self.uniforms['autofocus'] = bool(val)
 
     @property
     def fstop(self):
-        return self.settings['fstop']
+        return self.uniforms['fstop']
 
     @fstop.setter
     def fstop(self, val):
-        self.settings['fstop'] = float(val)
+        self.uniforms['fstop'] = float(val)
 
     @property
     def power(self):
-        return self.settings['power']
+        return self.uniforms['power']
 
     @power.setter
     def power(self, val):
-        self.settings['power'] = val
+        self.uniforms['power'] = val
 
     @property
     def samples(self):
-        return self.settings['samples']
+        return self.uniforms['samples']
 
     @samples.setter
     def samples(self, val):
-        self.settings['samples'] = int(val)
+        self.uniforms['samples'] = int(val)
```

### Comparing `uplogic-2.2/uplogic/shaders/droplets.py` & `uplogic-3.2/uplogic/shaders/droplets.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,20 +28,20 @@
 
 float width = bgl_RenderedTextureWidth;
 float height = bgl_RenderedTextureHeight;
 
 //a random texture generator, but you can also use a pre-computed perturbation texture
 vec4 rnm(in vec2 tc) 
 {
-    float noise =  sin(dot(tc ,vec2(12.9898,78.233))) * 43758.5453;
+    float noise = sin(dot(tc, vec2(12.9898, 78.233))) * 43758.5453;
 
-    float noiseR =  fract(noise)*2.0-1.0;
-    float noiseG =  fract(noise*1.2154)*2.0-1.0; 
-    float noiseB =  fract(noise*1.3453)*2.0-1.0;
-    float noiseA =  fract(noise*1.3647)*2.0-1.0;
+    float noiseR = fract(noise)*2.0-1.0;
+    float noiseG = fract(noise*1.2154)*2.0-1.0; 
+    float noiseB = fract(noise*1.3453)*2.0-1.0;
+    float noiseA = fract(noise*1.3647)*2.0-1.0;
     
     return vec4(noiseR,noiseG,noiseB,noiseA);
 }
 
 vec3 fblur(vec2 uv){
     float samples = 16;
     vec2 resolution = vec2(bgl_RenderedTextureWidth, bgl_RenderedTextureHeight);
@@ -201,29 +201,29 @@
 
 
 class Droplets(Filter2D):
 
     def __init__(self, color=(1, 1, 1), speed=1.0, blur=0.0, idx: int = None) -> None:
         now = logic.getRealTime()
         self.speed = speed
-        self.settings = {
+        self.uniforms = {
             'blur': float(blur),
             'color': Vector(color),
             'timer': float(now),
             'time': float(100.0),
             'randomtime': float(logic.getRandomFloat())
         }
         self._last_time = now
         self.randomize()
         super().__init__(glsl, idx, {
-            'blur': self.settings,
-            'color': self.settings,
-            'timer': self.settings,
-            'time': self.settings,
-            'randomtime': self.settings
+            'blur': self.uniforms,
+            'color': self.uniforms,
+            'timer': self.uniforms,
+            'time': self.uniforms,
+            'randomtime': self.uniforms
         })
 
     def update(self):
         now = logic.getRealTime()
         diff = (now - self._last_time) * self.speed
         self.timer += diff
         self._last_time = now
@@ -236,44 +236,44 @@
     def restart(self):
         self.randomize()
         self.time = 0.0
         self.timer = 0.0
 
     @property
     def blur(self):
-        return self.settings['blur']
+        return self.uniforms['blur']
 
     @blur.setter
     def blur(self, val):
-        self.settings['blur'] = float(val)
+        self.uniforms['blur'] = float(val)
 
     @property
     def color(self):
-        return self.settings['color']
+        return self.uniforms['color']
 
     @color.setter
     def color(self, val):
-        self.settings['color'] = Vector(val).to_3d()
+        self.uniforms['color'] = Vector(val).to_3d()
 
     @property
     def timer(self):
-        return self.settings['timer']
+        return self.uniforms['timer']
 
     @timer.setter
     def timer(self, val):
-        self.settings['timer'] = float(val)
+        self.uniforms['timer'] = float(val)
 
     @property
     def randomtime(self):
-        return self.settings['randomtime']
+        return self.uniforms['randomtime']
 
     @randomtime.setter
     def randomtime(self, val):
-        self.settings['randomtime'] = float(val)
+        self.uniforms['randomtime'] = float(val)
 
     @property
     def time(self):
-        return self.settings['time']
+        return self.uniforms['time']
 
     @time.setter
     def time(self, val):
-        self.settings['time'] = float(val)
+        self.uniforms['time'] = float(val)
```

### Comparing `uplogic-2.2/uplogic/shaders/fxaa.py` & `uplogic-3.2/uplogic/shaders/fxaa.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/shaders/grayscale.py` & `uplogic-3.2/uplogic/shaders/grayscale.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 }
 """
 
 
 class Grayscale(Filter2D):
 
     def __init__(self, power: float = 1.0, idx: int = None) -> None:
-        self.settings = {'power': float(power)}
-        super().__init__(glsl, idx, {'power': self.settings, 'color': self.settings})
+        self.uniforms = {'power': float(power)}
+        super().__init__(glsl, idx, {'power': self.uniforms})
 
     @property
     def power(self):
-        return self.settings['power']
+        return self.uniforms['power']
 
     @power.setter
     def power(self, val):
-        self.settings['power'] = val
+        self.uniforms['power'] = val
```

### Comparing `uplogic-2.2/uplogic/shaders/hbao.py` & `uplogic-3.2/uplogic/shaders/hbao.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 uniform sampler2D bgl_RenderedTexture;
 uniform float bgl_RenderedTextureWidth;
 uniform float bgl_RenderedTextureHeight;
 uniform float power;
 in vec4 bgl_TexCoord;
 out vec4 fragColor;
 
-//THIS NEEDS TO MATCH YOUR CAMERA SETTINGS---------------------
+//THIS NEEDS TO MATCH YOUR CAMERA uniforms---------------------
 uniform float znear;                    //Z-near
 uniform float zfar;                     //Z-far
 uniform float fov;                      //FoV
 //-------------------------------------------------------------
 
 //USER VARIABLES-----------------------------------------------
 const float intensity = 1.0;            //Intensity of the AO effect
@@ -300,35 +300,35 @@
 """
 
 
 class HBAO(Filter2D):
 
     def __init__(self, power=1.0, idx: int = None) -> None:
         cam = logic.getCurrentScene().active_camera
-        self.settings = {
+        self.uniforms = {
             'power': float(power),
             'znear': cam.near,
             'zfar': cam.far,
             'fov': cam.fov
         }
         super().__init__(glsl, idx, {
-            'power': self.settings,
-            'znear': self.settings,
-            'zfar': self.settings,
-            'fov': self.settings
+            'power': self.uniforms,
+            'znear': self.uniforms,
+            'zfar': self.uniforms,
+            'fov': self.uniforms
         })
 
     @property
     def power(self):
-        return self.settings['power']
+        return self.uniforms['power']
 
     @power.setter
     def power(self, val):
-        self.settings['power'] = val
+        self.uniforms['power'] = val
 
     def update(self):
         super().update()
         cam = logic.getCurrentScene().active_camera
-        self.settings['znear'] = cam.near
-        self.settings['zfar'] = cam.far
-        self.settings['fov'] = cam.fov
+        self.uniforms['znear'] = cam.near
+        self.uniforms['zfar'] = cam.far
+        self.uniforms['fov'] = cam.fov
```

### Comparing `uplogic-2.2/uplogic/shaders/lens.py` & `uplogic-3.2/uplogic/shaders/lens.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 }"""
 
 
 
 class Lens(Filter2D):
 
     def __init__(self, power=0.0, idx: int = None) -> None:
-        self.settings = {'power': float(power)}
-        super().__init__(glsl, idx, {'power': self.settings})
+        self.uniforms = {'power': float(power)}
+        super().__init__(glsl, idx, {'power': self.uniforms})
 
     @property
     def power(self):
-        return self.settings['power']
+        return self.uniforms['power']
 
     @power.setter
     def power(self, val):
-        self.settings['power'] = float(val)
+        self.uniforms['power'] = float(val)
```

### Comparing `uplogic-2.2/uplogic/shaders/letterbox.py` & `uplogic-3.2/uplogic/shaders/letterbox.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,25 +24,25 @@
 }
 """
 
 
 class Letterbox(Filter2D):
 
     def __init__(self, power: float = 1.0, factor: float = 0.1, idx: int = None) -> None:
-        self.settings = {'power': float(power), 'factor': float(factor)}
-        super().__init__(glsl, idx, {'power': self.settings, 'factor': self.settings})
+        self.uniforms = {'power': float(power), 'factor': float(factor)}
+        super().__init__(glsl, idx, {'power': self.uniforms, 'factor': self.uniforms})
 
     @property
     def power(self):
-        return self.settings['power']
+        return self.uniforms['power']
 
     @power.setter
     def power(self, val):
-        self.settings['power'] = float(val)
+        self.uniforms['power'] = float(val)
     
     @property
     def factor(self):
-        return self.settings['factor']
+        return self.uniforms['factor']
 
     @factor.setter
     def factor(self, val):
-        self.settings['factor'] = float(val)
+        self.uniforms['factor'] = float(val)
```

### Comparing `uplogic-2.2/uplogic/shaders/levels.py` & `uplogic-3.2/uplogic/shaders/levels.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     fragColor.a = 1.0;
 }
 """
 
 class Levels(Filter2D):
 
     def __init__(self, color=(1., 1., 1.), idx: int = None) -> None:
-        self.settings = {'color': Vector(color)}
-        super().__init__(glsl, idx, {'color': self.settings})
+        self.uniforms = {'color': Vector(color)}
+        super().__init__(glsl, idx, {'color': self.uniforms})
 
     @property
     def color(self):
-        return self.settings.get('color', Vector((0, 0, 0)))
+        return self.uniforms.get('color', Vector((0, 0, 0)))
 
     @color.setter
     def color(self, val):
-        self.settings['color'] = val
+        self.uniforms['color'] = val
```

### Comparing `uplogic-2.2/uplogic/shaders/mist.py` & `uplogic-3.2/uplogic/shaders/mist.py`

 * *Files 21% similar despite different names*

```diff
@@ -77,67 +77,67 @@
 """
 
 
 class Mist(Filter2D):
 
     def __init__(self, start=.1, density=0.5, color=(0.5, 0.7, 0.9), power=1.0, idx: int = None) -> None:
         cam = logic.getCurrentScene().active_camera
-        self.settings = {
+        self.uniforms = {
             'start': float(start),
             'density': float(density),
             'color': Vector(color),
             'power': float(power),
             'znear': cam.near,
             'zfar': cam.far,
             'fov': cam.fov,
             'aspect': render.getWindowWidth() / render.getWindowHeight()
         }
         super().__init__(glsl, idx, {
-            'start': self.settings,
-            'density': self.settings,
-            'color': self.settings,
-            'power': self.settings,
-            'znear': self.settings,
-            'zfar': self.settings,
-            'fov': self.settings,
-            'aspect': self.settings
+            'start': self.uniforms,
+            'density': self.uniforms,
+            'color': self.uniforms,
+            'power': self.uniforms,
+            'znear': self.uniforms,
+            'zfar': self.uniforms,
+            'fov': self.uniforms,
+            'aspect': self.uniforms
         })
 
     def update(self):
         super().update()
         cam = logic.getCurrentScene().active_camera
-        self.settings['znear'] = cam.near
-        self.settings['zfar'] = cam.far
-        self.settings['fov'] = cam.fov
-        self.settings['aspect'] = render.getWindowWidth() / render.getWindowHeight()
+        self.uniforms['znear'] = cam.near
+        self.uniforms['zfar'] = cam.far
+        self.uniforms['fov'] = cam.fov
+        self.uniforms['aspect'] = render.getWindowWidth() / render.getWindowHeight()
 
     @property
     def start(self):
-        return self.settings['start']
+        return self.uniforms['start']
 
     @start.setter
     def start(self, val):
-        self.settings['start'] = float(val)
+        self.uniforms['start'] = float(val)
 
     @property
     def density(self):
-        return self.settings['density']
+        return self.uniforms['density']
 
     @density.setter
     def density(self, val):
-        self.settings['density'] = float(val)
+        self.uniforms['density'] = float(val)
 
     @property
     def power(self):
-        return self.settings['power']
+        return self.uniforms['power']
 
     @power.setter
     def power(self, val):
-        self.settings['power'] = val
+        self.uniforms['power'] = val
 
     @property
     def color(self):
-        return self.settings['color']
+        return self.uniforms['color']
 
     @color.setter
     def color(self, val):
-        self.settings['color'] = Vector(val).to_3d()
+        self.uniforms['color'] = Vector(val).to_3d()
```

### Comparing `uplogic-2.2/uplogic/shaders/rendertoscreen.py` & `uplogic-3.2/uplogic/shaders/rendertoscreen.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/shaders/shader.py` & `uplogic-3.2/uplogic/shaders/shader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from bge import logic
 from mathutils import Vector, Matrix
 from uplogic.utils.errors import PassIndexOccupiedError
-from uplogic.utils import debug
+from uplogic.console import debug, warning
 from pathlib import Path
 import bpy, bge
 
 
 def load_glsl(filepath: str):
     return Path(filepath).read_text()
 
@@ -20,24 +20,24 @@
 
 
 def set_filter_state(pass_idx, state=True):
     filter = FilterSystem.get_filter(pass_idx)
     filter.active = state
 
 
-class ULFilter():
+class Filter2D():
     '''Wrapper for KX_2DFilter.
 
     :param `program`: GLSL code as `str`.
     :param `idx`: Pass Index for this filter.
     :param `uniforms`: A `dict` of [`str`: `dict`] binding dictionary values to
     the filter in the form "key of dictionary".
     '''
 
-    _deprecated = True
+    _deprecated = False
 
     @property
     def active(self):
         return self._filter.enabled
 
     @active.setter
     def active(self, val):
@@ -61,14 +61,24 @@
         self.idx = idx
         scene = logic.getCurrentScene()
         self.manager = scene.filterManager
         self._uniforms = uniforms
         self._filter = None
         FilterSystem.add_filter(self)
 
+    @property
+    def settings(self):
+        warning('"Filter2D.settings" will be replaced by "Filter2D.uniforms" in future releases!')
+        return self.uniforms
+
+    @settings.setter
+    def settings(self, val):
+        warning('"Filter2D.settings" will be replaced by "Filter2D.uniforms" in future releases!')
+        self.uniforms = val
+
     def startup(self):
         if FilterSystem.filters.get(self.idx) is not None:
             raise PassIndexOccupiedError(self.idx)
         FilterSystem.filters[self.idx] = self
         self._filter = self.manager.addFilter(self.idx, 12, self.program)
         uniforms = self._uniforms
         for uniform in uniforms:
@@ -133,21 +143,19 @@
                         [value[3][0], value[2][1], value[3][2], value[3][3]]
                     ),
                 )
         elif cls is bpy.types.Image:
             self._filter.setTexture(0, value.bindcode, name)
 
 
-class Filter2D(ULFilter):
-    _deprecated = False
-
+class ULFilter(Filter2D):
+    _deprecated = True
 
-class Attachment2D(ULFilter):
 
-    _deprecated = False
+class Attachment2D(Filter2D):
 
     def __init__(self, program: str, idx: int = None, uniforms: dict = {}) -> None:
         super().__init__(program, idx, uniforms)
 
 
 class FilterSystem:
     filters: dict[Filter2D] = {}
```

### Comparing `uplogic-2.2/uplogic/shaders/sharpen.py` & `uplogic-3.2/uplogic/shaders/sharpen.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,17 +70,17 @@
 }
 """
 
 
 class Sharpen(Filter2D):
 
     def __init__(self, sharpness=0.0, idx: int = None) -> None:
-        self.settings = {'sharpness': float(sharpness)}
-        super().__init__(glsl, idx, {'sharpness': self.settings})
+        self.uniforms = {'sharpness': float(sharpness)}
+        super().__init__(glsl, idx, {'sharpness': self.uniforms})
 
     @property
     def sharpness(self):
-        return self.settings['sharpness']
+        return self.uniforms['sharpness']
 
     @sharpness.setter
     def sharpness(self, val):
-        self.settings['sharpness'] = val
+        self.uniforms['sharpness'] = val
```

### Comparing `uplogic-2.2/uplogic/shaders/splitscreen.py` & `uplogic-3.2/uplogic/shaders/splitscreen.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/shaders/ssao.py` & `uplogic-3.2/uplogic/shaders/ssao.py`

 * *Files 4% similar despite different names*

```diff
@@ -184,31 +184,31 @@
 """
 
 
 class SSAO(Filter2D):
 
     def __init__(self, power=1.0, idx: int = None) -> None:
         cam = logic.getCurrentScene().active_camera
-        self.settings = {
+        self.uniforms = {
 			'power': float(power),
             'znear': cam.near,
             'zfar': cam.far
         }
         super().__init__(glsl, idx, {
-			'power': self.settings,
-            'znear': self.settings,
-            'zfar': self.settings
+			'power': self.uniforms,
+            'znear': self.uniforms,
+            'zfar': self.uniforms
         })
 
     @property
     def power(self):
-        return self.settings['power']
+        return self.uniforms['power']
 
     @power.setter
     def power(self, val):
-        self.settings['power'] = val
+        self.uniforms['power'] = val
 
     def update(self):
         super().update()
         cam = logic.getCurrentScene().active_camera
-        self.settings['znear'] = cam.near
-        self.settings['zfar'] = cam.far
+        self.uniforms['znear'] = cam.near
+        self.uniforms['zfar'] = cam.far
```

### Comparing `uplogic-2.2/uplogic/shaders/texture.py` & `uplogic-3.2/uplogic/shaders/texture.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,43 +47,47 @@
 class Texture(Filter2D):
 
     def __init__(self, texture: bpy.types.Image = None, opacity: float = 1.0, pos=Vector((0, 0)), size=Vector((1, 1)), idx: int = None) -> None:
         if not isinstance(texture, bpy.types.Image):
             error("'Texture': first argument requires an object of type 'bpy.types.Image'!")
             return
         texture.gl_load()
-        self.settings = {'tex': texture, 'opacity': float(opacity), 'pos': Vector(pos), 'size': Vector(size)}
-        super().__init__(glsl, idx, {'tex': self.settings, 'opacity': self.settings, 'pos': self.settings, 'size': self.settings})
+        self.free_textures = True
+        self.uniforms = {'tex': texture, 'opacity': float(opacity), 'pos': Vector(pos), 'size': Vector(size)}
+        super().__init__(glsl, idx, {'tex': self.uniforms, 'opacity': self.uniforms, 'pos': self.uniforms, 'size': self.uniforms})
 
     @property
     def texture(self):
-        return self.settings['tex']
+        return self.uniforms['tex']
 
     @texture.setter
     def texture(self, val):
+        if self.free_textures:
+            self.uniforms['tex'].gl_free()
         if not isinstance(val, bpy.types.Image):
             raise TypeError
-        self.settings['tex'] = val
+        val.gl_load()
+        self.uniforms['tex'] = val
 
     @property
     def opacity(self):
-        return self.settings['opacity']
+        return self.uniforms['opacity']
 
     @opacity.setter
     def opacity(self, val):
-        self.settings['opacity'] = float(val)
+        self.uniforms['opacity'] = float(val)
 
     @property
     def pos(self):
-        return self.settings['pos']
+        return self.uniforms['pos']
 
     @pos.setter
     def pos(self, val):
-        self.settings['pos'] = Vector(val).to_2d()
+        self.uniforms['pos'] = Vector(val).to_2d()
 
     @property
     def size(self):
-        return self.settings['size']
+        return self.uniforms['size']
 
     @size.setter
     def size(self, val):
-        self.settings['size'] = Vector(val).to_2d()
+        self.uniforms['size'] = Vector(val).to_2d()
```

### Comparing `uplogic-2.2/uplogic/shaders/vignette.py` & `uplogic-3.2/uplogic/shaders/vignette.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,27 +24,27 @@
 }
 """
 
 
 class Vignette(Filter2D):
 
     def __init__(self, power: float = 0.25, color=(0., 0., 0.), idx: int = None) -> None:
-        self.settings = {'power': float(power), 'color': Vector(color)}
-        super().__init__(glsl, idx, {'power': self.settings, 'color': self.settings})
+        self.uniforms = {'power': float(power), 'color': Vector(color)}
+        super().__init__(glsl, idx, {'power': self.uniforms, 'color': self.uniforms})
 
     @property
     def power(self):
-        return self.settings['power']
+        return self.uniforms['power']
 
     @power.setter
     def power(self, val):
-        self.settings['power'] = val
+        self.uniforms['power'] = val
 
     @property
     def color(self):
-        return self.settings['color']
+        return self.uniforms['color']
 
     @color.setter
     def color(self, val):
         if not isinstance(val, Vector):
             val = Vector(val)
-        self.settings['color'] = val
+        self.uniforms['color'] = val
```

### Comparing `uplogic-2.2/uplogic/ui/__init__.py` & `uplogic-3.2/uplogic/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/ui/behaviors.py` & `uplogic-3.2/uplogic/ui/behaviors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from bge import render
 from uplogic.input import MOUSE
 from uplogic.input.mouse import MOUSE_EVENTS, LMB, RMB
 from mathutils import Vector
+from uplogic.utils.math import rotate2d
 
 
 class HoverBehavior():
     @property
     def hover(self):
         if not self.active:
             return False
         screen_size = [render.getWindowWidth(), render.getWindowHeight()]
-        mpos = Vector((MOUSE.position.x, 1 - MOUSE.position.y))
+        mpos = Vector((MOUSE.position.x * screen_size[0], (1 - MOUSE.position.y) * screen_size[1]))
+        mpos = rotate2d(mpos, self.pivot, -self._draw_angle)
         dsize = self._draw_size
-        return (
-            self.pos_abs[0] <= mpos.x * screen_size[0] <= self.pos_abs[0] + dsize[0] and
-            self.pos_abs[1] <= mpos.y * screen_size[1] <= self.pos_abs[1] + dsize[1] and
+        is_hover = (
+            self.pos_abs[0] <= mpos.x <= self.pos_abs[0] + dsize[0] and
+            self.pos_abs[1] <= mpos.y <= self.pos_abs[1] + dsize[1] and
             not self.canvas._hover_consumed
         )
+        return is_hover
 
 
 class MouseListener():
     """Mixin class for widgets that need mouse input.
 
     You will need to call `MouseListener.evaluate(self)` to update the behavior state.\n
     This data is independent of hovering, it just gives generic mouse button information.
```

### Comparing `uplogic-2.2/uplogic/ui/button.py` & `uplogic-3.2/uplogic/ui/button.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         self._clicked = False
         self._released = False
         self._in_focus = False
         self._down = False
         self._hover = False
         if on_press is not None:
             self.on_press = on_press
+        self.start()
 
     @property
     def border_color(self):
         return self._border_color
 
     @border_color.setter
     def border_color(self, val):
@@ -61,15 +62,15 @@
 
     @hover_color.setter
     def hover_color(self, val):
         self._hover_color = list(val)
 
     @property
     def current_color(self):
-        return self.click_color if self._clicked else (self.hover_color if self._in_focus else self.bg_color).copy()
+        return self.click_color if self._clicked or self._down else (self.hover_color if self._in_focus else self.bg_color).copy()
 
     def draw(self):
         super()._setup_draw()
         self._released = False
         gpu.state.line_width_set(self.border_width)
         gpu.state.point_size_set(self.border_width)
         col = self.override_color if self.override_color is not None else self.current_color
@@ -94,29 +95,28 @@
         self._hover = self.hover
         if self._hover:
             self._in_focus = True
             self.on_hover(self)
             self.canvas._hover_consumed = True
         else:
             self._in_focus = False
-        if self._in_focus and MOUSE_EVENTS[LMB].active and not self.canvas._click_consumed:
+        if self._in_focus and MOUSE_EVENTS[LMB].active and not self.canvas._click_consumed and not self._down:
             self.on_click(self)
             self.on_press(self)
             self._clicked = True
             self.canvas._click_consumed = True
             self._down = True
         elif not MOUSE_EVENTS[LMB].active and self._down:
             self.on_release(self)
             self._down = False
             self._released = True
-            self.canvas._click_consumed = False
         elif self._down:
+            self.canvas._click_consumed = True
             self.on_hold(self)
         self.override_color = None
-        
 
     def on_enter(self, widget):
         pass
 
     def on_exit(self, widget):
         pass
 
@@ -185,14 +185,15 @@
             halign=halign,
             valign=valign,
             angle=angle,
             on_press=on_press
         )
         self.add_widget(self.label)
         self._in_focus = False
+        self.start()
 
     @property
     def text(self):
         return self.label.text
 
     @text.setter
     def text(self, val):
@@ -277,14 +278,15 @@
         super().__init__(pos, size, bg_color, relative, halign=halign, valign=valign, angle=angle, on_press=on_press, hover_color=hover_color, border_color=border_color, click_color=click_color)
         self.image = Image(relative={'size': True}, size=(1, 1), texture=texture)
         self._texture_name = texture
         self.idle_texture = texture
         self.hover_texture = hover_texture if hover_texture else texture
         self.click_texture = click_texture if click_texture else texture
         self.add_widget(self.image)
+        self.start()
 
     @property
     def texture(self):
         return self.image.texture
 
     @texture.setter
     def texture(self, val):
@@ -329,14 +331,15 @@
         self.image = Sprite(relative={'size': True}, size=(1, 1), texture=texture, rows=rows, cols=cols, idx=idx)
         self._texture_name = texture
 
         self.idle_texture = texture
         self.hover_texture = hover_texture if hover_texture else texture
         self.click_texture = click_texture if click_texture else texture
         self.add_widget(self.image)
+        self.start()
 
     @property
     def texture(self):
         return self.image.texture
 
     @texture.setter
     def texture(self, val):
```

### Comparing `uplogic-2.2/uplogic/ui/camera.py` & `uplogic-3.2/uplogic/ui/camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 
 class Camera(Widget):
 
     def __init__(self, pos=[0, 0], size=(100, 100), relative={}, camera=None, halign='left', valign='bottom') -> None:
         self.camera = camera
         Widget.__init__(self, pos, size, (0, 0, 0, 0), relative, halign, valign, 0)
+        self.start()
 
     @property
     def parent(self):
         """The widget whose position and size to use relatively."""
         return self._parent
 
     @parent.setter
```

### Comparing `uplogic-2.2/uplogic/ui/canvas.py` & `uplogic-3.2/uplogic/ui/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         self._hover_consumed = False
         self._click_consumed = False
         self._old_width = bge.render.getWindowWidth()
         self._old_height = bge.render.getWindowHeight()
         self.use_clipping = False
         self._to_evaluate: list[Widget] = []
         bge.logic.getCurrentScene().post_draw.append(self.draw)
+        self.start()
 
     def remove(self):
         while self.draw in bge.logic.getCurrentScene().post_draw:
             bge.logic.getCurrentScene().post_draw.remove(self.draw)
 
     def fetch_size(self):
         for c in self.children:
@@ -72,14 +73,15 @@
         self._old_width = width
         self._old_height = height
         if not self.show:
             return
         gpu.state.blend_set('ALPHA')
         super().draw()
         self._hover_consumed = False
+        self._click_consumed = False
         for w in self._to_evaluate.__reversed__():
             w.evaluate()
         while self._to_evaluate:
             self._to_evaluate.pop().update()
 
     def update(self):
         pass
```

### Comparing `uplogic-2.2/uplogic/ui/cursor.py` & `uplogic-3.2/uplogic/ui/cursor.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,25 +23,23 @@
 class Cursor(Widget):
 
     def __init__(self, texture=None, size=(30,30), offset=(0, 0), rows=1, cols=1, idx=0):
         self.offset = offset
         self.rows = rows
         self.cols = cols
         self._idx = idx
-        # self._idx = 0
-        # self._rows = 1
-        # self._cols = 1
         remove_custom_cursor()
         super().__init__(MOUSE.position, size)
         self._texture = None
         self._shader = None
         self.texture = texture
         self.pos = MOUSE.position
         self._last_visible = logic.mouse.visible
         bge.logic.getCurrentScene().post_draw.append(self._draw_custom_cursor)
+        self.start()
 
     @property
     def idx(self):
         return self._idx
 
     @idx.setter
     def idx(self, val):
```

### Comparing `uplogic-2.2/uplogic/ui/image.py` & `uplogic-3.2/uplogic/ui/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     def __init__(self, pos=[0, 0], size=(100, 100), relative={}, texture=None, halign='left', valign='bottom', use_aspect_ratio: bool = True, angle=0):
         self._texture = None
         self._image = None
         self.use_aspect_ratio = use_aspect_ratio
         self._opacity = 1
         super().__init__(pos, size, relative=relative, halign=halign, valign=valign, angle=angle)
         self.texture = texture
+        self.start()
 
     @property
     def texture(self):
         return self._texture
 
     @property
     def aspect_ratio(self):
```

### Comparing `uplogic-2.2/uplogic/ui/label.py` & `uplogic-3.2/uplogic/ui/label.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         self.font_color = font_color
         self.font = font
         self.wrap = wrap
         self.lines = []
         Widget.__init__(self, pos, (0, 0), (0, 0, 0, 0), relative, angle=angle)
         self.text_halign = halign
         self.text_valign = valign
+        self.start()
 
     @property
     def text(self):
         return self._text
 
     @text.setter
     def text(self, val):
@@ -140,14 +141,16 @@
         self.relative['size'] = size
         self.text_halign = halign
         self.text_valign = valign
         return self
 
     def draw(self):
         super()._setup_draw()
+        if self.parent is None:
+            return
         parsize = self.parent._draw_size
         relative = self.relative.get('font_size', False)
         font = self.font
         blf.size(font, parsize[1] * self.font_size if relative else self.font_size)
         col = self.font_color
         blf.color(font, col[0], col[1], col[2], col[3] * self.opacity)
         charsize = blf.dimensions(font, 'A')
```

### Comparing `uplogic-2.2/uplogic/ui/layout.py` & `uplogic-3.2/uplogic/ui/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         halign: str = 'left',
         valign: str = 'bottom',
         angle=0
     ):
         self.border_width = border_width
         self.border_color = border_color
         super().__init__(pos, size, bg_color, relative, halign=halign, valign=valign, angle=angle)
+        self.start()
 
     @property
     def border_color(self):
         return self._border_color
 
     @border_color.setter
     def border_color(self, color):
@@ -183,14 +184,15 @@
             angle=0
         ):
         self.orientation = orientation
         self.spacing = spacing
         self.children_align = ['left', 'bottom']
         super().__init__(pos, size, bg_color, relative, border_width, border_color, halign=halign, valign=valign, angle=angle)
         self.use_clipping = False
+        self.start()
 
     def arrange(self):
         '''Arrange the widgets according to the specified orientation.'''
         dsize = self._draw_size
         arrange_factor = {
             'left': 0,
             'center': .5,
@@ -264,14 +266,15 @@
             spacing,
             halign,
             valign,
             angle=angle
         )
         self.rows = rows
         self.cols = cols
+        self.start()
 
     def add_widget(self, widget):
         max = self.rows * self.cols
         if len(self.children) < max:
             super().add_widget(widget)
             self.arrange()
 
@@ -341,14 +344,15 @@
             border_color,
             halign,
             valign,
             angle
         )
         self.starting_angle = starting_angle
         self.distance = distance
+        self.start()
 
     @property
     def starting_angle(self):
         return self._starting_angle
 
     @starting_angle.setter
     def starting_angle(self, val):
```

### Comparing `uplogic-2.2/uplogic/ui/path.py` & `uplogic-3.2/uplogic/ui/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         line_color=(1.0, 1.0, 1.0, 1.0),
         angle=0
     ):
         Widget.__init__(self, pos, (0, 0), (0, 0, 0, 0), relative=relative, angle=angle)
         self.points = points
         self.line_color = line_color
         self.line_width = line_width
+        self.start()
 
     @property
     def line_color(self) -> list:
         return self._line_color
 
     @line_color.setter
     def line_color(self, val):
@@ -96,14 +97,15 @@
         line_width=1,
         line_color=(1.0, 1.0, 1.0, 1.0)
     ):
         Widget.__init__(self, (0, 0), (0, 0), (0, 0, 0, 0))
         self.points = points
         self.line_color = line_color
         self.line_width = line_width
+        self.start()
     
     def _build_shader(self):
         if self.parent is None:
             return
         points = []
         for point in self.points:
             point = world_to_screen(point)
@@ -124,14 +126,15 @@
         line_width=1,
         line_color=(1.0, 1.0, 1.0, 1.0)
     ):
         Widget.__init__(self, (0, 0), (0, 0), (0, 0, 0, 0))
         self.object: KX_GameObject = object
         self.line_color = line_color
         self.line_width = line_width
+        self.start()
 
     def _build_shader(self):
         if self.parent is None:
             return
         points = []
         mesh = self.object.blenderObject.data
         for edge in mesh.edges:
```

### Comparing `uplogic-2.2/uplogic/ui/render.py` & `uplogic-3.2/uplogic/ui/render.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 class RenderedTexture(Widget):
 
     def __init__(self):
         super().__init__()
         self.buffer = Buffer()
+        self.start()
 
     def _build_shader(self):
         size = self._draw_size
         self.view = gpu.types.GPUOffScreen(size[0], size[1])
 
         pos = self._draw_pos
         size = self._draw_size
```

### Comparing `uplogic-2.2/uplogic/ui/slider.py` & `uplogic-3.2/uplogic/ui/slider.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         self.add_widget(self.knob)
         self.steps = steps
         self.value = 0
         self._clicked = False
         self._released = False
         self._in_focus = False
         self._down = False
+        self.start()
 
     @property
     def parent(self):
         return self._parent
 
     @parent.setter
     def parent(self, val):
@@ -177,25 +178,27 @@
         self.add_widget(self.knob)
         self.steps = steps
         self.value = 0
         self._clicked = False
         self._released = False
         self._in_focus = False
         self._down = False
+        self.start()
 
 
 class ProgressSlider(FrameSlider):
 
     def __init__(self, pos=[0, 0], size=[100, 10], relative={}, halign='left', valign='bottom', orientation='horizontal', border_width=1, border_color=(0.8, 0.8, 0.8, 1), bg_color=(0, 0, 0, 0), bar_color=(1, 1, 1, 1), bar_hover_color=(0.1, 0.1, 0.1, 0.3), steps=-1, allow_bar_click=True, angle=0):
         self.bar = None
         self.knob = None
         super().__init__(pos, size, relative, halign, valign, orientation, border_width, border_color, bg_color, bar_color, bar_hover_color, steps, allow_bar_click, angle)
         self.knob.relative = {'size': True}
         self.knob.halign = 'left'
         self.knob.valign = 'bottom'
+        self.start()
 
     @property
     def value(self):
         return self._value
 
     @value.setter
     def value(self, value):
```

### Comparing `uplogic-2.2/uplogic/ui/textinput.py` & `uplogic-3.2/uplogic/ui/textinput.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,28 +42,30 @@
         shadow_color=[.0, .0, .0, 1.0],
         halign='left',
         valign='bottom',
         wrap=False,
         multiline=False,
         angle=0
     ):
+        self.lines = None
+        self.cursor_evt = None
+        self.cursor = Layout(bg_color=(1, 1, 1, 1), size=(0, 0))
+        self.cursor_flash_time = .5
         Label.__init__(self, pos, relative, text, font, font_color, font_size, line_height, shadow, shadow_offset, shadow_color, halign, valign, wrap, angle)
+        self.add_widget(self.cursor)
         self._key_evts = {}
         events = logic.keyboard.inputs.copy()
-        self.cursor_evt = None
         for evt in events.values():
             self._key_evts[evt] = 0.0
         self.multiline = multiline
-        self.cursor = Layout(bg_color=(1, 1, 1, 1), size=(0, 0))
-        self.add_widget(self.cursor)
         self.edit = False
         self._index = 0
         self.line_index = 0
         self.character_index = 0
-        self.cursor_flash_time = .3
+        self.start()
 
     def on_enter(self):
         self.edit = False
 
     @property
     def edit(self):
         return self._edit
@@ -104,16 +106,25 @@
 
     @property
     def text(self):
         return self._text
 
     @text.setter
     def text(self, val):
+        if self.cursor_evt:
+            self.cursor_evt.cancel()
+        self.cursor.show = False
+        self._cursor_visible()
         self._text = str(val)
 
+    def move_cursor_to_end(self):
+        line_length = len(self.lines[clamp(self.line_index, 0, len(self.lines) - 1)])
+        self.index = len(self.text) #line_length - self.character_index
+        self.edit = True
+
     def write(self, text):
         self.text += text
         self.index = len(self.text)
 
     @property
     def _current_char_pos(self):
         self.index = self.index
@@ -152,16 +163,14 @@
 
     def _listen(self):
         left_shift = logic.keyboard.inputs[events.LEFTSHIFTKEY].active
         right_shift = logic.keyboard.inputs[events.RIGHTSHIFTKEY].active
         keyboard_events = logic.keyboard.inputs.copy()
         tpf = (1 / (logic.getAverageFrameRate() or 0.01))
 
-        # print(logic.keyboard.activeInputs)
-
         for evt in keyboard_events.values():
 
             text = self.text
             if evt.active and self._key_evts[evt] == 0.0:
                 self._key_evts[evt] += tpf
                 if evt.type == 59:
                     self.text = text[:self.index][:-1] + text[self.index:]  # Backspace:
```

### Comparing `uplogic-2.2/uplogic/ui/widget.py` & `uplogic-3.2/uplogic/ui/widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import gpu
 from gpu_extras.batch import batch_for_shader
 from uplogic.utils.math import rotate2d
+from uplogic.events import schedule
 from mathutils import Vector
 
 
 class Widget():
     '''The widget Base class. a Widget has all the basic logic about
     sizing and positioning, but has no visual representation.
 
@@ -55,18 +56,17 @@
         self._vertices = None  # (Vector((0, 0)), Vector((0, 0)), Vector((0, 0)), Vector((0, 0)))
         self.angle = angle
         self._build_shader()
         self._clipped = [0, 0]
         self.use_clipping = False
         self.copy_height = False
         self.copy_width = False
-        self.opacity = 1
+        self.opacity = 1.
         self.z = 0
         self._active = True
-        self.start()
 
     def toggle(self, *args):
         """Toggle the widget on/off."""
         self.show = not self.show
 
     def set_visible(self, flag=True):
         self.show = flag
@@ -100,28 +100,29 @@
     @active.setter
     def active(self, val):
         self._active = val
 
     @property
     def show(self):
         """If `False`, this widget and all its children will not be rendered."""
-        return self._show
+        pshow = self.parent.show if self.parent is not None else True
+        return self._show and pshow
 
     @show.setter
     def show(self, val):
         if val != self._show:
             self._show = val
             if val:
                 self._rebuild = True
                 for child in self.children:
                     child.pos = child.pos
 
     @property
     def _children_reversed(self):
-        return self.children.__reversed__()
+        return list(self.children.__reversed__())
 
     @property
     def canvas(self):
         """Find the canvas this widget is attached to."""
         pa = self
         while pa.parent is not None:
             pa = pa.parent
@@ -160,15 +161,15 @@
     def _recurse(self):
         widgets = [self]
         for w in self.children:
             widgets.extend(w._recurse)
         return widgets
 
     @property
-    def childrenRecursive(self):
+    def childrenRecursive(self) -> list:
         """All children and children's children of this widget."""
         widgets = []
         for w in self.children:
             widgets.extend(w._recurse)
         return widgets
 
     @property
@@ -509,15 +510,15 @@
         for c in self.children:
             z = c._set_z(z)
         return z
 
     def remove_widget(self, widget):
         '''Remove a `Widget` from this widget.
 
-        :param `widget`: `Widget` which to remove.
+        :param `widget`: `Widget` to remove.
         '''
         if widget in self.children:
             self.children.remove(widget)
             widget.parent = None
 
     def remove(self):
         if self.parent:
```

### Comparing `uplogic-2.2/uplogic/utils/__init__.py` & `uplogic-3.2/uplogic/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -224,23 +224,29 @@
     return distances[min(distances.keys())]
 
 
 def is_water(game_object: GameObject):
     return WATER in game_object.getPropertyNames()
 
 
-def get_child_by_name(obj, child, recursive=True, partial=False):
+def get_child_by_name(obj: GameObject, child: str, recursive: bool = True, partial: bool = False) -> GameObject:
+    """Get a named child object.
+
+    :param `obj`: The parent object.
+    :param `child`: The child's name.
+    :param `recursive`: If True, children's children will be seached too.
+    :param `partial`: If a child object name has the given name in it, it counts as a hit.
+    """
     children = obj.childrenRecursive if recursive else obj.children
     if partial:
         for c in children:
             if child in c.name:
                 return c
     else:
         return children.get(child)
 
 
-def check_vr_session_status() -> tuple[Vector, Matrix]:
-    """Get the current position and orientation of connected VR headset.
-    :returns: `tuple` of (`Vector`, `Matrix`)
+def check_vr_session_status() -> bool:
+    """Check if a VR session is currently running.
     """
     session = bpy.context.window_manager.xr_session_state
     return session is not None
```

### Comparing `uplogic-2.2/uplogic/utils/constants.py` & `uplogic-3.2/uplogic/utils/constants.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/utils/engine.py` & `uplogic-3.2/uplogic/utils/engine.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/utils/errors.py` & `uplogic-3.2/uplogic/utils/errors.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/utils/lights.py` & `uplogic-3.2/uplogic/utils/lights.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     is the same as the original argument.
     '''
     lamp = light.blenderObject
     lamp.data = lamp.data.copy()
     return light
 
 
-class ULLight(GameObject):
+class Light(GameObject):
     """Wrapper for `KX_LightObject`. Can either convert a given scene light or create a new one.
 
     :param `name`: The name of the new light (only relevant if `light` argument is None).
     :param `type`: The type of the new light of [`"POINT"`, `"SUN"`, `"SPOT"`, `"AREA"`] (only relevant if `light` argument is None).
     :param `light`: The scene light to be converted. Leave at `None` to create new.
     """
 
-    _deprecated = True
+    _deprecated = False
 
     def __init__(
         self,
         name: str = '',
         type: str = 'POINT',
         light: KX_GameObject = None
     ) -> None:
@@ -135,9 +135,9 @@
         return self.game_object.blenderObject.data.shadow_soft_size
 
     @radius.setter
     def radius(self, val: float):
         self.game_object.blenderObject.data.shadow_soft_size = val
 
 
-class Light(ULLight):
-    _deprecated = False
+class ULLight(Light):
+    _deprecated = True
```

### Comparing `uplogic-2.2/uplogic/utils/math.py` & `uplogic-3.2/uplogic/utils/math.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/utils/nodetrees.py` & `uplogic-3.2/uplogic/utils/nodetrees.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/utils/objects.py` & `uplogic-3.2/uplogic/utils/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     target_pos,
     front_axis_code=1,
     factor=1
 ):
     local = get_local(rotating_object, target_pos)
     front = Vector((1, 0)) if front_axis_code in [0, 3] else Vector((0, 1))
     if front_axis_code > 2:
-        print(front)
         front.negate()
     angle = Vector((local.x, local.y))
     if angle.length < .001:
         return
     angle = angle.angle_signed(front)
     rotating_object.applyRotation((0, 0, angle*factor), True)
 
@@ -76,15 +75,14 @@
 ):
     """Rotate an object around a local axis towards a point"""
     front = front_axis
     if front > 2:
         front -= 3
     if rotation_axis == front:
         return
-    print(front_axis)
     if rotation_axis == 0:
         xrot_to(
             object,
             target,
             front_axis,
             factor
         )
@@ -425,28 +423,28 @@
 
 
 def get_curve_length(curve: KX_GameObject):
     depsgraph = bpy.context.evaluated_depsgraph_get()
     return sum(s.calc_length() for s in curve.blenderObject.evaluated_get(depsgraph).data.splines)
 
 
-class ULCurve(GameObject):
+class Curve(GameObject):
     """Wrapper class for creating and handling curves more easily.
 
     :param `name`: Name of this curve object.
     :param `bevel_depth`: Define the "thickness" of the curve. This will add
     geometry along the spline.
     :param `dimensions`: Set the coordinate space in which to calculate the
     curve.
     :param `material`: The material to use for bevel geometry.
     :param `collection`: The collection to which to add the curve. Leave at
     `None` to use scene collection.
     """
 
-    _deprecated = True
+    _deprecated = False
 
     def __init__(
         self,
         name: str,
         bevel_depth: float = 0.0,
         dimensions: int = 3,
         material: str or Material =None,
@@ -521,16 +519,16 @@
         return self.blenderObject.data.path_duration
 
     @path_duration.setter
     def path_duration(self, val):
         self.game_object.blenderObject.data.path_duration = val
 
 
-class Curve(ULCurve):
-    _deprecated = False
+class ULCurve(Curve):
+    _deprecated = True
 
 
 class Mesh():
 
     def __init__(self, mesh: bpy.types.Mesh):
         self.blenderMesh: bpy.types.Mesh = mesh
```

### Comparing `uplogic-2.2/uplogic/utils/pooling.py` & `uplogic-3.2/uplogic/utils/pooling.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/utils/raycasting.py` & `uplogic-3.2/uplogic/utils/raycasting.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/utils/scene.py` & `uplogic-3.2/uplogic/utils/scene.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/utils/visualize.py` & `uplogic-3.2/uplogic/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic/utils/visuals.py` & `uplogic-3.2/uplogic/utils/visuals.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.2/uplogic.egg-info/PKG-INFO` & `uplogic-3.2/uplogic.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: uplogic
-Version: 2.2
+Version: 3.2
 Summary: Uplogic utility for UPBGE.
 Home-page: https://github.com/UPBGE/uplogic
 Author: Leopold Auersperg-Castell
 Author-email: lauersperg@gmx.at
 License: GPLv2
-Download-URL: https://github.com/UPBGE/uplogic/archive/refs/tags/v2.2.tar.gz
+Download-URL: https://github.com/UPBGE/uplogic/archive/refs/tags/v3.2.tar.gz
 Keywords: Blender UPBGE logic
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python
 License-File: LICENSE.md
```

