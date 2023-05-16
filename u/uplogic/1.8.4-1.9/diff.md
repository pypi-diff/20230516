# Comparing `tmp/uplogic-1.8.4.tar.gz` & `tmp/uplogic-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uplogic-1.8.4.tar", last modified: Wed May 10 20:13:56 2023, max compression
+gzip compressed data, was "uplogic-1.9.tar", last modified: Tue May 16 11:20:06 2023, max compression
```

## Comparing `uplogic-1.8.4.tar` & `uplogic-1.9.tar`

### file list

```diff
@@ -1,378 +1,387 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 20:13:56.825852 uplogic-1.8.4/
--rw-rw-rw-   0        0        0      189 2022-01-15 11:35:38.000000 uplogic-1.8.4/LICENSE.md
--rw-rw-rw-   0        0        0     1049 2023-05-10 20:13:56.824852 uplogic-1.8.4/PKG-INFO
--rw-rw-rw-   0        0        0      262 2022-01-15 11:34:53.000000 uplogic-1.8.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-10 20:13:56.825852 uplogic-1.8.4/setup.cfg
--rw-rw-rw-   0        0        0     1683 2023-05-10 20:13:47.000000 uplogic-1.8.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:13:56.377385 uplogic-1.8.4/uplogic/
--rw-rw-rw-   0        0        0     5915 2023-01-20 16:10:14.000000 uplogic-1.8.4/uplogic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:13:56.401389 uplogic-1.8.4/uplogic/animation/
--rw-rw-rw-   0        0        0      343 2023-03-08 12:02:42.000000 uplogic-1.8.4/uplogic/animation/__init__.py
--rw-rw-rw-   0        0        0    12450 2023-05-01 16:59:42.000000 uplogic-1.8.4/uplogic/animation/action.py
--rw-rw-rw-   0        0        0     4016 2023-05-01 17:00:05.000000 uplogic-1.8.4/uplogic/animation/actionsystem.py
--rw-rw-rw-   0        0        0     6248 2023-05-05 15:03:47.000000 uplogic-1.8.4/uplogic/animation/sequence.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:13:56.406391 uplogic-1.8.4/uplogic/audio/
--rw-rw-rw-   0        0        0      606 2023-03-06 09:07:59.000000 uplogic-1.8.4/uplogic/audio/__init__.py
--rw-rw-rw-   0        0        0     7689 2023-04-24 21:26:30.000000 uplogic-1.8.4/uplogic/audio/audiosystem.py
--rw-rw-rw-   0        0        0     6823 2023-05-10 20:12:46.000000 uplogic-1.8.4/uplogic/audio/music.py
--rw-rw-rw-   0        0        0    23827 2023-05-05 15:07:21.000000 uplogic-1.8.4/uplogic/audio/sound.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:13:56.410392 uplogic-1.8.4/uplogic/data/
--rw-rw-rw-   0        0        0     1861 2022-10-06 13:43:59.000000 uplogic-1.8.4/uplogic/data/__init__.py
--rw-rw-rw-   0        0        0     3122 2023-04-07 16:35:00.000000 uplogic-1.8.4/uplogic/data/file.py
--rw-rw-rw-   0        0        0     7181 2022-09-08 16:41:11.000000 uplogic-1.8.4/uplogic/data/globaldb.py
--rw-rw-rw-   0        0        0     2050 2021-12-21 09:41:07.000000 uplogic-1.8.4/uplogic/data/serializers.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:13:56.411392 uplogic-1.8.4/uplogic/decorators/
--rw-rw-rw-   0        0        0     9022 2023-04-02 15:18:30.000000 uplogic-1.8.4/uplogic/decorators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:13:56.412393 uplogic-1.8.4/uplogic/events/
--rw-rw-rw-   0        0        0     7615 2023-04-04 13:17:19.000000 uplogic-1.8.4/uplogic/events/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:13:56.418394 uplogic-1.8.4/uplogic/input/
--rw-rw-rw-   0        0        0     1494 2023-03-06 08:52:33.000000 uplogic-1.8.4/uplogic/input/__init__.py
--rw-rw-rw-   0        0        0    15072 2023-03-06 08:31:48.000000 uplogic-1.8.4/uplogic/input/gamepad.py
--rw-rw-rw-   0        0        0     9607 2023-01-16 12:00:44.000000 uplogic-1.8.4/uplogic/input/keyboard.py
--rw-rw-rw-   0        0        0    14940 2023-05-05 15:02:36.000000 uplogic-1.8.4/uplogic/input/mouse.py
--rw-rw-rw-   0        0        0     9137 2023-03-06 08:38:54.000000 uplogic-1.8.4/uplogic/input/vr.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:13:56.418394 uplogic-1.8.4/uplogic/logging/
--rw-rw-rw-   0        0        0     3520 2022-09-24 11:49:44.000000 uplogic-1.8.4/uplogic/logging/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:13:56.421395 uplogic-1.8.4/uplogic/nodes/
--rw-rw-rw-   0        0        0     5171 2023-01-05 15:29:44.000000 uplogic-1.8.4/uplogic/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:13:56.591731 uplogic-1.8.4/uplogic/nodes/actions/
--rw-rw-rw-   0        0        0     7855 2023-04-26 12:34:19.000000 uplogic-1.8.4/uplogic/nodes/actions/__init__.py
--rw-rw-rw-   0        0        0     4065 2022-11-02 09:25:32.000000 uplogic-1.8.4/uplogic/nodes/actions/addfilter.py
--rw-rw-rw-   0        0        0     1308 2022-08-21 23:02:22.000000 uplogic-1.8.4/uplogic/nodes/actions/addobject.py
--rw-rw-rw-   0        0        0     2710 2022-04-24 07:51:50.000000 uplogic-1.8.4/uplogic/nodes/actions/addphysicsconstraint.py
--rw-rw-rw-   0        0        0      797 2023-03-01 15:33:33.000000 uplogic-1.8.4/uplogic/nodes/actions/adduiwidget.py
--rw-rw-rw-   0        0        0     1420 2022-10-28 14:13:34.000000 uplogic-1.8.4/uplogic/nodes/actions/alignaxistovector.py
--rw-rw-rw-   0        0        0     1056 2022-01-12 11:55:23.000000 uplogic-1.8.4/uplogic/nodes/actions/appendlistitem.py
--rw-rw-rw-   0        0        0     1007 2022-01-12 13:37:33.000000 uplogic-1.8.4/uplogic/nodes/actions/applyforce.py
--rw-rw-rw-   0        0        0     1187 2022-01-12 13:38:47.000000 uplogic-1.8.4/uplogic/nodes/actions/applyimpulse.py
--rw-rw-rw-   0        0        0     1074 2022-01-12 13:36:04.000000 uplogic-1.8.4/uplogic/nodes/actions/applymovement.py
--rw-rw-rw-   0        0        0     1237 2023-01-05 15:34:33.000000 uplogic-1.8.4/uplogic/nodes/actions/applyrotation.py
--rw-rw-rw-   0        0        0      984 2022-01-12 14:18:21.000000 uplogic-1.8.4/uplogic/nodes/actions/applytorque.py
--rw-rw-rw-   0        0        0     2560 2022-01-10 18:02:58.000000 uplogic-1.8.4/uplogic/nodes/actions/cameraraycast.py
--rw-rw-rw-   0        0        0     1014 2022-01-12 14:08:55.000000 uplogic-1.8.4/uplogic/nodes/actions/characterjump.py
--rw-rw-rw-   0        0        0     1536 2022-04-10 10:15:42.000000 uplogic-1.8.4/uplogic/nodes/actions/clampedmodifyproperty.py
--rw-rw-rw-   0        0        0     1643 2023-02-14 10:14:49.000000 uplogic-1.8.4/uplogic/nodes/actions/clearvariables.py
--rw-rw-rw-   0        0        0     1395 2022-04-09 10:45:53.000000 uplogic-1.8.4/uplogic/nodes/actions/copyproperty.py
--rw-rw-rw-   0        0        0     3483 2023-03-08 16:42:06.000000 uplogic-1.8.4/uplogic/nodes/actions/createuibutton.py
--rw-rw-rw-   0        0        0      821 2023-03-01 15:34:01.000000 uplogic-1.8.4/uplogic/nodes/actions/createuicanvas.py
--rw-rw-rw-   0        0        0     1695 2023-03-02 19:57:36.000000 uplogic-1.8.4/uplogic/nodes/actions/createuiimage.py
--rw-rw-rw-   0        0        0     2478 2023-03-02 21:54:35.000000 uplogic-1.8.4/uplogic/nodes/actions/createuilabel.py
--rw-rw-rw-   0        0        0     2292 2023-03-08 16:42:38.000000 uplogic-1.8.4/uplogic/nodes/actions/createuilayout.py
--rw-rw-rw-   0        0        0     1993 2022-01-12 13:17:55.000000 uplogic-1.8.4/uplogic/nodes/actions/createvehicle.py
--rw-rw-rw-   0        0        0     1523 2022-09-11 14:27:22.000000 uplogic-1.8.4/uplogic/nodes/actions/cursorbehavior.py
--rw-rw-rw-   0        0        0      797 2023-03-02 21:19:09.000000 uplogic-1.8.4/uplogic/nodes/actions/cursorvisibility.py
--rw-rw-rw-   0        0        0     1235 2022-01-20 14:17:51.000000 uplogic-1.8.4/uplogic/nodes/actions/dispatchevent.py
--rw-rw-rw-   0        0        0     1180 2022-08-23 18:36:57.000000 uplogic-1.8.4/uplogic/nodes/actions/drawbox.py
--rw-rw-rw-   0        0        0     1020 2022-08-23 18:28:02.000000 uplogic-1.8.4/uplogic/nodes/actions/drawcube.py
--rw-rw-rw-   0        0        0      980 2022-08-23 18:34:20.000000 uplogic-1.8.4/uplogic/nodes/actions/drawline.py
--rw-rw-rw-   0        0        0     3560 2022-01-12 12:12:44.000000 uplogic-1.8.4/uplogic/nodes/actions/editbone.py
--rw-rw-rw-   0        0        0      530 2022-07-18 15:47:27.000000 uplogic-1.8.4/uplogic/nodes/actions/endgame.py
--rw-rw-rw-   0        0        0     1019 2022-01-12 13:25:49.000000 uplogic-1.8.4/uplogic/nodes/actions/endobject.py
--rw-rw-rw-   0        0        0     1237 2022-02-07 22:47:57.000000 uplogic-1.8.4/uplogic/nodes/actions/executesubnetwork.py
--rw-rw-rw-   0        0        0     5553 2022-07-25 09:48:39.000000 uplogic-1.8.4/uplogic/nodes/actions/followpath.py
--rw-rw-rw-   0        0        0     4292 2022-01-31 12:24:47.000000 uplogic-1.8.4/uplogic/nodes/actions/gamepadlook.py
--rw-rw-rw-   0        0        0     1428 2022-01-10 11:08:34.000000 uplogic-1.8.4/uplogic/nodes/actions/gamepadvibration.py
--rw-rw-rw-   0        0        0     2383 2022-01-12 12:04:24.000000 uplogic-1.8.4/uplogic/nodes/actions/getperformanceprofile.py
--rw-rw-rw-   0        0        0     1373 2022-02-07 22:56:45.000000 uplogic-1.8.4/uplogic/nodes/actions/installsubnetwork.py
--rw-rw-rw-   0        0        0     1976 2023-04-26 12:34:19.000000 uplogic-1.8.4/uplogic/nodes/actions/instream.py
--rw-rw-rw-   0        0        0     1326 2022-01-12 15:09:37.000000 uplogic-1.8.4/uplogic/nodes/actions/listglobalvalues.py
--rw-rw-rw-   0        0        0     2143 2023-02-14 10:16:18.000000 uplogic-1.8.4/uplogic/nodes/actions/listvariables.py
--rw-rw-rw-   0        0        0      674 2022-01-10 11:08:34.000000 uplogic-1.8.4/uplogic/nodes/actions/loadblendfile.py
--rw-rw-rw-   0        0        0     1580 2022-10-05 11:16:42.000000 uplogic-1.8.4/uplogic/nodes/actions/loadfilecontent.py
--rw-rw-rw-   0        0        0     4299 2022-02-10 19:08:50.000000 uplogic-1.8.4/uplogic/nodes/actions/loadgame.py
--rw-rw-rw-   0        0        0     1652 2022-10-05 11:16:56.000000 uplogic-1.8.4/uplogic/nodes/actions/loadscene.py
--rw-rw-rw-   0        0        0     1051 2022-01-12 15:17:30.000000 uplogic-1.8.4/uplogic/nodes/actions/makeuniquelight.py
--rw-rw-rw-   0        0        0     1363 2022-04-10 10:15:35.000000 uplogic-1.8.4/uplogic/nodes/actions/modifyproperty.py
--rw-rw-rw-   0        0        0     4865 2023-01-08 15:11:47.000000 uplogic-1.8.4/uplogic/nodes/actions/mouselook.py
--rw-rw-rw-   0        0        0     2144 2022-01-10 18:01:11.000000 uplogic-1.8.4/uplogic/nodes/actions/mouseraycast.py
--rw-rw-rw-   0        0        0     1012 2022-01-10 11:08:34.000000 uplogic-1.8.4/uplogic/nodes/actions/mousesetposition.py
--rw-rw-rw-   0        0        0     1513 2022-01-12 15:30:33.000000 uplogic-1.8.4/uplogic/nodes/actions/moveto.py
--rw-rw-rw-   0        0        0     5201 2022-07-25 09:48:36.000000 uplogic-1.8.4/uplogic/nodes/actions/movetowithnavmesh.py
--rw-rw-rw-   0        0        0      626 2022-01-12 14:35:38.000000 uplogic-1.8.4/uplogic/nodes/actions/pausesound.py
--rw-rw-rw-   0        0        0     5385 2023-05-10 20:12:21.000000 uplogic-1.8.4/uplogic/nodes/actions/playaction.py
--rw-rw-rw-   0        0        0     2476 2023-02-12 11:22:41.000000 uplogic-1.8.4/uplogic/nodes/actions/playsequence.py
--rw-rw-rw-   0        0        0     1338 2022-01-12 11:46:36.000000 uplogic-1.8.4/uplogic/nodes/actions/popdictkey.py
--rw-rw-rw-   0        0        0      684 2022-01-21 13:19:20.000000 uplogic-1.8.4/uplogic/nodes/actions/printvalue.py
--rw-rw-rw-   0        0        0     3127 2022-12-30 21:45:25.000000 uplogic-1.8.4/uplogic/nodes/actions/projectileraycast.py
--rw-rw-rw-   0        0        0     3516 2022-09-11 15:14:18.000000 uplogic-1.8.4/uplogic/nodes/actions/raycast.py
--rw-rw-rw-   0        0        0      842 2022-09-06 10:05:33.000000 uplogic-1.8.4/uplogic/nodes/actions/removefilter.py
--rw-rw-rw-   0        0        0     1176 2022-01-12 11:59:50.000000 uplogic-1.8.4/uplogic/nodes/actions/removelistindex.py
--rw-rw-rw-   0        0        0     1207 2022-01-12 11:59:09.000000 uplogic-1.8.4/uplogic/nodes/actions/removelistvalue.py
--rw-rw-rw-   0        0        0      779 2022-01-10 11:08:34.000000 uplogic-1.8.4/uplogic/nodes/actions/removeoverlaycollection.py
--rw-rw-rw-   0        0        0      969 2022-02-01 19:49:18.000000 uplogic-1.8.4/uplogic/nodes/actions/removeparent.py
--rw-rw-rw-   0        0        0      974 2022-01-12 15:45:41.000000 uplogic-1.8.4/uplogic/nodes/actions/removephysicsconstraint.py
--rw-rw-rw-   0        0        0     1834 2023-02-14 10:14:02.000000 uplogic-1.8.4/uplogic/nodes/actions/removevariable.py
--rw-rw-rw-   0        0        0     1255 2022-01-12 15:43:12.000000 uplogic-1.8.4/uplogic/nodes/actions/replacemesh.py
--rw-rw-rw-   0        0        0      633 2022-02-10 19:19:01.000000 uplogic-1.8.4/uplogic/nodes/actions/restartgame.py
--rw-rw-rw-   0        0        0      628 2022-01-12 14:37:05.000000 uplogic-1.8.4/uplogic/nodes/actions/resumesound.py
--rw-rw-rw-   0        0        0     2171 2023-03-10 12:27:29.000000 uplogic-1.8.4/uplogic/nodes/actions/rotateto.py
--rw-rw-rw-   0        0        0     1199 2022-02-09 13:38:34.000000 uplogic-1.8.4/uplogic/nodes/actions/runactuator.py
--rw-rw-rw-   0        0        0     1706 2023-04-26 12:29:00.000000 uplogic-1.8.4/uplogic/nodes/actions/runpython.py
--rw-rw-rw-   0        0        0     7976 2022-02-08 15:48:21.000000 uplogic-1.8.4/uplogic/nodes/actions/savegame.py
--rw-rw-rw-   0        0        0     2005 2023-02-14 10:08:13.000000 uplogic-1.8.4/uplogic/nodes/actions/savevariable.py
--rw-rw-rw-   0        0        0     1738 2023-02-14 10:08:29.000000 uplogic-1.8.4/uplogic/nodes/actions/savevariabledict.py
--rw-rw-rw-   0        0        0     1180 2022-01-10 17:48:43.000000 uplogic-1.8.4/uplogic/nodes/actions/sendmessage.py
--rw-rw-rw-   0        0        0     2608 2023-02-13 17:09:10.000000 uplogic-1.8.4/uplogic/nodes/actions/setactionframe.py
--rw-rw-rw-   0        0        0     1135 2022-02-26 12:20:29.000000 uplogic-1.8.4/uplogic/nodes/actions/setactuatorvalue.py
--rw-rw-rw-   0        0        0     1532 2022-01-12 13:30:41.000000 uplogic-1.8.4/uplogic/nodes/actions/setboneconstraintattr.py
--rw-rw-rw-   0        0        0     1389 2022-01-12 12:09:35.000000 uplogic-1.8.4/uplogic/nodes/actions/setboneconstraintinfluence.py
--rw-rw-rw-   0        0        0     1382 2022-01-12 12:08:54.000000 uplogic-1.8.4/uplogic/nodes/actions/setboneconstrainttarget.py
--rw-rw-rw-   0        0        0     1488 2022-01-12 12:15:32.000000 uplogic-1.8.4/uplogic/nodes/actions/setboneposition.py
--rw-rw-rw-   0        0        0      944 2022-01-10 18:05:42.000000 uplogic-1.8.4/uplogic/nodes/actions/setcamera.py
--rw-rw-rw-   0        0        0      941 2022-01-23 23:21:22.000000 uplogic-1.8.4/uplogic/nodes/actions/setcamerafov.py
--rw-rw-rw-   0        0        0      966 2022-01-10 18:09:57.000000 uplogic-1.8.4/uplogic/nodes/actions/setcameraorthoscale.py
--rw-rw-rw-   0        0        0     1154 2022-01-12 14:13:53.000000 uplogic-1.8.4/uplogic/nodes/actions/setcharactergravity.py
--rw-rw-rw-   0        0        0     1102 2022-01-12 14:08:37.000000 uplogic-1.8.4/uplogic/nodes/actions/setcharacterjumpspeed.py
--rw-rw-rw-   0        0        0     1096 2022-01-12 14:09:24.000000 uplogic-1.8.4/uplogic/nodes/actions/setcharactermaxjumps.py
--rw-rw-rw-   0        0        0     1200 2022-01-12 14:17:03.000000 uplogic-1.8.4/uplogic/nodes/actions/setcharactervelocity.py
--rw-rw-rw-   0        0        0     1795 2022-01-12 14:14:18.000000 uplogic-1.8.4/uplogic/nodes/actions/setcharacterwalkdir.py
--rw-rw-rw-   0        0        0     1030 2022-01-12 13:44:27.000000 uplogic-1.8.4/uplogic/nodes/actions/setcollisiongroup.py
--rw-rw-rw-   0        0        0     1028 2022-01-12 13:45:39.000000 uplogic-1.8.4/uplogic/nodes/actions/setcollisionmask.py
--rw-rw-rw-   0        0        0     1493 2022-02-16 14:17:45.000000 uplogic-1.8.4/uplogic/nodes/actions/setcurvepoints.py
--rw-rw-rw-   0        0        0     1095 2023-05-03 10:24:19.000000 uplogic-1.8.4/uplogic/nodes/actions/setcustomcursor.py
--rw-rw-rw-   0        0        0     1105 2022-01-12 11:43:10.000000 uplogic-1.8.4/uplogic/nodes/actions/setdictkey.py
--rw-rw-rw-   0        0        0     1166 2022-09-07 10:43:04.000000 uplogic-1.8.4/uplogic/nodes/actions/setdynamics.py
--rw-rw-rw-   0        0        0      887 2022-01-12 15:03:06.000000 uplogic-1.8.4/uplogic/nodes/actions/seteeveeao.py
--rw-rw-rw-   0        0        0      891 2022-01-12 16:00:43.000000 uplogic-1.8.4/uplogic/nodes/actions/seteeveebloom.py
--rw-rw-rw-   0        0        0      895 2022-01-12 15:08:25.000000 uplogic-1.8.4/uplogic/nodes/actions/seteeveesmaa.py
--rw-rw-rw-   0        0        0      902 2022-01-12 15:12:11.000000 uplogic-1.8.4/uplogic/nodes/actions/seteeveesmaaquality.py
--rw-rw-rw-   0        0        0      887 2022-01-12 15:04:58.000000 uplogic-1.8.4/uplogic/nodes/actions/seteeveessr.py
--rw-rw-rw-   0        0        0      933 2022-01-12 15:05:54.000000 uplogic-1.8.4/uplogic/nodes/actions/seteeveevolumetrics.py
--rw-rw-rw-   0        0        0      920 2022-02-06 14:06:39.000000 uplogic-1.8.4/uplogic/nodes/actions/setexposure.py
--rw-rw-rw-   0        0        0      935 2022-09-06 10:37:29.000000 uplogic-1.8.4/uplogic/nodes/actions/setfilterstate.py
--rw-rw-rw-   0        0        0      858 2022-01-10 18:13:34.000000 uplogic-1.8.4/uplogic/nodes/actions/setfullscreen.py
--rw-rw-rw-   0        0        0     1938 2022-01-10 17:22:40.000000 uplogic-1.8.4/uplogic/nodes/actions/setgameobjectattr.py
--rw-rw-rw-   0        0        0      914 2022-01-12 15:01:16.000000 uplogic-1.8.4/uplogic/nodes/actions/setgamma.py
--rw-rw-rw-   0        0        0     1456 2022-01-12 15:57:52.000000 uplogic-1.8.4/uplogic/nodes/actions/setglobalvalue.py
--rw-rw-rw-   0        0        0      933 2022-01-12 13:28:24.000000 uplogic-1.8.4/uplogic/nodes/actions/setgravity.py
--rw-rw-rw-   0        0        0     1012 2022-01-12 15:24:08.000000 uplogic-1.8.4/uplogic/nodes/actions/setlightcolor.py
--rw-rw-rw-   0        0        0      959 2022-01-12 15:16:33.000000 uplogic-1.8.4/uplogic/nodes/actions/setlightenergy.py
--rw-rw-rw-   0        0        0      983 2022-01-12 15:19:36.000000 uplogic-1.8.4/uplogic/nodes/actions/setlightshadow.py
--rw-rw-rw-   0        0        0     1137 2022-01-12 11:56:28.000000 uplogic-1.8.4/uplogic/nodes/actions/setlistindex.py
--rw-rw-rw-   0        0        0     1321 2022-01-10 11:08:34.000000 uplogic-1.8.4/uplogic/nodes/actions/setmaterial.py
--rw-rw-rw-   0        0        0     1412 2022-01-10 12:35:51.000000 uplogic-1.8.4/uplogic/nodes/actions/setmatnodesocket.py
--rw-rw-rw-   0        0        0     1610 2022-01-10 11:08:34.000000 uplogic-1.8.4/uplogic/nodes/actions/setmatnodevalue.py
--rw-rw-rw-   0        0        0     1388 2022-01-10 11:08:34.000000 uplogic-1.8.4/uplogic/nodes/actions/setnodesocket.py
--rw-rw-rw-   0        0        0     1622 2022-01-10 11:08:34.000000 uplogic-1.8.4/uplogic/nodes/actions/setnodevalue.py
--rw-rw-rw-   0        0        0      863 2022-01-10 11:08:34.000000 uplogic-1.8.4/uplogic/nodes/actions/setoverlaycollection.py
--rw-rw-rw-   0        0        0     1188 2022-01-12 12:01:10.000000 uplogic-1.8.4/uplogic/nodes/actions/setparent.py
--rw-rw-rw-   0        0        0     1188 2022-01-12 16:00:43.000000 uplogic-1.8.4/uplogic/nodes/actions/setphysics.py
--rw-rw-rw-   0        0        0      838 2022-01-10 18:14:35.000000 uplogic-1.8.4/uplogic/nodes/actions/setprofile.py
--rw-rw-rw-   0        0        0     1383 2022-10-05 12:35:18.000000 uplogic-1.8.4/uplogic/nodes/actions/setproperty.py
--rw-rw-rw-   0        0        0      736 2022-01-10 11:08:34.000000 uplogic-1.8.4/uplogic/nodes/actions/setpyinstanceattr.py
--rw-rw-rw-   0        0        0      898 2022-01-23 23:21:22.000000 uplogic-1.8.4/uplogic/nodes/actions/setresolution.py
--rw-rw-rw-   0        0        0     1085 2022-01-12 13:12:07.000000 uplogic-1.8.4/uplogic/nodes/actions/setrigidbody.py
--rw-rw-rw-   0        0        0      820 2022-10-04 11:00:44.000000 uplogic-1.8.4/uplogic/nodes/actions/setscene.py
--rw-rw-rw-   0        0        0     1200 2022-02-04 18:03:35.000000 uplogic-1.8.4/uplogic/nodes/actions/setsensorvalue.py
--rw-rw-rw-   0        0        0      949 2022-01-12 13:27:30.000000 uplogic-1.8.4/uplogic/nodes/actions/settimescale.py
--rw-rw-rw-   0        0        0     2388 2023-03-02 19:55:31.000000 uplogic-1.8.4/uplogic/nodes/actions/setuiwidgetattr.py
--rw-rw-rw-   0        0        0     2913 2022-02-06 12:41:13.000000 uplogic-1.8.4/uplogic/nodes/actions/setvisibility.py
--rw-rw-rw-   0        0        0      828 2022-01-12 11:22:14.000000 uplogic-1.8.4/uplogic/nodes/actions/setvsync.py
--rw-rw-rw-   0        0        0      853 2022-01-10 18:19:10.000000 uplogic-1.8.4/uplogic/nodes/actions/showframerate.py
--rw-rw-rw-   0        0        0     1514 2022-11-03 22:18:05.000000 uplogic-1.8.4/uplogic/nodes/actions/slowfollow.py
--rw-rw-rw-   0        0        0     2051 2023-03-06 08:53:53.000000 uplogic-1.8.4/uplogic/nodes/actions/startsound.py
--rw-rw-rw-   0        0        0     3107 2023-03-06 08:54:22.000000 uplogic-1.8.4/uplogic/nodes/actions/startsound3d.py
--rw-rw-rw-   0        0        0     2541 2023-03-06 08:54:22.000000 uplogic-1.8.4/uplogic/nodes/actions/startspeaker.py
--rw-rw-rw-   0        0        0     1436 2022-02-07 22:56:23.000000 uplogic-1.8.4/uplogic/nodes/actions/startsubnetwork.py
--rw-rw-rw-   0        0        0     1597 2022-10-07 11:19:16.000000 uplogic-1.8.4/uplogic/nodes/actions/stopaction.py
--rw-rw-rw-   0        0        0      591 2022-01-12 14:34:57.000000 uplogic-1.8.4/uplogic/nodes/actions/stopallsounds.py
--rw-rw-rw-   0        0        0      624 2022-01-12 14:28:14.000000 uplogic-1.8.4/uplogic/nodes/actions/stopsound.py
--rw-rw-rw-   0        0        0     1209 2022-02-07 22:56:33.000000 uplogic-1.8.4/uplogic/nodes/actions/stopsubnetwork.py
--rw-rw-rw-   0        0        0      842 2022-09-06 10:25:56.000000 uplogic-1.8.4/uplogic/nodes/actions/togglefilter.py
--rw-rw-rw-   0        0        0     1227 2022-04-09 10:37:36.000000 uplogic-1.8.4/uplogic/nodes/actions/toggleproperty.py
--rw-rw-rw-   0        0        0     2809 2022-01-12 14:57:52.000000 uplogic-1.8.4/uplogic/nodes/actions/translate.py
--rw-rw-rw-   0        0        0     1381 2022-01-12 13:18:01.000000 uplogic-1.8.4/uplogic/nodes/actions/vehicleapplybraking.py
--rw-rw-rw-   0        0        0     1369 2022-01-12 13:18:26.000000 uplogic-1.8.4/uplogic/nodes/actions/vehicleapplyforce.py
--rw-rw-rw-   0        0        0     1382 2022-01-12 16:23:26.000000 uplogic-1.8.4/uplogic/nodes/actions/vehicleapplysteering.py
--rw-rw-rw-   0        0        0     3463 2022-01-23 23:21:22.000000 uplogic-1.8.4/uplogic/nodes/actions/vehiclesetattributes.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:13:56.664816 uplogic-1.8.4/uplogic/nodes/conditions/
--rw-rw-rw-   0        0        0     1946 2022-01-20 14:15:37.000000 uplogic-1.8.4/uplogic/nodes/conditions/__init__.py
--rw-rw-rw-   0        0        0      935 2022-01-12 13:06:20.000000 uplogic-1.8.4/uplogic/nodes/conditions/barrier.py
--rw-rw-rw-   0        0        0     2387 2022-02-07 18:36:03.000000 uplogic-1.8.4/uplogic/nodes/conditions/checkdistance.py
--rw-rw-rw-   0        0        0     4779 2023-01-14 13:34:38.000000 uplogic-1.8.4/uplogic/nodes/conditions/collision.py
--rw-rw-rw-   0        0        0     1488 2022-01-27 17:31:36.000000 uplogic-1.8.4/uplogic/nodes/conditions/compare.py
--rw-rw-rw-   0        0        0     2155 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/conditions/comparevectors.py
--rw-rw-rw-   0        0        0     3288 2022-01-10 17:39:46.000000 uplogic-1.8.4/uplogic/nodes/conditions/controllerstatus.py
--rw-rw-rw-   0        0        0     1487 2022-04-09 10:43:29.000000 uplogic-1.8.4/uplogic/nodes/conditions/evaluateproperty.py
--rw-rw-rw-   0        0        0      756 2022-01-28 16:50:48.000000 uplogic-1.8.4/uplogic/nodes/conditions/gamepadactive.py
--rw-rw-rw-   0        0        0     1493 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/conditions/gamepadbutton.py
--rw-rw-rw-   0        0        0     1772 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/conditions/gamepadbuttonup.py
--rw-rw-rw-   0        0        0     1083 2022-01-20 14:17:20.000000 uplogic-1.8.4/uplogic/nodes/conditions/handleevent.py
--rw-rw-rw-   0        0        0     1209 2022-04-09 08:17:22.000000 uplogic-1.8.4/uplogic/nodes/conditions/hasproperty.py
--rw-rw-rw-   0        0        0      303 2021-12-21 09:41:07.000000 uplogic-1.8.4/uplogic/nodes/conditions/keyboardactive.py
--rw-rw-rw-   0        0        0      812 2022-01-10 11:08:34.000000 uplogic-1.8.4/uplogic/nodes/conditions/keypressed.py
--rw-rw-rw-   0        0        0      756 2022-01-10 11:08:34.000000 uplogic-1.8.4/uplogic/nodes/conditions/keyreleased.py
--rw-rw-rw-   0        0        0     1705 2022-02-04 11:39:59.000000 uplogic-1.8.4/uplogic/nodes/conditions/logicand.py
--rw-rw-rw-   0        0        0      621 2022-02-04 11:45:26.000000 uplogic-1.8.4/uplogic/nodes/conditions/logicandnot.py
--rw-rw-rw-   0        0        0      325 2022-01-10 11:08:34.000000 uplogic-1.8.4/uplogic/nodes/conditions/logicnone.py
--rw-rw-rw-   0        0        0      758 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/conditions/logicnot.py
--rw-rw-rw-   0        0        0      334 2022-01-10 11:08:34.000000 uplogic-1.8.4/uplogic/nodes/conditions/logicnotnone.py
--rw-rw-rw-   0        0        0     1132 2022-02-04 18:24:10.000000 uplogic-1.8.4/uplogic/nodes/conditions/logicor.py
--rw-rw-rw-   0        0        0     1645 2022-01-21 17:57:37.000000 uplogic-1.8.4/uplogic/nodes/conditions/logictreestatus.py
--rw-rw-rw-   0        0        0      494 2022-09-11 14:46:42.000000 uplogic-1.8.4/uplogic/nodes/conditions/mousemoved.py
--rw-rw-rw-   0        0        0     3567 2022-09-11 14:47:44.000000 uplogic-1.8.4/uplogic/nodes/conditions/mouseover.py
--rw-rw-rw-   0        0        0     1303 2022-09-11 14:51:02.000000 uplogic-1.8.4/uplogic/nodes/conditions/mousepressed.py
--rw-rw-rw-   0        0        0     1730 2022-09-11 14:51:29.000000 uplogic-1.8.4/uplogic/nodes/conditions/mousepressedon.py
--rw-rw-rw-   0        0        0     1292 2022-09-11 14:52:33.000000 uplogic-1.8.4/uplogic/nodes/conditions/mousereleased.py
--rw-rw-rw-   0        0        0      700 2022-09-11 14:54:01.000000 uplogic-1.8.4/uplogic/nodes/conditions/mousescroll.py
--rw-rw-rw-   0        0        0     1071 2022-01-10 11:08:34.000000 uplogic-1.8.4/uplogic/nodes/conditions/once.py
--rw-rw-rw-   0        0        0      348 2021-12-21 09:41:07.000000 uplogic-1.8.4/uplogic/nodes/conditions/oninit.py
--rw-rw-rw-   0        0        0      704 2023-04-06 11:05:27.000000 uplogic-1.8.4/uplogic/nodes/conditions/onnexttick.py
--rw-rw-rw-   0        0        0      349 2021-12-21 09:41:07.000000 uplogic-1.8.4/uplogic/nodes/conditions/onupdate.py
--rw-rw-rw-   0        0        0     1270 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/conditions/onvaluechanged.py
--rw-rw-rw-   0        0        0     1228 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/conditions/onvaluechangedto.py
--rw-rw-rw-   0        0        0     1474 2022-05-25 09:41:06.000000 uplogic-1.8.4/uplogic/nodes/conditions/pulsify.py
--rw-rw-rw-   0        0        0     1069 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/conditions/sensorpositive.py
--rw-rw-rw-   0        0        0      940 2022-01-17 10:41:45.000000 uplogic-1.8.4/uplogic/nodes/conditions/timedelay.py
--rw-rw-rw-   0        0        0      918 2022-01-10 11:08:34.000000 uplogic-1.8.4/uplogic/nodes/conditions/timer.py
--rw-rw-rw-   0        0        0      548 2022-01-10 11:08:34.000000 uplogic-1.8.4/uplogic/nodes/conditions/truefalse.py
--rw-rw-rw-   0        0        0      377 2022-01-10 11:08:34.000000 uplogic-1.8.4/uplogic/nodes/conditions/valuevalid.py
--rw-rw-rw-   0        0        0     8520 2023-03-06 08:59:44.000000 uplogic-1.8.4/uplogic/nodes/logictree.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:13:56.773841 uplogic-1.8.4/uplogic/nodes/parameters/
--rw-rw-rw-   0        0        0     4683 2023-03-02 22:49:47.000000 uplogic-1.8.4/uplogic/nodes/parameters/__init__.py
--rw-rw-rw-   0        0        0      638 2022-01-10 14:17:56.000000 uplogic-1.8.4/uplogic/nodes/parameters/absolutevalue.py
--rw-rw-rw-   0        0        0     1703 2022-01-23 23:18:50.000000 uplogic-1.8.4/uplogic/nodes/parameters/actionstatus.py
--rw-rw-rw-   0        0        0      575 2021-12-21 09:41:07.000000 uplogic-1.8.4/uplogic/nodes/parameters/activecamera.py
--rw-rw-rw-   0        0        0      889 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/axisvector.py
--rw-rw-rw-   0        0        0     1913 2022-01-10 11:08:34.000000 uplogic-1.8.4/uplogic/nodes/parameters/bonestatus.py
--rw-rw-rw-   0        0        0     1911 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/characterinfo.py
--rw-rw-rw-   0        0        0     1148 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/childbyindex.py
--rw-rw-rw-   0        0        0      893 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/childbyname.py
--rw-rw-rw-   0        0        0     1106 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/clamp.py
--rw-rw-rw-   0        0        0      782 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/colorrgb.py
--rw-rw-rw-   0        0        0      719 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/colorrgba.py
--rw-rw-rw-   0        0        0      911 2022-02-17 16:47:54.000000 uplogic-1.8.4/uplogic/nodes/parameters/dictvalue.py
--rw-rw-rw-   0        0        0      910 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/distance.py
--rw-rw-rw-   0        0        0      910 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/euler.py
--rw-rw-rw-   0        0        0      786 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/eulertomatrix.py
--rw-rw-rw-   0        0        0     1274 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/formattedstring.py
--rw-rw-rw-   0        0        0     2158 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/formula.py
--rw-rw-rw-   0        0        0     1825 2023-02-06 12:32:50.000000 uplogic-1.8.4/uplogic/nodes/parameters/gamepadsticks.py
--rw-rw-rw-   0        0        0     1553 2022-01-28 16:40:04.000000 uplogic-1.8.4/uplogic/nodes/parameters/gamepadtrigger.py
--rw-rw-rw-   0        0        0     1087 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/getactuatorvalue.py
--rw-rw-rw-   0        0        0      602 2022-01-10 11:08:34.000000 uplogic-1.8.4/uplogic/nodes/parameters/getcollection.py
--rw-rw-rw-   0        0        0     1046 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/getcollectionobjectnames.py
--rw-rw-rw-   0        0        0     1037 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/getcollectionobjects.py
--rw-rw-rw-   0        0        0     1055 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/getcurvepoints.py
--rw-rw-rw-   0        0        0      527 2023-03-02 19:33:55.000000 uplogic-1.8.4/uplogic/nodes/parameters/getfont.py
--rw-rw-rw-   0        0        0      385 2022-01-12 11:04:44.000000 uplogic-1.8.4/uplogic/nodes/parameters/getfullscreen.py
--rw-rw-rw-   0        0        0     1080 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/getglobalvalue.py
--rw-rw-rw-   0        0        0      432 2021-12-21 09:41:07.000000 uplogic-1.8.4/uplogic/nodes/parameters/getgravity.py
--rw-rw-rw-   0        0        0      534 2022-01-10 11:08:34.000000 uplogic-1.8.4/uplogic/nodes/parameters/getimage.py
--rw-rw-rw-   0        0        0      638 2022-01-12 15:26:03.000000 uplogic-1.8.4/uplogic/nodes/parameters/getlightcolor.py
--rw-rw-rw-   0        0        0      644 2022-01-12 15:25:51.000000 uplogic-1.8.4/uplogic/nodes/parameters/getlightenergy.py
--rw-rw-rw-   0        0        0     1410 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/getnodeattribute.py
--rw-rw-rw-   0        0        0     1284 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/getnodesocket.py
--rw-rw-rw-   0        0        0      589 2022-07-18 16:33:11.000000 uplogic-1.8.4/uplogic/nodes/parameters/getobject.py
--rw-rw-rw-   0        0        0      432 2021-12-21 09:41:07.000000 uplogic-1.8.4/uplogic/nodes/parameters/getowner.py
--rw-rw-rw-   0        0        0      604 2022-01-10 11:08:34.000000 uplogic-1.8.4/uplogic/nodes/parameters/getparent.py
--rw-rw-rw-   0        0        0     1044 2022-04-09 10:37:26.000000 uplogic-1.8.4/uplogic/nodes/parameters/getproperty.py
--rw-rw-rw-   0        0        0      705 2022-02-04 12:00:42.000000 uplogic-1.8.4/uplogic/nodes/parameters/getpyinstanceattr.py
--rw-rw-rw-   0        0        0      760 2022-01-12 11:11:52.000000 uplogic-1.8.4/uplogic/nodes/parameters/getresolution.py
--rw-rw-rw-   0        0        0      384 2021-12-21 09:41:07.000000 uplogic-1.8.4/uplogic/nodes/parameters/getscene.py
--rw-rw-rw-   0        0        0      944 2022-01-10 11:08:34.000000 uplogic-1.8.4/uplogic/nodes/parameters/getsensorvalue.py
--rw-rw-rw-   0        0        0      562 2022-01-10 11:08:34.000000 uplogic-1.8.4/uplogic/nodes/parameters/getsound.py
--rw-rw-rw-   0        0        0      385 2021-12-21 09:41:07.000000 uplogic-1.8.4/uplogic/nodes/parameters/gettimescale.py
--rw-rw-rw-   0        0        0     1070 2023-03-02 22:50:45.000000 uplogic-1.8.4/uplogic/nodes/parameters/getuiwidgetattr.py
--rw-rw-rw-   0        0        0      375 2022-01-12 11:01:47.000000 uplogic-1.8.4/uplogic/nodes/parameters/getvsync.py
--rw-rw-rw-   0        0        0      429 2022-01-12 11:37:03.000000 uplogic-1.8.4/uplogic/nodes/parameters/initemptydict.py
--rw-rw-rw-   0        0        0      599 2022-01-26 18:13:15.000000 uplogic-1.8.4/uplogic/nodes/parameters/initemptylist.py
--rw-rw-rw-   0        0        0      642 2022-01-12 11:39:31.000000 uplogic-1.8.4/uplogic/nodes/parameters/initnewdict.py
--rw-rw-rw-   0        0        0      863 2022-12-30 12:20:44.000000 uplogic-1.8.4/uplogic/nodes/parameters/interpolate.py
--rw-rw-rw-   0        0        0      620 2022-01-10 14:18:19.000000 uplogic-1.8.4/uplogic/nodes/parameters/invertvalue.py
--rw-rw-rw-   0        0        0      316 2022-01-10 11:08:17.000000 uplogic-1.8.4/uplogic/nodes/parameters/keycode.py
--rw-rw-rw-   0        0        0     1465 2022-04-09 08:53:46.000000 uplogic-1.8.4/uplogic/nodes/parameters/limitrange.py
--rw-rw-rw-   0        0        0      610 2022-01-10 11:08:17.000000 uplogic-1.8.4/uplogic/nodes/parameters/listduplicate.py
--rw-rw-rw-   0        0        0      813 2022-02-20 18:34:49.000000 uplogic-1.8.4/uplogic/nodes/parameters/listextend.py
--rw-rw-rw-   0        0        0      697 2022-12-21 14:09:17.000000 uplogic-1.8.4/uplogic/nodes/parameters/listfromitems.py
--rw-rw-rw-   0        0        0      817 2022-01-10 11:08:17.000000 uplogic-1.8.4/uplogic/nodes/parameters/listindex.py
--rw-rw-rw-   0        0        0      825 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/listindexrandom.py
--rw-rw-rw-   0        0        0     1941 2023-02-14 10:11:02.000000 uplogic-1.8.4/uplogic/nodes/parameters/loadvariable.py
--rw-rw-rw-   0        0        0     1479 2023-02-14 10:12:26.000000 uplogic-1.8.4/uplogic/nodes/parameters/loadvariabledict.py
--rw-rw-rw-   0        0        0     1422 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/materialgetattribute.py
--rw-rw-rw-   0        0        0      789 2022-01-10 11:08:17.000000 uplogic-1.8.4/uplogic/nodes/parameters/materialgetnode.py
--rw-rw-rw-   0        0        0     1290 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/materialgetsocket.py
--rw-rw-rw-   0        0        0     2539 2022-04-09 08:52:07.000000 uplogic-1.8.4/uplogic/nodes/parameters/math.py
--rw-rw-rw-   0        0        0      672 2022-01-30 10:48:51.000000 uplogic-1.8.4/uplogic/nodes/parameters/matrixtoxyz.py
--rw-rw-rw-   0        0        0     1268 2022-09-11 14:27:39.000000 uplogic-1.8.4/uplogic/nodes/parameters/mousedata.py
--rw-rw-rw-   0        0        0     1027 2022-01-10 11:08:17.000000 uplogic-1.8.4/uplogic/nodes/parameters/objectattr.py
--rw-rw-rw-   0        0        0      591 2022-01-10 11:08:17.000000 uplogic-1.8.4/uplogic/nodes/parameters/objectdataname.py
--rw-rw-rw-   0        0        0     1136 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/objectdatavertices.py
--rw-rw-rw-   0        0        0     1212 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/randomfloat.py
--rw-rw-rw-   0        0        0     1157 2022-01-12 14:52:54.000000 uplogic-1.8.4/uplogic/nodes/parameters/randomint.py
--rw-rw-rw-   0        0        0      979 2022-01-16 18:24:15.000000 uplogic-1.8.4/uplogic/nodes/parameters/randomvect.py
--rw-rw-rw-   0        0        0     1022 2022-04-09 08:53:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/rangedthreshold.py
--rw-rw-rw-   0        0        0      835 2022-01-10 11:08:17.000000 uplogic-1.8.4/uplogic/nodes/parameters/screenposition.py
--rw-rw-rw-   0        0        0      417 2022-01-10 11:08:17.000000 uplogic-1.8.4/uplogic/nodes/parameters/simplevalue.py
--rw-rw-rw-   0        0        0      623 2022-08-21 21:33:43.000000 uplogic-1.8.4/uplogic/nodes/parameters/storevalue.py
--rw-rw-rw-   0        0        0     1092 2022-04-09 08:53:22.000000 uplogic-1.8.4/uplogic/nodes/parameters/threshold.py
--rw-rw-rw-   0        0        0      997 2022-09-28 19:47:00.000000 uplogic-1.8.4/uplogic/nodes/parameters/timedata.py
--rw-rw-rw-   0        0        0      978 2022-01-10 11:08:17.000000 uplogic-1.8.4/uplogic/nodes/parameters/typecastvalue.py
--rw-rw-rw-   0        0        0     4487 2023-03-11 17:19:18.000000 uplogic-1.8.4/uplogic/nodes/parameters/valueswitch.py
--rw-rw-rw-   0        0        0      715 2022-01-10 11:08:17.000000 uplogic-1.8.4/uplogic/nodes/parameters/vectorabsolute.py
--rw-rw-rw-   0        0        0      876 2022-01-10 11:08:17.000000 uplogic-1.8.4/uplogic/nodes/parameters/vectorangle.py
--rw-rw-rw-   0        0        0     1365 2022-01-10 11:08:17.000000 uplogic-1.8.4/uplogic/nodes/parameters/vectoranglecheck.py
--rw-rw-rw-   0        0        0      610 2022-01-10 11:08:17.000000 uplogic-1.8.4/uplogic/nodes/parameters/vectorlength.py
--rw-rw-rw-   0        0        0     3616 2022-12-30 12:09:49.000000 uplogic-1.8.4/uplogic/nodes/parameters/vectormath.py
--rw-rw-rw-   0        0        0      717 2022-01-10 11:08:17.000000 uplogic-1.8.4/uplogic/nodes/parameters/vectorsplitxy.py
--rw-rw-rw-   0        0        0     1032 2022-01-30 14:47:33.000000 uplogic-1.8.4/uplogic/nodes/parameters/vectorsplitxyz.py
--rw-rw-rw-   0        0        0      691 2023-03-03 08:53:48.000000 uplogic-1.8.4/uplogic/nodes/parameters/vectorxy.py
--rw-rw-rw-   0        0        0      818 2022-01-10 11:08:17.000000 uplogic-1.8.4/uplogic/nodes/parameters/vectorxyz.py
--rw-rw-rw-   0        0        0      945 2022-01-10 11:08:17.000000 uplogic-1.8.4/uplogic/nodes/parameters/vectorxyzw.py
--rw-rw-rw-   0        0        0     1378 2023-03-06 09:01:43.000000 uplogic-1.8.4/uplogic/nodes/parameters/vrcontrollervalues.py
--rw-rw-rw-   0        0        0      583 2023-03-06 09:01:01.000000 uplogic-1.8.4/uplogic/nodes/parameters/vrheadsetvalues.py
--rw-rw-rw-   0        0        0     1016 2022-04-09 08:53:55.000000 uplogic-1.8.4/uplogic/nodes/parameters/withinrange.py
--rw-rw-rw-   0        0        0     1257 2022-01-10 11:25:35.000000 uplogic-1.8.4/uplogic/nodes/parameters/worldposition.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:13:56.779842 uplogic-1.8.4/uplogic/physics/
--rw-rw-rw-   0        0        0      540 2023-03-06 11:18:24.000000 uplogic-1.8.4/uplogic/physics/__init__.py
--rw-rw-rw-   0        0        0     4183 2023-03-06 11:13:23.000000 uplogic-1.8.4/uplogic/physics/buoyancy.py
--rw-rw-rw-   0        0        0     3651 2023-03-06 11:14:11.000000 uplogic-1.8.4/uplogic/physics/character.py
--rw-rw-rw-   0        0        0     3474 2023-03-06 11:17:18.000000 uplogic-1.8.4/uplogic/physics/collision.py
--rw-rw-rw-   0        0        0     8340 2023-04-01 06:57:51.000000 uplogic-1.8.4/uplogic/physics/constraints.py
--rw-rw-rw-   0        0        0    10086 2023-03-06 11:09:35.000000 uplogic-1.8.4/uplogic/physics/vehicle.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:13:56.803847 uplogic-1.8.4/uplogic/shaders/
--rw-rw-rw-   0        0        0      675 2023-04-01 06:53:28.000000 uplogic-1.8.4/uplogic/shaders/__init__.py
--rw-rw-rw-   0        0        0      872 2023-04-01 06:53:25.000000 uplogic-1.8.4/uplogic/shaders/adaptivetonemapping.py
--rw-rw-rw-   0        0        0     1631 2023-04-01 06:53:32.000000 uplogic-1.8.4/uplogic/shaders/blur.py
--rw-rw-rw-   0        0        0      685 2023-04-01 06:54:25.000000 uplogic-1.8.4/uplogic/shaders/brightness.py
--rw-rw-rw-   0        0        0     1050 2023-04-01 06:54:25.000000 uplogic-1.8.4/uplogic/shaders/chromaticaberration.py
--rw-rw-rw-   0        0        0     8869 2023-04-01 06:54:25.000000 uplogic-1.8.4/uplogic/shaders/distort.py
--rw-rw-rw-   0        0        0     9818 2023-04-01 06:54:25.000000 uplogic-1.8.4/uplogic/shaders/dof.py
--rw-rw-rw-   0        0        0     9106 2023-04-01 06:54:25.000000 uplogic-1.8.4/uplogic/shaders/droplets.py
--rw-rw-rw-   0        0        0    33424 2023-04-01 06:54:25.000000 uplogic-1.8.4/uplogic/shaders/fxaa.py
--rw-rw-rw-   0        0        0      916 2023-04-01 06:54:25.000000 uplogic-1.8.4/uplogic/shaders/grayscale.py
--rw-rw-rw-   0        0        0     9684 2023-04-01 06:54:25.000000 uplogic-1.8.4/uplogic/shaders/hbao.py
--rw-rw-rw-   0        0        0     1173 2023-04-01 06:54:25.000000 uplogic-1.8.4/uplogic/shaders/letterbox.py
--rw-rw-rw-   0        0        0     1027 2023-04-01 06:54:25.000000 uplogic-1.8.4/uplogic/shaders/levels.py
--rw-rw-rw-   0        0        0     4209 2023-04-01 06:54:25.000000 uplogic-1.8.4/uplogic/shaders/mist.py
--rw-rw-rw-   0        0        0     5411 2023-04-01 07:02:38.000000 uplogic-1.8.4/uplogic/shaders/shader.py
--rw-rw-rw-   0        0        0     2268 2023-04-01 06:54:25.000000 uplogic-1.8.4/uplogic/shaders/sharpen.py
--rw-rw-rw-   0        0        0     5737 2023-04-01 06:54:25.000000 uplogic-1.8.4/uplogic/shaders/ssao.py
--rw-rw-rw-   0        0        0     1190 2023-04-01 06:54:25.000000 uplogic-1.8.4/uplogic/shaders/vignette.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:13:56.812850 uplogic-1.8.4/uplogic/ui/
--rw-rw-rw-   0        0        0      365 2023-04-02 16:26:08.000000 uplogic-1.8.4/uplogic/ui/__init__.py
--rw-rw-rw-   0        0        0      579 2023-04-02 14:03:20.000000 uplogic-1.8.4/uplogic/ui/behaviors.py
--rw-rw-rw-   0        0        0     4937 2023-04-26 12:34:19.000000 uplogic-1.8.4/uplogic/ui/button.py
--rw-rw-rw-   0        0        0     1239 2023-04-02 14:15:27.000000 uplogic-1.8.4/uplogic/ui/canvas.py
--rw-rw-rw-   0        0        0     2438 2023-04-26 12:34:19.000000 uplogic-1.8.4/uplogic/ui/cursor.py
--rw-rw-rw-   0        0        0     3222 2023-04-26 12:34:19.000000 uplogic-1.8.4/uplogic/ui/image.py
--rw-rw-rw-   0        0        0     5480 2023-04-26 12:34:19.000000 uplogic-1.8.4/uplogic/ui/label.py
--rw-rw-rw-   0        0        0     6030 2023-04-26 12:34:19.000000 uplogic-1.8.4/uplogic/ui/layout.py
--rw-rw-rw-   0        0        0     8601 2023-04-26 12:34:19.000000 uplogic-1.8.4/uplogic/ui/widget.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:13:56.823851 uplogic-1.8.4/uplogic/utils/
--rw-rw-rw-   0        0        0    18428 2023-04-01 11:07:38.000000 uplogic-1.8.4/uplogic/utils/__init__.py
--rw-rw-rw-   0        0        0      854 2022-09-08 15:54:10.000000 uplogic-1.8.4/uplogic/utils/errors.py
--rw-rw-rw-   0        0        0     6307 2023-03-06 11:22:43.000000 uplogic-1.8.4/uplogic/utils/lights.py
--rw-rw-rw-   0        0        0     4801 2022-08-22 17:00:51.000000 uplogic-1.8.4/uplogic/utils/nodetrees.py
--rw-rw-rw-   0        0        0     7207 2023-03-06 11:22:26.000000 uplogic-1.8.4/uplogic/utils/objects.py
--rw-rw-rw-   0        0        0      131 2023-01-25 17:06:07.000000 uplogic-1.8.4/uplogic/utils/pooling.py
--rw-rw-rw-   0        0        0    13150 2023-01-05 12:26:27.000000 uplogic-1.8.4/uplogic/utils/raycasting.py
--rw-rw-rw-   0        0        0     5831 2022-10-05 11:16:36.000000 uplogic-1.8.4/uplogic/utils/scene.py
--rw-rw-rw-   0        0        0     1633 2023-01-05 12:25:57.000000 uplogic-1.8.4/uplogic/utils/visuals.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:13:56.397388 uplogic-1.8.4/uplogic.egg-info/
--rw-rw-rw-   0        0        0     1049 2023-05-10 20:13:56.000000 uplogic-1.8.4/uplogic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    13220 2023-05-10 20:13:56.000000 uplogic-1.8.4/uplogic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 20:13:56.000000 uplogic-1.8.4/uplogic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-10 20:13:56.000000 uplogic-1.8.4/uplogic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-10 20:13:56.000000 uplogic-1.8.4/uplogic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-03-17 18:28:53.000000 uplogic-1.8.4/uplogic.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-05-16 11:20:06.954567 uplogic-1.9/
+-rw-rw-rw-   0        0        0      189 2022-01-15 11:35:38.000000 uplogic-1.9/LICENSE.md
+-rw-rw-rw-   0        0        0     1045 2023-05-16 11:20:06.953566 uplogic-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2022-01-15 11:34:53.000000 uplogic-1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 11:20:06.954567 uplogic-1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1709 2023-05-16 11:20:03.000000 uplogic-1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:20:06.371409 uplogic-1.9/uplogic/
+-rw-rw-rw-   0        0        0     5944 2023-05-14 15:49:19.000000 uplogic-1.9/uplogic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:20:06.411416 uplogic-1.9/uplogic/animation/
+-rw-rw-rw-   0        0        0      343 2023-03-08 12:02:42.000000 uplogic-1.9/uplogic/animation/__init__.py
+-rw-rw-rw-   0        0        0    12497 2023-05-14 08:46:23.000000 uplogic-1.9/uplogic/animation/action.py
+-rw-rw-rw-   0        0        0     4016 2023-05-01 17:00:05.000000 uplogic-1.9/uplogic/animation/actionsystem.py
+-rw-rw-rw-   0        0        0     6224 2023-05-14 08:46:37.000000 uplogic-1.9/uplogic/animation/sequence.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:20:06.425420 uplogic-1.9/uplogic/audio/
+-rw-rw-rw-   0        0        0      606 2023-03-06 09:07:59.000000 uplogic-1.9/uplogic/audio/__init__.py
+-rw-rw-rw-   0        0        0     7689 2023-04-24 21:26:30.000000 uplogic-1.9/uplogic/audio/audiosystem.py
+-rw-rw-rw-   0        0        0     6839 2023-05-14 08:47:09.000000 uplogic-1.9/uplogic/audio/music.py
+-rw-rw-rw-   0        0        0    23984 2023-05-14 08:48:10.000000 uplogic-1.9/uplogic/audio/sound.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:20:06.439424 uplogic-1.9/uplogic/data/
+-rw-rw-rw-   0        0        0     1861 2022-10-06 13:43:59.000000 uplogic-1.9/uplogic/data/__init__.py
+-rw-rw-rw-   0        0        0     3122 2023-04-07 16:35:00.000000 uplogic-1.9/uplogic/data/file.py
+-rw-rw-rw-   0        0        0     7148 2023-05-14 08:48:26.000000 uplogic-1.9/uplogic/data/globaldb.py
+-rw-rw-rw-   0        0        0     2050 2021-12-21 09:41:07.000000 uplogic-1.9/uplogic/data/serializers.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:20:06.441424 uplogic-1.9/uplogic/decorators/
+-rw-rw-rw-   0        0        0     9022 2023-04-02 15:18:30.000000 uplogic-1.9/uplogic/decorators/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:20:06.444424 uplogic-1.9/uplogic/events/
+-rw-rw-rw-   0        0        0     7615 2023-04-04 13:17:19.000000 uplogic-1.9/uplogic/events/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:20:06.460428 uplogic-1.9/uplogic/input/
+-rw-rw-rw-   0        0        0     1494 2023-03-06 08:52:33.000000 uplogic-1.9/uplogic/input/__init__.py
+-rw-rw-rw-   0        0        0    15062 2023-05-14 08:49:03.000000 uplogic-1.9/uplogic/input/gamepad.py
+-rw-rw-rw-   0        0        0     9607 2023-01-16 12:00:44.000000 uplogic-1.9/uplogic/input/keyboard.py
+-rw-rw-rw-   0        0        0    14930 2023-05-14 08:49:32.000000 uplogic-1.9/uplogic/input/mouse.py
+-rw-rw-rw-   0        0        0     9131 2023-05-14 08:49:48.000000 uplogic-1.9/uplogic/input/vr.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:20:06.464429 uplogic-1.9/uplogic/logging/
+-rw-rw-rw-   0        0        0     5303 2023-05-16 10:30:34.000000 uplogic-1.9/uplogic/logging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:20:06.471431 uplogic-1.9/uplogic/nodes/
+-rw-rw-rw-   0        0        0     5191 2023-05-14 08:50:46.000000 uplogic-1.9/uplogic/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:20:06.699483 uplogic-1.9/uplogic/nodes/actions/
+-rw-rw-rw-   0        0        0     8023 2023-05-16 08:46:11.000000 uplogic-1.9/uplogic/nodes/actions/__init__.py
+-rw-rw-rw-   0        0        0     4065 2022-11-02 09:25:32.000000 uplogic-1.9/uplogic/nodes/actions/addfilter.py
+-rw-rw-rw-   0        0        0     1308 2022-08-21 23:02:22.000000 uplogic-1.9/uplogic/nodes/actions/addobject.py
+-rw-rw-rw-   0        0        0     2710 2022-04-24 07:51:50.000000 uplogic-1.9/uplogic/nodes/actions/addphysicsconstraint.py
+-rw-rw-rw-   0        0        0      797 2023-03-01 15:33:33.000000 uplogic-1.9/uplogic/nodes/actions/adduiwidget.py
+-rw-rw-rw-   0        0        0     1420 2022-10-28 14:13:34.000000 uplogic-1.9/uplogic/nodes/actions/alignaxistovector.py
+-rw-rw-rw-   0        0        0     1056 2022-01-12 11:55:23.000000 uplogic-1.9/uplogic/nodes/actions/appendlistitem.py
+-rw-rw-rw-   0        0        0     1007 2022-01-12 13:37:33.000000 uplogic-1.9/uplogic/nodes/actions/applyforce.py
+-rw-rw-rw-   0        0        0     1187 2022-01-12 13:38:47.000000 uplogic-1.9/uplogic/nodes/actions/applyimpulse.py
+-rw-rw-rw-   0        0        0     1074 2022-01-12 13:36:04.000000 uplogic-1.9/uplogic/nodes/actions/applymovement.py
+-rw-rw-rw-   0        0        0     1237 2023-01-05 15:34:33.000000 uplogic-1.9/uplogic/nodes/actions/applyrotation.py
+-rw-rw-rw-   0        0        0      984 2022-01-12 14:18:21.000000 uplogic-1.9/uplogic/nodes/actions/applytorque.py
+-rw-rw-rw-   0        0        0     2560 2022-01-10 18:02:58.000000 uplogic-1.9/uplogic/nodes/actions/cameraraycast.py
+-rw-rw-rw-   0        0        0     1014 2022-01-12 14:08:55.000000 uplogic-1.9/uplogic/nodes/actions/characterjump.py
+-rw-rw-rw-   0        0        0     1536 2022-04-10 10:15:42.000000 uplogic-1.9/uplogic/nodes/actions/clampedmodifyproperty.py
+-rw-rw-rw-   0        0        0     1610 2023-05-14 08:51:40.000000 uplogic-1.9/uplogic/nodes/actions/clearvariables.py
+-rw-rw-rw-   0        0        0     1395 2022-04-09 10:45:53.000000 uplogic-1.9/uplogic/nodes/actions/copyproperty.py
+-rw-rw-rw-   0        0        0     3483 2023-03-08 16:42:06.000000 uplogic-1.9/uplogic/nodes/actions/createuibutton.py
+-rw-rw-rw-   0        0        0      821 2023-03-01 15:34:01.000000 uplogic-1.9/uplogic/nodes/actions/createuicanvas.py
+-rw-rw-rw-   0        0        0     1695 2023-03-02 19:57:36.000000 uplogic-1.9/uplogic/nodes/actions/createuiimage.py
+-rw-rw-rw-   0        0        0     2478 2023-03-02 21:54:35.000000 uplogic-1.9/uplogic/nodes/actions/createuilabel.py
+-rw-rw-rw-   0        0        0     2292 2023-03-08 16:42:38.000000 uplogic-1.9/uplogic/nodes/actions/createuilayout.py
+-rw-rw-rw-   0        0        0     2003 2023-05-14 08:51:47.000000 uplogic-1.9/uplogic/nodes/actions/createvehicle.py
+-rw-rw-rw-   0        0        0     1523 2022-09-11 14:27:22.000000 uplogic-1.9/uplogic/nodes/actions/cursorbehavior.py
+-rw-rw-rw-   0        0        0      797 2023-03-02 21:19:09.000000 uplogic-1.9/uplogic/nodes/actions/cursorvisibility.py
+-rw-rw-rw-   0        0        0     1245 2023-05-14 08:51:57.000000 uplogic-1.9/uplogic/nodes/actions/dispatchevent.py
+-rw-rw-rw-   0        0        0     1188 2023-05-14 08:52:09.000000 uplogic-1.9/uplogic/nodes/actions/drawbox.py
+-rw-rw-rw-   0        0        0     1028 2023-05-14 08:52:17.000000 uplogic-1.9/uplogic/nodes/actions/drawcube.py
+-rw-rw-rw-   0        0        0      980 2022-08-23 18:34:20.000000 uplogic-1.9/uplogic/nodes/actions/drawline.py
+-rw-rw-rw-   0        0        0     3560 2022-01-12 12:12:44.000000 uplogic-1.9/uplogic/nodes/actions/editbone.py
+-rw-rw-rw-   0        0        0      530 2022-07-18 15:47:27.000000 uplogic-1.9/uplogic/nodes/actions/endgame.py
+-rw-rw-rw-   0        0        0     1019 2022-01-12 13:25:49.000000 uplogic-1.9/uplogic/nodes/actions/endobject.py
+-rw-rw-rw-   0        0        0     1237 2022-02-07 22:47:57.000000 uplogic-1.9/uplogic/nodes/actions/executesubnetwork.py
+-rw-rw-rw-   0        0        0     5569 2023-05-14 08:52:39.000000 uplogic-1.9/uplogic/nodes/actions/followpath.py
+-rw-rw-rw-   0        0        0     4120 2023-05-14 08:52:59.000000 uplogic-1.9/uplogic/nodes/actions/gamepadlook.py
+-rw-rw-rw-   0        0        0     1395 2023-05-14 08:53:21.000000 uplogic-1.9/uplogic/nodes/actions/gamepadvibration.py
+-rw-rw-rw-   0        0        0     2383 2022-01-12 12:04:24.000000 uplogic-1.9/uplogic/nodes/actions/getperformanceprofile.py
+-rw-rw-rw-   0        0        0     1373 2022-02-07 22:56:45.000000 uplogic-1.9/uplogic/nodes/actions/installsubnetwork.py
+-rw-rw-rw-   0        0        0     1976 2023-04-26 12:34:19.000000 uplogic-1.9/uplogic/nodes/actions/instream.py
+-rw-rw-rw-   0        0        0     1326 2022-01-12 15:09:37.000000 uplogic-1.9/uplogic/nodes/actions/listglobalvalues.py
+-rw-rw-rw-   0        0        0     2110 2023-05-14 08:53:38.000000 uplogic-1.9/uplogic/nodes/actions/listvariables.py
+-rw-rw-rw-   0        0        0      674 2022-01-10 11:08:34.000000 uplogic-1.9/uplogic/nodes/actions/loadblendfile.py
+-rw-rw-rw-   0        0        0     1586 2023-05-14 08:53:49.000000 uplogic-1.9/uplogic/nodes/actions/loadfilecontent.py
+-rw-rw-rw-   0        0        0     4266 2023-05-14 08:54:00.000000 uplogic-1.9/uplogic/nodes/actions/loadgame.py
+-rw-rw-rw-   0        0        0     1658 2023-05-14 08:54:06.000000 uplogic-1.9/uplogic/nodes/actions/loadscene.py
+-rw-rw-rw-   0        0        0     2515 2023-05-16 10:27:44.000000 uplogic-1.9/uplogic/nodes/actions/localclient.py
+-rw-rw-rw-   0        0        0     2391 2023-05-16 10:27:30.000000 uplogic-1.9/uplogic/nodes/actions/localserver.py
+-rw-rw-rw-   0        0        0     1051 2022-01-12 15:17:30.000000 uplogic-1.9/uplogic/nodes/actions/makeuniquelight.py
+-rw-rw-rw-   0        0        0     1363 2022-04-10 10:15:35.000000 uplogic-1.9/uplogic/nodes/actions/modifyproperty.py
+-rw-rw-rw-   0        0        0     4870 2023-05-14 08:54:21.000000 uplogic-1.9/uplogic/nodes/actions/mouselook.py
+-rw-rw-rw-   0        0        0     2144 2022-01-10 18:01:11.000000 uplogic-1.9/uplogic/nodes/actions/mouseraycast.py
+-rw-rw-rw-   0        0        0     1012 2022-01-10 11:08:34.000000 uplogic-1.9/uplogic/nodes/actions/mousesetposition.py
+-rw-rw-rw-   0        0        0     1521 2023-05-14 08:54:30.000000 uplogic-1.9/uplogic/nodes/actions/moveto.py
+-rw-rw-rw-   0        0        0     5217 2023-05-14 08:54:42.000000 uplogic-1.9/uplogic/nodes/actions/movetowithnavmesh.py
+-rw-rw-rw-   0        0        0      626 2022-01-12 14:35:38.000000 uplogic-1.9/uplogic/nodes/actions/pausesound.py
+-rw-rw-rw-   0        0        0     5400 2023-05-14 08:54:59.000000 uplogic-1.9/uplogic/nodes/actions/playaction.py
+-rw-rw-rw-   0        0        0     2476 2023-02-12 11:22:41.000000 uplogic-1.9/uplogic/nodes/actions/playsequence.py
+-rw-rw-rw-   0        0        0     1338 2023-05-14 08:55:21.000000 uplogic-1.9/uplogic/nodes/actions/popdictkey.py
+-rw-rw-rw-   0        0        0      762 2023-05-16 10:26:49.000000 uplogic-1.9/uplogic/nodes/actions/printvalue.py
+-rw-rw-rw-   0        0        0     3218 2023-05-16 10:40:40.000000 uplogic-1.9/uplogic/nodes/actions/projectileraycast.py
+-rw-rw-rw-   0        0        0     3516 2022-09-11 15:14:18.000000 uplogic-1.9/uplogic/nodes/actions/raycast.py
+-rw-rw-rw-   0        0        0      842 2022-09-06 10:05:33.000000 uplogic-1.9/uplogic/nodes/actions/removefilter.py
+-rw-rw-rw-   0        0        0     1176 2022-01-12 11:59:50.000000 uplogic-1.9/uplogic/nodes/actions/removelistindex.py
+-rw-rw-rw-   0        0        0     1207 2022-01-12 11:59:09.000000 uplogic-1.9/uplogic/nodes/actions/removelistvalue.py
+-rw-rw-rw-   0        0        0      779 2022-01-10 11:08:34.000000 uplogic-1.9/uplogic/nodes/actions/removeoverlaycollection.py
+-rw-rw-rw-   0        0        0      969 2022-02-01 19:49:18.000000 uplogic-1.9/uplogic/nodes/actions/removeparent.py
+-rw-rw-rw-   0        0        0      974 2022-01-12 15:45:41.000000 uplogic-1.9/uplogic/nodes/actions/removephysicsconstraint.py
+-rw-rw-rw-   0        0        0     1834 2023-02-14 10:14:02.000000 uplogic-1.9/uplogic/nodes/actions/removevariable.py
+-rw-rw-rw-   0        0        0     1255 2022-01-12 15:43:12.000000 uplogic-1.9/uplogic/nodes/actions/replacemesh.py
+-rw-rw-rw-   0        0        0      633 2022-02-10 19:19:01.000000 uplogic-1.9/uplogic/nodes/actions/restartgame.py
+-rw-rw-rw-   0        0        0      628 2022-01-12 14:37:05.000000 uplogic-1.9/uplogic/nodes/actions/resumesound.py
+-rw-rw-rw-   0        0        0     2212 2023-05-14 09:02:36.000000 uplogic-1.9/uplogic/nodes/actions/rotateto.py
+-rw-rw-rw-   0        0        0     1199 2022-02-09 13:38:34.000000 uplogic-1.9/uplogic/nodes/actions/runactuator.py
+-rw-rw-rw-   0        0        0     1716 2023-05-15 10:27:54.000000 uplogic-1.9/uplogic/nodes/actions/runpython.py
+-rw-rw-rw-   0        0        0     7976 2022-02-08 15:48:21.000000 uplogic-1.9/uplogic/nodes/actions/savegame.py
+-rw-rw-rw-   0        0        0     2005 2023-02-14 10:08:13.000000 uplogic-1.9/uplogic/nodes/actions/savevariable.py
+-rw-rw-rw-   0        0        0     1738 2023-02-14 10:08:29.000000 uplogic-1.9/uplogic/nodes/actions/savevariabledict.py
+-rw-rw-rw-   0        0        0     1180 2022-01-10 17:48:43.000000 uplogic-1.9/uplogic/nodes/actions/sendmessage.py
+-rw-rw-rw-   0        0        0      849 2023-05-16 09:59:36.000000 uplogic-1.9/uplogic/nodes/actions/sendnetworkmessage.py
+-rw-rw-rw-   0        0        0     2608 2023-02-13 17:09:10.000000 uplogic-1.9/uplogic/nodes/actions/setactionframe.py
+-rw-rw-rw-   0        0        0     1135 2022-02-26 12:20:29.000000 uplogic-1.9/uplogic/nodes/actions/setactuatorvalue.py
+-rw-rw-rw-   0        0        0     1532 2022-01-12 13:30:41.000000 uplogic-1.9/uplogic/nodes/actions/setboneconstraintattr.py
+-rw-rw-rw-   0        0        0     1389 2022-01-12 12:09:35.000000 uplogic-1.9/uplogic/nodes/actions/setboneconstraintinfluence.py
+-rw-rw-rw-   0        0        0     1382 2022-01-12 12:08:54.000000 uplogic-1.9/uplogic/nodes/actions/setboneconstrainttarget.py
+-rw-rw-rw-   0        0        0     1488 2022-01-12 12:15:32.000000 uplogic-1.9/uplogic/nodes/actions/setboneposition.py
+-rw-rw-rw-   0        0        0      944 2022-01-10 18:05:42.000000 uplogic-1.9/uplogic/nodes/actions/setcamera.py
+-rw-rw-rw-   0        0        0      941 2022-01-23 23:21:22.000000 uplogic-1.9/uplogic/nodes/actions/setcamerafov.py
+-rw-rw-rw-   0        0        0      966 2022-01-10 18:09:57.000000 uplogic-1.9/uplogic/nodes/actions/setcameraorthoscale.py
+-rw-rw-rw-   0        0        0     1154 2022-01-12 14:13:53.000000 uplogic-1.9/uplogic/nodes/actions/setcharactergravity.py
+-rw-rw-rw-   0        0        0     1102 2022-01-12 14:08:37.000000 uplogic-1.9/uplogic/nodes/actions/setcharacterjumpspeed.py
+-rw-rw-rw-   0        0        0     1096 2022-01-12 14:09:24.000000 uplogic-1.9/uplogic/nodes/actions/setcharactermaxjumps.py
+-rw-rw-rw-   0        0        0     1200 2022-01-12 14:17:03.000000 uplogic-1.9/uplogic/nodes/actions/setcharactervelocity.py
+-rw-rw-rw-   0        0        0     1795 2022-01-12 14:14:18.000000 uplogic-1.9/uplogic/nodes/actions/setcharacterwalkdir.py
+-rw-rw-rw-   0        0        0     1030 2022-01-12 13:44:27.000000 uplogic-1.9/uplogic/nodes/actions/setcollisiongroup.py
+-rw-rw-rw-   0        0        0     1028 2022-01-12 13:45:39.000000 uplogic-1.9/uplogic/nodes/actions/setcollisionmask.py
+-rw-rw-rw-   0        0        0     1493 2022-02-16 14:17:45.000000 uplogic-1.9/uplogic/nodes/actions/setcurvepoints.py
+-rw-rw-rw-   0        0        0     1095 2023-05-03 10:24:19.000000 uplogic-1.9/uplogic/nodes/actions/setcustomcursor.py
+-rw-rw-rw-   0        0        0     1105 2022-01-12 11:43:10.000000 uplogic-1.9/uplogic/nodes/actions/setdictkey.py
+-rw-rw-rw-   0        0        0     1166 2022-09-07 10:43:04.000000 uplogic-1.9/uplogic/nodes/actions/setdynamics.py
+-rw-rw-rw-   0        0        0      887 2022-01-12 15:03:06.000000 uplogic-1.9/uplogic/nodes/actions/seteeveeao.py
+-rw-rw-rw-   0        0        0      891 2022-01-12 16:00:43.000000 uplogic-1.9/uplogic/nodes/actions/seteeveebloom.py
+-rw-rw-rw-   0        0        0      895 2022-01-12 15:08:25.000000 uplogic-1.9/uplogic/nodes/actions/seteeveesmaa.py
+-rw-rw-rw-   0        0        0      902 2022-01-12 15:12:11.000000 uplogic-1.9/uplogic/nodes/actions/seteeveesmaaquality.py
+-rw-rw-rw-   0        0        0      887 2022-01-12 15:04:58.000000 uplogic-1.9/uplogic/nodes/actions/seteeveessr.py
+-rw-rw-rw-   0        0        0      933 2022-01-12 15:05:54.000000 uplogic-1.9/uplogic/nodes/actions/seteeveevolumetrics.py
+-rw-rw-rw-   0        0        0      920 2022-02-06 14:06:39.000000 uplogic-1.9/uplogic/nodes/actions/setexposure.py
+-rw-rw-rw-   0        0        0      935 2022-09-06 10:37:29.000000 uplogic-1.9/uplogic/nodes/actions/setfilterstate.py
+-rw-rw-rw-   0        0        0      858 2022-01-10 18:13:34.000000 uplogic-1.9/uplogic/nodes/actions/setfullscreen.py
+-rw-rw-rw-   0        0        0     1938 2022-01-10 17:22:40.000000 uplogic-1.9/uplogic/nodes/actions/setgameobjectattr.py
+-rw-rw-rw-   0        0        0      914 2022-01-12 15:01:16.000000 uplogic-1.9/uplogic/nodes/actions/setgamma.py
+-rw-rw-rw-   0        0        0     1456 2022-01-12 15:57:52.000000 uplogic-1.9/uplogic/nodes/actions/setglobalvalue.py
+-rw-rw-rw-   0        0        0      933 2022-01-12 13:28:24.000000 uplogic-1.9/uplogic/nodes/actions/setgravity.py
+-rw-rw-rw-   0        0        0     1012 2022-01-12 15:24:08.000000 uplogic-1.9/uplogic/nodes/actions/setlightcolor.py
+-rw-rw-rw-   0        0        0      959 2022-01-12 15:16:33.000000 uplogic-1.9/uplogic/nodes/actions/setlightenergy.py
+-rw-rw-rw-   0        0        0      983 2022-01-12 15:19:36.000000 uplogic-1.9/uplogic/nodes/actions/setlightshadow.py
+-rw-rw-rw-   0        0        0     1137 2022-01-12 11:56:28.000000 uplogic-1.9/uplogic/nodes/actions/setlistindex.py
+-rw-rw-rw-   0        0        0     1321 2022-01-10 11:08:34.000000 uplogic-1.9/uplogic/nodes/actions/setmaterial.py
+-rw-rw-rw-   0        0        0     1412 2022-01-10 12:35:51.000000 uplogic-1.9/uplogic/nodes/actions/setmatnodesocket.py
+-rw-rw-rw-   0        0        0     1610 2022-01-10 11:08:34.000000 uplogic-1.9/uplogic/nodes/actions/setmatnodevalue.py
+-rw-rw-rw-   0        0        0     1388 2022-01-10 11:08:34.000000 uplogic-1.9/uplogic/nodes/actions/setnodesocket.py
+-rw-rw-rw-   0        0        0     1622 2022-01-10 11:08:34.000000 uplogic-1.9/uplogic/nodes/actions/setnodevalue.py
+-rw-rw-rw-   0        0        0      863 2022-01-10 11:08:34.000000 uplogic-1.9/uplogic/nodes/actions/setoverlaycollection.py
+-rw-rw-rw-   0        0        0     1188 2022-01-12 12:01:10.000000 uplogic-1.9/uplogic/nodes/actions/setparent.py
+-rw-rw-rw-   0        0        0     1188 2022-01-12 16:00:43.000000 uplogic-1.9/uplogic/nodes/actions/setphysics.py
+-rw-rw-rw-   0        0        0      838 2022-01-10 18:14:35.000000 uplogic-1.9/uplogic/nodes/actions/setprofile.py
+-rw-rw-rw-   0        0        0     1383 2022-10-05 12:35:18.000000 uplogic-1.9/uplogic/nodes/actions/setproperty.py
+-rw-rw-rw-   0        0        0      736 2022-01-10 11:08:34.000000 uplogic-1.9/uplogic/nodes/actions/setpyinstanceattr.py
+-rw-rw-rw-   0        0        0      898 2022-01-23 23:21:22.000000 uplogic-1.9/uplogic/nodes/actions/setresolution.py
+-rw-rw-rw-   0        0        0     1085 2022-01-12 13:12:07.000000 uplogic-1.9/uplogic/nodes/actions/setrigidbody.py
+-rw-rw-rw-   0        0        0      820 2022-10-04 11:00:44.000000 uplogic-1.9/uplogic/nodes/actions/setscene.py
+-rw-rw-rw-   0        0        0     1200 2022-02-04 18:03:35.000000 uplogic-1.9/uplogic/nodes/actions/setsensorvalue.py
+-rw-rw-rw-   0        0        0      949 2022-01-12 13:27:30.000000 uplogic-1.9/uplogic/nodes/actions/settimescale.py
+-rw-rw-rw-   0        0        0     2388 2023-03-02 19:55:31.000000 uplogic-1.9/uplogic/nodes/actions/setuiwidgetattr.py
+-rw-rw-rw-   0        0        0     2913 2022-02-06 12:41:13.000000 uplogic-1.9/uplogic/nodes/actions/setvisibility.py
+-rw-rw-rw-   0        0        0      828 2022-01-12 11:22:14.000000 uplogic-1.9/uplogic/nodes/actions/setvsync.py
+-rw-rw-rw-   0        0        0      853 2022-01-10 18:19:10.000000 uplogic-1.9/uplogic/nodes/actions/showframerate.py
+-rw-rw-rw-   0        0        0     1519 2023-05-14 08:56:41.000000 uplogic-1.9/uplogic/nodes/actions/slowfollow.py
+-rw-rw-rw-   0        0        0     3572 2023-05-16 11:15:30.000000 uplogic-1.9/uplogic/nodes/actions/spawnpool.py
+-rw-rw-rw-   0        0        0     2051 2023-03-06 08:53:53.000000 uplogic-1.9/uplogic/nodes/actions/startsound.py
+-rw-rw-rw-   0        0        0     3107 2023-03-06 08:54:22.000000 uplogic-1.9/uplogic/nodes/actions/startsound3d.py
+-rw-rw-rw-   0        0        0     2541 2023-03-06 08:54:22.000000 uplogic-1.9/uplogic/nodes/actions/startspeaker.py
+-rw-rw-rw-   0        0        0     1436 2023-05-14 08:57:02.000000 uplogic-1.9/uplogic/nodes/actions/startsubnetwork.py
+-rw-rw-rw-   0        0        0     1597 2022-10-07 11:19:16.000000 uplogic-1.9/uplogic/nodes/actions/stopaction.py
+-rw-rw-rw-   0        0        0      591 2022-01-12 14:34:57.000000 uplogic-1.9/uplogic/nodes/actions/stopallsounds.py
+-rw-rw-rw-   0        0        0      624 2022-01-12 14:28:14.000000 uplogic-1.9/uplogic/nodes/actions/stopsound.py
+-rw-rw-rw-   0        0        0     1209 2022-02-07 22:56:33.000000 uplogic-1.9/uplogic/nodes/actions/stopsubnetwork.py
+-rw-rw-rw-   0        0        0      842 2022-09-06 10:25:56.000000 uplogic-1.9/uplogic/nodes/actions/togglefilter.py
+-rw-rw-rw-   0        0        0     1227 2022-04-09 10:37:36.000000 uplogic-1.9/uplogic/nodes/actions/toggleproperty.py
+-rw-rw-rw-   0        0        0     2809 2022-01-12 14:57:52.000000 uplogic-1.9/uplogic/nodes/actions/translate.py
+-rw-rw-rw-   0        0        0     1391 2023-05-14 08:57:16.000000 uplogic-1.9/uplogic/nodes/actions/vehicleapplybraking.py
+-rw-rw-rw-   0        0        0     1379 2023-05-14 08:57:23.000000 uplogic-1.9/uplogic/nodes/actions/vehicleapplyforce.py
+-rw-rw-rw-   0        0        0     1392 2023-05-14 08:57:30.000000 uplogic-1.9/uplogic/nodes/actions/vehicleapplysteering.py
+-rw-rw-rw-   0        0        0     3473 2023-05-14 08:57:36.000000 uplogic-1.9/uplogic/nodes/actions/vehiclesetattributes.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:20:06.756495 uplogic-1.9/uplogic/nodes/conditions/
+-rw-rw-rw-   0        0        0     1946 2022-01-20 14:15:37.000000 uplogic-1.9/uplogic/nodes/conditions/__init__.py
+-rw-rw-rw-   0        0        0      935 2022-01-12 13:06:20.000000 uplogic-1.9/uplogic/nodes/conditions/barrier.py
+-rw-rw-rw-   0        0        0     2397 2023-05-14 08:57:52.000000 uplogic-1.9/uplogic/nodes/conditions/checkdistance.py
+-rw-rw-rw-   0        0        0     4779 2023-01-14 13:34:38.000000 uplogic-1.9/uplogic/nodes/conditions/collision.py
+-rw-rw-rw-   0        0        0     1508 2023-05-14 08:58:21.000000 uplogic-1.9/uplogic/nodes/conditions/compare.py
+-rw-rw-rw-   0        0        0     2175 2023-05-14 08:58:27.000000 uplogic-1.9/uplogic/nodes/conditions/comparevectors.py
+-rw-rw-rw-   0        0        0     3288 2022-01-10 17:39:46.000000 uplogic-1.9/uplogic/nodes/conditions/controllerstatus.py
+-rw-rw-rw-   0        0        0     1497 2023-05-14 08:58:34.000000 uplogic-1.9/uplogic/nodes/conditions/evaluateproperty.py
+-rw-rw-rw-   0        0        0      756 2022-01-28 16:50:48.000000 uplogic-1.9/uplogic/nodes/conditions/gamepadactive.py
+-rw-rw-rw-   0        0        0     1503 2023-05-14 08:58:39.000000 uplogic-1.9/uplogic/nodes/conditions/gamepadbutton.py
+-rw-rw-rw-   0        0        0     1782 2023-05-14 08:58:43.000000 uplogic-1.9/uplogic/nodes/conditions/gamepadbuttonup.py
+-rw-rw-rw-   0        0        0     1093 2023-05-14 08:58:51.000000 uplogic-1.9/uplogic/nodes/conditions/handleevent.py
+-rw-rw-rw-   0        0        0     1219 2023-05-14 08:58:56.000000 uplogic-1.9/uplogic/nodes/conditions/hasproperty.py
+-rw-rw-rw-   0        0        0      303 2021-12-21 09:41:07.000000 uplogic-1.9/uplogic/nodes/conditions/keyboardactive.py
+-rw-rw-rw-   0        0        0      812 2022-01-10 11:08:34.000000 uplogic-1.9/uplogic/nodes/conditions/keypressed.py
+-rw-rw-rw-   0        0        0      756 2022-01-10 11:08:34.000000 uplogic-1.9/uplogic/nodes/conditions/keyreleased.py
+-rw-rw-rw-   0        0        0     1705 2022-02-04 11:39:59.000000 uplogic-1.9/uplogic/nodes/conditions/logicand.py
+-rw-rw-rw-   0        0        0      621 2022-02-04 11:45:26.000000 uplogic-1.9/uplogic/nodes/conditions/logicandnot.py
+-rw-rw-rw-   0        0        0      325 2022-01-10 11:08:34.000000 uplogic-1.9/uplogic/nodes/conditions/logicnone.py
+-rw-rw-rw-   0        0        0      768 2023-05-14 08:59:42.000000 uplogic-1.9/uplogic/nodes/conditions/logicnot.py
+-rw-rw-rw-   0        0        0      334 2022-01-10 11:08:34.000000 uplogic-1.9/uplogic/nodes/conditions/logicnotnone.py
+-rw-rw-rw-   0        0        0     1168 2023-05-14 09:15:28.000000 uplogic-1.9/uplogic/nodes/conditions/logicor.py
+-rw-rw-rw-   0        0        0     1681 2023-05-14 09:15:55.000000 uplogic-1.9/uplogic/nodes/conditions/logictreestatus.py
+-rw-rw-rw-   0        0        0      494 2022-09-11 14:46:42.000000 uplogic-1.9/uplogic/nodes/conditions/mousemoved.py
+-rw-rw-rw-   0        0        0     3567 2022-09-11 14:47:44.000000 uplogic-1.9/uplogic/nodes/conditions/mouseover.py
+-rw-rw-rw-   0        0        0     1313 2023-05-14 09:00:04.000000 uplogic-1.9/uplogic/nodes/conditions/mousepressed.py
+-rw-rw-rw-   0        0        0     1740 2023-05-14 09:00:09.000000 uplogic-1.9/uplogic/nodes/conditions/mousepressedon.py
+-rw-rw-rw-   0        0        0     1302 2023-05-14 09:00:16.000000 uplogic-1.9/uplogic/nodes/conditions/mousereleased.py
+-rw-rw-rw-   0        0        0      700 2022-09-11 14:54:01.000000 uplogic-1.9/uplogic/nodes/conditions/mousescroll.py
+-rw-rw-rw-   0        0        0     1071 2022-01-10 11:08:34.000000 uplogic-1.9/uplogic/nodes/conditions/once.py
+-rw-rw-rw-   0        0        0      358 2023-05-14 09:00:22.000000 uplogic-1.9/uplogic/nodes/conditions/oninit.py
+-rw-rw-rw-   0        0        0      704 2023-04-06 11:05:27.000000 uplogic-1.9/uplogic/nodes/conditions/onnexttick.py
+-rw-rw-rw-   0        0        0      359 2023-05-14 09:00:29.000000 uplogic-1.9/uplogic/nodes/conditions/onupdate.py
+-rw-rw-rw-   0        0        0     1270 2022-01-10 11:25:35.000000 uplogic-1.9/uplogic/nodes/conditions/onvaluechanged.py
+-rw-rw-rw-   0        0        0     1238 2023-05-14 09:00:33.000000 uplogic-1.9/uplogic/nodes/conditions/onvaluechangedto.py
+-rw-rw-rw-   0        0        0     1474 2022-05-25 09:41:06.000000 uplogic-1.9/uplogic/nodes/conditions/pulsify.py
+-rw-rw-rw-   0        0        0     1105 2023-05-14 09:16:25.000000 uplogic-1.9/uplogic/nodes/conditions/sensorpositive.py
+-rw-rw-rw-   0        0        0      940 2022-01-17 10:41:45.000000 uplogic-1.9/uplogic/nodes/conditions/timedelay.py
+-rw-rw-rw-   0        0        0      918 2022-01-10 11:08:34.000000 uplogic-1.9/uplogic/nodes/conditions/timer.py
+-rw-rw-rw-   0        0        0      548 2022-01-10 11:08:34.000000 uplogic-1.9/uplogic/nodes/conditions/truefalse.py
+-rw-rw-rw-   0        0        0      377 2022-01-10 11:08:34.000000 uplogic-1.9/uplogic/nodes/conditions/valuevalid.py
+-rw-rw-rw-   0        0        0     8487 2023-05-14 08:51:12.000000 uplogic-1.9/uplogic/nodes/logictree.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:20:06.889526 uplogic-1.9/uplogic/nodes/parameters/
+-rw-rw-rw-   0        0        0     4727 2023-05-16 09:26:14.000000 uplogic-1.9/uplogic/nodes/parameters/__init__.py
+-rw-rw-rw-   0        0        0      648 2023-05-14 09:00:44.000000 uplogic-1.9/uplogic/nodes/parameters/absolutevalue.py
+-rw-rw-rw-   0        0        0     1713 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/actionstatus.py
+-rw-rw-rw-   0        0        0      585 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/activecamera.py
+-rw-rw-rw-   0        0        0      909 2023-05-14 09:01:31.000000 uplogic-1.9/uplogic/nodes/parameters/axisvector.py
+-rw-rw-rw-   0        0        0     1923 2023-05-14 09:01:36.000000 uplogic-1.9/uplogic/nodes/parameters/bonestatus.py
+-rw-rw-rw-   0        0        0     1911 2022-01-10 11:25:35.000000 uplogic-1.9/uplogic/nodes/parameters/characterinfo.py
+-rw-rw-rw-   0        0        0     1158 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/childbyindex.py
+-rw-rw-rw-   0        0        0      903 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/childbyname.py
+-rw-rw-rw-   0        0        0     1116 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/clamp.py
+-rw-rw-rw-   0        0        0      792 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/colorrgb.py
+-rw-rw-rw-   0        0        0      719 2022-01-10 11:25:35.000000 uplogic-1.9/uplogic/nodes/parameters/colorrgba.py
+-rw-rw-rw-   0        0        0      911 2022-02-17 16:47:54.000000 uplogic-1.9/uplogic/nodes/parameters/dictvalue.py
+-rw-rw-rw-   0        0        0      920 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/distance.py
+-rw-rw-rw-   0        0        0      910 2022-01-10 11:25:35.000000 uplogic-1.9/uplogic/nodes/parameters/euler.py
+-rw-rw-rw-   0        0        0      786 2022-01-10 11:25:35.000000 uplogic-1.9/uplogic/nodes/parameters/eulertomatrix.py
+-rw-rw-rw-   0        0        0     1284 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/formattedstring.py
+-rw-rw-rw-   0        0        0     2158 2022-01-10 11:25:35.000000 uplogic-1.9/uplogic/nodes/parameters/formula.py
+-rw-rw-rw-   0        0        0     1825 2023-02-06 12:32:50.000000 uplogic-1.9/uplogic/nodes/parameters/gamepadsticks.py
+-rw-rw-rw-   0        0        0     1563 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/gamepadtrigger.py
+-rw-rw-rw-   0        0        0     1097 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/getactuatorvalue.py
+-rw-rw-rw-   0        0        0      612 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/getcollection.py
+-rw-rw-rw-   0        0        0     1056 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/getcollectionobjectnames.py
+-rw-rw-rw-   0        0        0     1047 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/getcollectionobjects.py
+-rw-rw-rw-   0        0        0     1055 2022-01-10 11:25:35.000000 uplogic-1.9/uplogic/nodes/parameters/getcurvepoints.py
+-rw-rw-rw-   0        0        0      527 2023-03-02 19:33:55.000000 uplogic-1.9/uplogic/nodes/parameters/getfont.py
+-rw-rw-rw-   0        0        0      385 2022-01-12 11:04:44.000000 uplogic-1.9/uplogic/nodes/parameters/getfullscreen.py
+-rw-rw-rw-   0        0        0     1100 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/getglobalvalue.py
+-rw-rw-rw-   0        0        0      432 2021-12-21 09:41:07.000000 uplogic-1.9/uplogic/nodes/parameters/getgravity.py
+-rw-rw-rw-   0        0        0      534 2022-01-10 11:08:34.000000 uplogic-1.9/uplogic/nodes/parameters/getimage.py
+-rw-rw-rw-   0        0        0      648 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/getlightcolor.py
+-rw-rw-rw-   0        0        0      654 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/getlightenergy.py
+-rw-rw-rw-   0        0        0     1420 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/getnodeattribute.py
+-rw-rw-rw-   0        0        0     1294 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/getnodesocket.py
+-rw-rw-rw-   0        0        0      762 2023-05-16 10:12:45.000000 uplogic-1.9/uplogic/nodes/parameters/getobject.py
+-rw-rw-rw-   0        0        0      442 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/getowner.py
+-rw-rw-rw-   0        0        0      614 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/getparent.py
+-rw-rw-rw-   0        0        0     1080 2023-05-14 16:12:28.000000 uplogic-1.9/uplogic/nodes/parameters/getproperty.py
+-rw-rw-rw-   0        0        0      715 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/getpyinstanceattr.py
+-rw-rw-rw-   0        0        0      760 2022-01-12 11:11:52.000000 uplogic-1.9/uplogic/nodes/parameters/getresolution.py
+-rw-rw-rw-   0        0        0      384 2021-12-21 09:41:07.000000 uplogic-1.9/uplogic/nodes/parameters/getscene.py
+-rw-rw-rw-   0        0        0      954 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/getsensorvalue.py
+-rw-rw-rw-   0        0        0      572 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/getsound.py
+-rw-rw-rw-   0        0        0      385 2021-12-21 09:41:07.000000 uplogic-1.9/uplogic/nodes/parameters/gettimescale.py
+-rw-rw-rw-   0        0        0     1070 2023-03-02 22:50:45.000000 uplogic-1.9/uplogic/nodes/parameters/getuiwidgetattr.py
+-rw-rw-rw-   0        0        0      375 2022-01-12 11:01:47.000000 uplogic-1.9/uplogic/nodes/parameters/getvsync.py
+-rw-rw-rw-   0        0        0      429 2022-01-12 11:37:03.000000 uplogic-1.9/uplogic/nodes/parameters/initemptydict.py
+-rw-rw-rw-   0        0        0      599 2022-01-26 18:13:15.000000 uplogic-1.9/uplogic/nodes/parameters/initemptylist.py
+-rw-rw-rw-   0        0        0      652 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/initnewdict.py
+-rw-rw-rw-   0        0        0      873 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/interpolate.py
+-rw-rw-rw-   0        0        0      620 2022-01-10 14:18:19.000000 uplogic-1.9/uplogic/nodes/parameters/invertvalue.py
+-rw-rw-rw-   0        0        0      316 2022-01-10 11:08:17.000000 uplogic-1.9/uplogic/nodes/parameters/keycode.py
+-rw-rw-rw-   0        0        0     1475 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/limitrange.py
+-rw-rw-rw-   0        0        0      620 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/listduplicate.py
+-rw-rw-rw-   0        0        0      823 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/listextend.py
+-rw-rw-rw-   0        0        0      697 2022-12-21 14:09:17.000000 uplogic-1.9/uplogic/nodes/parameters/listfromitems.py
+-rw-rw-rw-   0        0        0      827 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/listindex.py
+-rw-rw-rw-   0        0        0      835 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/listindexrandom.py
+-rw-rw-rw-   0        0        0     1951 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/loadvariable.py
+-rw-rw-rw-   0        0        0     1479 2023-02-14 10:12:26.000000 uplogic-1.9/uplogic/nodes/parameters/loadvariabledict.py
+-rw-rw-rw-   0        0        0     1432 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/materialgetattribute.py
+-rw-rw-rw-   0        0        0      799 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/materialgetnode.py
+-rw-rw-rw-   0        0        0     1300 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/materialgetsocket.py
+-rw-rw-rw-   0        0        0     2549 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/math.py
+-rw-rw-rw-   0        0        0      672 2022-01-30 10:48:51.000000 uplogic-1.9/uplogic/nodes/parameters/matrixtoxyz.py
+-rw-rw-rw-   0        0        0     1278 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/mousedata.py
+-rw-rw-rw-   0        0        0     1037 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/objectattr.py
+-rw-rw-rw-   0        0        0      601 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/objectdataname.py
+-rw-rw-rw-   0        0        0     1146 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/objectdatavertices.py
+-rw-rw-rw-   0        0        0     1222 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/randomfloat.py
+-rw-rw-rw-   0        0        0     1167 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/randomint.py
+-rw-rw-rw-   0        0        0      979 2022-01-16 18:24:15.000000 uplogic-1.9/uplogic/nodes/parameters/randomvect.py
+-rw-rw-rw-   0        0        0     1032 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/rangedthreshold.py
+-rw-rw-rw-   0        0        0      871 2023-05-14 16:12:38.000000 uplogic-1.9/uplogic/nodes/parameters/screenposition.py
+-rw-rw-rw-   0        0        0      829 2023-05-16 09:25:56.000000 uplogic-1.9/uplogic/nodes/parameters/serializedata.py
+-rw-rw-rw-   0        0        0      417 2022-01-10 11:08:17.000000 uplogic-1.9/uplogic/nodes/parameters/simplevalue.py
+-rw-rw-rw-   0        0        0      623 2022-08-21 21:33:43.000000 uplogic-1.9/uplogic/nodes/parameters/storevalue.py
+-rw-rw-rw-   0        0        0     1102 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/threshold.py
+-rw-rw-rw-   0        0        0     1007 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/timedata.py
+-rw-rw-rw-   0        0        0      988 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/typecastvalue.py
+-rw-rw-rw-   0        0        0     4507 2023-05-14 09:01:49.000000 uplogic-1.9/uplogic/nodes/parameters/valueswitch.py
+-rw-rw-rw-   0        0        0      751 2023-05-14 16:12:43.000000 uplogic-1.9/uplogic/nodes/parameters/vectorabsolute.py
+-rw-rw-rw-   0        0        0      886 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/vectorangle.py
+-rw-rw-rw-   0        0        0     1385 2023-05-14 09:01:59.000000 uplogic-1.9/uplogic/nodes/parameters/vectoranglecheck.py
+-rw-rw-rw-   0        0        0      646 2023-05-14 16:12:48.000000 uplogic-1.9/uplogic/nodes/parameters/vectorlength.py
+-rw-rw-rw-   0        0        0     3625 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/vectormath.py
+-rw-rw-rw-   0        0        0      717 2022-01-10 11:08:17.000000 uplogic-1.9/uplogic/nodes/parameters/vectorsplitxy.py
+-rw-rw-rw-   0        0        0     1032 2022-01-30 14:47:33.000000 uplogic-1.9/uplogic/nodes/parameters/vectorsplitxyz.py
+-rw-rw-rw-   0        0        0      691 2023-03-03 08:53:48.000000 uplogic-1.9/uplogic/nodes/parameters/vectorxy.py
+-rw-rw-rw-   0        0        0      818 2022-01-10 11:08:17.000000 uplogic-1.9/uplogic/nodes/parameters/vectorxyz.py
+-rw-rw-rw-   0        0        0      945 2022-01-10 11:08:17.000000 uplogic-1.9/uplogic/nodes/parameters/vectorxyzw.py
+-rw-rw-rw-   0        0        0     1378 2023-03-06 09:01:43.000000 uplogic-1.9/uplogic/nodes/parameters/vrcontrollervalues.py
+-rw-rw-rw-   0        0        0      583 2023-03-06 09:01:01.000000 uplogic-1.9/uplogic/nodes/parameters/vrheadsetvalues.py
+-rw-rw-rw-   0        0        0     1026 2023-05-14 09:01:09.000000 uplogic-1.9/uplogic/nodes/parameters/withinrange.py
+-rw-rw-rw-   0        0        0     1293 2023-05-14 16:12:52.000000 uplogic-1.9/uplogic/nodes/parameters/worldposition.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:20:06.896528 uplogic-1.9/uplogic/physics/
+-rw-rw-rw-   0        0        0      540 2023-03-06 11:18:24.000000 uplogic-1.9/uplogic/physics/__init__.py
+-rw-rw-rw-   0        0        0     4196 2023-05-14 08:28:32.000000 uplogic-1.9/uplogic/physics/buoyancy.py
+-rw-rw-rw-   0        0        0     3627 2023-05-14 08:30:29.000000 uplogic-1.9/uplogic/physics/character.py
+-rw-rw-rw-   0        0        0     3450 2023-05-14 08:29:19.000000 uplogic-1.9/uplogic/physics/collision.py
+-rw-rw-rw-   0        0        0     8370 2023-05-14 08:38:03.000000 uplogic-1.9/uplogic/physics/constraints.py
+-rw-rw-rw-   0        0        0    10072 2023-05-14 08:30:19.000000 uplogic-1.9/uplogic/physics/vehicle.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:20:06.898527 uplogic-1.9/uplogic/serialize/
+-rw-rw-rw-   0        0        0     2945 2023-05-16 08:33:09.000000 uplogic-1.9/uplogic/serialize/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:20:06.923534 uplogic-1.9/uplogic/shaders/
+-rw-rw-rw-   0        0        0      675 2023-04-01 06:53:28.000000 uplogic-1.9/uplogic/shaders/__init__.py
+-rw-rw-rw-   0        0        0      872 2023-04-01 06:53:25.000000 uplogic-1.9/uplogic/shaders/adaptivetonemapping.py
+-rw-rw-rw-   0        0        0     1631 2023-04-01 06:53:32.000000 uplogic-1.9/uplogic/shaders/blur.py
+-rw-rw-rw-   0        0        0      685 2023-04-01 06:54:25.000000 uplogic-1.9/uplogic/shaders/brightness.py
+-rw-rw-rw-   0        0        0     1050 2023-04-01 06:54:25.000000 uplogic-1.9/uplogic/shaders/chromaticaberration.py
+-rw-rw-rw-   0        0        0     8869 2023-04-01 06:54:25.000000 uplogic-1.9/uplogic/shaders/distort.py
+-rw-rw-rw-   0        0        0     9818 2023-04-01 06:54:25.000000 uplogic-1.9/uplogic/shaders/dof.py
+-rw-rw-rw-   0        0        0     9106 2023-04-01 06:54:25.000000 uplogic-1.9/uplogic/shaders/droplets.py
+-rw-rw-rw-   0        0        0    33424 2023-04-01 06:54:25.000000 uplogic-1.9/uplogic/shaders/fxaa.py
+-rw-rw-rw-   0        0        0      916 2023-04-01 06:54:25.000000 uplogic-1.9/uplogic/shaders/grayscale.py
+-rw-rw-rw-   0        0        0     9684 2023-04-01 06:54:25.000000 uplogic-1.9/uplogic/shaders/hbao.py
+-rw-rw-rw-   0        0        0     1173 2023-04-01 06:54:25.000000 uplogic-1.9/uplogic/shaders/letterbox.py
+-rw-rw-rw-   0        0        0     1027 2023-04-01 06:54:25.000000 uplogic-1.9/uplogic/shaders/levels.py
+-rw-rw-rw-   0        0        0     4209 2023-04-01 06:54:25.000000 uplogic-1.9/uplogic/shaders/mist.py
+-rw-rw-rw-   0        0        0     5411 2023-04-01 07:02:38.000000 uplogic-1.9/uplogic/shaders/shader.py
+-rw-rw-rw-   0        0        0     2268 2023-04-01 06:54:25.000000 uplogic-1.9/uplogic/shaders/sharpen.py
+-rw-rw-rw-   0        0        0     5737 2023-04-01 06:54:25.000000 uplogic-1.9/uplogic/shaders/ssao.py
+-rw-rw-rw-   0        0        0     1190 2023-04-01 06:54:25.000000 uplogic-1.9/uplogic/shaders/vignette.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:20:06.936536 uplogic-1.9/uplogic/ui/
+-rw-rw-rw-   0        0        0      365 2023-04-02 16:26:08.000000 uplogic-1.9/uplogic/ui/__init__.py
+-rw-rw-rw-   0        0        0      579 2023-04-02 14:03:20.000000 uplogic-1.9/uplogic/ui/behaviors.py
+-rw-rw-rw-   0        0        0     4937 2023-04-26 12:34:19.000000 uplogic-1.9/uplogic/ui/button.py
+-rw-rw-rw-   0        0        0     1239 2023-04-02 14:15:27.000000 uplogic-1.9/uplogic/ui/canvas.py
+-rw-rw-rw-   0        0        0     2438 2023-04-26 12:34:19.000000 uplogic-1.9/uplogic/ui/cursor.py
+-rw-rw-rw-   0        0        0     3222 2023-05-12 15:59:52.000000 uplogic-1.9/uplogic/ui/image.py
+-rw-rw-rw-   0        0        0     5620 2023-05-15 12:47:52.000000 uplogic-1.9/uplogic/ui/label.py
+-rw-rw-rw-   0        0        0     6030 2023-05-14 16:02:11.000000 uplogic-1.9/uplogic/ui/layout.py
+-rw-rw-rw-   0        0        0     8601 2023-05-14 16:03:51.000000 uplogic-1.9/uplogic/ui/widget.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:20:06.951570 uplogic-1.9/uplogic/utils/
+-rw-rw-rw-   0        0        0     6837 2023-05-14 08:44:45.000000 uplogic-1.9/uplogic/utils/__init__.py
+-rw-rw-rw-   0        0        0     1204 2023-05-14 08:28:15.000000 uplogic-1.9/uplogic/utils/constants.py
+-rw-rw-rw-   0        0        0      854 2022-09-08 15:54:10.000000 uplogic-1.9/uplogic/utils/errors.py
+-rw-rw-rw-   0        0        0     6307 2023-03-06 11:22:43.000000 uplogic-1.9/uplogic/utils/lights.py
+-rw-rw-rw-   0        0        0     6976 2023-05-14 08:37:25.000000 uplogic-1.9/uplogic/utils/math.py
+-rw-rw-rw-   0        0        0     4801 2022-08-22 17:00:51.000000 uplogic-1.9/uplogic/utils/nodetrees.py
+-rw-rw-rw-   0        0        0    11371 2023-05-14 08:33:12.000000 uplogic-1.9/uplogic/utils/objects.py
+-rw-rw-rw-   0        0        0     5971 2023-05-14 19:09:35.000000 uplogic-1.9/uplogic/utils/pooling.py
+-rw-rw-rw-   0        0        0    13346 2023-05-14 16:52:14.000000 uplogic-1.9/uplogic/utils/raycasting.py
+-rw-rw-rw-   0        0        0     5831 2022-10-05 11:16:36.000000 uplogic-1.9/uplogic/utils/scene.py
+-rw-rw-rw-   0        0        0     1633 2023-01-05 12:25:57.000000 uplogic-1.9/uplogic/utils/visuals.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:20:06.396413 uplogic-1.9/uplogic.egg-info/
+-rw-rw-rw-   0        0        0     1045 2023-05-16 11:20:06.000000 uplogic-1.9/uplogic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13494 2023-05-16 11:20:06.000000 uplogic-1.9/uplogic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 11:20:06.000000 uplogic-1.9/uplogic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-16 11:20:06.000000 uplogic-1.9/uplogic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-16 11:20:06.000000 uplogic-1.9/uplogic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-03-17 18:28:53.000000 uplogic-1.9/uplogic.egg-info/zip-safe
```

### Comparing `uplogic-1.8.4/PKG-INFO` & `uplogic-1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: uplogic
-Version: 1.8.4
+Version: 1.9
 Summary: Uplogic utility for UPBGE.
 Home-page: https://github.com/UPBGE/uplogic
 Author: Leopold Auersperg-Castell
 Author-email: lauersperg@gmx.at
 License: GPLv2
-Download-URL: https://github.com/UPBGE/uplogic/archive/refs/tags/v1.8.4.tar.gz
+Download-URL: https://github.com/UPBGE/uplogic/archive/refs/tags/v1.9.tar.gz
 Keywords: Blender UPBGE logic
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python
 License-File: LICENSE.md
```

### Comparing `uplogic-1.8.4/setup.py` & `uplogic-1.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def read_file(name):
     with open(os.path.join(os.path.dirname(__file__), name)) as f:
         return f.read()
 
 
-version = 'v1.8.4'
+version = 'v1.9'
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
-    download_url='https://github.com/UPBGE/uplogic/archive/refs/tags/v1.8.4.tar.gz',
+    download_url='https://github.com/UPBGE/uplogic/archive/refs/tags/v1.9.tar.gz',
     license='GPLv2',
     packages=[
         'uplogic',
         'uplogic.animation',
         'uplogic.audio',
         'uplogic.data',
         'uplogic.decorators',
@@ -43,14 +43,15 @@
         'uplogic.input',
         'uplogic.logging',
         'uplogic.nodes',
         'uplogic.nodes.actions',
         'uplogic.nodes.conditions',
         'uplogic.nodes.parameters',
         'uplogic.physics',
+        'uplogic.serialize',
         'uplogic.shaders',
         'uplogic.ui',
         'uplogic.utils'
     ],
     # ext_modules=cythonize([
     #     'uplogic\\nodes\\__init__.pyx',
     #     'uplogic\\utils\\visuals.pyx',
```

### Comparing `uplogic-1.8.4/uplogic/__init__.py` & `uplogic-1.9/uplogic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     get_mainloop().stop(
 """
 
 from collections import deque
 
 from .utils import load_user_module
 from .input import key_tap
+from .logging import enable
 import bge
 import bpy
 import signal
 import time
 
 
 class MainLoop:
```

### Comparing `uplogic-1.8.4/uplogic/animation/action.py` & `uplogic-1.9/uplogic/animation/action.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from bge.types import KX_GameObject as GameObject
 from random import randint
 from random import random
 from uplogic.animation import ULActionSystem
 from uplogic.animation.actionsystem import get_action_system
 from uplogic.events import schedule
 import bpy
-from uplogic.utils import clamp, debug
+from uplogic.utils.math import clamp
 
 
 PLAY_MODES = {
     'play': logic.KX_ACTION_MODE_PLAY,
     'pingpong': logic.KX_ACTION_MODE_PING_PONG,
     'loop': logic.KX_ACTION_MODE_LOOP
 }
@@ -29,15 +29,15 @@
 
 ACTION_STARTED = 'ACTION_STARTED'
 ACTION_FINISHED = 'ACTION_FINISHED'
 
 
 class ULAction():
     '''
-    [DEPRECATED]
+    [DEPRECATED] Use `uplogic.animation.action` instead.
 
     Wrapper class for animated actions that provides additional parameters
     and quick access properties.
 
     :param `game_object`: The `KX_GameObject` on which to play the action.
     :param `action_name`: The name of the action  of `bpy.data.actions`.
     :param `start_frame`: The first frame of the action.
@@ -71,15 +71,15 @@
         play_mode: str = 'play',
         speed: float = 1,
         intensity: float = 1,
         blend_mode: str = 'blend',
         keep: bool = False
     ):
         if self._deprecated:
-            debug('ULAction class will be renamed to "Action" in future releases!')
+            print('Warning: ULAction class will be renamed to "Action" in future releases!')
         self._fps_factor = bpy.context.scene.render.fps / 60
         self._locked = False
         self._speed = speed
         self._frozen_speed = speed
         self.finished = False
         '''Finish state of the animation.'''
         self.keep = keep
```

### Comparing `uplogic-1.8.4/uplogic/animation/actionsystem.py` & `uplogic-1.9/uplogic/animation/actionsystem.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/animation/sequence.py` & `uplogic-1.9/uplogic/animation/sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from bge import logic
 from uplogic.animation.action import PLAY_MODES
 import bpy
-from uplogic.utils import debug
 import time
 
 
 class ULSequence():
     '''[DEPRECATED] Use `uplogic.animation.Sequence` instead
 
     Play an image animation through a material node.
@@ -27,15 +26,15 @@
         node: str,
         start_frame: int,
         end_frame: int,
         fps: int = 60,
         mode: str = 'play'
     ) -> None:
         if self._deprecated:
-            debug('ULSequence class will be renamed to "ULSequence" in future releases!')
+            print('Warning: ULSequence class will be renamed to "ULSequence" in future releases!')
 
         self.material = material
         """The material this sequence is played on."""
         self.node = node
         """Name of the node the image animation is loaded on."""
         self.start_frame = start_frame
         """Starting frame of the animation."""
```

### Comparing `uplogic-1.8.4/uplogic/audio/__init__.py` & `uplogic-1.9/uplogic/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/audio/audiosystem.py` & `uplogic-1.9/uplogic/audio/audiosystem.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/audio/music.py` & `uplogic-1.9/uplogic/audio/music.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from uplogic.audio.audiosystem import get_audio_system
 from .sound import Sound2D
 from uuid import uuid4
-from uplogic.utils import debug, interpolate
+from uplogic.utils.math import interpolate
 from uplogic.events import schedule_callback
 
 
 class ULMusicEffect():
     '''Base class for sounds played as music.'''
     def __init__(
         self
@@ -56,15 +56,15 @@
 
     def __init__(
         self,
         name: str = '',
         audio_system: str = 'music'
     ):
         if self._deprecated:
-            debug('ULMusic class will be renamed to "Music" in future releases!')
+            print('Warning: ULMusic class will be renamed to "Music" in future releases!')
         super().__init__()
         self.name = name if name else uuid4()
         self.audio_system = get_audio_system(audio_system, '2D')
         self.tracks: list[ULMusicTrack] = []
 
     @property
     def position(self):
@@ -131,15 +131,15 @@
         
         :param `track`: Index or name of the track to be removed.'''
         if isinstance(track, str):
             for t in self.tracks:
                 if t.name == track:
                     t.remove()
                     return
-            debug(f'Track "{track}" not found!')
+            print(f'Track "{track}" not found!')
         else:
             self.tracks[track].remove()
 
     def get_track(self, name):
         '''Get track by name.
         
         :param `name`: Name of the track.'''
@@ -181,15 +181,15 @@
     def __init__(
         self,
         music: Music,
         sound: str or Sound2D,
         name: str
     ):
         if self._deprecated:
-            debug('ULMusic class will be renamed to "Music" in future releases!')
+            print('Warning: ULMusic class will be renamed to "Music" in future releases!')
         super().__init__()
         self.music = music
         self.name = name
         sound = Sound2D(
             sound,
             aud_sys=self.music.audio_system
         ) if isinstance(sound, str) else sound
```

### Comparing `uplogic-1.8.4/uplogic/audio/sound.py` & `uplogic-1.9/uplogic/audio/sound.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os.path import isfile
 from bge import logic
 from bge.types import KX_GameObject as GameObject
 from mathutils import Vector
 from uplogic.audio import ULAudioSystem
 from uplogic.audio import get_audio_system
 from uplogic.events import schedule_callback
-from uplogic.utils import debug, interpolate
+from uplogic.utils.math import interpolate
 import aud
 
 
 class ULReverb():
     """Reverb sound added by `Sound3D` on demand.
     """
 
@@ -141,15 +141,17 @@
         self.sound.resume()
     
     def on_finish(self):
         pass
 
 
 class ULSound2D(ULSound):
-    '''Non-spacial sound, e.g. Music or Voice-Overs.\n
+    '''[DEPRECATED] Use `uplogic.audio.Sound2D` instead
+    
+    Non-spacial sound, e.g. Music or Voice-Overs.\n
     This class allows for modification of pitch and volume while playing.
 
     :param `file`: Path to the sound file.
     :param `volume`: Initial volume.
     :param `pitch`: Initial pitch.
     :param `loop_count`: Plays the sound this many times (0 for once, -1 for endless).
     :param `aud_sys`: Audiosystem to play this sound on.
@@ -164,25 +166,25 @@
         pitch: float = 1,
         loop_count: int = 0,
         lowpass = False,
         ignore_timescale = True,
         aud_sys: str = 'default'
     ):
         if self._deprecated:
-            debug('ULSound2D class will be renamed to "Sound2D" in future releases!')
+            print('Warning: ULSound2D class will be renamed to "Sound2D" in future releases!')
         self.file = file
         self._volume = 1
         self.finished = False
         if not (file):
             return
         self.aud_system = get_audio_system(aud_sys)
         soundfile = logic.expandPath(file)
         self.ignore_timescale = ignore_timescale
         if not isfile(soundfile):
-            debug(f'Soundfile {soundfile} could not be loaded!')
+            print(f'Soundfile {soundfile} could not be loaded!')
             return
         sound = self.soundfile = aud.Sound(soundfile)
         lowpass = self.aud_system.lowpass or lowpass
         if lowpass:
             sound = self.soundfile = sound.lowpass(lowpass, .5)
         device = self.aud_system.device
         self.sound = handle = device.play(sound)
@@ -248,15 +250,17 @@
             self.finished = True
             self.on_finish()
             self.aud_system.remove(self)
             return
 
 
 class Sound2D(ULSound2D):
-    '''Non-spacial sound, e.g. Music or Voice-Overs.\n
+    '''[DEPRECATED] Use `uplogic.audio.MusicTrack` instead
+    
+    Non-spacial sound, e.g. Music or Voice-Overs.\n
     This class allows for modification of pitch and volume while playing.
 
     :param `file`: Path to the sound file.
     :param `volume`: Initial volume.
     :param `pitch`: Initial pitch.
     :param `loop_count`: Plays the sound this many times (0 for once, -1 for endless).
     :param `aud_sys`: Audiosystem to play this sound on.
@@ -295,15 +299,15 @@
         self.finished = False
         if not (file):
             return
         self.aud_system = get_audio_system(aud_sys)
         soundfile = logic.expandPath(file)
         self.ignore_timescale = ignore_timescale
         if not isfile(soundfile):
-            debug(f'Soundfile {soundfile} could not be loaded!')
+            print(f'Soundfile {soundfile} could not be loaded!')
             return
         sound = self.soundfile = aud.Sound(soundfile)
         if sample[1]:
             sound = sound.limit(sample[0], sample[1])
         lowpass = self.aud_system.lowpass or lowpass
         if lowpass:
             sound = self.soundfile = sound.lowpass(lowpass, .5)
@@ -352,15 +356,15 @@
         distance_ref: float = 1,
         cone_angle: list[float] = [360, 360],
         cone_outer_volume: float = 0,
         ignore_timescale: bool = False,
         aud_sys: str = 'default'
     ):
         if self._deprecated:
-            debug('ULSound3D class will be renamed to "Sound3D" in future releases!')
+            print('Warning: ULSound3D class will be renamed to "Sound3D" in future releases!')
         self._is_vector = isinstance(speaker, Vector)
         self.file = file
         self.finished = False
         if not (file and speaker):
             return
         self._clear_sound = 0 if occlusion else 1
         self._sustained = 1
@@ -375,15 +379,15 @@
         self.pitch = pitch
         self.cone_outer_volume = cone_outer_volume
         master_volume = self.aud_system.volume
         self.transition = transition_speed
         self.ignore_timescale = ignore_timescale
         soundfile = logic.expandPath(file)
         if not isfile(soundfile):
-            debug(f'Soundfile {soundfile} could not be loaded!')
+            print(f'Soundfile {soundfile} could not be loaded!')
             return
         sound = self.soundpath = aud.Sound(soundfile).rechannel(1)
         device = self.aud_system.device
         handle = device.play(sound)
         handle.volume = 0
         if occlusion:
             soundlow = aud.Sound.lowpass(sound, 4400 * cutoff_frequency, .5).rechannel(1)
@@ -579,15 +583,15 @@
         self.pitch = pitch
         self.cone_outer_volume = cone_outer_volume
         master_volume = self.aud_system.volume
         self.transition = transition_speed
         self.ignore_timescale = ignore_timescale
         soundfile = logic.expandPath(file)
         if not isfile(soundfile):
-            debug(f'Soundfile {soundfile} could not be loaded!')
+            print(f'Soundfile {soundfile} could not be loaded!')
             return
         sound = self.soundpath = aud.Sound(soundfile).rechannel(1)
         device = self.aud_system.device
         if sample[1]:
             sound = sound.limit(sample[0], sample[1])
         handle = device.play(sound)
         handle.volume = 0
@@ -637,15 +641,15 @@
         speaker: GameObject,
         loop_count: int = 0,
         lowpass=False,
         ignore_timescale: bool = False,
         aud_sys: str = 'default'
     ):
         if self._deprecated:
-            debug('ULSpeaker2D class will be renamed to "Speaker2D" in future releases!')
+            print('Warning: ULSpeaker2D class will be renamed to "Speaker2D" in future releases!')
         speaker_data = speaker.blenderObject.data
         ULSound2D()
         super().__init__(
             speaker_data.sound.filepath,
             speaker_data.volume,
             speaker_data.pitch,
             loop_count,
@@ -671,15 +675,15 @@
         cutoff_frequency: float = 0.1,
         loop_count: int = 0,
         reverb=False,
         ignore_timescale: bool = False,
         aud_sys: str = 'default'
     ):
         if self._deprecated:
-            debug('ULSpeaker3D class will be renamed to "Speaker3D" in future releases!')
+            print('Warning: ULSpeaker3D class will be renamed to "Speaker3D" in future releases!')
         speaker_data = speaker.blenderObject.data
         super().__init__(
             speaker,
             speaker_data.sound.filepath,
             occlusion,
             transition_speed,
             cutoff_frequency,
```

### Comparing `uplogic-1.8.4/uplogic/data/__init__.py` & `uplogic-1.9/uplogic/data/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/data/file.py` & `uplogic-1.9/uplogic/data/file.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/data/globaldb.py` & `uplogic-1.9/uplogic/data/globaldb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 '''TODO: Documentation
 '''
 
 from bge import logic
 import bpy
 import os
-from uplogic.utils import debug
 from uplogic.utils import unload_nodes
 
 
 class GlobalDB(object):
     '''TODO: Documentation
     '''
     index: int
@@ -156,15 +155,15 @@
                 remove_f.append(f)
         for f in remove_f:
             bpy.app.handlers.game_post.remove(f)
         bpy.app.handlers.game_post.append(unload_nodes)
 
         log_size = GlobalDB.read(self.fname, self.content)
         if log_size > (5 * len(self.content)):
-            debug("Compressing sld {}".format(file_name))
+            print("Compressing sld {}".format(file_name))
             GlobalDB.compress(self.fname, self.content)
 
     def lock(self, item, event):
         self.locked[item] = event
 
     def unlock(self, item):
         self.locked.pop(item)
@@ -251,9 +250,9 @@
             db = GlobalDB.retrieve(c.name)
             msg += f' {c.name},'
             for v in c.content:
                 val = getattr(v, dat.get(v.value_type, 'FLOAT'), 0)
                 db.put(v.name, val, v.persistent)
 
         if msg:
-            debug(f'Globals Initialized:{msg[:-1]}')
+            print(f'Globals Initialized:{msg[:-1]}')
         GlobalDB.initialized = True
```

### Comparing `uplogic-1.8.4/uplogic/data/serializers.py` & `uplogic-1.9/uplogic/data/serializers.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/decorators/__init__.py` & `uplogic-1.9/uplogic/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/events/__init__.py` & `uplogic-1.9/uplogic/events/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/input/__init__.py` & `uplogic-1.9/uplogic/input/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/input/gamepad.py` & `uplogic-1.9/uplogic/input/gamepad.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from bge import logic
 from bge.types import KX_GameObject as GameObject
 from math import pi
 from mathutils import Vector
-from uplogic.utils import debug
-from uplogic.utils import interpolate
+from uplogic.utils.math import interpolate
 from uplogic.events import schedule_callback
 
 
 XBOX = {
     'A': 0,
     'B': 1,
     'X': 2,
@@ -239,15 +238,15 @@
 def gamepad_vibrate(idx: int = 0, strength: tuple = (.5, .5), time: float = 1.0):
     """Start the vibrators of the gamepad if available.
 
     :param `idx`: 
     """
     joystick = logic.joysticks[idx]
     if not joystick or not joystick.hasVibration:
-        debug(f'Joystick at index {idx} has no vibration!')
+        print(f'Joystick at index {idx} has no vibration!')
     joystick.strengthLeft = strength[0]
     joystick.strengthRight = strength[1]
     joystick.duration = int(round(time * 1000))
 
     joystick.startVibration()
 
 
@@ -265,19 +264,19 @@
 
     def __init__(
         self,
         idx: int = 0,
         layout: dict = XBOX
     ) -> None:
         if self._deprecated:
-            debug('ULGamePad class will be renamed to "Gamepad" in future releases!')
+            print('Warning: ULGamePad class will be renamed to "Gamepad" in future releases!')
         self.idx = idx
         self.layout = layout
         if not logic.joysticks[idx]:
-            debug(f'No Joystick found at index: {idx}')
+            print(f'No Joystick found at index: {idx}')
         self.joystick = logic.joysticks[idx]
 
     def button_down(self, button: str):
         return gamepad_down(button, self.idx, self.layout)
         
     def button_tap(self, button: str):
         return gamepad_tap(button, self.idx, self.layout)
@@ -286,15 +285,15 @@
         return gamepad_up(button, self.idx, self.layout)
 
     def sticks(self, stick: str = LS, threshold: float = 0.07):
         return gamepad_stick(stick, self.idx, threshold)
     
     def vibrate(self, strength: tuple = (.5, .5), time: float = 1.0):
         if not self.joystick.hasVibration:
-            debug('Joystick at index {} has no vibration!'.format(self.idx))
+            print('Joystick at index {} has no vibration!'.format(self.idx))
             return
         self.joystick.strengthLeft = strength[0]
         self.joystick.strengthRight = strength[1]
         self.joystick.duration = int(round(time * 1000))
 
         self.joystick.startVibration()
 
@@ -343,15 +342,15 @@
         idx: int = 0,
         stick: int = 'RS',
         threshold: float = 0.07,
         exponent: float = 2.3,
         active=True
     ) -> None:
         if self._deprecated:
-            debug('ULGamepadLook class will be renamed to "GamepadLook" in future releases!')
+            print('Warning: ULGamepadLook class will be renamed to "GamepadLook" in future releases!')
         self.obj = obj
         self.head = head if head else obj
         self._defaults = [
             obj.localOrientation.copy(),
             head.localOrientation.copy()
             if head else
             obj.localOrientation.copy()]
```

### Comparing `uplogic-1.8.4/uplogic/input/keyboard.py` & `uplogic-1.9/uplogic/input/keyboard.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/input/mouse.py` & `uplogic-1.9/uplogic/input/mouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from math import pi
 from bge import logic
 from bge import events
 from bge import render
 from bge.types import KX_GameObject as GameObject
 from mathutils import Vector
-from uplogic.utils import interpolate
+from uplogic.utils.math import interpolate
 from uplogic.events import schedule_callback
-from uplogic.utils import debug
 
 
 MOUSE_EVENTS = logic.mouse.inputs
 '''Reference to `bge.logic.mouse.inputs`
 '''
 
 LMB = events.LEFTMOUSE
@@ -154,15 +153,15 @@
 class ULMouse():
     """Mouse Wrapper for accessing mouse data."""
 
     _deprecated = True
 
     def __init__(self) -> None:
         if self._deprecated:
-            debug('ULMouse class will be renamed to "Mouse" in future releases!')
+            print('Warning: ULMouse class will be renamed to "Mouse" in future releases!')
         self._position = get_mouse_position()
         """Staggered updated mouse position for pos difference calculation."""
         self.movement = (0, 0)
         """Movement of the mouse as a tuple `(x, y)`."""
         self.active = True
 
     @property
@@ -288,15 +287,15 @@
         invert: tuple = (False, True),
         smoothing: float = 0.0,
         local: bool = True,
         front: int = 1,
         active: bool = True
     ) -> None:
         if self._deprecated:
-            debug('ULMouseLook class will be renamed to "MouseLook" in future releases!')
+            print('Warning: ULMouseLook class will be renamed to "MouseLook" in future releases!')
         self.obj = obj
         self.head = head if head else obj
         self._defaults = [
             obj.localOrientation.copy(),
             head.localOrientation.copy()
             if head else
             obj.localOrientation.copy()
```

### Comparing `uplogic-1.8.4/uplogic/input/vr.py` & `uplogic-1.9/uplogic/input/vr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import bpy
 from mathutils import Quaternion
 from mathutils import Matrix
 from mathutils import Vector
 from bge import logic
-from uplogic.utils import debug
 from bge.types import KX_GameObject as GameObject
 from uplogic.utils.errors import NoXRSessionError
 
 
 def get_vr_headset_data() -> tuple[Vector, Matrix]:
     """Get the current position and orientation of connected VR headset.
 
@@ -28,15 +27,15 @@
     :param `idx`: Controller index; 0 for left, 1 for right controller.
     """
 
     _deprecated = True
 
     def __init__(self, idx: int=0) -> None:
         if self._deprecated:
-            debug('ULControllerVR class will be renamed to "VRController" in future releases!')
+            print('Warning: ULControllerVR class will be renamed to "VRController" in future releases!')
         self.idx = idx
         self.stick_threshold = 0.0
         self.session = bpy.context.window_manager.xr_session_state
         if not self.session:
             raise NoXRSessionError
 
     @property
@@ -147,15 +146,15 @@
     attribute.
     """
 
     _deprecated = True
 
     def __init__(self) -> None:
         if self._deprecated:
-            debug('ULHeadsetVR class will be renamed to "VRHeadset" in future releases!')
+            print('Warning: ULHeadsetVR class will be renamed to "VRHeadset" in future releases!')
         self.session = bpy.context.window_manager.xr_session_state
         if not self.session:
             raise NoXRSessionError
 
     @property
     def position(self) -> Vector:
         return Vector(self.session.viewer_pose_location)
@@ -220,15 +219,15 @@
     _deprecated = True
     def __init__(
         self,
         left_hand_object: GameObject = None,
         right_hand_object: GameObject = None
     ) -> None:
         if self._deprecated:
-            debug('ULCharacterVR class will be renamed to "VRCharacter" in future releases!')
+            print('Warning: ULCharacterVR class will be renamed to "VRCharacter" in future releases!')
         self.session = bpy.context.window_manager.xr_session_state
         if not self.session:
             raise NoXRSessionError
         self.hand_left = ULControllerVR(0)
         self.hand_right = ULControllerVR(1)
         self.head = ULHeadsetVR()
         self.hand_left_object = left_hand_object
```

### Comparing `uplogic-1.8.4/uplogic/logging/__init__.py` & `uplogic-1.9/uplogic/nodes/actions/addfilter.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,126 +1,101 @@
-from bge import logic
-from bge import render
-from bgui.bgui_utils import Layout
-from bgui.bgui_utils import System
-from bgui.label import Label
-from io import StringIO
-from uplogic.data import GlobalDB
-from uplogic.utils import lerp
-from uplogic.events import schedule_callback
-import sys
-
-
-def set_depth(depth):
-    LoggerLayout.max_msg = depth
-
-
-def enable():
-    sys.stdout = Logger()
-    sys.stderr = ErrorLogger()
-
-
-def disable():
-    sys.stdout = sys.__stdout__
-    sys.stderr = sys.__stderr__
-
-
-class Logger(StringIO):
-
-    def write(self, __s: str) -> int:
-        log(__s)
-        sys.__stdout__.write(__s)
-
-
-class ErrorLogger(StringIO):
-    def write(self, __s: str) -> int:
-        error(__s)
-        sys.__stderr__.write(__s)
-
-
-class LoggerLayout(Layout):
-    colors = {
-        'INFO': [1, 1, 1, 1],
-        'WARNING': [1, 1, .3, 1],
-        'ERROR': [1, .3, .3, 1]
-    }
-    max_msg = 20
-    opacity = 1
-
-    def __init__(self, system, data):
-        super().__init__(system, data)
-        self.messages: list[Label] = []
-        self.fade_event = None
-        if disable not in logic.getCurrentScene().onRemove:
-            logic.getCurrentScene().onRemove.append(disable)
-
-    def fade_out(self):
-        for msg in self.messages:
-            msg.color[3] = lerp(msg.color[3], self.messages[0].color[3], .02)
-        if self.messages[-1].color[3] != .1:
-            self.fade_event = schedule_callback(self.fade_out)
-        else:
-            self.fade_event = None
-
-    def add_message(self, msg, type='INFO'):
-        if len(self.messages) > self.max_msg:
-            self._remove_widget(self.messages[0])
-            self.messages.pop(0)
-        if self._system:
-            self.messages.append(Label(
-                self,
-                text=str(msg),
-                pt_size=0,
-                color=self.colors.get(type, [1, 1, 1, 1]).copy(),
-                pos=[0.02, 0],
-                outline_color=(1, 0, 0, 1)
-            ))
-        for i, log in enumerate(reversed(self.messages)):
-            size = 11 * (1080 / render.getWindowHeight())
-            log.position[1] = 13 * (i+1)
-            log.color[3] = 1 - (i/(self.max_msg + 5))
-            log.pt_size = size
-        if self.fade_event:
-            self.fade_event.cancel()
-        self.fade_event = schedule_callback(self.fade_out, 3)
-
-
-def get_logger() -> LoggerLayout:
-    loggers = GlobalDB.retrieve('uplogic.loggers')
-    layout = loggers.get('default')
-    if layout is None:
-        system = System()
-        system.load_layout(LoggerLayout, None)
-        loggers.put('default', system.layout)
-        layout = system.layout
-        logic.getCurrentScene().post_draw.append(system.run)
-    return layout
-
-
-def log(msg):
-    logger = get_logger()
-    if logger is None:
-        return
-    for msg in str(msg).split('\n'):
-        if msg:
-            msg = msg.replace('  ', '    ')
-            logger.add_message(f'INFO:\t{msg}')
-
-
-def warning(msg):
-    logger = get_logger()
-    if logger is None:
-        return
-    for msg in str(msg).split('\n'):
-        if msg:
-            msg.replace('  ', '    ')
-            logger.add_message(f'WARNING:\t{msg}', 'WARNING')
-
-
-def error(msg):
-    logger = get_logger()
-    if logger is None:
-        return
-    for msg in str(msg).split('\n'):
-        if msg:
-            msg.replace('  ', '    ')
-            logger.add_message(f'ERROR:\t{msg}', 'ERROR')
+from uplogic.nodes import ULActionNode
+from uplogic.nodes import ULOutSocket
+from uplogic.utils import not_met
+from uplogic.shaders import FXAA
+from uplogic.shaders import HBAO
+from uplogic.shaders import SSAO
+from uplogic.shaders import Vignette
+from uplogic.shaders import Brightness
+from uplogic.shaders import ChromaticAberration
+from uplogic.shaders import Grayscale
+from uplogic.shaders import Levels
+from uplogic.shaders import Mist
+
+
+class ULAddFilter(ULActionNode):
+    def __init__(self):
+        ULActionNode.__init__(self)
+        self.condition = None
+        self.pass_idx = None
+        self.brightness = None
+        self.power = None
+        self.density = None
+        self.color = None
+        self.start = None
+        self.end = None
+        self.filter = None
+        self.filter_type = 'FXAA'
+        self.done = False
+        self.OUT = ULOutSocket(self, self._get_done)
+
+    def _get_done(self):
+        return self.done
+
+    def evaluate(self):
+        self.done = False
+        condition = self.get_input(self.condition)
+        ftype = self.filter_type
+        if not_met(condition) or self.filter:
+            if self.filter:
+                if ftype == 'VIGNETTE':
+                    self.filter.settings['power'] = self.get_input(self.power)
+                    self.filter.settings['color'] = self.get_input(self.color)
+                elif ftype == 'BRIGHTNESS':
+                    self.filter.settings['brightness'] = self.get_input(self.brightness)
+                elif ftype == 'CHROMAB':
+                    self.filter.settings['power'] = self.get_input(self.power)
+                elif ftype == 'GRAYSCALE':
+                    self.filter.settings['power'] = self.get_input(self.power)
+                elif ftype == 'LEVELS':
+                    self.filter.settings['color'] = self.get_input(self.color)
+                elif ftype == 'MIST':
+                    self.filter.settings['power'] = self.get_input(self.power)
+                    self.filter.settings['color'] = self.get_input(self.color)
+                    self.filter.settings['start'] = self.get_input(self.start)
+                    self.filter.settings['density'] = self.get_input(self.density)
+                elif ftype in ['HBAO', 'SSAO']:
+                    self.filter.settings['power'] = self.get_input(self.power)
+            return
+        self._set_ready()
+
+        if ftype == 'FXAA':
+            self.filter = FXAA(self.get_input(self.pass_idx))
+        elif ftype == 'HBAO':
+            self.filter = HBAO(self.get_input(self.power), self.get_input(self.pass_idx))
+        elif ftype == 'SSAO':
+            self.filter = SSAO(self.get_input(self.power), self.get_input(self.pass_idx))
+        elif ftype == 'VIGNETTE':
+            self.filter = Vignette(
+                self.get_input(self.power),
+                self.get_input(self.color),
+                self.get_input(self.pass_idx)
+            )
+        elif ftype == 'BRIGHTNESS':
+            self.filter = Brightness(
+                self.get_input(self.brightness),
+                self.get_input(self.pass_idx)
+            )
+        elif ftype == 'CHROMAB':
+            self.filter = ChromaticAberration(
+                self.get_input(self.power),
+                self.get_input(self.pass_idx)
+            )
+        elif ftype == 'GRAYSCALE':
+            self.filter = Grayscale(
+                self.get_input(self.power),
+                self.get_input(self.pass_idx)
+            )
+        elif ftype == 'LEVELS':
+            self.filter = Levels(
+                self.get_input(self.color),
+                self.get_input(self.pass_idx)
+            )
+        elif ftype == 'MIST':
+            self.filter = Mist(
+                self.get_input(self.start),
+                self.get_input(self.density),
+                self.get_input(self.color),
+                self.get_input(self.power),
+                self.get_input(self.pass_idx)
+            )
+        self.done = True
```

### Comparing `uplogic-1.8.4/uplogic/nodes/__init__.py` & `uplogic-1.9/uplogic/nodes/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from bge import logic
-from uplogic.utils import STATUS_READY
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_READY
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import check_game_object
 import Cython
 
 
 def alpha_move(a, b, fac):
     if a < b:
         return a + fac
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/__init__.py` & `uplogic-1.9/uplogic/nodes/actions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,7 +145,11 @@
 from .createuicanvas import ULCreateUICanvas
 from .createuilayout import ULCreateUILayout
 from .adduiwidget import ULAddUIWidget
 from .createuibutton import ULCreateUIButton
 from .setuiwidgetattr import ULSetUIWidgetAttr
 from .createuilabel import ULCreateUILabel
 from .createuiimage import ULCreateUIImage
+from .spawnpool import ULSpawnPool
+from .localserver import ULLocalServer
+from .localclient import ULLocalClient
+from .sendnetworkmessage import ULSendNetworkMessage
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/addobject.py` & `uplogic-1.9/uplogic/nodes/actions/addobject.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/addphysicsconstraint.py` & `uplogic-1.9/uplogic/nodes/actions/addphysicsconstraint.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/adduiwidget.py` & `uplogic-1.9/uplogic/nodes/actions/adduiwidget.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/alignaxistovector.py` & `uplogic-1.9/uplogic/nodes/actions/alignaxistovector.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/appendlistitem.py` & `uplogic-1.9/uplogic/nodes/actions/appendlistitem.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/applyforce.py` & `uplogic-1.9/uplogic/nodes/actions/applyforce.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/applyimpulse.py` & `uplogic-1.9/uplogic/nodes/actions/applyimpulse.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/applymovement.py` & `uplogic-1.9/uplogic/nodes/actions/applymovement.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/applyrotation.py` & `uplogic-1.9/uplogic/nodes/actions/applyrotation.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/applytorque.py` & `uplogic-1.9/uplogic/nodes/actions/applytorque.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/cameraraycast.py` & `uplogic-1.9/uplogic/nodes/actions/cameraraycast.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/characterjump.py` & `uplogic-1.9/uplogic/nodes/actions/characterjump.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/clampedmodifyproperty.py` & `uplogic-1.9/uplogic/nodes/actions/clampedmodifyproperty.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/clearvariables.py` & `uplogic-1.9/uplogic/nodes/actions/clearvariables.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from uplogic.nodes import ULActionNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import debug
 from uplogic.utils import not_met
 import bpy
 import json
 import os
 
 
 class ULClearVariables(ULActionNode):
@@ -24,15 +23,15 @@
         if not path.endswith('.json'):
             path = path + f'{self.get_input(self.file_name)}.json'
         if os.path.isfile(path):
             data = {}
             f = open(path, 'w')
             json.dump(data, f, indent=2)
         else:
-            debug('File does not exist - creating...')
+            print('File does not exist - creating...')
             f = open(path, 'w')
             data = {}
             json.dump(data, f, indent=2)
         f.close()
 
     def get_custom_path(self, path):
         if not path.endswith('/') and not path.endswith('json'):
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/copyproperty.py` & `uplogic-1.9/uplogic/nodes/actions/copyproperty.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/createuibutton.py` & `uplogic-1.9/uplogic/nodes/actions/createuibutton.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/createuicanvas.py` & `uplogic-1.9/uplogic/nodes/actions/createuicanvas.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/createuiimage.py` & `uplogic-1.9/uplogic/nodes/actions/createuiimage.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/createuilabel.py` & `uplogic-1.9/uplogic/nodes/actions/createuilabel.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/createuilayout.py` & `uplogic-1.9/uplogic/nodes/actions/createuilayout.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/createvehicle.py` & `uplogic-1.9/uplogic/nodes/actions/createvehicle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from uplogic.nodes import ULActionNode
 from uplogic.nodes import ULOutSocket
 from uplogic.physics.vehicle import ULVehicle
-from uplogic.utils import VEHICLE
+from uplogic.utils.constants import VEHICLE
 from uplogic.utils import is_waiting
 from uplogic.utils import not_met
 
 
 class ULCreateVehicle(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/cursorbehavior.py` & `uplogic-1.9/uplogic/nodes/actions/cursorbehavior.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/cursorvisibility.py` & `uplogic-1.9/uplogic/nodes/actions/cursorvisibility.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/dispatchevent.py` & `uplogic-1.9/uplogic/nodes/actions/dispatchevent.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from uplogic.events import send
 from uplogic.nodes import ULActionNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_INVALID
+from uplogic.utils.constants import STATUS_INVALID
 from uplogic.utils import is_invalid
 from uplogic.utils import is_waiting
 from uplogic.utils import not_met
 
 
 class ULDispatchEvent(ULActionNode):
     def __init__(self):
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/drawbox.py` & `uplogic-1.9/uplogic/nodes/actions/drawbox.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from mathutils import Vector
 from uplogic.nodes import ULActionNode
 from uplogic.utils import is_invalid
 from uplogic.utils import not_met
-from uplogic.utils import draw_box
+from uplogic.utils.visuals import draw_box
 
 
 class ULDrawBox(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.color = None
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/drawcube.py` & `uplogic-1.9/uplogic/nodes/actions/printvalue.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,28 @@
-from mathutils import Vector
 from uplogic.nodes import ULActionNode
-from uplogic.utils import is_invalid
+from uplogic.nodes import ULOutSocket
 from uplogic.utils import not_met
-from uplogic.utils import draw_cube
+from uplogic.logging import log
 
 
-class ULDrawCube(ULActionNode):
+class ULPrintValue(ULActionNode):
+
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.color = None
-        self.origin = None
-        self.width = None
-        self.use_volume_origin = False
+        self.value = None
+        self.done = None
+        self.msg_type = 'INFO'
+        self.OUT = ULOutSocket(self, self.get_done)
+
+    def get_done(self):
+        return self.done
 
     def evaluate(self):
+        self.done = False
         condition = self.get_input(self.condition)
         if not_met(condition):
             return
-        origin = self.get_input(self.origin)
-        width = self.get_input(self.width)
-        color = self.get_input(self.color)
-        if is_invalid(origin, width, color):
-            return
-        origin = origin.copy()
+        value = self.get_input(self.value)
         self._set_ready()
-        if self.use_volume_origin:
-            offset = width * 0.5
-            origin -= Vector((offset, offset, offset))
-        draw_cube(origin, width, color)
-        self._set_value(True)
+        log(value, self.msg_type)
+        self.done = True
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/drawline.py` & `uplogic-1.9/uplogic/nodes/actions/drawline.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/editbone.py` & `uplogic-1.9/uplogic/nodes/actions/editbone.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/endgame.py` & `uplogic-1.9/uplogic/nodes/actions/endgame.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/endobject.py` & `uplogic-1.9/uplogic/nodes/actions/endobject.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/executesubnetwork.py` & `uplogic-1.9/uplogic/nodes/actions/executesubnetwork.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/followpath.py` & `uplogic-1.9/uplogic/nodes/actions/followpath.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from mathutils import Vector
 from uplogic.nodes import ULActionNode
 from uplogic.nodes import ULOutSocket
 from uplogic.utils import is_invalid
 from uplogic.utils import not_met
-from uplogic.utils import rot_to
-from uplogic.utils import move_to
+from uplogic.utils.objects import rot_to
+from uplogic.utils.objects import move_to
 
 
 class ULFollowPath(ULActionNode):
     class MotionPath(object):
         def __init__(self):
             self.points = []
             self.cursor = 0
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/gamepadlook.py` & `uplogic-1.9/uplogic/nodes/actions/gamepadlook.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from bge import logic
 from bge.types import KX_GameObject as GameObject
 from mathutils import Vector
 from uplogic.nodes import ULActionNode
 from uplogic.nodes import ULOutSocket
 from uplogic.utils import is_invalid
-from uplogic.utils import debug
 from uplogic.utils import not_met
 
 
 class ULGamepadLook(ULActionNode):
     def __init__(self, axis=0):
         ULActionNode.__init__(self)
         self.axis: int = axis
@@ -37,15 +36,14 @@
         if not_met(condition):
             return
         main_obj: GameObject = self.get_input(self.main_obj)
         head_obj: GameObject = self.get_input(self.head_obj)
         if is_invalid(head_obj):
             head_obj = main_obj
         if is_invalid(axis):
-            debug('Gamepad Sticks Node: Invalid Controller Stick!')
             return
         inverted: bool = self.get_input(self.inverted)
         index: int = self.get_input(self.index)
         sensitivity: float = self.get_input(self.sensitivity)
         exponent: float = self.get_input(self.exponent)
         threshold: float = self.get_input(self.threshold)
         use_cap_x: Vector = self.get_input(self.use_cap_x)
@@ -57,15 +55,14 @@
         uppercapY: float = cap_y.x
         lowercapY: float = -cap_y.y
 
         self._set_ready()
         if logic.joysticks[index]:
             joystick = logic.joysticks[index]
         else:
-            debug('Gamepad Sticks Node: No Joystick at that Index!')
             return
         if is_invalid(joystick):
             return
         raw_values = joystick.axisValues
         if axis == 0:
             x, y = raw_values[0], raw_values[1]
         elif axis == 1:
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/gamepadvibration.py` & `uplogic-1.9/uplogic/nodes/actions/gamepadvibration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from bge import logic
 from uplogic.nodes import ULActionNode
 from uplogic.nodes import ULOutSocket
 from uplogic.utils import not_met
 from uplogic.utils import is_waiting
-from uplogic.utils import debug
 
 
 class ULGamepadVibration(ULActionNode):
     def __init__(self, axis=0):
         ULActionNode.__init__(self)
         self.condition = None
         self.index = None
@@ -32,15 +31,15 @@
         if is_waiting(index, left, right, time):
             return
 
         if not logic.joysticks[index]:
             return
         joystick = logic.joysticks[index]
         if not joystick.hasVibration:
-            debug('Joystick at index {} has no vibration!'.format(index))
+            print('Joystick at index {} has no vibration!'.format(index))
             return
 
         joystick.strengthLeft = left
         joystick.strengthRight = right
         joystick.duration = int(round(time * 1000))
 
         joystick.startVibration()
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/getperformanceprofile.py` & `uplogic-1.9/uplogic/nodes/actions/getperformanceprofile.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/installsubnetwork.py` & `uplogic-1.9/uplogic/nodes/actions/installsubnetwork.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/instream.py` & `uplogic-1.9/uplogic/nodes/actions/instream.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/listglobalvalues.py` & `uplogic-1.9/uplogic/nodes/actions/listglobalvalues.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/listvariables.py` & `uplogic-1.9/uplogic/nodes/actions/removevariable.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,65 @@
 from uplogic.nodes import ULActionNode
 from uplogic.nodes import ULOutSocket
 from uplogic.utils import debug
-from uplogic.utils import is_waiting
 from uplogic.utils import not_met
+from uplogic.utils import is_waiting
 import bpy
 import json
 import os
 
 
-class ULListVariables(ULActionNode):
+class ULRemoveVariable(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.print_list = None
+        self.name = None
         self.file_name = None
         self.path = ''
         self.done = None
-        self.items = None
         self.OUT = ULOutSocket(self, self.get_done)
-        self.LIST = ULOutSocket(self, self.get_list)
 
     def get_done(self):
         return self.done
 
-    def get_list(self):
-        return self.items
-
-    def write_to_json(self, path, p_l):
+    def write_to_json(self, path, name):
         data = None
         if not path.endswith('.json'):
             path = path + f'{self.get_input(self.file_name)}.json'
         if os.path.isfile(path):
             f = open(path, 'r')
             data = json.load(f)
-            if len(data) == 0:
-                debug('There are no saved variables')
-                return
-            li = []
-            for x in data:
-                if p_l:
-                    print('{}\t->\t{}'.format(x, data[x]))
-                li.append(x)
-            self.items = li
+            if name in data:
+                del data[name]
+            f.close()
+            f = open(path, 'w')
+            json.dump(data, f, indent=2)
+            f.close()
         else:
-            debug('There are no saved variables')
-        f.close()
+            debug('File does not exist!')
 
     def get_custom_path(self, path):
         if not path.endswith('/') and not path.endswith('json'):
             path = path + '/'
         return path
 
     def evaluate(self):
         self.done = False
         condition = self.get_input(self.condition)
         if not_met(condition):
             return
-        print_list = self.get_input(self.print_list)
-        if is_waiting(print_list):
+        name = self.get_input(self.name)
+        if is_waiting(name):
             return
         self._set_ready()
+
         cust_path = self.get_custom_path(self.path)
 
         path = (
             bpy.path.abspath('//Data/')
             if self.path == ''
             else bpy.path.abspath(cust_path)
         )
         os.makedirs(path, exist_ok=True)
 
-        self.write_to_json(path, print_list)
+        self.write_to_json(path, name)
         self.done = True
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/loadblendfile.py` & `uplogic-1.9/uplogic/nodes/actions/loadblendfile.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/loadfilecontent.py` & `uplogic-1.9/uplogic/nodes/actions/loadfilecontent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from bge import logic
 from uplogic.nodes import ULActionNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import FileLoader
+from uplogic.utils.scene import FileLoader
 
 
 class ULLoadFileContent(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.done = False
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/loadgame.py` & `uplogic-1.9/uplogic/nodes/actions/loadgame.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from bge import logic, constraints
 from mathutils import Euler
 from uplogic.nodes import ULActionNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import debug
 from uplogic.utils import is_waiting
 from uplogic.utils import not_met
 import bpy
 import json
 
 
 class ULLoadGame(ULActionNode):
@@ -56,15 +55,15 @@
                 for obj in data['objects']:
                     # print(obj)
                     if obj['name'] in scene.objects:
                         game_obj = scene.objects[obj['name']]
                     else:
                         game_obj = scene.convertBlenderObject(bpy.data.objects[obj['name']])
                         # game_obj = scene.addObject(game_obj)
-                        # debug(
+                        # print(
                         #     'Could not load Object {}: Not in active Scene!'
                         #     .format(obj['name'])
                         # )
                         # continue
 
                     lPos = self.get_game_vec(obj['data']['localPosition'])
                     lOri = self.get_game_vec(obj['data']['localOrientation'])
@@ -103,12 +102,12 @@
                             .getCharacter(game_obj)
                             .walkDirection
                         ) = wDir
 
                     for prop in obj['data']['props']:
                         game_obj[prop['name']] = prop['value']
         except Exception as e:
-            debug(
+            print(
                 f'Load Game Node: Could not load saved game on slot {slot}!\n{e}'
             )
 
         self.done = True
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/loadscene.py` & `uplogic-1.9/uplogic/nodes/actions/loadscene.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from bge import logic
 from uplogic.nodes import ULActionNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import SceneLoader
+from uplogic.utils.scene import SceneLoader
 
 
 class ULLoadScene(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.scene = None
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/makeuniquelight.py` & `uplogic-1.9/uplogic/nodes/actions/makeuniquelight.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/modifyproperty.py` & `uplogic-1.9/uplogic/nodes/actions/modifyproperty.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/mouselook.py` & `uplogic-1.9/uplogic/nodes/actions/mouselook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from bge import render
 from bge import logic
 from mathutils import Vector
 from uplogic.nodes import ULActionNode
 from uplogic.nodes import ULOutSocket
 from uplogic.utils import is_invalid
 from uplogic.utils import not_met
-from uplogic.utils import interpolate
+from uplogic.utils.math import interpolate
 import cython
 
 
 class ULMouseLook(ULActionNode):
     x = None
     y = None
     screen_center = None
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/mouseraycast.py` & `uplogic-1.9/uplogic/nodes/actions/mouseraycast.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/mousesetposition.py` & `uplogic-1.9/uplogic/nodes/actions/mousesetposition.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/moveto.py` & `uplogic-1.9/uplogic/nodes/actions/moveto.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from uplogic.nodes import ULActionNode
 from uplogic.utils import is_waiting
 from uplogic.utils import not_met
-from uplogic.utils import move_to
+from uplogic.utils.objects import move_to
 
 
 # Action "Move To": an object will follow a point
 class ULMoveTo(ULActionNode):
 
     def __init__(self):
         ULActionNode.__init__(self)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/movetowithnavmesh.py` & `uplogic-1.9/uplogic/nodes/actions/movetowithnavmesh.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from bge import render
 from bge.types import KX_GameObject as GameObject
 from uplogic.nodes import ULActionNode, ULOutSocket
 from uplogic.utils import is_invalid
 from uplogic.utils import not_met
-from uplogic.utils import rot_to
-from uplogic.utils import move_to
+from uplogic.utils.objects import rot_to
+from uplogic.utils.objects import move_to
 
 
 class ULMoveToWithNavmesh(ULActionNode):
 
     class MotionPath(object):
         def __init__(self):
             self.points: list = []
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/pausesound.py` & `uplogic-1.9/uplogic/nodes/actions/pausesound.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/playaction.py` & `uplogic-1.9/uplogic/nodes/actions/playaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from uplogic.data import GlobalDB
 from uplogic.animation import Action
 from uplogic.animation import ACTION_STARTED
 from uplogic.animation import ACTION_FINISHED
 from uplogic.events import receive
 from uplogic.nodes import ULActionNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_INVALID, STATUS_WAITING
+from uplogic.utils.constants import STATUS_INVALID, STATUS_WAITING
 from uplogic.utils import is_invalid
 from uplogic.utils import is_waiting
 from uplogic.utils import not_met
-from uplogic.utils import clamp
+from uplogic.utils.math import clamp
 
 
 class ULPlayAction(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.game_object = None
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/playsequence.py` & `uplogic-1.9/uplogic/nodes/actions/playsequence.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/popdictkey.py` & `uplogic-1.9/uplogic/nodes/actions/popdictkey.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/printvalue.py` & `uplogic-1.9/uplogic/nodes/actions/setresolution.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,31 @@
+from bge import render
 from uplogic.nodes import ULActionNode
 from uplogic.nodes import ULOutSocket
+from uplogic.utils import is_waiting
 from uplogic.utils import not_met
 
 
-class ULPrintValue(ULActionNode):
-
+class ULSetResolution(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.value = None
+        self.x_res = None
+        self.y_res = None
         self.done = None
         self.OUT = ULOutSocket(self, self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         condition = self.get_input(self.condition)
         if not_met(condition):
             return
-        value = self.get_input(self.value)
+        x_res = self.get_input(self.x_res)
+        y_res = self.get_input(self.y_res)
+        if is_waiting(x_res, y_res):
+            return
         self._set_ready()
-        print(value)
+        render.setWindowSize(x_res, y_res)
         self.done = True
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/projectileraycast.py` & `uplogic-1.9/uplogic/nodes/actions/projectileraycast.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from bge import logic
 from bge import render
 from mathutils import Vector
 from uplogic.nodes import ULActionNode
 from uplogic.nodes import ULOutSocket
 from uplogic.utils import is_waiting
 from uplogic.utils import not_met
-from uplogic.utils import raycast_projectile
+from uplogic.utils.raycasting import raycast_projectile
 
 
 class ULProjectileRayCast(ULActionNode):
 
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.origin = None
         self.destination = None
+        self.local: bool = None
         self.power: float = None
         self.resolution: float = None
         self.property_name: str = None
         self.xray: bool = None
         self.distance: float = None
         self.visualize: bool = None
         self._picked_object = None
@@ -77,14 +78,15 @@
 
         self._set_ready()
 
         obj, point, normal, points = raycast_projectile(
             caster=owner,
             origin=Vector(origin),
             aim=Vector(destination),
+            local=self.get_input(self.local),
             power=power,
             distance=distance,
             resolution=resolution,
             prop=property_name,
             xray=xray,
             visualize=visualize
         )
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/raycast.py` & `uplogic-1.9/uplogic/nodes/actions/raycast.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/removefilter.py` & `uplogic-1.9/uplogic/nodes/actions/removefilter.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/removelistindex.py` & `uplogic-1.9/uplogic/nodes/actions/removelistindex.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/removelistvalue.py` & `uplogic-1.9/uplogic/nodes/actions/removelistvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/removeoverlaycollection.py` & `uplogic-1.9/uplogic/nodes/actions/removeoverlaycollection.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/removeparent.py` & `uplogic-1.9/uplogic/nodes/actions/removeparent.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/removephysicsconstraint.py` & `uplogic-1.9/uplogic/nodes/actions/removephysicsconstraint.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/removevariable.py` & `uplogic-1.9/uplogic/nodes/actions/savevariable.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,65 +1,69 @@
 from uplogic.nodes import ULActionNode
 from uplogic.nodes import ULOutSocket
 from uplogic.utils import debug
-from uplogic.utils import not_met
 from uplogic.utils import is_waiting
+from uplogic.utils import not_met
 import bpy
 import json
 import os
 
 
-class ULRemoveVariable(ULActionNode):
+class ULSaveVariable(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.name = None
+        self.val = None
         self.file_name = None
         self.path = ''
         self.done = None
         self.OUT = ULOutSocket(self, self.get_done)
 
     def get_done(self):
         return self.done
 
-    def write_to_json(self, path, name):
+    def write_to_json(self, path, name, val):
         data = None
         if not path.endswith('.json'):
             path = path + f'{self.get_input(self.file_name)}.json'
         if os.path.isfile(path):
             f = open(path, 'r')
             data = json.load(f)
-            if name in data:
-                del data[name]
+            data[name] = val
             f.close()
             f = open(path, 'w')
             json.dump(data, f, indent=2)
-            f.close()
         else:
-            debug('File does not exist!')
+            debug('Variable file does not exist - creating...')
+            f = open(path, 'w')
+            data = {name: val}
+            json.dump(data, f, indent=2)
+        f.close()
 
     def get_custom_path(self, path):
         if not path.endswith('/') and not path.endswith('json'):
             path = path + '/'
         return path
 
     def evaluate(self):
         self.done = False
         condition = self.get_input(self.condition)
         if not_met(condition):
             return
         name = self.get_input(self.name)
-        if is_waiting(name):
+        val = self.get_input(self.val)
+        if is_waiting(name, val):
             return
         self._set_ready()
 
         cust_path = self.get_custom_path(self.path)
-
         path = (
             bpy.path.abspath('//Data/')
             if self.path == ''
             else bpy.path.abspath(cust_path)
         )
+
         os.makedirs(path, exist_ok=True)
 
-        self.write_to_json(path, name)
+        self.write_to_json(path, name, val)
         self.done = True
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/replacemesh.py` & `uplogic-1.9/uplogic/nodes/actions/replacemesh.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/restartgame.py` & `uplogic-1.9/uplogic/nodes/actions/restartgame.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/resumesound.py` & `uplogic-1.9/uplogic/nodes/actions/resumesound.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/rotateto.py` & `uplogic-1.9/uplogic/nodes/actions/rotateto.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from uplogic.nodes import ULActionNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING, is_invalid
+from uplogic.utils.constants import STATUS_WAITING
+from uplogic.utils.math import get_local
+from uplogic.utils import is_invalid
 from uplogic.utils import is_waiting
-from uplogic.utils import get_local
 from uplogic.utils import not_met
 
 
 class ULActionRotateTo(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/runactuator.py` & `uplogic-1.9/uplogic/nodes/actions/runactuator.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/runpython.py` & `uplogic-1.9/uplogic/nodes/actions/runpython.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULActionNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_INVALID
+from uplogic.utils.constants import STATUS_INVALID
 from uplogic.utils import is_waiting
 from uplogic.utils import not_met
 
 
 class ULRunPython(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/savegame.py` & `uplogic-1.9/uplogic/nodes/actions/savegame.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/savevariable.py` & `uplogic-1.9/uplogic/nodes/actions/savevariabledict.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,66 +4,57 @@
 from uplogic.utils import is_waiting
 from uplogic.utils import not_met
 import bpy
 import json
 import os
 
 
-class ULSaveVariable(ULActionNode):
+class ULSaveVariableDict(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.name = None
         self.val = None
         self.file_name = None
         self.path = ''
         self.done = None
         self.OUT = ULOutSocket(self, self.get_done)
 
     def get_done(self):
         return self.done
 
-    def write_to_json(self, path, name, val):
-        data = None
+    def write_to_json(self, path, val):
         if not path.endswith('.json'):
             path = path + f'{self.get_input(self.file_name)}.json'
         if os.path.isfile(path):
-            f = open(path, 'r')
-            data = json.load(f)
-            data[name] = val
-            f.close()
             f = open(path, 'w')
-            json.dump(data, f, indent=2)
+            json.dump(val, f, indent=2)
         else:
-            debug('Variable file does not exist - creating...')
+            debug('file does not exist - creating...')
             f = open(path, 'w')
-            data = {name: val}
-            json.dump(data, f, indent=2)
+            json.dump(val, f, indent=2)
         f.close()
 
     def get_custom_path(self, path):
         if not path.endswith('/') and not path.endswith('json'):
             path = path + '/'
         return path
 
     def evaluate(self):
         self.done = False
         condition = self.get_input(self.condition)
         if not_met(condition):
             return
-        name = self.get_input(self.name)
         val = self.get_input(self.val)
-        if is_waiting(name, val):
+        if is_waiting(val):
             return
         self._set_ready()
 
         cust_path = self.get_custom_path(self.path)
         path = (
             bpy.path.abspath('//Data/')
             if self.path == ''
             else bpy.path.abspath(cust_path)
         )
-
         os.makedirs(path, exist_ok=True)
 
-        self.write_to_json(path, name, val)
+        self.write_to_json(path, val)
         self.done = True
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/savevariabledict.py` & `uplogic-1.9/uplogic/nodes/parameters/loadvariable.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,62 @@
-from uplogic.nodes import ULActionNode
+from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import debug
 from uplogic.utils import is_waiting
-from uplogic.utils import not_met
 import bpy
 import json
 import os
 
 
-class ULSaveVariableDict(ULActionNode):
+class ULLoadVariable(ULParameterNode):
     def __init__(self):
-        ULActionNode.__init__(self)
-        self.condition = None
-        self.val = None
+        ULParameterNode.__init__(self)
+        self.name = None
+        self.default_value = None
         self.file_name = None
         self.path = ''
-        self.done = None
-        self.OUT = ULOutSocket(self, self.get_done)
+        self.VAR = ULOutSocket(self, self.get_var)
 
-    def get_done(self):
-        return self.done
+    def get_var(self):
+        socket = self.get_output('var')
+        if socket is None:
+            name = self.get_input(self.name)
+            if is_waiting(name):
+                return self.set_output('var', STATUS_WAITING)
+            cust_path = self.get_custom_path(self.path)
+
+            path = (
+                bpy.path.abspath('//Data/')
+                if self.path == ''
+                else bpy.path.abspath(cust_path)
+            )
+            os.makedirs(path, exist_ok=True)
+
+            return self.set_output(
+                'var',
+                self.read_from_json(path, name)
+            )
+        return socket
 
-    def write_to_json(self, path, val):
+    def read_from_json(self, path, name):
         if not path.endswith('.json'):
             path = path + f'{self.get_input(self.file_name)}.json'
-        if os.path.isfile(path):
-            f = open(path, 'w')
-            json.dump(val, f, indent=2)
+        if path:
+            f = open(path, 'r')
+            data = json.load(f)
+            if name not in data:
+                debug(f'"{name}" is not a saved Variabe!')
+                return self.get_input(self.default_value)
+            f.close()
+            return data.get(name)
         else:
-            debug('file does not exist - creating...')
-            f = open(path, 'w')
-            json.dump(val, f, indent=2)
-        f.close()
+            debug('No saved variables!')
+            return self.get_input(self.default_value)
 
     def get_custom_path(self, path):
         if not path.endswith('/') and not path.endswith('json'):
             path = path + '/'
         return path
 
     def evaluate(self):
-        self.done = False
-        condition = self.get_input(self.condition)
-        if not_met(condition):
-            return
-        val = self.get_input(self.val)
-        if is_waiting(val):
-            return
         self._set_ready()
-
-        cust_path = self.get_custom_path(self.path)
-        path = (
-            bpy.path.abspath('//Data/')
-            if self.path == ''
-            else bpy.path.abspath(cust_path)
-        )
-        os.makedirs(path, exist_ok=True)
-
-        self.write_to_json(path, val)
-        self.done = True
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/sendmessage.py` & `uplogic-1.9/uplogic/nodes/actions/sendmessage.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setactionframe.py` & `uplogic-1.9/uplogic/nodes/actions/setactionframe.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setactuatorvalue.py` & `uplogic-1.9/uplogic/nodes/actions/setactuatorvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setboneconstraintattr.py` & `uplogic-1.9/uplogic/nodes/actions/setboneconstraintattr.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setboneconstraintinfluence.py` & `uplogic-1.9/uplogic/nodes/actions/setboneconstraintinfluence.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setboneconstrainttarget.py` & `uplogic-1.9/uplogic/nodes/actions/setboneconstrainttarget.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setboneposition.py` & `uplogic-1.9/uplogic/nodes/actions/setboneposition.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setcamera.py` & `uplogic-1.9/uplogic/nodes/actions/setcamera.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setcamerafov.py` & `uplogic-1.9/uplogic/nodes/actions/setcamerafov.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setcameraorthoscale.py` & `uplogic-1.9/uplogic/nodes/actions/setcameraorthoscale.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setcharactergravity.py` & `uplogic-1.9/uplogic/nodes/actions/setcharactergravity.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setcharacterjumpspeed.py` & `uplogic-1.9/uplogic/nodes/actions/setcharacterjumpspeed.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setcharactermaxjumps.py` & `uplogic-1.9/uplogic/nodes/actions/setcharactermaxjumps.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setcharactervelocity.py` & `uplogic-1.9/uplogic/nodes/actions/setcharactervelocity.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setcharacterwalkdir.py` & `uplogic-1.9/uplogic/nodes/actions/setcharacterwalkdir.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setcollisiongroup.py` & `uplogic-1.9/uplogic/nodes/actions/setcollisiongroup.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setcollisionmask.py` & `uplogic-1.9/uplogic/nodes/actions/setcollisionmask.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setcurvepoints.py` & `uplogic-1.9/uplogic/nodes/actions/setcurvepoints.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setcustomcursor.py` & `uplogic-1.9/uplogic/nodes/actions/setcustomcursor.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setdictkey.py` & `uplogic-1.9/uplogic/nodes/actions/setdictkey.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setdynamics.py` & `uplogic-1.9/uplogic/nodes/actions/setdynamics.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/seteeveeao.py` & `uplogic-1.9/uplogic/nodes/actions/seteeveeao.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/seteeveebloom.py` & `uplogic-1.9/uplogic/nodes/actions/seteeveebloom.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/seteeveesmaa.py` & `uplogic-1.9/uplogic/nodes/actions/seteeveesmaa.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/seteeveesmaaquality.py` & `uplogic-1.9/uplogic/nodes/actions/seteeveesmaaquality.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/seteeveessr.py` & `uplogic-1.9/uplogic/nodes/actions/seteeveessr.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/seteeveevolumetrics.py` & `uplogic-1.9/uplogic/nodes/actions/seteeveevolumetrics.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setexposure.py` & `uplogic-1.9/uplogic/nodes/actions/setexposure.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setfilterstate.py` & `uplogic-1.9/uplogic/nodes/actions/setfilterstate.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setfullscreen.py` & `uplogic-1.9/uplogic/nodes/actions/setfullscreen.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setgameobjectattr.py` & `uplogic-1.9/uplogic/nodes/actions/setgameobjectattr.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setgamma.py` & `uplogic-1.9/uplogic/nodes/actions/setgamma.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setglobalvalue.py` & `uplogic-1.9/uplogic/nodes/actions/setglobalvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setgravity.py` & `uplogic-1.9/uplogic/nodes/actions/setgravity.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setlightcolor.py` & `uplogic-1.9/uplogic/nodes/actions/setlightcolor.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setlightenergy.py` & `uplogic-1.9/uplogic/nodes/actions/setlightenergy.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setlightshadow.py` & `uplogic-1.9/uplogic/nodes/actions/setlightshadow.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setlistindex.py` & `uplogic-1.9/uplogic/nodes/actions/setlistindex.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setmaterial.py` & `uplogic-1.9/uplogic/nodes/actions/setmaterial.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setmatnodesocket.py` & `uplogic-1.9/uplogic/nodes/actions/setmatnodesocket.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setmatnodevalue.py` & `uplogic-1.9/uplogic/nodes/actions/setmatnodevalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setnodesocket.py` & `uplogic-1.9/uplogic/nodes/actions/setnodesocket.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setnodevalue.py` & `uplogic-1.9/uplogic/nodes/actions/setnodevalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setoverlaycollection.py` & `uplogic-1.9/uplogic/nodes/actions/setoverlaycollection.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setparent.py` & `uplogic-1.9/uplogic/nodes/actions/setparent.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setphysics.py` & `uplogic-1.9/uplogic/nodes/actions/setphysics.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setprofile.py` & `uplogic-1.9/uplogic/nodes/actions/setprofile.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setproperty.py` & `uplogic-1.9/uplogic/nodes/actions/setproperty.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setpyinstanceattr.py` & `uplogic-1.9/uplogic/nodes/actions/setpyinstanceattr.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setresolution.py` & `uplogic-1.9/uplogic/nodes/actions/setvsync.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from bge import render
 from uplogic.nodes import ULActionNode
 from uplogic.nodes import ULOutSocket
 from uplogic.utils import is_waiting
 from uplogic.utils import not_met
 
 
-class ULSetResolution(ULActionNode):
+class ULSetVSync(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.x_res = None
-        self.y_res = None
+        self.vsync_mode = None
         self.done = None
         self.OUT = ULOutSocket(self, self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         condition = self.get_input(self.condition)
         if not_met(condition):
             return
-        x_res = self.get_input(self.x_res)
-        y_res = self.get_input(self.y_res)
-        if is_waiting(x_res, y_res):
+        vsync_mode = self.get_input(self.vsync_mode)
+        if is_waiting(vsync_mode):
             return
         self._set_ready()
-        render.setWindowSize(x_res, y_res)
+        render.setVsync(vsync_mode)
         self.done = True
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setrigidbody.py` & `uplogic-1.9/uplogic/nodes/actions/setrigidbody.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setscene.py` & `uplogic-1.9/uplogic/nodes/actions/setscene.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setsensorvalue.py` & `uplogic-1.9/uplogic/nodes/actions/setsensorvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/settimescale.py` & `uplogic-1.9/uplogic/nodes/actions/settimescale.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setuiwidgetattr.py` & `uplogic-1.9/uplogic/nodes/actions/setuiwidgetattr.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setvisibility.py` & `uplogic-1.9/uplogic/nodes/actions/setvisibility.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/setvsync.py` & `uplogic-1.9/uplogic/nodes/conditions/logicnot.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-from bge import render
-from uplogic.nodes import ULActionNode
+from uplogic.nodes import ULConditionNode
 from uplogic.nodes import ULOutSocket
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_waiting
-from uplogic.utils import not_met
 
 
-class ULSetVSync(ULActionNode):
+class ULNot(ULConditionNode):
     def __init__(self):
-        ULActionNode.__init__(self)
+        ULConditionNode.__init__(self)
         self.condition = None
-        self.vsync_mode = None
-        self.done = None
-        self.OUT = ULOutSocket(self, self.get_done)
+        self.OUT = ULOutSocket(self, self.get_out)
 
-    def get_done(self):
-        return self.done
+    def get_out(self):
+        socket = self.get_output('out')
+        if socket is None:
+            condition = self.get_input(self.condition)
+            if is_waiting(condition):
+                return STATUS_WAITING
+            return self.set_output(
+                'out',
+                not condition
+            )
+        return socket
 
     def evaluate(self):
-        self.done = False
-        condition = self.get_input(self.condition)
-        if not_met(condition):
-            return
-        vsync_mode = self.get_input(self.vsync_mode)
-        if is_waiting(vsync_mode):
-            return
         self._set_ready()
-        render.setVsync(vsync_mode)
-        self.done = True
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/showframerate.py` & `uplogic-1.9/uplogic/nodes/actions/showframerate.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/slowfollow.py` & `uplogic-1.9/uplogic/nodes/actions/slowfollow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from uplogic.nodes import ULActionNode
 from uplogic.nodes import ULOutSocket
 from uplogic.utils import is_waiting
 from uplogic.utils import not_met
 from uplogic.utils import debug
-from uplogic.utils import interpolate
+from uplogic.utils.math import interpolate
 
 
 class ULSlowFollow(ULActionNode):
     def __init__(self, value_type='worldPosition'):
         ULActionNode.__init__(self)
         self.value_type = str(value_type)
         self.condition = NotImplementedError
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/startsound.py` & `uplogic-1.9/uplogic/nodes/actions/startsound.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/startsound3d.py` & `uplogic-1.9/uplogic/nodes/actions/startsound3d.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/startspeaker.py` & `uplogic-1.9/uplogic/nodes/actions/startspeaker.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/startsubnetwork.py` & `uplogic-1.9/uplogic/nodes/actions/startsubnetwork.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/stopaction.py` & `uplogic-1.9/uplogic/nodes/actions/stopaction.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/stopallsounds.py` & `uplogic-1.9/uplogic/nodes/actions/stopallsounds.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/stopsound.py` & `uplogic-1.9/uplogic/nodes/actions/stopsound.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/stopsubnetwork.py` & `uplogic-1.9/uplogic/nodes/actions/stopsubnetwork.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/togglefilter.py` & `uplogic-1.9/uplogic/nodes/actions/togglefilter.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/toggleproperty.py` & `uplogic-1.9/uplogic/nodes/actions/toggleproperty.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/translate.py` & `uplogic-1.9/uplogic/nodes/actions/translate.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/vehicleapplybraking.py` & `uplogic-1.9/uplogic/nodes/actions/vehicleapplybraking.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from uplogic.nodes import ULActionNode
 from uplogic.nodes import ULOutSocket
 from uplogic.physics import RWD
-from uplogic.utils import VEHICLE
+from uplogic.utils.constants import VEHICLE
 from uplogic.utils import is_invalid
 from uplogic.utils import is_waiting
 from uplogic.utils import not_met
 
 
 class ULVehicleApplyBraking(ULActionNode):
     def __init__(self, value_type=RWD):
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/vehicleapplyforce.py` & `uplogic-1.9/uplogic/nodes/actions/vehicleapplyforce.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from uplogic.nodes import ULActionNode
 from uplogic.nodes import ULOutSocket
 from uplogic.physics import RWD
-from uplogic.utils import VEHICLE
+from uplogic.utils.constants import VEHICLE
 from uplogic.utils import is_waiting
 from uplogic.utils import is_invalid
 from uplogic.utils import not_met
 
 
 class ULVehicleApplyForce(ULActionNode):
     def __init__(self, value_type=RWD):
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/vehicleapplysteering.py` & `uplogic-1.9/uplogic/nodes/actions/vehicleapplysteering.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from uplogic.nodes import ULActionNode
 from uplogic.nodes import ULOutSocket
 from uplogic.physics import RWD
-from uplogic.utils import VEHICLE
+from uplogic.utils.constants import VEHICLE
 from uplogic.utils import is_waiting
 from uplogic.utils import is_invalid
 from uplogic.utils import not_met
 
 
 class ULVehicleApplySteering(ULActionNode):
     def __init__(self, value_type=RWD):
```

### Comparing `uplogic-1.8.4/uplogic/nodes/actions/vehiclesetattributes.py` & `uplogic-1.9/uplogic/nodes/actions/vehiclesetattributes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULActionNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import VEHICLE
+from uplogic.utils.constants import VEHICLE
 from uplogic.utils import is_waiting
 from uplogic.utils import is_invalid
 from uplogic.utils import not_met
 from uplogic.physics import FWD
 from uplogic.physics import RWD
 from uplogic.physics import FOURWD
```

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/__init__.py` & `uplogic-1.9/uplogic/nodes/conditions/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/barrier.py` & `uplogic-1.9/uplogic/nodes/conditions/barrier.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/checkdistance.py` & `uplogic-1.9/uplogic/nodes/conditions/checkdistance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from mathutils import Vector
 from uplogic.nodes import ULConditionNode
-from uplogic.utils import LOGIC_OPERATORS
+from uplogic.utils.constants import LOGIC_OPERATORS
 from uplogic.utils import is_invalid
 from uplogic.utils import is_waiting
 from uplogic.utils import compute_distance
 
 
 class ULCheckDistance(ULConditionNode):
     def __init__(self):
```

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/collision.py` & `uplogic-1.9/uplogic/nodes/conditions/collision.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/compare.py` & `uplogic-1.9/uplogic/nodes/conditions/compare.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from uplogic.nodes import ULConditionNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import LOGIC_OPERATORS
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import LOGIC_OPERATORS
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_waiting
 
 
 class ULCompare(ULConditionNode):
     def __init__(self, operator='GREATER'):
         ULConditionNode.__init__(self)
         self.operator = operator
```

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/comparevectors.py` & `uplogic-1.9/uplogic/nodes/conditions/comparevectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from mathutils import Vector
 from uplogic.nodes import ULConditionNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import LOGIC_OPERATORS
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import LOGIC_OPERATORS
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_waiting
 
 
 class ULCompareVectors(ULConditionNode):
     def __init__(self, operator='GREATER'):
         ULConditionNode.__init__(self)
         self.operator = operator
```

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/controllerstatus.py` & `uplogic-1.9/uplogic/nodes/conditions/controllerstatus.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/evaluateproperty.py` & `uplogic-1.9/uplogic/nodes/conditions/evaluateproperty.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULConditionNode
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 from uplogic.utils import is_waiting
 
 
 class ULEvaluateProperty(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/gamepadactive.py` & `uplogic-1.9/uplogic/nodes/conditions/gamepadactive.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/gamepadbutton.py` & `uplogic-1.9/uplogic/nodes/conditions/gamepadbutton.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from bge import logic
 from uplogic.nodes import ULConditionNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 
 
 class ULGamepadButton(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
         self.pulse = False
```

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/gamepadbuttonup.py` & `uplogic-1.9/uplogic/nodes/conditions/gamepadbuttonup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from bge import logic
 from uplogic.nodes import ULConditionNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 
 
 class ULGamepadButtonUp(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
         self.pulse = False
```

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/handleevent.py` & `uplogic-1.9/uplogic/nodes/conditions/handleevent.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from uplogic.events import receive
 from uplogic.events import ULEvent
 from uplogic.nodes import ULConditionNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 
 
 class ULHandleEvent(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
         self.subject = None
```

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/hasproperty.py` & `uplogic-1.9/uplogic/nodes/conditions/hasproperty.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULConditionNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 
 
 class ULHasProperty(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
         self.game_object = None
```

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/keypressed.py` & `uplogic-1.9/uplogic/nodes/conditions/keypressed.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/keyreleased.py` & `uplogic-1.9/uplogic/nodes/conditions/keyreleased.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/logicand.py` & `uplogic-1.9/uplogic/nodes/conditions/logicand.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/logicandnot.py` & `uplogic-1.9/uplogic/nodes/conditions/logicandnot.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/logicnot.py` & `uplogic-1.9/uplogic/nodes/conditions/truefalse.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 from uplogic.nodes import ULConditionNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
-from uplogic.utils import is_waiting
 
 
-class ULNot(ULConditionNode):
+class ULTrueFalse(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
-        self.condition = None
-        self.OUT = ULOutSocket(self, self.get_out)
+        self.state = None
+        self.TRUE = ULOutSocket(self, self.get_true_value)
+        self.FALSE = ULOutSocket(self, self.get_false_value)
 
-    def get_out(self):
-        socket = self.get_output('out')
-        if socket is None:
-            condition = self.get_input(self.condition)
-            if is_waiting(condition):
-                return STATUS_WAITING
-            return self.set_output(
-                'out',
-                not condition
-            )
-        return socket
+    def get_true_value(self):
+        return self.get_input(self.state)
+
+    def get_false_value(self):
+        return not self.get_input(self.state)
 
     def evaluate(self):
         self._set_ready()
```

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/logicor.py` & `uplogic-1.9/uplogic/nodes/conditions/logicor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from uplogic.nodes import ULConditionNode
-from uplogic.utils import STATUS_WAITING, is_waiting
+from uplogic.utils.constants import STATUS_WAITING
+from uplogic.utils import is_waiting
 
 
 class ULOr(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
         self.ca = False
         self.cb = False
```

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/logictreestatus.py` & `uplogic-1.9/uplogic/nodes/conditions/logictreestatus.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from uplogic.nodes import ULConditionNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING, is_invalid
+from uplogic.utils.constants import STATUS_WAITING
+from uplogic.utils import is_invalid
 from uplogic.utils import is_waiting
 
 
 class ULLogicTreeStatus(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
         self.game_object = None
```

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/mouseover.py` & `uplogic-1.9/uplogic/nodes/conditions/mouseover.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/mousepressed.py` & `uplogic-1.9/uplogic/nodes/conditions/mousepressed.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULConditionNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_waiting
 from uplogic.input import mouse_down
 from uplogic.input import mouse_tap
 from bge.logic import mouse
 
 
 class ULMousePressed(ULConditionNode):
```

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/mousepressedon.py` & `uplogic-1.9/uplogic/nodes/conditions/mousepressedon.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from bge import logic
 from uplogic.nodes import ULConditionNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 from uplogic.utils import is_waiting
 
 
 class ULMousePressedOn(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/mousereleased.py` & `uplogic-1.9/uplogic/nodes/conditions/mousereleased.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULConditionNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_waiting
 from bge import logic
 
 
 class ULMouseReleased(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/mousescroll.py` & `uplogic-1.9/uplogic/nodes/conditions/mousescroll.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/once.py` & `uplogic-1.9/uplogic/nodes/conditions/once.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/onnexttick.py` & `uplogic-1.9/uplogic/nodes/conditions/onnexttick.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/onvaluechanged.py` & `uplogic-1.9/uplogic/nodes/conditions/onvaluechanged.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/onvaluechangedto.py` & `uplogic-1.9/uplogic/nodes/conditions/onvaluechangedto.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULConditionNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_waiting
 
 
 class ULValueChangedTo(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
         self.monitored_value = None
```

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/pulsify.py` & `uplogic-1.9/uplogic/nodes/conditions/pulsify.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/sensorpositive.py` & `uplogic-1.9/uplogic/nodes/conditions/sensorpositive.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULConditionNode
-from uplogic.utils import STATUS_WAITING, is_invalid
+from uplogic.utils.constants import STATUS_WAITING
+from uplogic.utils import is_invalid
 from uplogic.utils import is_waiting
 
 
 class ULSensorPositive(ULConditionNode):
 
     def __init__(self):
         ULConditionNode.__init__(self)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/timedelay.py` & `uplogic-1.9/uplogic/nodes/conditions/timedelay.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/timer.py` & `uplogic-1.9/uplogic/nodes/conditions/timer.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/conditions/truefalse.py` & `uplogic-1.9/uplogic/nodes/parameters/getresolution.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,27 @@
-from uplogic.nodes import ULConditionNode
+from bge import render
+from mathutils import Vector
 from uplogic.nodes import ULOutSocket
+from uplogic.nodes import ULParameterNode
 
 
-class ULTrueFalse(ULConditionNode):
+class ULGetResolution(ULParameterNode):
     def __init__(self):
-        ULConditionNode.__init__(self)
-        self.state = None
-        self.TRUE = ULOutSocket(self, self.get_true_value)
-        self.FALSE = ULOutSocket(self, self.get_false_value)
+        ULParameterNode.__init__(self)
+        self.width = None
+        self.height = None
+        self.res = None
+        self.WIDTH = ULOutSocket(self, self.get_width)
+        self.HEIGHT = ULOutSocket(self, self.get_height)
+        self.RES = ULOutSocket(self, self.get_res)
 
-    def get_true_value(self):
-        return self.get_input(self.state)
+    def get_width(self):
+        return render.getWindowWidth()
 
-    def get_false_value(self):
-        return not self.get_input(self.state)
+    def get_height(self):
+        return render.getWindowHeight()
+
+    def get_res(self):
+        return Vector((self.width, self.height))
 
     def evaluate(self):
         self._set_ready()
```

### Comparing `uplogic-1.8.4/uplogic/nodes/logictree.py` & `uplogic-1.9/uplogic/nodes/logictree.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from bge import logic
 from bge.types import KX_GameObject as GameObject
 from uplogic.audio import ULAudioSystem
 from uplogic.data import GlobalDB
 from uplogic.nodes import STATUS_READY
 from uplogic.nodes import STATUS_WAITING
 from uplogic.nodes import ULLogicContainer
-from uplogic.utils import debug
 from uplogic.utils import load_user_module
 from uplogic.utils import make_valid_name
 import bpy
 # from uplogic import get_mainloop
 from bge.types import SCA_PythonKeyboard as Keyboard
 import collections
 import time
@@ -80,15 +79,15 @@
                 db = GlobalDB.retrieve(c.name)
                 msg += f' {c.name},'
                 for v in c.content:
                     val = getattr(v, dat.get(v.value_type, 'FLOAT'), 0)
                     db.put(v.name, val, v.persistent)
 
             if msg:
-                debug(f'Globals Initialized:{msg[:-1]}')
+                print(f'Globals Initialized:{msg[:-1]}')
             bpy.types.Scene.nl_globals_initialized = True
 
     def ray_cast(
         self,
         caster_object,
         ray_origin,
         ray_destination,
@@ -202,34 +201,34 @@
         cells = self._iter
         max_loop_count = len(cells)
         loop_index = 0
         done_cells = []
         max_blocking_loop_count = self._max_blocking_loop_count
         while cells:
             if loop_index == max_blocking_loop_count:
-                debug(
+                print(
                     "Network found a blocking condition" +
                     " (due to unconnected or non responsive cell)"
                 )
-                debug("Stopping network...")
+                print("Stopping network...")
                 self.stop()
                 return
             cell = cells.popleft()
             if cell in done_cells:
                 continue
             else:
                 done_cells.append(cell)
             cell.evaluate()
             self.evaluated_cells += 1
             if not cell.has_status(STATUS_READY):
                 cells.append(cell)
             loop_index += 1
         done_cells = []
         if(loop_index > max_loop_count):
-            debug(
+            print(
                 "Wrong sorting alghorithm!",
                 loop_index,
                 max_loop_count
             )
         for cell in self._cells:
             cell.reset()
             if cell.has_status(STATUS_WAITING):
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/__init__.py` & `uplogic-1.9/uplogic/nodes/parameters/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,7 +88,8 @@
 from .getlightcolor import ULGetLightColor  # noqa
 from .absolutevalue import ULAbsoluteValue  # noqa
 from .vrcontrollervalues import ULGetVRControllerValues  # noqa
 from .vrheadsetvalues import ULGetVRHeadsetValues  # noqa
 from .storevalue import ULStoreValue  #noqa
 from .getfont import ULGetFont
 from .getuiwidgetattr import ULGetUIWidgetAttr
+from .serializedata import ULSerializeData
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/absolutevalue.py` & `uplogic-1.9/uplogic/nodes/parameters/absolutevalue.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 import math
 
 
 class ULAbsoluteValue(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/actionstatus.py` & `uplogic-1.9/uplogic/nodes/parameters/actionstatus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from uplogic.animation import ULActionSystem
 from uplogic.data import GlobalDB
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 from uplogic.utils import is_waiting
 
 
 class ULActionStatus(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/activecamera.py` & `uplogic-1.9/uplogic/nodes/parameters/activecamera.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from bge import logic
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 
 
 class ULActiveCamera(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.OUT = ULOutSocket(self, self.get_camera)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/axisvector.py` & `uplogic-1.9/uplogic/nodes/parameters/axisvector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import LO_AXIS_TO_VECTOR
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import LO_AXIS_TO_VECTOR
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 
 
 class ULAxisVector(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.game_object = None
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/bonestatus.py` & `uplogic-1.9/uplogic/nodes/parameters/bonestatus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from bge import logic
 from mathutils import Euler
 from mathutils import Quaternion
 from mathutils import Vector
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import NO_VALUE
+from uplogic.utils.constants import NO_VALUE
 from uplogic.utils import is_invalid
 
 
 class ULBoneStatus(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.armature = None
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/characterinfo.py` & `uplogic-1.9/uplogic/nodes/parameters/characterinfo.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/childbyindex.py` & `uplogic-1.9/uplogic/nodes/parameters/childbyindex.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from bge.types import KX_GameObject as GameObject
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 from uplogic.utils import is_waiting
 
 
 class ULChildByIndex(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/childbyname.py` & `uplogic-1.9/uplogic/nodes/parameters/childbyname.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 
 
 class ULChildByName(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.from_parent = None
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/clamp.py` & `uplogic-1.9/uplogic/nodes/parameters/clamp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_waiting
 from uplogic.utils import is_invalid
 
 
 class ULClamp(ULParameterNode):
 
     def __init__(self):
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/colorrgb.py` & `uplogic-1.9/uplogic/nodes/parameters/colorrgb.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_waiting
 
 
 class ULColorRGB(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.color = None
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/colorrgba.py` & `uplogic-1.9/uplogic/nodes/parameters/colorrgba.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/dictvalue.py` & `uplogic-1.9/uplogic/nodes/parameters/dictvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/distance.py` & `uplogic-1.9/uplogic/nodes/parameters/distance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_waiting
 from uplogic.utils import compute_distance
 
 
 class ULDistance(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/euler.py` & `uplogic-1.9/uplogic/nodes/parameters/euler.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/eulertomatrix.py` & `uplogic-1.9/uplogic/nodes/parameters/eulertomatrix.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/formattedstring.py` & `uplogic-1.9/uplogic/nodes/parameters/formattedstring.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_waiting
 from uplogic.utils import is_invalid
 
 
 class ULFormattedString(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/formula.py` & `uplogic-1.9/uplogic/nodes/parameters/formula.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/gamepadsticks.py` & `uplogic-1.9/uplogic/nodes/parameters/gamepadsticks.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/gamepadtrigger.py` & `uplogic-1.9/uplogic/nodes/parameters/gamepadtrigger.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from bge import logic
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 
 
 class ULGamepadTrigger(ULParameterNode):
     def __init__(self, axis=0):
         ULParameterNode.__init__(self)
         self.axis = axis
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/getactuatorvalue.py` & `uplogic-1.9/uplogic/nodes/parameters/getactuatorvalue.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 
 
 class ULGetActuatorValue(ULParameterNode):
 
     def __init__(self):
         ULParameterNode.__init__(self)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/getcollection.py` & `uplogic-1.9/uplogic/nodes/parameters/getcollection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 
 
 class ULGetCollection(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.collection = None
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/getcollectionobjectnames.py` & `uplogic-1.9/uplogic/nodes/parameters/getcollectionobjectnames.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 import bpy
 
 
 class ULGetCollectionObjectNames(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/getcollectionobjects.py` & `uplogic-1.9/uplogic/nodes/parameters/getcollectionobjects.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 from uplogic.utils import check_game_object
 import bpy
 
 
 class ULGetCollectionObjects(ULParameterNode):
     def __init__(self):
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/getcurvepoints.py` & `uplogic-1.9/uplogic/nodes/parameters/getcurvepoints.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/getfont.py` & `uplogic-1.9/uplogic/nodes/parameters/getfont.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/getglobalvalue.py` & `uplogic-1.9/uplogic/nodes/parameters/getglobalvalue.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from uplogic.data import GlobalDB
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_INVALID
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_INVALID
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_waiting
 
 
 class ULGetGlobalValue(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.data_id = None
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/getimage.py` & `uplogic-1.9/uplogic/nodes/parameters/getimage.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/getlightcolor.py` & `uplogic-1.9/uplogic/nodes/parameters/getlightcolor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_waiting
 
 
 class ULGetLightColor(ULParameterNode):
 
     def __init__(self):
         ULParameterNode.__init__(self)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/getlightenergy.py` & `uplogic-1.9/uplogic/nodes/parameters/getlightenergy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_waiting
 
 
 class ULGetLightEnergy(ULParameterNode):
 
     def __init__(self):
         ULParameterNode.__init__(self)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/getnodeattribute.py` & `uplogic-1.9/uplogic/nodes/parameters/getnodeattribute.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 from uplogic.utils import is_waiting
 import bpy
 
 
 class ULGetNodeAttribute(ULParameterNode):
     def __init__(self):
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/getnodesocket.py` & `uplogic-1.9/uplogic/nodes/parameters/getnodesocket.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 from uplogic.utils import is_waiting
 import bpy
 
 
 class ULGetNodeSocket(ULParameterNode):
     def __init__(self):
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/getobject.py` & `uplogic-1.9/uplogic/nodes/parameters/getparent.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 
 
-class ULGetObject(ULParameterNode):
+class ULGetParent(ULParameterNode):
+
     def __init__(self):
         ULParameterNode.__init__(self)
         self.game_object = None
-        self.OUT = ULOutSocket(self, self.get_obj)
+        self.OUT = ULOutSocket(self, self.get_parent)
 
-    def get_obj(self):
+    def get_parent(self):
         game_object = self.get_input(self.game_object)
         if is_invalid(game_object):
             return STATUS_WAITING
-        return game_object
+        return game_object.parent
 
     def evaluate(self):
         self._set_ready()
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/getparent.py` & `uplogic-1.9/uplogic/nodes/parameters/listduplicate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 
 
-class ULGetParent(ULParameterNode):
-
+class ULListDuplicate(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
-        self.game_object = None
-        self.OUT = ULOutSocket(self, self.get_parent)
+        self.condition = None
+        self.items = None
+        self.OUT = ULOutSocket(self, self.get_points)
 
-    def get_parent(self):
-        game_object = self.get_input(self.game_object)
-        if is_invalid(game_object):
+    def get_points(self):
+        list_d = self.get_input(self.items)
+        if is_invalid(list_d):
             return STATUS_WAITING
-        return game_object.parent
+        return list_d.copy()
 
     def evaluate(self):
         self._set_ready()
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/getproperty.py` & `uplogic-1.9/uplogic/nodes/parameters/getproperty.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from uplogic.nodes import ULOutSocket, ULParameterNode
-from uplogic.utils import STATUS_WAITING, is_invalid
+from uplogic.utils.constants import STATUS_WAITING
+from uplogic.utils import is_invalid
 
 
 class ULGetProperty(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.game_object = None
         self.property_name = None
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/getpyinstanceattr.py` & `uplogic-1.9/uplogic/nodes/parameters/getpyinstanceattr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_INVALID, STATUS_WAITING
+from uplogic.utils.constants import STATUS_INVALID, STATUS_WAITING
 from uplogic.utils import is_waiting
 
 
 class ULGetPyInstanceAttr(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.instance = None
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/getresolution.py` & `uplogic-1.9/uplogic/nodes/parameters/initemptylist.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,23 @@
-from bge import render
-from mathutils import Vector
+
+
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
+from uplogic.utils import is_waiting
 
 
-class ULGetResolution(ULParameterNode):
+class ULInitEmptyList(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
-        self.width = None
-        self.height = None
-        self.res = None
-        self.WIDTH = ULOutSocket(self, self.get_width)
-        self.HEIGHT = ULOutSocket(self, self.get_height)
-        self.RES = ULOutSocket(self, self.get_res)
-
-    def get_width(self):
-        return render.getWindowWidth()
-
-    def get_height(self):
-        return render.getWindowHeight()
-
-    def get_res(self):
-        return Vector((self.width, self.height))
+        self.condition = None
+        self.length = None
+        self.items = None
+        self.LIST = ULOutSocket(self, self.get_list)
+
+    def get_list(self):
+        length = self.get_input(self.length)
+        if is_waiting(length):
+            return
+        return [None for x in range(length)]
 
     def evaluate(self):
         self._set_ready()
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/getsensorvalue.py` & `uplogic-1.9/uplogic/nodes/parameters/getsensorvalue.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 from bge.types import KX_GameObject as GameObject
 
 
 class ULGetSensorValue(ULParameterNode):
 
     def __init__(self):
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/getsound.py` & `uplogic-1.9/uplogic/nodes/parameters/objectdataname.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.nodes import ULParameterNode
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 
 
-class ULGetSound(ULParameterNode):
-
+class ULObjectDataName(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
-        self.sound = None
-        self.OUT = ULOutSocket(self, self.get_done)
+        self.game_object = None
+        self.OUT = ULOutSocket(self, self.get_name)
 
-    def get_done(self):
-        sound = self.get_input(self.sound)
-        if is_invalid(sound):
+    def get_name(self):
+        obj = self.get_input(self.game_object)
+        if is_invalid(obj):
             return STATUS_WAITING
-        return sound
+        return obj.blenderObject.name
 
     def evaluate(self):
         self._set_ready()
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/getuiwidgetattr.py` & `uplogic-1.9/uplogic/nodes/parameters/getuiwidgetattr.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/initemptylist.py` & `uplogic-1.9/uplogic/nodes/parameters/listfromitems.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-
-
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
+from uplogic.utils import is_invalid
 from uplogic.utils import is_waiting
 
 
-class ULInitEmptyList(ULParameterNode):
+class ULListFromItems(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
-        self.condition = None
-        self.length = None
         self.items = None
+        self.list: list = None
         self.LIST = ULOutSocket(self, self.get_list)
 
     def get_list(self):
-        length = self.get_input(self.length)
-        if is_waiting(length):
-            return
-        return [None for x in range(length)]
+        socket = self.get_output('list')
+        if socket is None:
+            self.list = self.get_input(self.items)
+            return self.set_output('list', [self.get_input(item) for item in self.list])
+        return socket
 
     def evaluate(self):
         self._set_ready()
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/initnewdict.py` & `uplogic-1.9/uplogic/nodes/parameters/initnewdict.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_waiting
 
 
 class ULInitNewDict(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.key = None
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/interpolate.py` & `uplogic-1.9/uplogic/nodes/parameters/interpolate.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import lerp
 from uplogic.utils import is_invalid
 
 
 class ULInterpolate(ULParameterNode):
 
     def __init__(self):
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/invertvalue.py` & `uplogic-1.9/uplogic/nodes/parameters/invertvalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/limitrange.py` & `uplogic-1.9/uplogic/nodes/parameters/limitrange.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from mathutils import Vector
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_waiting
 
 
 class ULLimitRange(ULParameterNode):
 
     def __init__(self):
         ULParameterNode.__init__(self)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/listduplicate.py` & `uplogic-1.9/uplogic/nodes/parameters/materialgetnode.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,27 @@
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_WAITING
+from uplogic.nodes import ULOutSocket
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
+import bpy
 
 
-class ULListDuplicate(ULParameterNode):
+class ULGetMaterialNode(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
-        self.condition = None
-        self.items = None
-        self.OUT = ULOutSocket(self, self.get_points)
+        self.mat_name = None
+        self.node_name = None
+        self.OUT = ULOutSocket(self, self._get_val)
 
-    def get_points(self):
-        list_d = self.get_input(self.items)
-        if is_invalid(list_d):
+    def _get_val(self):
+        mat_name = self.get_input(self.mat_name)
+        node_name = self.get_input(self.node_name)
+        if is_invalid(mat_name, node_name):
             return STATUS_WAITING
-        return list_d.copy()
+        return (
+            bpy.data.materials[mat_name]
+            .node_tree
+            .nodes[node_name]
+        )
 
     def evaluate(self):
         self._set_ready()
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/listextend.py` & `uplogic-1.9/uplogic/nodes/parameters/listextend.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_waiting
 
 
 class ULExtendList(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.list_1: list = None
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/listfromitems.py` & `uplogic-1.9/uplogic/nodes/parameters/vectorsplitxyz.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,35 @@
+from mathutils import Vector
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
 from uplogic.utils import is_invalid
-from uplogic.utils import is_waiting
 
 
-class ULListFromItems(ULParameterNode):
+class ULVectorSplitXYZ(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
-        self.items = None
-        self.list: list = None
-        self.LIST = ULOutSocket(self, self.get_list)
-
-    def get_list(self):
-        socket = self.get_output('list')
-        if socket is None:
-            self.list = self.get_input(self.items)
-            return self.set_output('list', [self.get_input(item) for item in self.list])
-        return socket
+        self.input_v = None
+        self.output_v = Vector()
+        self.OUTX = ULOutSocket(self, self.get_out_x)
+        self.OUTY = ULOutSocket(self, self.get_out_y)
+        self.OUTZ = ULOutSocket(self, self.get_out_z)
+
+    def get_out_x(self):
+        vector = self.get_output('vector')
+        if vector is None:
+            vector = self.set_output(
+                'vector',
+                self.get_input(self.input_v)
+            )
+        return self.output_v.x
+
+    def get_out_y(self):
+        return self.output_v.y
+
+    def get_out_z(self):
+        return self.output_v.z
 
     def evaluate(self):
         self._set_ready()
+        vec = self.get_input(self.input_v)
+        if not is_invalid(vec):
+            self.output_v = vec
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/listindex.py` & `uplogic-1.9/uplogic/nodes/parameters/listindex.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 from uplogic.utils import is_waiting
 
 
 class ULListIndex(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/listindexrandom.py` & `uplogic-1.9/uplogic/nodes/parameters/listindexrandom.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 import random
 
 
 class ULListIndexRandom(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/loadvariable.py` & `uplogic-1.9/uplogic/nodes/actions/listvariables.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,72 @@
-from uplogic.nodes import ULParameterNode
+from uplogic.nodes import ULActionNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
-from uplogic.utils import debug
 from uplogic.utils import is_waiting
+from uplogic.utils import not_met
 import bpy
 import json
 import os
 
 
-class ULLoadVariable(ULParameterNode):
+class ULListVariables(ULActionNode):
     def __init__(self):
-        ULParameterNode.__init__(self)
-        self.name = None
-        self.default_value = None
+        ULActionNode.__init__(self)
+        self.condition = None
+        self.print_list = None
         self.file_name = None
         self.path = ''
-        self.VAR = ULOutSocket(self, self.get_var)
+        self.done = None
+        self.items = None
+        self.OUT = ULOutSocket(self, self.get_done)
+        self.LIST = ULOutSocket(self, self.get_list)
 
-    def get_var(self):
-        socket = self.get_output('var')
-        if socket is None:
-            name = self.get_input(self.name)
-            if is_waiting(name):
-                return self.set_output('var', STATUS_WAITING)
-            cust_path = self.get_custom_path(self.path)
-
-            path = (
-                bpy.path.abspath('//Data/')
-                if self.path == ''
-                else bpy.path.abspath(cust_path)
-            )
-            os.makedirs(path, exist_ok=True)
-
-            return self.set_output(
-                'var',
-                self.read_from_json(path, name)
-            )
-        return socket
+    def get_done(self):
+        return self.done
 
-    def read_from_json(self, path, name):
+    def get_list(self):
+        return self.items
+
+    def write_to_json(self, path, p_l):
+        data = None
         if not path.endswith('.json'):
             path = path + f'{self.get_input(self.file_name)}.json'
-        if path:
+        if os.path.isfile(path):
             f = open(path, 'r')
             data = json.load(f)
-            if name not in data:
-                debug(f'"{name}" is not a saved Variabe!')
-                return self.get_input(self.default_value)
-            f.close()
-            return data.get(name)
+            if len(data) == 0:
+                print('There are no saved variables')
+                return
+            li = []
+            for x in data:
+                if p_l:
+                    print('{}\t->\t{}'.format(x, data[x]))
+                li.append(x)
+            self.items = li
         else:
-            debug('No saved variables!')
-            return self.get_input(self.default_value)
+            print('There are no saved variables')
+        f.close()
 
     def get_custom_path(self, path):
         if not path.endswith('/') and not path.endswith('json'):
             path = path + '/'
         return path
 
     def evaluate(self):
+        self.done = False
+        condition = self.get_input(self.condition)
+        if not_met(condition):
+            return
+        print_list = self.get_input(self.print_list)
+        if is_waiting(print_list):
+            return
         self._set_ready()
+        cust_path = self.get_custom_path(self.path)
+
+        path = (
+            bpy.path.abspath('//Data/')
+            if self.path == ''
+            else bpy.path.abspath(cust_path)
+        )
+        os.makedirs(path, exist_ok=True)
+
+        self.write_to_json(path, print_list)
+        self.done = True
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/loadvariabledict.py` & `uplogic-1.9/uplogic/nodes/parameters/loadvariabledict.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/materialgetattribute.py` & `uplogic-1.9/uplogic/nodes/parameters/materialgetattribute.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 from uplogic.utils import is_waiting
 import bpy
 
 
 class ULGetMaterialAttribute(ULParameterNode):
     def __init__(self):
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/materialgetnode.py` & `uplogic-1.9/uplogic/nodes/parameters/materialgetsocket.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,40 @@
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
+from uplogic.utils import is_waiting
 import bpy
 
 
-class ULGetMaterialNode(ULParameterNode):
+class ULGetMaterialSocket(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.mat_name = None
         self.node_name = None
+        self.input_slot = None
         self.OUT = ULOutSocket(self, self._get_val)
 
     def _get_val(self):
-        mat_name = self.get_input(self.mat_name)
-        node_name = self.get_input(self.node_name)
-        if is_invalid(mat_name, node_name):
-            return STATUS_WAITING
-        return (
-            bpy.data.materials[mat_name]
-            .node_tree
-            .nodes[node_name]
-        )
+        socket = self.get_output('val')
+        if socket is None:
+            mat_name = self.get_input(self.mat_name)
+            node_name = self.get_input(self.node_name)
+            if is_invalid(mat_name, node_name):
+                return STATUS_WAITING
+            input_slot = self.get_input(self.input_slot)
+            if is_waiting(mat_name):
+                return STATUS_WAITING
+            return self.set_output(
+                'val',
+                (
+                    bpy.data.materials[mat_name]
+                    .node_tree
+                    .nodes[node_name]
+                    .inputs[input_slot]
+                    .default_value
+                )
+            )
+        return socket
 
     def evaluate(self):
         self._set_ready()
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/materialgetsocket.py` & `uplogic-1.9/uplogic/nodes/parameters/vectoranglecheck.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,45 @@
-from uplogic.nodes import ULParameterNode
+from mathutils import Vector
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.nodes import ULParameterNode
+from uplogic.utils.constants import LOGIC_OPERATORS
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 from uplogic.utils import is_waiting
-import bpy
+import math
 
 
-class ULGetMaterialSocket(ULParameterNode):
+class ULVectorAngleCheck(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
-        self.mat_name = None
-        self.node_name = None
-        self.input_slot = None
-        self.OUT = ULOutSocket(self, self._get_val)
+        self.op: str = None
+        self.vector: Vector = None
+        self.vector_2: Vector = None
+        self.value = None
+        self._angle = 0
+        self.OUT = ULOutSocket(self, self.get_done)
+        self.ANGLE = ULOutSocket(self, self.get_angle)
+
+    def get_angle(self):
+        return self._angle
 
-    def _get_val(self):
-        socket = self.get_output('val')
-        if socket is None:
-            mat_name = self.get_input(self.mat_name)
-            node_name = self.get_input(self.node_name)
-            if is_invalid(mat_name, node_name):
-                return STATUS_WAITING
-            input_slot = self.get_input(self.input_slot)
-            if is_waiting(mat_name):
-                return STATUS_WAITING
-            return self.set_output(
-                'val',
-                (
-                    bpy.data.materials[mat_name]
-                    .node_tree
-                    .nodes[node_name]
-                    .inputs[input_slot]
-                    .default_value
-                )
-            )
-        return socket
+    def get_done(self):
+        op: str = self.get_input(self.op)
+        if is_waiting(
+            op
+        ):
+            return STATUS_WAITING
+        value: float = self.get_input(self.value)
+        return LOGIC_OPERATORS[int(op)](self._angle, value)
 
     def evaluate(self):
+        vector: Vector = self.get_input(self.vector)
+        vector_2: Vector = self.get_input(self.vector_2)
+        if is_invalid(
+            vector,
+            vector_2
+        ):
+            return
         self._set_ready()
+        rad: float = vector.angle(vector_2)
+        deg: float = rad * 180/math.pi
+        self._angle = deg
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/math.py` & `uplogic-1.9/uplogic/nodes/parameters/math.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from mathutils import Vector
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 
 
 class ULMath(ULParameterNode):
 
     def __init__(self):
         ULParameterNode.__init__(self)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/matrixtoxyz.py` & `uplogic-1.9/uplogic/nodes/parameters/matrixtoxyz.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/mousedata.py` & `uplogic-1.9/uplogic/nodes/parameters/mousedata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from mathutils import Vector
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_READY
+from uplogic.utils.constants import STATUS_READY
 
 
 class ULMouseData(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.MX = ULOutSocket(self, self.getmx)
         self.MY = ULOutSocket(self, self.getmy)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/objectattr.py` & `uplogic-1.9/uplogic/nodes/parameters/objectattr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from mathutils import Vector
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_waiting
 from uplogic.utils import is_invalid
 
 
 class ULObjectAttribute(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/objectdataname.py` & `uplogic-1.9/uplogic/nodes/actions/sendnetworkmessage.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,28 @@
-from uplogic.nodes import ULOutSocket
-from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_WAITING
-from uplogic.utils import is_invalid
+from uplogic.nodes import ULActionNode, ULOutSocket
+from uplogic.utils import is_waiting
+from uplogic.utils import not_met
 
 
-class ULObjectDataName(ULParameterNode):
+class ULSendNetworkMessage(ULActionNode):
     def __init__(self):
-        ULParameterNode.__init__(self)
-        self.game_object = None
-        self.OUT = ULOutSocket(self, self.get_name)
+        ULActionNode.__init__(self)
+        self.condition = None
+        self.entity = None
+        self.data = None
+        self.subject = None
+        self._done = False
+        self.OUT = ULOutSocket(self, self.get_done)
 
-    def get_name(self):
-        obj = self.get_input(self.game_object)
-        if is_invalid(obj):
-            return STATUS_WAITING
-        return obj.blenderObject.name
+    def get_done(self):
+        return self._done
 
     def evaluate(self):
-        self._set_ready()
+        self._done = False
+        condition = self.get_input(self.condition)
+        if not_met(condition):
+            self._set_ready()
+            return
+        entity = self.get_input(self.entity)
+        if entity:
+            entity.send(self.get_input(self.data), self.get_input(self.subject))
+        self._done = True
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/objectdatavertices.py` & `uplogic-1.9/uplogic/nodes/parameters/objectdatavertices.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from mathutils import Vector
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 
 
 class ULObjectDataVertices(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.game_object = None
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/randomfloat.py` & `uplogic-1.9/uplogic/nodes/parameters/randomfloat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_waiting
 import sys
 import random
 
 
 class ULRandomFloat(ULParameterNode):
     def __init__(self):
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/randomint.py` & `uplogic-1.9/uplogic/nodes/parameters/randomint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_waiting
 import random
 import sys
 
 
 class ULRandomInt(ULParameterNode):
     def __init__(self):
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/randomvect.py` & `uplogic-1.9/uplogic/nodes/parameters/randomvect.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/rangedthreshold.py` & `uplogic-1.9/uplogic/nodes/parameters/rangedthreshold.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_waiting
 
 
 class ULRangedThreshold(ULParameterNode):
 
     def __init__(self):
         ULParameterNode.__init__(self)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/screenposition.py` & `uplogic-1.9/uplogic/nodes/parameters/serializedata.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING, is_invalid
-from mathutils import Vector
+from uplogic.serialize import Vec2, Vec3, Vec4, Mat3, Mat4, GameObj
 
 
-class ULScreenPosition(ULParameterNode):
+class ULSerializeData(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
-        self.game_object = None
-        self.camera = None
-        self.pos = None
-        self.OUT = ULOutSocket(self, self.get_pos)
+        self.data = None
+        self.serialize_as = 'builtin'
+        self.dattypes = {
+            'Vec2': Vec2,
+            'Vec3': Vec3,
+            'Vec4': Vec4,
+            'Mat3': Mat3,
+            'Mat4': Mat4,
+            'GameObj': GameObj,
+        }
+        self.OUT = ULOutSocket(self, self.get_data)
 
-    def get_pos(self):
-        game_object = self.get_input(self.game_object)
-        camera = self.get_input(self.camera)
-        if is_invalid(game_object) or is_invalid(camera):
-            return STATUS_WAITING
-        position = camera.getScreenPosition(game_object)
-        self._set_value(position)
-        return Vector((position[0], position[1]))
+    def get_data(self):
+        dat = self.get_input(self.data)
+        if self.serialize_as == 'builtin':
+            return dat
+        return self.dattypes[self.serialize_as](dat)
 
     def evaluate(self):
         self._set_ready()
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/storevalue.py` & `uplogic-1.9/uplogic/nodes/parameters/storevalue.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/threshold.py` & `uplogic-1.9/uplogic/nodes/parameters/threshold.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 
 
 class ULThreshold(ULParameterNode):
 
     def __init__(self):
         ULParameterNode.__init__(self)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/timedata.py` & `uplogic-1.9/uplogic/nodes/parameters/timedata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_READY
+from uplogic.utils.constants import STATUS_READY
 from bge import logic
 
 
 class ULTimeData(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.network = None
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/typecastvalue.py` & `uplogic-1.9/uplogic/nodes/parameters/typecastvalue.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_waiting
 
 
 class ULTypeCastValue(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.value = None
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/valueswitch.py` & `uplogic-1.9/uplogic/nodes/parameters/valueswitch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import LOGIC_OPERATORS
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import LOGIC_OPERATORS
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_waiting
 
 
 class ULValueSwitch(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.conditon = None
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/vectorabsolute.py` & `uplogic-1.9/uplogic/nodes/parameters/vectorlength.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from mathutils import Vector
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_WAITING, is_invalid
+from uplogic.utils.constants import STATUS_WAITING
+from uplogic.utils import is_invalid
 
 
-class ULVectorAbsolute(ULParameterNode):
+class ULVectorLength(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.input_v = None
         self.output_v = Vector()
         self.OUTV = ULOutSocket(self, self.get_out_v)
 
     def get_out_v(self):
         vec = self.get_input(self.input_v)
         if is_invalid(vec):
             return STATUS_WAITING
-        vec = vec.copy()
-        vec.x = abs(vec.x)
-        vec.y = abs(vec.y)
-        vec.z = abs(vec.z)
-        return vec
+        return vec.length
 
     def evaluate(self):
         self._set_ready()
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/vectorangle.py` & `uplogic-1.9/uplogic/nodes/parameters/vectorangle.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from mathutils import Vector
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_invalid
 import math
 
 
 class ULVectorAngle(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/vectorlength.py` & `uplogic-1.9/uplogic/nodes/parameters/vectorsplitxy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from mathutils import Vector
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import STATUS_WAITING, is_invalid
+from uplogic.utils import is_invalid
 
 
-class ULVectorLength(ULParameterNode):
+class ULVectorSplitXY(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.input_v = None
         self.output_v = Vector()
-        self.OUTV = ULOutSocket(self, self.get_out_v)
+        self.OUTX = ULOutSocket(self, self.get_out_x)
+        self.OUTY = ULOutSocket(self, self.get_out_y)
 
-    def get_out_v(self):
-        vec = self.get_input(self.input_v)
-        if is_invalid(vec):
-            return STATUS_WAITING
-        return vec.length
+    def get_out_x(self):
+        return self.output_v.x
+
+    def get_out_y(self):
+        return self.output_v.y
 
     def evaluate(self):
         self._set_ready()
+        vec = self.get_input(self.input_v)
+        if not is_invalid(vec):
+            self.output_v = vec
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/vectormath.py` & `uplogic-1.9/uplogic/nodes/parameters/vectormath.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
+from uplogic.utils.constants import STATUS_WAITING
 from uplogic.utils import is_waiting
 from uplogic.utils import is_invalid
 
 
 class ULVectorMath(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
@@ -91,15 +91,15 @@
     def get_cross(self, vec, vec2, vec3, fac, scale):
         return vec.cross(vec2)
 
     def get_multadd(self, vec, vec2, vec3, fac, scale):
         return (vec * vec2) + vec3
 
     def get_divide(self, vec, vec2, vec3, fac, scale):
-        return vec / vec2
+        return vec / fac
 
     def get_multiply(self, vec, vec2, vec3, fac, scale):
         return vec * vec2
 
     def get_subtract(self, vec, vec2, vec3, fac, scale):
         return vec - vec2
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/vectorsplitxy.py` & `uplogic-1.9/uplogic/nodes/parameters/withinrange.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,34 @@
-from mathutils import Vector
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-from uplogic.utils import is_invalid
+from uplogic.nodes import ULOutSocket
+from uplogic.utils.constants import STATUS_WAITING
+from uplogic.utils import is_waiting
+
 
+class ULWithinRange(ULParameterNode):
 
-class ULVectorSplitXY(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
-        self.input_v = None
-        self.output_v = Vector()
-        self.OUTX = ULOutSocket(self, self.get_out_x)
-        self.OUTY = ULOutSocket(self, self.get_out_y)
+        self.value = None
+        self.range = None
+        self.operator = None
+        self.OUT = ULOutSocket(self, self.get_done)
 
-    def get_out_x(self):
-        return self.output_v.x
+    def get_done(self):
+        v = self.get_input(self.value)
+        r = self.get_input(self.range)
+        if is_waiting(v, r):
+            return STATUS_WAITING
+        value = self.calc_range(self.operator, v, r)
+        if (v is None) or (r is None):
+            return STATUS_WAITING
+        else:
+            return value
 
-    def get_out_y(self):
-        return self.output_v.y
+    def calc_range(self, op, v, r):
+        if op == 'OUTSIDE':
+            return True if (v < r.x or v > r.y) else False
+        if op == 'INSIDE':
+            return True if (r.x < v < r.y) else False
 
     def evaluate(self):
         self._set_ready()
-        vec = self.get_input(self.input_v)
-        if not is_invalid(vec):
-            self.output_v = vec
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/vectorsplitxyz.py` & `uplogic-1.9/uplogic/nodes/parameters/vectorxyz.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 from mathutils import Vector
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
 from uplogic.utils import is_invalid
 
 
-class ULVectorSplitXYZ(ULParameterNode):
+class ULVectorXYZ(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
-        self.input_v = None
-        self.output_v = Vector()
-        self.OUTX = ULOutSocket(self, self.get_out_x)
-        self.OUTY = ULOutSocket(self, self.get_out_y)
-        self.OUTZ = ULOutSocket(self, self.get_out_z)
-
-    def get_out_x(self):
-        vector = self.get_output('vector')
-        if vector is None:
-            vector = self.set_output(
-                'vector',
-                self.get_input(self.input_v)
-            )
-        return self.output_v.x
-
-    def get_out_y(self):
-        return self.output_v.y
-
-    def get_out_z(self):
-        return self.output_v.z
+        self.input_x = None
+        self.input_y = None
+        self.input_z = None
+        self.OUTV = ULOutSocket(self, self.get_out_v)
+
+    def get_out_v(self):
+        x = self.get_input(self.input_x)
+        y = self.get_input(self.input_y)
+        z = self.get_input(self.input_z)
+        v = Vector((0, 0, 0))
+        if not is_invalid(x):
+            v.x = x
+        if not is_invalid(y):
+            v.y = y
+        if not is_invalid(y):
+            v.z = z
+        return v.copy()
 
     def evaluate(self):
         self._set_ready()
-        vec = self.get_input(self.input_v)
-        if not is_invalid(vec):
-            self.output_v = vec
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/vectorxy.py` & `uplogic-1.9/uplogic/nodes/parameters/vectorxy.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/vectorxyz.py` & `uplogic-1.9/uplogic/nodes/parameters/vectorxyzw.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from mathutils import Vector
 from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
 from uplogic.utils import is_invalid
 
 
-class ULVectorXYZ(ULParameterNode):
+class ULVectorXYZW(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.input_x = None
         self.input_y = None
         self.input_z = None
+        self.input_w = None
         self.OUTV = ULOutSocket(self, self.get_out_v)
 
     def get_out_v(self):
         x = self.get_input(self.input_x)
         y = self.get_input(self.input_y)
         z = self.get_input(self.input_z)
-        v = Vector((0, 0, 0))
+        w = self.get_input(self.input_w)
+        v = Vector((0, 0, 0, 0))
         if not is_invalid(x):
             v.x = x
         if not is_invalid(y):
             v.y = y
         if not is_invalid(y):
             v.z = z
+        if not is_invalid(y):
+            v.w = w
         return v.copy()
 
     def evaluate(self):
         self._set_ready()
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/vrcontrollervalues.py` & `uplogic-1.9/uplogic/nodes/parameters/vrcontrollervalues.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/vrheadsetvalues.py` & `uplogic-1.9/uplogic/nodes/parameters/vrheadsetvalues.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/withinrange.py` & `uplogic-1.9/uplogic/nodes/parameters/screenposition.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING
-from uplogic.utils import is_waiting
+from uplogic.utils.constants import STATUS_WAITING
+from uplogic.utils import is_invalid
+from mathutils import Vector
 
 
-class ULWithinRange(ULParameterNode):
-
+class ULScreenPosition(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
-        self.value = None
-        self.range = None
-        self.operator = None
-        self.OUT = ULOutSocket(self, self.get_done)
-
-    def get_done(self):
-        v = self.get_input(self.value)
-        r = self.get_input(self.range)
-        if is_waiting(v, r):
+        self.game_object = None
+        self.camera = None
+        self.pos = None
+        self.OUT = ULOutSocket(self, self.get_pos)
+
+    def get_pos(self):
+        game_object = self.get_input(self.game_object)
+        camera = self.get_input(self.camera)
+        if is_invalid(game_object) or is_invalid(camera):
             return STATUS_WAITING
-        value = self.calc_range(self.operator, v, r)
-        if (v is None) or (r is None):
-            return STATUS_WAITING
-        else:
-            return value
-
-    def calc_range(self, op, v, r):
-        if op == 'OUTSIDE':
-            return True if (v < r.x or v > r.y) else False
-        if op == 'INSIDE':
-            return True if (r.x < v < r.y) else False
+        position = camera.getScreenPosition(game_object)
+        self._set_value(position)
+        return Vector((position[0], position[1]))
 
     def evaluate(self):
         self._set_ready()
```

### Comparing `uplogic-1.8.4/uplogic/nodes/parameters/worldposition.py` & `uplogic-1.9/uplogic/nodes/parameters/worldposition.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from uplogic.nodes import ULParameterNode
 from uplogic.nodes import ULOutSocket
-from uplogic.utils import STATUS_WAITING, is_invalid
+from uplogic.utils.constants import STATUS_WAITING
+from uplogic.utils import is_invalid
 
 
 class ULWorldPosition(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.camera = None
         self.screen_x = None
```

### Comparing `uplogic-1.8.4/uplogic/physics/__init__.py` & `uplogic-1.9/uplogic/physics/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/physics/buoyancy.py` & `uplogic-1.9/uplogic/physics/buoyancy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from bge import logic
 from mathutils import Vector
-from uplogic.utils import debug
-from uplogic.utils import vec_clamp
-from uplogic.utils import raycast
-from uplogic.utils import FLOTSAM
-from uplogic.utils import SHIP
-from uplogic.utils import WATER
+from uplogic.utils.math import vec_clamp
+from uplogic.utils.raycasting import raycast
+from uplogic.utils.constants import FLOTSAM
+from uplogic.utils.constants import SHIP
+from uplogic.utils.constants import WATER
 
 
 class ULBuoy():
 
     def __init__(self) -> None:
         self._active = True
 
@@ -24,15 +23,15 @@
 
 
 class ULFlotsam(ULBuoy):
     _deprecated = True
 
     def __init__(self, game_object, buoyancy=1, height=200, align=True) -> None:
         if self._deprecated:
-            debug('ULFlotsam class will be renamed to "Flotsam" in future releases!')
+            print('ULFlotsam class will be renamed to "Flotsam" in future releases!')
         super().__init__()
         self.game_object = game_object
         game_object[FLOTSAM] = self
         self.height = height
         self.buoyancy = buoyancy
         self.align = align
         logic.getCurrentScene().pre_draw.append(self.update)
@@ -76,15 +75,15 @@
 
 
 class ULShip(ULBuoy):
     _deprecated = True
 
     def __init__(self, game_object, buoyancy=1, height=200, water=None) -> None:
         if self._deprecated:
-            debug('ULShip class will be renamed to "Ship" in future releases!')
+            print('ULShip class will be renamed to "Ship" in future releases!')
         super().__init__()
         self.game_object = game_object
         self.linear_damping = game_object.linearDamping
         self.angular_damping = game_object.angularDamping
         game_object[SHIP] = self
         self.height = height
         if water:
```

### Comparing `uplogic-1.8.4/uplogic/physics/character.py` & `uplogic-1.9/uplogic/physics/character.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from bge import logic
 from bge.constraints import getCharacter
 from bge.types import KX_GameObject as GameObject
 from mathutils import Vector
-from uplogic.utils import debug
 import bpy
 
 
 class ULCharacter():
     _deprecated = True
 
     def __init__(self, owner: GameObject) -> None:
         if self._deprecated:
-            debug('ULCharacter class will be renamed to "Character" in future releases!')
+            print('Warning: ULCharacter class will be renamed to "Character" in future releases!')
         self.owner = owner
         self.wrapper = getCharacter(owner)
         self._old_position = owner.worldPosition.copy()
         self.velocity = Vector((0, 0, 0))
         self.is_walking = False
         self._on_ground = self.wrapper.onGround
         self.landed = False
```

### Comparing `uplogic-1.8.4/uplogic/physics/collision.py` & `uplogic-1.9/uplogic/physics/collision.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Callable
 from bge import logic
 from bge.types import KX_GameObject as GameObject
-from uplogic.utils import debug
 
 
 class ULCollision():
     """Collision Handler.
 
     Not intended for manual use."""
     target = None
@@ -26,15 +25,15 @@
         callback: Callable,
         prop: str = '',
         mat: str = '',
         tap: bool = False,
         post_call: bool = False
     ):
         if self._deprecated:
-            debug('ULCollision class will be renamed to "Collision" in future releases!')
+            print('Warning: ULCollision class will be renamed to "Collision" in future releases!')
         self.callback: Callable = callback
         self.prop: str = prop
         self.mat: str = mat
         self.tap: bool = tap
         self.post_call = post_call
         self.game_object: GameObject = game_object
         self.register()
```

### Comparing `uplogic-1.8.4/uplogic/physics/constraints.py` & `uplogic-1.9/uplogic/physics/constraints.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from bge import constraints
 from bge import logic
 from bge import render
 from bge.types import KX_ConstraintWrapper as GameConstraint
 from bge.types import KX_GameObject as GameObject
 from mathutils import Vector
-from uplogic.utils import debug, get_direction
-from uplogic.utils import set_curve_points
-from uplogic.utils import xrot_to
-from uplogic.utils import yrot_to
-from uplogic.utils import zrot_to
+from uplogic.utils.math import get_direction
+from uplogic.utils.objects import set_curve_points
+from uplogic.utils.objects import xrot_to
+from uplogic.utils.objects import yrot_to
+from uplogic.utils.objects import zrot_to
 
 
 CONSTRAINT_TYPES = {
     'point': 0,
     'hinge': 1,
     'angular': 2,
     'conetwist': 3,
```

### Comparing `uplogic-1.8.4/uplogic/physics/vehicle.py` & `uplogic-1.9/uplogic/physics/vehicle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from bge import logic
 from bge.types import KX_GameObject
 from bge.constraints import createVehicle
 from mathutils import Euler
 from mathutils import Vector
-from uplogic.utils import VEHICLE
-from uplogic.utils import debug
+from uplogic.utils.constants import VEHICLE
 
 FWD = 'FRONT'
 """Front Wheel Drive\n
 This will adress wheel indices starting in the front."""
 
 RWD = 'REAR'
 """Rear Wheel Drive\n
@@ -30,15 +29,15 @@
         damping: float = 5.0,
         friction: float = 2.0,
         wheel_size: float = 1.0,
         drive: str = FWD,
         steer_axle: str = FWD
     ) -> None:
         if self._deprecated:
-            debug('ULVehicle class will be renamed to "Vehicle" in future releases!')
+            print('Warning: ULVehicle class will be renamed to "Vehicle" in future releases!')
         orig_ori = body.localOrientation.copy()
         body.localOrientation = Euler((0, 0, 0), 'XYZ')
         ph_id = body.getPhysicsId()
         car = createVehicle(ph_id)
         down = Vector((0, 0, -1))
         axle_dir = body.getAxisVect(Vector((-1, 0, 0)))
         wheels = []
```

### Comparing `uplogic-1.8.4/uplogic/shaders/__init__.py` & `uplogic-1.9/uplogic/shaders/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/shaders/adaptivetonemapping.py` & `uplogic-1.9/uplogic/shaders/adaptivetonemapping.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/shaders/blur.py` & `uplogic-1.9/uplogic/shaders/blur.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/shaders/brightness.py` & `uplogic-1.9/uplogic/shaders/brightness.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/shaders/chromaticaberration.py` & `uplogic-1.9/uplogic/shaders/chromaticaberration.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/shaders/distort.py` & `uplogic-1.9/uplogic/shaders/distort.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/shaders/dof.py` & `uplogic-1.9/uplogic/shaders/dof.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/shaders/droplets.py` & `uplogic-1.9/uplogic/shaders/droplets.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/shaders/fxaa.py` & `uplogic-1.9/uplogic/shaders/fxaa.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/shaders/grayscale.py` & `uplogic-1.9/uplogic/shaders/grayscale.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/shaders/hbao.py` & `uplogic-1.9/uplogic/shaders/hbao.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/shaders/letterbox.py` & `uplogic-1.9/uplogic/shaders/letterbox.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/shaders/levels.py` & `uplogic-1.9/uplogic/shaders/levels.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/shaders/mist.py` & `uplogic-1.9/uplogic/shaders/mist.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/shaders/shader.py` & `uplogic-1.9/uplogic/shaders/shader.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/shaders/sharpen.py` & `uplogic-1.9/uplogic/shaders/sharpen.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/shaders/ssao.py` & `uplogic-1.9/uplogic/shaders/ssao.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/shaders/vignette.py` & `uplogic-1.9/uplogic/shaders/vignette.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/ui/behaviors.py` & `uplogic-1.9/uplogic/ui/behaviors.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/ui/button.py` & `uplogic-1.9/uplogic/ui/button.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/ui/canvas.py` & `uplogic-1.9/uplogic/ui/canvas.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/ui/cursor.py` & `uplogic-1.9/uplogic/ui/cursor.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/ui/image.py` & `uplogic-1.9/uplogic/ui/image.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -46,18 +46,18 @@
         self._batch.draw(self._shader)
         super().draw()
 
 
 class Icon(Image):
 
     def __init__(self, pos=[0, 0], size=(100, 100), relative={}, texture=None, icon=0, rows=1, cols=1, halign='left', valign='bottom'):
-        super().__init__(pos, size, relative, texture, halign=halign, valign=valign)
         self.icon = icon
         self.rows = rows
         self.cols = cols
+        super().__init__(pos, size, relative, texture, halign=halign, valign=valign)
 
     @property
     def rows(self):
         return self._rows
 
     @rows.setter
     def rows(self, val):
```

### Comparing `uplogic-1.8.4/uplogic/ui/label.py` & `uplogic-1.9/uplogic/ui/label.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,38 +94,42 @@
         return self._font_color[3]
 
     @font_opacity.setter
     def font_opacity(self, val):
         self._font_color[3] = val * self.opacity
 
     @property
+    def dimensions(self):
+        return blf.dimensions(self.font, self.text)
+
+    @property
     def _draw_size(self):
         # if self.parent is None:
         #     return [0, 0]
         return blf.dimensions(self.font, self.text)
 
     def draw(self):
         super()._setup_draw()
+        blf.size(self.font, self.font_size)
+        blf.color(self.font, self.font_color[0], self.font_color[1], self.font_color[2], self.font_color[3])
+        charsize = blf.dimensions(self.font, 'A')
         if self.parent.use_clipping:
             verts = self.parent._vertices
             blf.enable(self.font, blf.CLIPPING)
-            blf.clipping(self.font, verts[0][0], verts[0][1], verts[2][0], verts[2][1])
+            blf.clipping(self.font, verts[0][0], verts[0][1] + charsize[1], verts[2][0], verts[2][1])
         else:
             blf.disable(self.font, blf.CLIPPING)
-        if self.wrap:
+        if self.wrap and self.parent:
             blf.enable(self.font, blf.WORD_WRAP)
-            blf.word_wrap(self.font, self.size[0])
+            blf.word_wrap(self.font, self.parent._draw_size[0])
         if self.shadow:
             col = self.shadow_color
             blf.enable(self.font, blf.SHADOW)
             blf.shadow(self.font, 0, col[0], col[1], col[2], col[3])
             blf.shadow_offset(self.font, int(self.shadow_offset[0]), int(self.shadow_offset[1]))
-        blf.size(self.font, self.font_size)
-        blf.color(self.font, self.font_color[0], self.font_color[1], self.font_color[2], self.font_color[3])
-        charsize = blf.dimensions(self.font, 'A')
         lines = [t for t in self.text.split('\n')]
         if len(lines) > 1:
             for i, txt in enumerate(lines):
                 pos = self._draw_pos.copy()
                 dimensions = blf.dimensions(self.font, txt)
                 lheight = (charsize[1] * self.line_height)
                 if self.text_halign == 'center':
```

### Comparing `uplogic-1.8.4/uplogic/ui/layout.py` & `uplogic-1.9/uplogic/ui/layout.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,17 @@
         bg_color: list = [0, 0, 0, 0],
         relative: dict = {},
         border_width: int = 1,
         border_color: list = [0, 0, 0, 0],
         halign: str = 'left',
         valign: str = 'bottom'
     ):
-        super().__init__(pos, size, bg_color, relative, halign=halign, valign=valign)
         self.border_width = border_width
         self.border_color = border_color
+        super().__init__(pos, size, bg_color, relative, halign=halign, valign=valign)
 
     @property
     def opacity(self):
         return self.bg_color[3]
 
     @opacity.setter
     def opacity(self, val):
```

### Comparing `uplogic-1.8.4/uplogic/ui/widget.py` & `uplogic-1.9/uplogic/ui/widget.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/utils/errors.py` & `uplogic-1.9/uplogic/utils/errors.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/utils/lights.py` & `uplogic-1.9/uplogic/utils/lights.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/utils/nodetrees.py` & `uplogic-1.9/uplogic/utils/nodetrees.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/utils/raycasting.py` & `uplogic-1.9/uplogic/utils/raycasting.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,17 +262,25 @@
         return self[1]
 
     @property
     def normal(self) -> Vector:
         return self[2]
 
     @property
-    def points(self) -> list:
+    def points(self) -> list[Vector]:
         return self[3]
 
+    @property
+    def direction(self) -> Vector:
+        p = self.points
+        if len(p) > 1:
+            return (p[-1] - p[-2]).normalized()
+        else:
+            return Vector((0, 0, 0))
+
 
 def raycast_projectile(
     caster: GameObject,
     origin: Vector,
     aim: Vector,
     power: float,
     distance: float = 100,
@@ -301,19 +309,19 @@
     :returns: (`obj`, `point`, `normal`, `points`)
     """
     def calc_projectile(t, vel, pos, gravity):
         half: float = gravity * (.5 * t * t)
         vel = vel * t
         return half + vel + pos
 
+    if not local:
+        aim = aim - origin
     aim.normalize()
     aim *= power
     origin = getattr(origin, 'worldPosition', origin)
-    if local:
-        origin = origin + caster.worldPosition
 
     points: list = [origin]
     color: list = [1, 0, 0]
     idx = 0
     total_dist: float = 0
 
     grav = gravity if gravity else logic.getCurrentScene().gravity
```

### Comparing `uplogic-1.8.4/uplogic/utils/scene.py` & `uplogic-1.9/uplogic/utils/scene.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic/utils/visuals.py` & `uplogic-1.9/uplogic/utils/visuals.py`

 * *Files identical despite different names*

### Comparing `uplogic-1.8.4/uplogic.egg-info/PKG-INFO` & `uplogic-1.9/uplogic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: uplogic
-Version: 1.8.4
+Version: 1.9
 Summary: Uplogic utility for UPBGE.
 Home-page: https://github.com/UPBGE/uplogic
 Author: Leopold Auersperg-Castell
 Author-email: lauersperg@gmx.at
 License: GPLv2
-Download-URL: https://github.com/UPBGE/uplogic/archive/refs/tags/v1.8.4.tar.gz
+Download-URL: https://github.com/UPBGE/uplogic/archive/refs/tags/v1.9.tar.gz
 Keywords: Blender UPBGE logic
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python
 License-File: LICENSE.md
```

### Comparing `uplogic-1.8.4/uplogic.egg-info/SOURCES.txt` & `uplogic-1.9/uplogic.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -71,14 +71,16 @@
 uplogic/nodes/actions/instream.py
 uplogic/nodes/actions/listglobalvalues.py
 uplogic/nodes/actions/listvariables.py
 uplogic/nodes/actions/loadblendfile.py
 uplogic/nodes/actions/loadfilecontent.py
 uplogic/nodes/actions/loadgame.py
 uplogic/nodes/actions/loadscene.py
+uplogic/nodes/actions/localclient.py
+uplogic/nodes/actions/localserver.py
 uplogic/nodes/actions/makeuniquelight.py
 uplogic/nodes/actions/modifyproperty.py
 uplogic/nodes/actions/mouselook.py
 uplogic/nodes/actions/mouseraycast.py
 uplogic/nodes/actions/mousesetposition.py
 uplogic/nodes/actions/moveto.py
 uplogic/nodes/actions/movetowithnavmesh.py
@@ -102,14 +104,15 @@
 uplogic/nodes/actions/rotateto.py
 uplogic/nodes/actions/runactuator.py
 uplogic/nodes/actions/runpython.py
 uplogic/nodes/actions/savegame.py
 uplogic/nodes/actions/savevariable.py
 uplogic/nodes/actions/savevariabledict.py
 uplogic/nodes/actions/sendmessage.py
+uplogic/nodes/actions/sendnetworkmessage.py
 uplogic/nodes/actions/setactionframe.py
 uplogic/nodes/actions/setactuatorvalue.py
 uplogic/nodes/actions/setboneconstraintattr.py
 uplogic/nodes/actions/setboneconstraintinfluence.py
 uplogic/nodes/actions/setboneconstrainttarget.py
 uplogic/nodes/actions/setboneposition.py
 uplogic/nodes/actions/setcamera.py
@@ -160,14 +163,15 @@
 uplogic/nodes/actions/setsensorvalue.py
 uplogic/nodes/actions/settimescale.py
 uplogic/nodes/actions/setuiwidgetattr.py
 uplogic/nodes/actions/setvisibility.py
 uplogic/nodes/actions/setvsync.py
 uplogic/nodes/actions/showframerate.py
 uplogic/nodes/actions/slowfollow.py
+uplogic/nodes/actions/spawnpool.py
 uplogic/nodes/actions/startsound.py
 uplogic/nodes/actions/startsound3d.py
 uplogic/nodes/actions/startspeaker.py
 uplogic/nodes/actions/startsubnetwork.py
 uplogic/nodes/actions/stopaction.py
 uplogic/nodes/actions/stopallsounds.py
 uplogic/nodes/actions/stopsound.py
@@ -290,14 +294,15 @@
 uplogic/nodes/parameters/objectdataname.py
 uplogic/nodes/parameters/objectdatavertices.py
 uplogic/nodes/parameters/randomfloat.py
 uplogic/nodes/parameters/randomint.py
 uplogic/nodes/parameters/randomvect.py
 uplogic/nodes/parameters/rangedthreshold.py
 uplogic/nodes/parameters/screenposition.py
+uplogic/nodes/parameters/serializedata.py
 uplogic/nodes/parameters/simplevalue.py
 uplogic/nodes/parameters/storevalue.py
 uplogic/nodes/parameters/threshold.py
 uplogic/nodes/parameters/timedata.py
 uplogic/nodes/parameters/typecastvalue.py
 uplogic/nodes/parameters/valueswitch.py
 uplogic/nodes/parameters/vectorabsolute.py
@@ -316,14 +321,15 @@
 uplogic/nodes/parameters/worldposition.py
 uplogic/physics/__init__.py
 uplogic/physics/buoyancy.py
 uplogic/physics/character.py
 uplogic/physics/collision.py
 uplogic/physics/constraints.py
 uplogic/physics/vehicle.py
+uplogic/serialize/__init__.py
 uplogic/shaders/__init__.py
 uplogic/shaders/adaptivetonemapping.py
 uplogic/shaders/blur.py
 uplogic/shaders/brightness.py
 uplogic/shaders/chromaticaberration.py
 uplogic/shaders/distort.py
 uplogic/shaders/dof.py
@@ -344,15 +350,17 @@
 uplogic/ui/canvas.py
 uplogic/ui/cursor.py
 uplogic/ui/image.py
 uplogic/ui/label.py
 uplogic/ui/layout.py
 uplogic/ui/widget.py
 uplogic/utils/__init__.py
+uplogic/utils/constants.py
 uplogic/utils/errors.py
 uplogic/utils/lights.py
+uplogic/utils/math.py
 uplogic/utils/nodetrees.py
 uplogic/utils/objects.py
 uplogic/utils/pooling.py
 uplogic/utils/raycasting.py
 uplogic/utils/scene.py
 uplogic/utils/visuals.py
```

