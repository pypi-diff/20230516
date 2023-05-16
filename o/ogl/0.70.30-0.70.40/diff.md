# Comparing `tmp/ogl-0.70.30.tar.gz` & `tmp/ogl-0.70.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogl-0.70.30.tar", last modified: Mon May 15 00:20:45 2023, max compression
+gzip compressed data, was "ogl-0.70.40.tar", last modified: Tue May 16 17:13:27 2023, max compression
```

## Comparing `ogl-0.70.30.tar` & `ogl-0.70.40.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:20:45.213016 ogl-0.70.30/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-23 23:19:08.000000 ogl-0.70.30/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2357 2023-05-15 00:20:45.212892 ogl-0.70.30/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1999 2023-04-12 19:50:00.000000 ogl-0.70.30/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:20:45.205310 ogl-0.70.30/miniogl/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5038 2023-03-22 20:23:56.000000 ogl-0.70.30/miniogl/AnchorPoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1022 2023-02-21 19:19:18.000000 ogl-0.70.30/miniogl/AttachmentSide.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2916 2022-05-18 20:30:08.000000 ogl-0.70.30/miniogl/Common.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       87 2022-05-18 20:30:08.000000 ogl-0.70.30/miniogl/Constants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1365 2022-05-18 20:30:08.000000 ogl-0.70.30/miniogl/ControlPoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3743 2023-02-11 18:19:50.000000 ogl-0.70.30/miniogl/Diagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    40698 2023-03-25 20:34:07.000000 ogl-0.70.30/miniogl/DiagramFrame.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4713 2023-03-22 20:23:56.000000 ogl-0.70.30/miniogl/DlgDebugDiagramFrame.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1669 2022-05-18 20:30:08.000000 ogl-0.70.30/miniogl/LinePoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13202 2023-03-22 20:23:56.000000 ogl-0.70.30/miniogl/LineShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3594 2023-02-21 21:15:44.000000 ogl-0.70.30/miniogl/LollipopLine.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1747 2023-02-11 19:23:36.000000 ogl-0.70.30/miniogl/MiniOglColorEnum.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1684 2022-05-18 20:30:08.000000 ogl-0.70.30/miniogl/MiniOglPenStyle.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      170 2022-05-18 20:30:08.000000 ogl-0.70.30/miniogl/MiniOglUtils.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2771 2022-05-18 20:30:08.000000 ogl-0.70.30/miniogl/PointShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10767 2023-05-03 16:34:04.000000 ogl-0.70.30/miniogl/RectangleShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1076 2022-05-18 20:30:08.000000 ogl-0.70.30/miniogl/RectangleShapeModel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4772 2022-11-13 14:57:11.000000 ogl-0.70.30/miniogl/RotatableShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2156 2023-03-22 20:23:56.000000 ogl-0.70.30/miniogl/SelectAnchorPoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21669 2023-03-22 20:23:56.000000 ogl-0.70.30/miniogl/Shape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2322 2022-05-18 20:30:08.000000 ogl-0.70.30/miniogl/ShapeEventHandler.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1632 2023-03-22 20:23:56.000000 ogl-0.70.30/miniogl/ShapeModel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1452 2022-05-18 20:30:08.000000 ogl-0.70.30/miniogl/SizerShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7511 2023-03-25 21:42:57.000000 ogl-0.70.30/miniogl/TextShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      649 2022-05-18 20:30:08.000000 ogl-0.70.30/miniogl/TextShapeModel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5650 2022-11-13 14:38:42.000000 ogl-0.70.30/miniogl/VShapes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.30/miniogl/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.30/miniogl/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:20:45.208340 ogl-0.70.30/ogl/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      126 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/IllegalOperationException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3747 2022-06-08 19:34:57.000000 ogl-0.70.30/ogl/OglActor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1463 2022-11-01 13:15:29.000000 ogl-0.70.30/ogl/OglAggregation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12912 2023-03-25 20:34:07.000000 ogl-0.70.30/ogl/OglAssociation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      204 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/OglAssociationLabel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    20392 2023-03-25 20:34:07.000000 ogl-0.70.30/ogl/OglClass.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1409 2023-03-22 20:23:56.000000 ogl-0.70.30/ogl/OglComposition.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      668 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/OglConstants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      717 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/OglDimensions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1460 2023-01-31 22:21:10.000000 ogl-0.70.30/ogl/OglInheritance.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3541 2023-03-31 00:59:54.000000 ogl-0.70.30/ogl/OglInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6199 2023-02-21 19:19:18.000000 ogl-0.70.30/ogl/OglInterface2.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    15577 2023-03-22 20:23:56.000000 ogl-0.70.30/ogl/OglLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3115 2023-03-26 22:27:03.000000 ogl-0.70.30/ogl/OglLinkFactory.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2693 2022-08-28 23:27:21.000000 ogl-0.70.30/ogl/OglNote.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1180 2023-02-19 02:02:00.000000 ogl-0.70.30/ogl/OglNoteLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5544 2023-05-03 16:33:14.000000 ogl-0.70.30/ogl/OglObject.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      473 2022-07-18 19:30:46.000000 ogl-0.70.30/ogl/OglPosition.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8713 2023-03-22 20:23:56.000000 ogl-0.70.30/ogl/OglText.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      226 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/OglTextFontFamily.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2197 2022-06-08 20:23:03.000000 ogl-0.70.30/ogl/OglUseCase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4349 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/OglUtils.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       37 2023-05-14 21:20:56.000000 ogl-0.70.30/ogl/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       24 2023-05-15 00:08:21.000000 ogl-0.70.30/ogl/_version.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:20:45.209696 ogl-0.70.30/ogl/events/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      543 2023-01-15 21:02:48.000000 ogl-0.70.30/ogl/events/IOglEventEngine.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       52 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/events/InvalidKeywordException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4566 2023-01-15 21:06:24.000000 ogl-0.70.30/ogl/events/OglEventEngine.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      780 2022-11-14 22:52:55.000000 ogl-0.70.30/ogl/events/OglEvents.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      239 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/events/ShapeSelectedEventData.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/events/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.30/ogl/events/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:20:45.210009 ogl-0.70.30/ogl/preferences/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21282 2023-05-14 20:59:24.000000 ogl-0.70.30/ogl/preferences/OglPreferences.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/preferences/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.30/ogl/preferences/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.30/ogl/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:20:45.210097 ogl-0.70.30/ogl/resources/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/resources/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:20:45.210587 ogl-0.70.30/ogl/resources/img/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1350 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/resources/img/Display.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1702 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/resources/img/DoNotDisplay.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2238 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/resources/img/UnSpecified.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/resources/img/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.30/ogl/resources/img/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:20:45.210988 ogl-0.70.30/ogl/resources/img/textdetails/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1543 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/resources/img/textdetails/DecreaseTextSize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1575 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/resources/img/textdetails/IncreaseTextSize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/resources/img/textdetails/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.30/ogl/resources/img/textdetails/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:20:45.211480 ogl-0.70.30/ogl/sd/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      904 2023-05-12 20:37:54.000000 ogl-0.70.30/ogl/sd/OglInstanceName.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6876 2023-03-26 01:49:15.000000 ogl-0.70.30/ogl/sd/OglSDInstance.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6874 2023-05-14 21:08:57.000000 ogl-0.70.30/ogl/sd/OglSDMessage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.30/ogl/sd/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.30/ogl/sd/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:20:45.211986 ogl-0.70.30/ogl/ui/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      657 2023-02-08 20:22:10.000000 ogl-0.70.30/ogl/ui/BaseOglPreferencesPage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3967 2023-02-19 20:46:44.000000 ogl-0.70.30/ogl/ui/DefaultValuesPreferencesPage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12232 2023-02-19 22:08:38.000000 ogl-0.70.30/ogl/ui/DiagramPreferencesPage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 14:43:49.000000 ogl-0.70.30/ogl/ui/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.30/ogl/ui/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:20:45.212730 ogl-0.70.30/ogl/ui/valuecontrols/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2279 2023-02-11 21:29:46.000000 ogl-0.70.30/ogl/ui/valuecontrols/AssociationAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5065 2023-02-11 20:04:09.000000 ogl-0.70.30/ogl/ui/valuecontrols/ClassAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2987 2023-02-11 20:20:38.000000 ogl-0.70.30/ogl/ui/valuecontrols/DefaultNamesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1943 2023-03-26 22:24:15.000000 ogl-0.70.30/ogl/ui/valuecontrols/NoteAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2686 2023-03-26 22:24:31.000000 ogl-0.70.30/ogl/ui/valuecontrols/SDAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5284 2023-05-14 22:17:09.000000 ogl-0.70.30/ogl/ui/valuecontrols/TextAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-09 15:30:26.000000 ogl-0.70.30/ogl/ui/valuecontrols/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 00:20:45.208952 ogl-0.70.30/ogl.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2357 2023-05-15 00:20:45.000000 ogl-0.70.30/ogl.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2516 2023-05-15 00:20:45.000000 ogl-0.70.30/ogl.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-05-15 00:20:45.000000 ogl-0.70.30/ogl.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       90 2023-05-15 00:20:45.000000 ogl-0.70.30/ogl.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-05-15 00:20:45.000000 ogl-0.70.30/ogl.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-05-15 00:20:45.213049 ogl-0.70.30/setup.cfg
--rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)     1565 2023-05-14 21:30:41.000000 ogl-0.70.30/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-16 17:13:27.604852 ogl-0.70.40/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-23 23:19:08.000000 ogl-0.70.40/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2357 2023-05-16 17:13:27.604706 ogl-0.70.40/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1999 2023-04-12 19:50:00.000000 ogl-0.70.40/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-16 17:13:27.591069 ogl-0.70.40/miniogl/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5038 2023-03-22 20:23:56.000000 ogl-0.70.40/miniogl/AnchorPoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1022 2023-02-21 19:19:18.000000 ogl-0.70.40/miniogl/AttachmentSide.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2916 2022-05-18 20:30:08.000000 ogl-0.70.40/miniogl/Common.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       87 2022-05-18 20:30:08.000000 ogl-0.70.40/miniogl/Constants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1365 2022-05-18 20:30:08.000000 ogl-0.70.40/miniogl/ControlPoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3743 2023-05-15 20:23:59.000000 ogl-0.70.40/miniogl/Diagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    40698 2023-05-16 01:00:55.000000 ogl-0.70.40/miniogl/DiagramFrame.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4713 2023-03-22 20:23:56.000000 ogl-0.70.40/miniogl/DlgDebugDiagramFrame.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1669 2022-05-18 20:30:08.000000 ogl-0.70.40/miniogl/LinePoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13202 2023-03-22 20:23:56.000000 ogl-0.70.40/miniogl/LineShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3594 2023-02-21 21:15:44.000000 ogl-0.70.40/miniogl/LollipopLine.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1747 2023-02-11 19:23:36.000000 ogl-0.70.40/miniogl/MiniOglColorEnum.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1684 2022-05-18 20:30:08.000000 ogl-0.70.40/miniogl/MiniOglPenStyle.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      170 2022-05-18 20:30:08.000000 ogl-0.70.40/miniogl/MiniOglUtils.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2771 2022-05-18 20:30:08.000000 ogl-0.70.40/miniogl/PointShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10767 2023-05-16 01:00:24.000000 ogl-0.70.40/miniogl/RectangleShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1076 2022-05-18 20:30:08.000000 ogl-0.70.40/miniogl/RectangleShapeModel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4772 2022-11-13 14:57:11.000000 ogl-0.70.40/miniogl/RotatableShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2156 2023-03-22 20:23:56.000000 ogl-0.70.40/miniogl/SelectAnchorPoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21669 2023-05-15 20:23:15.000000 ogl-0.70.40/miniogl/Shape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2336 2023-05-16 16:52:43.000000 ogl-0.70.40/miniogl/ShapeEventHandler.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1632 2023-03-22 20:23:56.000000 ogl-0.70.40/miniogl/ShapeModel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1452 2023-05-16 00:57:28.000000 ogl-0.70.40/miniogl/SizerShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7511 2023-03-25 21:42:57.000000 ogl-0.70.40/miniogl/TextShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      649 2022-05-18 20:30:08.000000 ogl-0.70.40/miniogl/TextShapeModel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5650 2022-11-13 14:38:42.000000 ogl-0.70.40/miniogl/VShapes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.40/miniogl/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.40/miniogl/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-16 17:13:27.596349 ogl-0.70.40/ogl/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      126 2022-05-18 20:30:08.000000 ogl-0.70.40/ogl/IllegalOperationException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4646 2023-05-16 01:11:07.000000 ogl-0.70.40/ogl/OglActor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1463 2022-11-01 13:15:29.000000 ogl-0.70.40/ogl/OglAggregation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12912 2023-03-25 20:34:07.000000 ogl-0.70.40/ogl/OglAssociation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      204 2022-05-18 20:30:08.000000 ogl-0.70.40/ogl/OglAssociationLabel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    20392 2023-05-16 00:59:29.000000 ogl-0.70.40/ogl/OglClass.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1409 2023-03-22 20:23:56.000000 ogl-0.70.40/ogl/OglComposition.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      668 2022-05-18 20:30:08.000000 ogl-0.70.40/ogl/OglConstants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      717 2022-05-18 20:30:08.000000 ogl-0.70.40/ogl/OglDimensions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1460 2023-01-31 22:21:10.000000 ogl-0.70.40/ogl/OglInheritance.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3541 2023-03-31 00:59:54.000000 ogl-0.70.40/ogl/OglInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6199 2023-02-21 19:19:18.000000 ogl-0.70.40/ogl/OglInterface2.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    15577 2023-03-22 20:23:56.000000 ogl-0.70.40/ogl/OglLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3115 2023-03-26 22:27:03.000000 ogl-0.70.40/ogl/OglLinkFactory.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2693 2022-08-28 23:27:21.000000 ogl-0.70.40/ogl/OglNote.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1180 2023-02-19 02:02:00.000000 ogl-0.70.40/ogl/OglNoteLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5529 2023-05-16 16:51:16.000000 ogl-0.70.40/ogl/OglObject.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      473 2022-07-18 19:30:46.000000 ogl-0.70.40/ogl/OglPosition.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8683 2023-05-15 20:22:45.000000 ogl-0.70.40/ogl/OglText.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      226 2022-05-18 20:30:08.000000 ogl-0.70.40/ogl/OglTextFontFamily.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2197 2022-06-08 20:23:03.000000 ogl-0.70.40/ogl/OglUseCase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4349 2022-05-18 20:30:08.000000 ogl-0.70.40/ogl/OglUtils.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       37 2023-05-14 21:20:56.000000 ogl-0.70.40/ogl/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       24 2023-05-16 14:01:40.000000 ogl-0.70.40/ogl/_version.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-16 17:13:27.598441 ogl-0.70.40/ogl/events/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      543 2023-01-15 21:02:48.000000 ogl-0.70.40/ogl/events/IOglEventEngine.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       52 2022-05-18 20:30:08.000000 ogl-0.70.40/ogl/events/InvalidKeywordException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4566 2023-01-15 21:06:24.000000 ogl-0.70.40/ogl/events/OglEventEngine.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      780 2022-11-14 22:52:55.000000 ogl-0.70.40/ogl/events/OglEvents.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      239 2022-05-18 20:30:08.000000 ogl-0.70.40/ogl/events/ShapeSelectedEventData.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.40/ogl/events/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.40/ogl/events/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-16 17:13:27.599121 ogl-0.70.40/ogl/preferences/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21282 2023-05-14 20:59:24.000000 ogl-0.70.40/ogl/preferences/OglPreferences.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.40/ogl/preferences/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.40/ogl/preferences/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.40/ogl/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-16 17:13:27.599248 ogl-0.70.40/ogl/resources/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.40/ogl/resources/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-16 17:13:27.600129 ogl-0.70.40/ogl/resources/img/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1350 2022-05-18 20:30:08.000000 ogl-0.70.40/ogl/resources/img/Display.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1702 2022-05-18 20:30:08.000000 ogl-0.70.40/ogl/resources/img/DoNotDisplay.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2238 2022-05-18 20:30:08.000000 ogl-0.70.40/ogl/resources/img/UnSpecified.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.40/ogl/resources/img/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.40/ogl/resources/img/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-16 17:13:27.600713 ogl-0.70.40/ogl/resources/img/textdetails/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1543 2022-05-18 20:30:08.000000 ogl-0.70.40/ogl/resources/img/textdetails/DecreaseTextSize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1575 2022-05-18 20:30:08.000000 ogl-0.70.40/ogl/resources/img/textdetails/IncreaseTextSize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.40/ogl/resources/img/textdetails/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.40/ogl/resources/img/textdetails/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-16 17:13:27.601712 ogl-0.70.40/ogl/sd/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      904 2023-05-12 20:37:54.000000 ogl-0.70.40/ogl/sd/OglInstanceName.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6876 2023-05-16 01:17:51.000000 ogl-0.70.40/ogl/sd/OglSDInstance.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6874 2023-05-14 21:08:57.000000 ogl-0.70.40/ogl/sd/OglSDMessage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.40/ogl/sd/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.40/ogl/sd/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-16 17:13:27.602757 ogl-0.70.40/ogl/ui/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      657 2023-05-16 00:59:48.000000 ogl-0.70.40/ogl/ui/BaseOglPreferencesPage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3967 2023-02-19 20:46:44.000000 ogl-0.70.40/ogl/ui/DefaultValuesPreferencesPage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12232 2023-02-19 22:08:38.000000 ogl-0.70.40/ogl/ui/DiagramPreferencesPage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 14:43:49.000000 ogl-0.70.40/ogl/ui/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.40/ogl/ui/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-16 17:13:27.604546 ogl-0.70.40/ogl/ui/valuecontrols/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2279 2023-02-11 21:29:46.000000 ogl-0.70.40/ogl/ui/valuecontrols/AssociationAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5065 2023-02-11 20:04:09.000000 ogl-0.70.40/ogl/ui/valuecontrols/ClassAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2987 2023-02-11 20:20:38.000000 ogl-0.70.40/ogl/ui/valuecontrols/DefaultNamesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1943 2023-03-26 22:24:15.000000 ogl-0.70.40/ogl/ui/valuecontrols/NoteAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2686 2023-03-26 22:24:31.000000 ogl-0.70.40/ogl/ui/valuecontrols/SDAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5284 2023-05-14 22:17:09.000000 ogl-0.70.40/ogl/ui/valuecontrols/TextAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-09 15:30:26.000000 ogl-0.70.40/ogl/ui/valuecontrols/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-16 17:13:27.597010 ogl-0.70.40/ogl.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2357 2023-05-16 17:13:27.000000 ogl-0.70.40/ogl.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2516 2023-05-16 17:13:27.000000 ogl-0.70.40/ogl.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-05-16 17:13:27.000000 ogl-0.70.40/ogl.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       90 2023-05-16 17:13:27.000000 ogl-0.70.40/ogl.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-05-16 17:13:27.000000 ogl-0.70.40/ogl.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-05-16 17:13:27.604885 ogl-0.70.40/setup.cfg
+-rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)     1565 2023-05-15 00:33:33.000000 ogl-0.70.40/setup.py
```

### Comparing `ogl-0.70.30/LICENSE` & `ogl-0.70.40/LICENSE`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/PKG-INFO` & `ogl-0.70.40/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogl
-Version: 0.70.30
+Version: 0.70.40
 Summary: External Pyut Graphical Shapes
 Home-page: https://github.com/hasii2011/ogl
 Author: Humberto A. Sanchez II
 Author-email: Humberto.A.Sanchez.II@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ogl Version: 0.70.30 Summary: External Pyut
+Metadata-Version: 2.1 Name: ogl Version: 0.70.40 Summary: External Pyut
 Graphical Shapes Home-page: https://github.com/hasii2011/ogl Author: Humberto
 A. Sanchez II Author-email: Humberto.A.Sanchez.II@gmail.com Maintainer:
 Humberto A. Sanchez II Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown License-File: LICENSE [./developer/
 agpl-license-web-badge-version-2-256x48.png] [![Maintenance](https://
 img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/
 StrapDown.js/graphs/commit-activity) [![CircleCI](https://dl.circleci.com/
```

### Comparing `ogl-0.70.30/README.md` & `ogl-0.70.40/README.md`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/miniogl/AnchorPoint.py` & `ogl-0.70.40/miniogl/AnchorPoint.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/miniogl/AttachmentSide.py` & `ogl-0.70.40/miniogl/AttachmentSide.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/miniogl/Common.py` & `ogl-0.70.40/miniogl/Common.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/miniogl/ControlPoint.py` & `ogl-0.70.40/miniogl/ControlPoint.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/miniogl/Diagram.py` & `ogl-0.70.40/miniogl/Diagram.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/miniogl/DiagramFrame.py` & `ogl-0.70.40/miniogl/DiagramFrame.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/miniogl/DlgDebugDiagramFrame.py` & `ogl-0.70.40/miniogl/DlgDebugDiagramFrame.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/miniogl/LinePoint.py` & `ogl-0.70.40/miniogl/LinePoint.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/miniogl/LineShape.py` & `ogl-0.70.40/miniogl/LineShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/miniogl/LollipopLine.py` & `ogl-0.70.40/miniogl/LollipopLine.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/miniogl/MiniOglColorEnum.py` & `ogl-0.70.40/miniogl/MiniOglColorEnum.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/miniogl/MiniOglPenStyle.py` & `ogl-0.70.40/miniogl/MiniOglPenStyle.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/miniogl/PointShape.py` & `ogl-0.70.40/miniogl/PointShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/miniogl/RectangleShape.py` & `ogl-0.70.40/miniogl/RectangleShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/miniogl/RectangleShapeModel.py` & `ogl-0.70.40/miniogl/RectangleShapeModel.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/miniogl/RotatableShape.py` & `ogl-0.70.40/miniogl/RotatableShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/miniogl/SelectAnchorPoint.py` & `ogl-0.70.40/miniogl/SelectAnchorPoint.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/miniogl/Shape.py` & `ogl-0.70.40/miniogl/Shape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/miniogl/ShapeEventHandler.py` & `ogl-0.70.40/miniogl/ShapeEventHandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
     clsLogger: Logger = getLogger(__name__)
 
     def __init__(self):
         """
         Let a shape receive mouse events directly.
         """
+        pass
+
     def OnLeftDown(self, event: MouseEvent):
         """
         Callback for left clicks.
         Args:
             event:
         """
         ShapeEventHandler.clsLogger.info("Unhandled left down")
```

### Comparing `ogl-0.70.30/miniogl/ShapeModel.py` & `ogl-0.70.40/miniogl/ShapeModel.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/miniogl/SizerShape.py` & `ogl-0.70.40/miniogl/SizerShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/miniogl/TextShape.py` & `ogl-0.70.40/miniogl/TextShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/miniogl/TextShapeModel.py` & `ogl-0.70.40/miniogl/TextShapeModel.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/miniogl/VShapes.py` & `ogl-0.70.40/miniogl/VShapes.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/OglAggregation.py` & `ogl-0.70.40/ogl/OglAggregation.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/OglAssociation.py` & `ogl-0.70.40/ogl/OglAssociation.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/OglClass.py` & `ogl-0.70.40/ogl/OglClass.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/OglComposition.py` & `ogl-0.70.40/ogl/OglComposition.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/OglConstants.py` & `ogl-0.70.40/ogl/OglConstants.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/OglDimensions.py` & `ogl-0.70.40/ogl/OglDimensions.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/OglInheritance.py` & `ogl-0.70.40/ogl/OglInheritance.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/OglInterface.py` & `ogl-0.70.40/ogl/OglInterface.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/OglInterface2.py` & `ogl-0.70.40/ogl/OglInterface2.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/OglLink.py` & `ogl-0.70.40/ogl/OglLink.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/OglLinkFactory.py` & `ogl-0.70.40/ogl/OglLinkFactory.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/OglNote.py` & `ogl-0.70.40/ogl/OglNote.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/OglNoteLink.py` & `ogl-0.70.40/ogl/OglNoteLink.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/OglObject.py` & `ogl-0.70.40/ogl/OglObject.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,15 @@
 
         Args:
             pyutObject: Associated PyutObject
             width:      Initial width
             height:     Initial height
         """
         self._pyutObject = pyutObject
-        RectangleShape.__init__(self, 0, 0, width, height)
-
+        super().__init__(0, 0, width, height)
         # Default font
         self._defaultFont: Font           = Font(DEFAULT_FONT_SIZE, FONTFAMILY_SWISS, FONTSTYLE_NORMAL, FONTWEIGHT_NORMAL)
         self._prefs:       OglPreferences = OglPreferences()
 
         # TODO This is also used by sequence diagrams to store OglSDMessage links
         self._oglLinks: List[OglLink] = []     # Connected links
         self._modifyCommand = None
@@ -177,8 +176,7 @@
         # from org.pyut.ui.Mediator import ACTION_ZOOM_OUT   # avoid circular import
 
         # mediator: Mediator = Mediator()
         # if mediator.getCurrentAction() != ACTION_ZOOM_OUT:
         # TODO:  I took this out because could never cause this to happen;  Conveniently, this removes all mediator calls
         # RectangleShape.SetSelected(self, state)
         self.selected = state
-
```

### Comparing `ogl-0.70.30/ogl/OglText.py` & `ogl-0.70.40/ogl/OglText.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+from typing import List
 from typing import cast
 
 from logging import Logger
 from logging import getLogger
 
 from wx import BLACK_PEN
 from wx import RED_PEN
@@ -20,15 +21,14 @@
 
 from wx import DC
 from wx import Font
 from wx import Menu
 from wx import MenuItem
 from wx import MouseEvent
 
-
 from miniogl.DiagramFrame import DiagramFrame
 
 from ogl.OglObject import OglObject
 from ogl.OglTextFontFamily import OglTextFontFamily
 
 from ogl.OglUtils import OglUtils
 
@@ -83,15 +83,15 @@
         self._textSize:       int  = preferences.textFontSize
         self._isBold:         bool = preferences.textBold
         self._isItalicized:   bool = preferences.textItalicize
 
         self._textFont:  Font            = self._defaultFont.GetBaseFont()
         self._textFont.SetFamily(OglUtils.oglFontFamilyToWxFontFamily(self._textFontFamily))
 
-        self._redColor:   Colour  = ColourDatabase().Find('Red')
+        self._redColor:   Colour = ColourDatabase().Find('Red')
         self._blackColor: Colour = ColourDatabase().Find('Black')
 
         self.__initializeTextDisplay()
         self._menu: Menu = cast(Menu, None)
 
     @property
     def pyutText(self) -> PyutText:
@@ -149,52 +149,49 @@
         if self._menu is None:
             self._menu = self._createMenu()
 
         frame = self._diagram.GetPanel()
 
         x: int = event.GetX()
         y: int = event.GetY()
-        self.logger.debug(f'OglClass - x,y: {x},{y}')
 
         frame.PopupMenu(self._menu, x, y)
 
     def Draw(self, dc: DC, withChildren: bool = False):
         """
         Paint handler, draws the content of the shape.
 
         Args:
             dc:     device context to draw to
             withChildren:   Redraw children or not
         """
         if self._selected:
-            dc.SetPen(RED_PEN)
             dc.SetTextForeground(self._redColor)
-        else:
-            dc.SetPen(BLACK_PEN)
-            dc.SetTextForeground(self._blackColor)
 
-        OglObject.Draw(self, dc)
+        # OglObject.Draw(self, dc)
+        super().Draw(dc)
         dc.SetFont(self._textFont)
 
         w, h = self.GetSize()
 
         baseX, baseY = self.GetPosition()
 
         dc.SetClippingRegion(baseX, baseY, w, h)
 
-        noteContent = self.pyutObject.content
-        lines = OglUtils.lineSplitter(noteContent, dc, w - 2 * OglText.MARGIN)
+        textContent: str       = self.pyutObject.content
+        lines:       List[str] = OglUtils.lineSplitter(textContent, dc, w - 2 * OglText.MARGIN)
 
         x = baseX + OglText.MARGIN
         y = baseY + OglText.MARGIN
 
         for line in range(len(lines)):
             dc.DrawText(lines[line], x, y + line * (dc.GetCharHeight() + 5))
 
         dc.DestroyClippingRegion()
+        dc.SetTextForeground(self._blackColor)      # reset back after done
 
     def _createMenu(self) -> Menu:
 
         menu: Menu = Menu()
 
         increaseItem: MenuItem = menu.Append(ID_MENU_INCREASE_SIZE, 'Increase Size', 'Increase Text Size by 2 points')
         decreaseItem: MenuItem = menu.Append(ID_MENU_DECREASE_SIZE, 'Decrease Size', 'Decrease Text Size by 2 points')
```

### Comparing `ogl-0.70.30/ogl/OglUseCase.py` & `ogl-0.70.40/ogl/OglUseCase.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/OglUtils.py` & `ogl-0.70.40/ogl/OglUtils.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/events/IOglEventEngine.py` & `ogl-0.70.40/ogl/events/IOglEventEngine.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/events/OglEventEngine.py` & `ogl-0.70.40/ogl/events/OglEventEngine.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/events/OglEvents.py` & `ogl-0.70.40/ogl/events/OglEvents.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/preferences/OglPreferences.py` & `ogl-0.70.40/ogl/preferences/OglPreferences.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/resources/img/Display.py` & `ogl-0.70.40/ogl/resources/img/Display.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/resources/img/DoNotDisplay.py` & `ogl-0.70.40/ogl/resources/img/DoNotDisplay.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/resources/img/UnSpecified.py` & `ogl-0.70.40/ogl/resources/img/UnSpecified.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/resources/img/textdetails/DecreaseTextSize.py` & `ogl-0.70.40/ogl/resources/img/textdetails/DecreaseTextSize.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/resources/img/textdetails/IncreaseTextSize.py` & `ogl-0.70.40/ogl/resources/img/textdetails/IncreaseTextSize.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/sd/OglInstanceName.py` & `ogl-0.70.40/ogl/sd/OglInstanceName.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/sd/OglSDInstance.py` & `ogl-0.70.40/ogl/sd/OglSDInstance.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/sd/OglSDMessage.py` & `ogl-0.70.40/ogl/sd/OglSDMessage.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/ui/BaseOglPreferencesPage.py` & `ogl-0.70.40/ogl/ui/BaseOglPreferencesPage.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/ui/DefaultValuesPreferencesPage.py` & `ogl-0.70.40/ogl/ui/DefaultValuesPreferencesPage.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/ui/DiagramPreferencesPage.py` & `ogl-0.70.40/ogl/ui/DiagramPreferencesPage.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/ui/valuecontrols/AssociationAttributesControl.py` & `ogl-0.70.40/ogl/ui/valuecontrols/AssociationAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/ui/valuecontrols/ClassAttributesControl.py` & `ogl-0.70.40/ogl/ui/valuecontrols/ClassAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/ui/valuecontrols/DefaultNamesControl.py` & `ogl-0.70.40/ogl/ui/valuecontrols/DefaultNamesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/ui/valuecontrols/NoteAttributesControl.py` & `ogl-0.70.40/ogl/ui/valuecontrols/NoteAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/ui/valuecontrols/SDAttributesControl.py` & `ogl-0.70.40/ogl/ui/valuecontrols/SDAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl/ui/valuecontrols/TextAttributesControl.py` & `ogl-0.70.40/ogl/ui/valuecontrols/TextAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/ogl.egg-info/PKG-INFO` & `ogl-0.70.40/ogl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogl
-Version: 0.70.30
+Version: 0.70.40
 Summary: External Pyut Graphical Shapes
 Home-page: https://github.com/hasii2011/ogl
 Author: Humberto A. Sanchez II
 Author-email: Humberto.A.Sanchez.II@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ogl Version: 0.70.30 Summary: External Pyut
+Metadata-Version: 2.1 Name: ogl Version: 0.70.40 Summary: External Pyut
 Graphical Shapes Home-page: https://github.com/hasii2011/ogl Author: Humberto
 A. Sanchez II Author-email: Humberto.A.Sanchez.II@gmail.com Maintainer:
 Humberto A. Sanchez II Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown License-File: LICENSE [./developer/
 agpl-license-web-badge-version-2-256x48.png] [![Maintenance](https://
 img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/
 StrapDown.js/graphs/commit-activity) [![CircleCI](https://dl.circleci.com/
```

### Comparing `ogl-0.70.30/ogl.egg-info/SOURCES.txt` & `ogl-0.70.40/ogl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ogl-0.70.30/setup.py` & `ogl-0.70.40/setup.py`

 * *Files identical despite different names*

