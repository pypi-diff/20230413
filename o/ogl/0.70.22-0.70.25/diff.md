# Comparing `tmp/ogl-0.70.22.tar.gz` & `tmp/ogl-0.70.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogl-0.70.22.tar", last modified: Wed Mar 29 23:47:03 2023, max compression
+gzip compressed data, was "ogl-0.70.25.tar", last modified: Thu Apr 13 18:33:29 2023, max compression
```

## Comparing `ogl-0.70.22.tar` & `ogl-0.70.25.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 23:47:03.204453 ogl-0.70.22/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-23 23:19:08.000000 ogl-0.70.22/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1997 2023-03-29 23:47:03.204327 ogl-0.70.22/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1639 2023-01-12 22:09:37.000000 ogl-0.70.22/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 23:47:03.192594 ogl-0.70.22/miniogl/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5038 2023-03-22 20:23:56.000000 ogl-0.70.22/miniogl/AnchorPoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1022 2023-02-21 19:19:18.000000 ogl-0.70.22/miniogl/AttachmentSide.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2916 2022-05-18 20:30:08.000000 ogl-0.70.22/miniogl/Common.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       87 2022-05-18 20:30:08.000000 ogl-0.70.22/miniogl/Constants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1365 2022-05-18 20:30:08.000000 ogl-0.70.22/miniogl/ControlPoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3743 2023-02-11 18:19:50.000000 ogl-0.70.22/miniogl/Diagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    40698 2023-03-25 20:34:07.000000 ogl-0.70.22/miniogl/DiagramFrame.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4713 2023-03-22 20:23:56.000000 ogl-0.70.22/miniogl/DlgDebugDiagramFrame.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1669 2022-05-18 20:30:08.000000 ogl-0.70.22/miniogl/LinePoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13202 2023-03-22 20:23:56.000000 ogl-0.70.22/miniogl/LineShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3594 2023-02-21 21:15:44.000000 ogl-0.70.22/miniogl/LollipopLine.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1747 2023-02-11 19:23:36.000000 ogl-0.70.22/miniogl/MiniOglColorEnum.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1684 2022-05-18 20:30:08.000000 ogl-0.70.22/miniogl/MiniOglPenStyle.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      170 2022-05-18 20:30:08.000000 ogl-0.70.22/miniogl/MiniOglUtils.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2771 2022-05-18 20:30:08.000000 ogl-0.70.22/miniogl/PointShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10735 2023-03-22 20:23:56.000000 ogl-0.70.22/miniogl/RectangleShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1076 2022-05-18 20:30:08.000000 ogl-0.70.22/miniogl/RectangleShapeModel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4772 2022-11-13 14:57:11.000000 ogl-0.70.22/miniogl/RotatableShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2156 2023-03-22 20:23:56.000000 ogl-0.70.22/miniogl/SelectAnchorPoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21669 2023-03-22 20:23:56.000000 ogl-0.70.22/miniogl/Shape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2322 2022-05-18 20:30:08.000000 ogl-0.70.22/miniogl/ShapeEventHandler.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1632 2023-03-22 20:23:56.000000 ogl-0.70.22/miniogl/ShapeModel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1452 2022-05-18 20:30:08.000000 ogl-0.70.22/miniogl/SizerShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7511 2023-03-25 21:42:57.000000 ogl-0.70.22/miniogl/TextShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      649 2022-05-18 20:30:08.000000 ogl-0.70.22/miniogl/TextShapeModel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5650 2022-11-13 14:38:42.000000 ogl-0.70.22/miniogl/VShapes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.22/miniogl/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.22/miniogl/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 23:47:03.197054 ogl-0.70.22/ogl/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      126 2022-05-18 20:30:08.000000 ogl-0.70.22/ogl/IllegalOperationException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3747 2022-06-08 19:34:57.000000 ogl-0.70.22/ogl/OglActor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1463 2022-11-01 13:15:29.000000 ogl-0.70.22/ogl/OglAggregation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12912 2023-03-25 20:34:07.000000 ogl-0.70.22/ogl/OglAssociation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      204 2022-05-18 20:30:08.000000 ogl-0.70.22/ogl/OglAssociationLabel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    20392 2023-03-25 20:34:07.000000 ogl-0.70.22/ogl/OglClass.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1409 2023-03-22 20:23:56.000000 ogl-0.70.22/ogl/OglComposition.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      668 2022-05-18 20:30:08.000000 ogl-0.70.22/ogl/OglConstants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      717 2022-05-18 20:30:08.000000 ogl-0.70.22/ogl/OglDimensions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1460 2023-01-31 22:21:10.000000 ogl-0.70.22/ogl/OglInheritance.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3449 2022-11-01 13:26:22.000000 ogl-0.70.22/ogl/OglInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6199 2023-02-21 19:19:18.000000 ogl-0.70.22/ogl/OglInterface2.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    15577 2023-03-22 20:23:56.000000 ogl-0.70.22/ogl/OglLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3115 2023-03-26 22:27:03.000000 ogl-0.70.22/ogl/OglLinkFactory.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2693 2022-08-28 23:27:21.000000 ogl-0.70.22/ogl/OglNote.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1180 2023-02-19 02:02:00.000000 ogl-0.70.22/ogl/OglNoteLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5511 2023-02-11 18:20:44.000000 ogl-0.70.22/ogl/OglObject.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      473 2022-07-18 19:30:46.000000 ogl-0.70.22/ogl/OglPosition.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8713 2023-03-22 20:23:56.000000 ogl-0.70.22/ogl/OglText.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      226 2022-05-18 20:30:08.000000 ogl-0.70.22/ogl/OglTextFontFamily.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2197 2022-06-08 20:23:03.000000 ogl-0.70.22/ogl/OglUseCase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4349 2022-05-18 20:30:08.000000 ogl-0.70.22/ogl/OglUtils.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.22/ogl/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 23:47:03.198754 ogl-0.70.22/ogl/events/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      543 2023-01-15 21:02:48.000000 ogl-0.70.22/ogl/events/IOglEventEngine.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       52 2022-05-18 20:30:08.000000 ogl-0.70.22/ogl/events/InvalidKeywordException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4566 2023-01-15 21:06:24.000000 ogl-0.70.22/ogl/events/OglEventEngine.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      780 2022-11-14 22:52:55.000000 ogl-0.70.22/ogl/events/OglEvents.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      239 2022-05-18 20:30:08.000000 ogl-0.70.22/ogl/events/ShapeSelectedEventData.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.22/ogl/events/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.22/ogl/events/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 23:47:03.199430 ogl-0.70.22/ogl/preferences/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21283 2023-03-26 21:40:46.000000 ogl-0.70.22/ogl/preferences/OglPreferences.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.22/ogl/preferences/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.22/ogl/preferences/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.22/ogl/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 23:47:03.199533 ogl-0.70.22/ogl/resources/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.22/ogl/resources/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 23:47:03.200177 ogl-0.70.22/ogl/resources/img/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1350 2022-05-18 20:30:08.000000 ogl-0.70.22/ogl/resources/img/Display.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1702 2022-05-18 20:30:08.000000 ogl-0.70.22/ogl/resources/img/DoNotDisplay.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2238 2022-05-18 20:30:08.000000 ogl-0.70.22/ogl/resources/img/UnSpecified.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.22/ogl/resources/img/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.22/ogl/resources/img/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 23:47:03.200668 ogl-0.70.22/ogl/resources/img/textdetails/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1543 2022-05-18 20:30:08.000000 ogl-0.70.22/ogl/resources/img/textdetails/DecreaseTextSize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1575 2022-05-18 20:30:08.000000 ogl-0.70.22/ogl/resources/img/textdetails/IncreaseTextSize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.22/ogl/resources/img/textdetails/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.22/ogl/resources/img/textdetails/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 23:47:03.201533 ogl-0.70.22/ogl/sd/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1212 2022-05-18 20:30:08.000000 ogl-0.70.22/ogl/sd/OglInstanceName.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6876 2023-03-26 01:49:15.000000 ogl-0.70.22/ogl/sd/OglSDInstance.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7333 2023-03-26 01:50:44.000000 ogl-0.70.22/ogl/sd/OglSDMessage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.22/ogl/sd/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.22/ogl/sd/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 23:47:03.202489 ogl-0.70.22/ogl/ui/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      657 2023-02-08 20:22:10.000000 ogl-0.70.22/ogl/ui/BaseOglPreferencesPage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3967 2023-02-19 20:46:44.000000 ogl-0.70.22/ogl/ui/DefaultValuesPreferencesPage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12232 2023-02-19 22:08:38.000000 ogl-0.70.22/ogl/ui/DiagramPreferencesPage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 14:43:49.000000 ogl-0.70.22/ogl/ui/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.22/ogl/ui/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 23:47:03.204176 ogl-0.70.22/ogl/ui/valuecontrols/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2279 2023-02-11 21:29:46.000000 ogl-0.70.22/ogl/ui/valuecontrols/AssociationAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5065 2023-02-11 20:04:09.000000 ogl-0.70.22/ogl/ui/valuecontrols/ClassAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2987 2023-02-11 20:20:38.000000 ogl-0.70.22/ogl/ui/valuecontrols/DefaultNamesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1943 2023-03-26 22:24:15.000000 ogl-0.70.22/ogl/ui/valuecontrols/NoteAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2686 2023-03-26 22:24:31.000000 ogl-0.70.22/ogl/ui/valuecontrols/SDAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4427 2023-02-09 23:51:26.000000 ogl-0.70.22/ogl/ui/valuecontrols/TextAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-09 15:30:26.000000 ogl-0.70.22/ogl/ui/valuecontrols/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 23:47:03.197564 ogl-0.70.22/ogl.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1997 2023-03-29 23:47:03.000000 ogl-0.70.22/ogl.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2500 2023-03-29 23:47:03.000000 ogl-0.70.22/ogl.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-03-29 23:47:03.000000 ogl-0.70.22/ogl.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       90 2023-03-29 23:47:03.000000 ogl-0.70.22/ogl.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-03-29 23:47:03.000000 ogl-0.70.22/ogl.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-03-29 23:47:03.204486 ogl-0.70.22/setup.cfg
--rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)     1519 2023-03-29 23:46:02.000000 ogl-0.70.22/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:33:29.337686 ogl-0.70.25/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-23 23:19:08.000000 ogl-0.70.25/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2357 2023-04-13 18:33:29.337553 ogl-0.70.25/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1999 2023-04-12 19:50:00.000000 ogl-0.70.25/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:33:29.329224 ogl-0.70.25/miniogl/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5038 2023-03-22 20:23:56.000000 ogl-0.70.25/miniogl/AnchorPoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1022 2023-02-21 19:19:18.000000 ogl-0.70.25/miniogl/AttachmentSide.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2916 2022-05-18 20:30:08.000000 ogl-0.70.25/miniogl/Common.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       87 2022-05-18 20:30:08.000000 ogl-0.70.25/miniogl/Constants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1365 2022-05-18 20:30:08.000000 ogl-0.70.25/miniogl/ControlPoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3743 2023-02-11 18:19:50.000000 ogl-0.70.25/miniogl/Diagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    40698 2023-03-25 20:34:07.000000 ogl-0.70.25/miniogl/DiagramFrame.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4713 2023-03-22 20:23:56.000000 ogl-0.70.25/miniogl/DlgDebugDiagramFrame.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1669 2022-05-18 20:30:08.000000 ogl-0.70.25/miniogl/LinePoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13202 2023-03-22 20:23:56.000000 ogl-0.70.25/miniogl/LineShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3594 2023-02-21 21:15:44.000000 ogl-0.70.25/miniogl/LollipopLine.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1747 2023-02-11 19:23:36.000000 ogl-0.70.25/miniogl/MiniOglColorEnum.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1684 2022-05-18 20:30:08.000000 ogl-0.70.25/miniogl/MiniOglPenStyle.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      170 2022-05-18 20:30:08.000000 ogl-0.70.25/miniogl/MiniOglUtils.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2771 2022-05-18 20:30:08.000000 ogl-0.70.25/miniogl/PointShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10735 2023-03-22 20:23:56.000000 ogl-0.70.25/miniogl/RectangleShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1076 2022-05-18 20:30:08.000000 ogl-0.70.25/miniogl/RectangleShapeModel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4772 2022-11-13 14:57:11.000000 ogl-0.70.25/miniogl/RotatableShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2156 2023-03-22 20:23:56.000000 ogl-0.70.25/miniogl/SelectAnchorPoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21669 2023-03-22 20:23:56.000000 ogl-0.70.25/miniogl/Shape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2322 2022-05-18 20:30:08.000000 ogl-0.70.25/miniogl/ShapeEventHandler.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1632 2023-03-22 20:23:56.000000 ogl-0.70.25/miniogl/ShapeModel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1452 2022-05-18 20:30:08.000000 ogl-0.70.25/miniogl/SizerShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7511 2023-03-25 21:42:57.000000 ogl-0.70.25/miniogl/TextShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      649 2022-05-18 20:30:08.000000 ogl-0.70.25/miniogl/TextShapeModel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5650 2022-11-13 14:38:42.000000 ogl-0.70.25/miniogl/VShapes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.25/miniogl/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.25/miniogl/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:33:29.332097 ogl-0.70.25/ogl/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      126 2022-05-18 20:30:08.000000 ogl-0.70.25/ogl/IllegalOperationException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3747 2022-06-08 19:34:57.000000 ogl-0.70.25/ogl/OglActor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1463 2022-11-01 13:15:29.000000 ogl-0.70.25/ogl/OglAggregation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12912 2023-03-25 20:34:07.000000 ogl-0.70.25/ogl/OglAssociation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      204 2022-05-18 20:30:08.000000 ogl-0.70.25/ogl/OglAssociationLabel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    20392 2023-03-25 20:34:07.000000 ogl-0.70.25/ogl/OglClass.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1409 2023-03-22 20:23:56.000000 ogl-0.70.25/ogl/OglComposition.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      668 2022-05-18 20:30:08.000000 ogl-0.70.25/ogl/OglConstants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      717 2022-05-18 20:30:08.000000 ogl-0.70.25/ogl/OglDimensions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1460 2023-01-31 22:21:10.000000 ogl-0.70.25/ogl/OglInheritance.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3541 2023-03-31 00:59:54.000000 ogl-0.70.25/ogl/OglInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6199 2023-02-21 19:19:18.000000 ogl-0.70.25/ogl/OglInterface2.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    15577 2023-03-22 20:23:56.000000 ogl-0.70.25/ogl/OglLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3115 2023-03-26 22:27:03.000000 ogl-0.70.25/ogl/OglLinkFactory.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2693 2022-08-28 23:27:21.000000 ogl-0.70.25/ogl/OglNote.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1180 2023-02-19 02:02:00.000000 ogl-0.70.25/ogl/OglNoteLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5511 2023-02-11 18:20:44.000000 ogl-0.70.25/ogl/OglObject.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      473 2022-07-18 19:30:46.000000 ogl-0.70.25/ogl/OglPosition.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8713 2023-03-22 20:23:56.000000 ogl-0.70.25/ogl/OglText.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      226 2022-05-18 20:30:08.000000 ogl-0.70.25/ogl/OglTextFontFamily.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2197 2022-06-08 20:23:03.000000 ogl-0.70.25/ogl/OglUseCase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4349 2022-05-18 20:30:08.000000 ogl-0.70.25/ogl/OglUtils.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.25/ogl/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:33:29.333786 ogl-0.70.25/ogl/events/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      543 2023-01-15 21:02:48.000000 ogl-0.70.25/ogl/events/IOglEventEngine.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       52 2022-05-18 20:30:08.000000 ogl-0.70.25/ogl/events/InvalidKeywordException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4566 2023-01-15 21:06:24.000000 ogl-0.70.25/ogl/events/OglEventEngine.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      780 2022-11-14 22:52:55.000000 ogl-0.70.25/ogl/events/OglEvents.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      239 2022-05-18 20:30:08.000000 ogl-0.70.25/ogl/events/ShapeSelectedEventData.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.25/ogl/events/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.25/ogl/events/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:33:29.334174 ogl-0.70.25/ogl/preferences/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21283 2023-03-26 21:40:46.000000 ogl-0.70.25/ogl/preferences/OglPreferences.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.25/ogl/preferences/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.25/ogl/preferences/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.25/ogl/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:33:29.334294 ogl-0.70.25/ogl/resources/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.25/ogl/resources/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:33:29.334946 ogl-0.70.25/ogl/resources/img/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1350 2022-05-18 20:30:08.000000 ogl-0.70.25/ogl/resources/img/Display.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1702 2022-05-18 20:30:08.000000 ogl-0.70.25/ogl/resources/img/DoNotDisplay.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2238 2022-05-18 20:30:08.000000 ogl-0.70.25/ogl/resources/img/UnSpecified.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.25/ogl/resources/img/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.25/ogl/resources/img/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:33:29.335456 ogl-0.70.25/ogl/resources/img/textdetails/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1543 2022-05-18 20:30:08.000000 ogl-0.70.25/ogl/resources/img/textdetails/DecreaseTextSize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1575 2022-05-18 20:30:08.000000 ogl-0.70.25/ogl/resources/img/textdetails/IncreaseTextSize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.25/ogl/resources/img/textdetails/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.25/ogl/resources/img/textdetails/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:33:29.336063 ogl-0.70.25/ogl/sd/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1212 2022-05-18 20:30:08.000000 ogl-0.70.25/ogl/sd/OglInstanceName.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6876 2023-03-26 01:49:15.000000 ogl-0.70.25/ogl/sd/OglSDInstance.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7333 2023-03-26 01:50:44.000000 ogl-0.70.25/ogl/sd/OglSDMessage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.25/ogl/sd/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.25/ogl/sd/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:33:29.336606 ogl-0.70.25/ogl/ui/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      657 2023-02-08 20:22:10.000000 ogl-0.70.25/ogl/ui/BaseOglPreferencesPage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3967 2023-02-19 20:46:44.000000 ogl-0.70.25/ogl/ui/DefaultValuesPreferencesPage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12232 2023-02-19 22:08:38.000000 ogl-0.70.25/ogl/ui/DiagramPreferencesPage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 14:43:49.000000 ogl-0.70.25/ogl/ui/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.25/ogl/ui/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:33:29.337377 ogl-0.70.25/ogl/ui/valuecontrols/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2279 2023-02-11 21:29:46.000000 ogl-0.70.25/ogl/ui/valuecontrols/AssociationAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5065 2023-02-11 20:04:09.000000 ogl-0.70.25/ogl/ui/valuecontrols/ClassAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2987 2023-02-11 20:20:38.000000 ogl-0.70.25/ogl/ui/valuecontrols/DefaultNamesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1943 2023-03-26 22:24:15.000000 ogl-0.70.25/ogl/ui/valuecontrols/NoteAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2686 2023-03-26 22:24:31.000000 ogl-0.70.25/ogl/ui/valuecontrols/SDAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4427 2023-02-09 23:51:26.000000 ogl-0.70.25/ogl/ui/valuecontrols/TextAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-09 15:30:26.000000 ogl-0.70.25/ogl/ui/valuecontrols/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:33:29.332908 ogl-0.70.25/ogl.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2357 2023-04-13 18:33:29.000000 ogl-0.70.25/ogl.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2500 2023-04-13 18:33:29.000000 ogl-0.70.25/ogl.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-04-13 18:33:29.000000 ogl-0.70.25/ogl.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       90 2023-04-13 18:33:29.000000 ogl-0.70.25/ogl.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-04-13 18:33:29.000000 ogl-0.70.25/ogl.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-04-13 18:33:29.337719 ogl-0.70.25/setup.cfg
+-rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)     1519 2023-04-13 18:31:22.000000 ogl-0.70.25/setup.py
```

### Comparing `ogl-0.70.22/LICENSE` & `ogl-0.70.25/LICENSE`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/PKG-INFO` & `ogl-0.70.25/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6f67 6c0a  : 2.1.Name: ogl.
-00000020: 5665 7273 696f 6e3a 2030 2e37 302e 3232  Version: 0.70.22
+00000020: 5665 7273 696f 6e3a 2030 2e37 302e 3235  Version: 0.70.25
 00000030: 0a53 756d 6d61 7279 3a20 4578 7465 726e  .Summary: Extern
 00000040: 616c 2050 7975 7420 4772 6170 6869 6361  al Pyut Graphica
 00000050: 6c20 5368 6170 6573 0a48 6f6d 652d 7061  l Shapes.Home-pa
 00000060: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
 00000070: 7562 2e63 6f6d 2f68 6173 6969 3230 3131  ub.com/hasii2011
 00000080: 2f6f 676c 0a41 7574 686f 723a 2048 756d  /ogl.Author: Hum
 00000090: 6265 7274 6f20 412e 2053 616e 6368 657a  berto A. Sanchez
@@ -65,61 +65,84 @@
 00000400: 6573 206d 6f64 756c 6520 666f 7220 5079  es module for Py
 00000410: 7574 0a74 6861 7420 616c 6c6f 7773 2066  ut.that allows f
 00000420: 6f72 2065 7874 6572 6e61 6c20 706c 7567  or external plug
 00000430: 696e 2064 6576 656c 6f70 6d65 6e74 3b0a  in development;.
 00000440: 0a54 6869 7320 7072 6f6a 6563 7420 6465  .This project de
 00000450: 7065 6e64 7320 6f6e 2070 7975 746d 6f64  pends on pyutmod
 00000460: 656c 2061 6e64 2077 7850 7974 686f 6e0a  el and wxPython.
-00000470: 0a0a 2d2d 2d2d 2d2d 0a0a 0a21 5b48 756d  ..------...![Hum
-00000480: 6265 7274 6f27 7320 4d6f 6469 6669 6564  berto's Modified
-00000490: 204c 6f67 6f5d 2868 7474 7073 3a2f 2f72   Logo](https://r
-000004a0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-000004b0: 7465 6e74 2e63 6f6d 2f77 696b 692f 6861  tent.com/wiki/ha
-000004c0: 7369 6932 3031 312f 6769 7474 6f64 6f69  sii2011/gittodoi
-000004d0: 7374 636c 6f6e 652f 696d 6167 6573 2f53  stclone/images/S
-000004e0: 696c 6c79 4769 7448 7562 2e70 6e67 290a  illyGitHub.png).
-000004f0: 0a49 2061 6d20 636f 6e63 6572 6e65 6420  .I am concerned 
-00000500: 6162 6f75 7420 4769 7448 7562 2773 2043  about GitHub's C
-00000510: 6f70 696c 6f74 2070 726f 6a65 6374 0a0a  opilot project..
-00000520: 0a0a 4920 7572 6765 2079 6f75 2074 6f20  ..I urge you to 
-00000530: 7265 6164 2061 626f 7574 2074 6865 0a5b  read about the.[
-00000540: 4769 7665 2075 7020 4769 7448 7562 5d28  Give up GitHub](
-00000550: 6874 7470 733a 2f2f 4769 7665 5570 4769  https://GiveUpGi
-00000560: 7448 7562 2e6f 7267 2920 6361 6d70 6169  tHub.org) campai
-00000570: 676e 2066 726f 6d0a 5b74 6865 2053 6f66  gn from.[the Sof
-00000580: 7477 6172 6520 4672 6565 646f 6d20 436f  tware Freedom Co
-00000590: 6e73 6572 7661 6e63 795d 2868 7474 7073  nservancy](https
-000005a0: 3a2f 2f73 6663 6f6e 7365 7276 616e 6379  ://sfconservancy
-000005b0: 2e6f 7267 292e 0a0a 5768 696c 6520 4920  .org)...While I 
-000005c0: 646f 206e 6f74 2061 6476 6f63 6174 6520  do not advocate 
-000005d0: 666f 7220 616c 6c20 7468 6520 6973 7375  for all the issu
-000005e0: 6573 206c 6973 7465 6420 7468 6572 6520  es listed there 
-000005f0: 4920 646f 206e 6f74 206c 696b 6520 7468  I do not like th
-00000600: 6174 0a61 2063 6f6d 7061 6e79 206c 696b  at.a company lik
-00000610: 6520 4d69 6372 6f73 6f66 7420 6d61 7920  e Microsoft may 
-00000620: 7072 6f66 6974 2066 726f 6d20 6f70 656e  profit from open
-00000630: 2073 6f75 7263 6520 7072 6f6a 6563 7473   source projects
-00000640: 2e0a 0a49 2063 6f6e 7469 6e75 6520 746f  ...I continue to
-00000650: 2075 7365 2047 6974 4875 6220 6265 6361   use GitHub beca
-00000660: 7573 6520 6974 206f 6666 6572 7320 7468  use it offers th
-00000670: 6520 7365 7276 6963 6573 2049 206e 6565  e services I nee
-00000680: 6420 666f 7220 6672 6565 2e20 2042 7574  d for free.  But
-00000690: 2c20 4920 636f 6e74 696e 7565 0a74 6f20  , I continue.to 
-000006a0: 6d6f 6e69 746f 7220 7468 6569 7220 7465  monitor their te
-000006b0: 726d 7320 6f66 2073 6572 7669 6365 2e0a  rms of service..
-000006c0: 0a41 6e79 2075 7365 206f 6620 7468 6973  .Any use of this
-000006d0: 2070 726f 6a65 6374 2773 2063 6f64 6520   project's code 
-000006e0: 6279 2047 6974 4875 6220 436f 7069 6c6f  by GitHub Copilo
-000006f0: 742c 2070 6173 7420 6f72 2070 7265 7365  t, past or prese
-00000700: 6e74 2c20 6973 2064 6f6e 650a 7769 7468  nt, is done.with
-00000710: 6f75 7420 6d79 2070 6572 6d69 7373 696f  out my permissio
-00000720: 6e2e 2020 4920 646f 206e 6f74 2063 6f6e  n.  I do not con
-00000730: 7365 6e74 2074 6f20 4769 7448 7562 2773  sent to GitHub's
-00000740: 2075 7365 206f 6620 7468 6973 2070 726f   use of this pro
-00000750: 6a65 6374 2773 0a63 6f64 6520 696e 2043  ject's.code in C
-00000760: 6f70 696c 6f74 2e0a 0a41 2072 6570 6f73  opilot...A repos
-00000770: 6974 6f72 7920 6f77 6e65 7220 6d61 7920  itory owner may 
-00000780: 6f70 7420 6f75 7420 6f66 2043 6f70 696c  opt out of Copil
-00000790: 6f74 2062 7920 6368 616e 6769 6e67 2053  ot by changing S
-000007a0: 6574 7469 6e67 7320 2d2d 3e20 4769 7448  ettings --> GitH
-000007b0: 7562 2043 6f70 696c 6f74 2e0a 0a49 2068  ub Copilot...I h
-000007c0: 6176 6520 646f 6e65 2073 6f2e 0a         ave done so..
+00000470: 0a5f 5f5f 0a0a 2323 2044 6576 656c 6f70  .___..## Develop
+00000480: 6572 204e 6f74 6573 0a54 6869 7320 7072  er Notes.This pr
+00000490: 6f6a 6563 7420 7573 6573 205b 6275 696c  oject uses [buil
+000004a0: 646c 6163 6b65 795d 2868 7474 7073 3a2f  dlackey](https:/
+000004b0: 2f67 6974 6875 622e 636f 6d2f 6861 7369  /github.com/hasi
+000004c0: 6932 3031 312f 6275 696c 646c 6163 6b65  i2011/buildlacke
+000004d0: 7929 2066 6f72 2064 6179 2074 6f20 6461  y) for day to da
+000004e0: 7920 6465 7665 6c6f 706d 656e 7420 6275  y development bu
+000004f0: 696c 6473 0a0a 5f5f 5f0a 0a57 7269 7474  ilds..___..Writt
+00000500: 656e 2062 7920 3c61 2068 7265 663d 226d  en by <a href="m
+00000510: 6169 6c74 6f3a 656d 6169 6c40 6875 6d62  ailto:email@humb
+00000520: 6572 746f 2e61 2e73 616e 6368 657a 2e69  erto.a.sanchez.i
+00000530: 6940 676d 6169 6c2e 636f 6d3f 7375 626a  i@gmail.com?subj
+00000540: 6563 743d 4865 6c6c 6f20 4875 6d62 6572  ect=Hello Humber
+00000550: 746f 223e 4875 6d62 6572 746f 2041 2e20  to">Humberto A. 
+00000560: 5361 6e63 6865 7a20 4949 3c2f 613e 2020  Sanchez II</a>  
+00000570: 2843 2920 3230 3233 0a0a 2323 204e 6f74  (C) 2023..## Not
+00000580: 650a 466f 7220 616c 6c20 6b69 6e64 206f  e.For all kind o
+00000590: 6620 7072 6f62 6c65 6d73 2c20 7265 7175  f problems, requ
+000005a0: 6573 7473 2c20 656e 6861 6e63 656d 656e  ests, enhancemen
+000005b0: 7473 2c20 6275 6720 7265 706f 7274 732c  ts, bug reports,
+000005c0: 2065 7463 2e2c 0a70 6c65 6173 6520 6472   etc.,.please dr
+000005d0: 6f70 206d 6520 616e 2065 2d6d 6169 6c2e  op me an e-mail.
+000005e0: 0a0a 0a21 5b48 756d 6265 7274 6f27 7320  ...![Humberto's 
+000005f0: 4d6f 6469 6669 6564 204c 6f67 6f5d 2868  Modified Logo](h
+00000600: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00000610: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00000620: 2f77 696b 692f 6861 7369 6932 3031 312f  /wiki/hasii2011/
+00000630: 6769 7474 6f64 6f69 7374 636c 6f6e 652f  gittodoistclone/
+00000640: 696d 6167 6573 2f53 696c 6c79 4769 7448  images/SillyGitH
+00000650: 7562 2e70 6e67 290a 0a49 2061 6d20 636f  ub.png)..I am co
+00000660: 6e63 6572 6e65 6420 6162 6f75 7420 4769  ncerned about Gi
+00000670: 7448 7562 2773 2043 6f70 696c 6f74 2070  tHub's Copilot p
+00000680: 726f 6a65 6374 0a0a 0a0a 4920 7572 6765  roject....I urge
+00000690: 2079 6f75 2074 6f20 7265 6164 2061 626f   you to read abo
+000006a0: 7574 2074 6865 205b 4769 7665 2075 7020  ut the [Give up 
+000006b0: 4769 7448 7562 5d28 6874 7470 733a 2f2f  GitHub](https://
+000006c0: 4769 7665 5570 4769 7448 7562 2e6f 7267  GiveUpGitHub.org
+000006d0: 2920 6361 6d70 6169 676e 2066 726f 6d20  ) campaign from 
+000006e0: 5b74 6865 2053 6f66 7477 6172 6520 4672  [the Software Fr
+000006f0: 6565 646f 6d20 436f 6e73 6572 7661 6e63  eedom Conservanc
+00000700: 795d 2868 7474 7073 3a2f 2f73 6663 6f6e  y](https://sfcon
+00000710: 7365 7276 616e 6379 2e6f 7267 292e 0a0a  servancy.org)...
+00000720: 5768 696c 6520 4920 646f 206e 6f74 2061  While I do not a
+00000730: 6476 6f63 6174 6520 666f 7220 616c 6c20  dvocate for all 
+00000740: 7468 6520 6973 7375 6573 206c 6973 7465  the issues liste
+00000750: 6420 7468 6572 6520 4920 646f 206e 6f74  d there I do not
+00000760: 206c 696b 6520 7468 6174 2061 2063 6f6d   like that a com
+00000770: 7061 6e79 206c 696b 6520 4d69 6372 6f73  pany like Micros
+00000780: 6f66 7420 6d61 7920 7072 6f66 6974 2066  oft may profit f
+00000790: 726f 6d20 6f70 656e 2073 6f75 7263 6520  rom open source 
+000007a0: 7072 6f6a 6563 7473 2e0a 0a49 2063 6f6e  projects...I con
+000007b0: 7469 6e75 6520 746f 2075 7365 2047 6974  tinue to use Git
+000007c0: 4875 6220 6265 6361 7573 6520 6974 206f  Hub because it o
+000007d0: 6666 6572 7320 7468 6520 7365 7276 6963  ffers the servic
+000007e0: 6573 2049 206e 6565 6420 666f 7220 6672  es I need for fr
+000007f0: 6565 2e20 2042 7574 2c20 4920 636f 6e74  ee.  But, I cont
+00000800: 696e 7565 2074 6f20 6d6f 6e69 746f 7220  inue to monitor 
+00000810: 7468 6569 7220 7465 726d 7320 6f66 2073  their terms of s
+00000820: 6572 7669 6365 2e0a 0a41 6e79 2075 7365  ervice...Any use
+00000830: 206f 6620 7468 6973 2070 726f 6a65 6374   of this project
+00000840: 2773 2063 6f64 6520 6279 2047 6974 4875  's code by GitHu
+00000850: 6220 436f 7069 6c6f 742c 2070 6173 7420  b Copilot, past 
+00000860: 6f72 2070 7265 7365 6e74 2c20 6973 2064  or present, is d
+00000870: 6f6e 6520 7769 7468 6f75 7420 6d79 2070  one without my p
+00000880: 6572 6d69 7373 696f 6e2e 2020 4920 646f  ermission.  I do
+00000890: 206e 6f74 2063 6f6e 7365 6e74 2074 6f20   not consent to 
+000008a0: 4769 7448 7562 2773 2075 7365 206f 6620  GitHub's use of 
+000008b0: 7468 6973 2070 726f 6a65 6374 2773 0a63  this project's.c
+000008c0: 6f64 6520 696e 2043 6f70 696c 6f74 2e0a  ode in Copilot..
+000008d0: 0a41 2072 6570 6f73 6974 6f72 7920 6f77  .A repository ow
+000008e0: 6e65 7220 6d61 7920 6f70 7420 6f75 7420  ner may opt out 
+000008f0: 6f66 2043 6f70 696c 6f74 2062 7920 6368  of Copilot by ch
+00000900: 616e 6769 6e67 2053 6574 7469 6e67 7320  anging Settings 
+00000910: 2d2d 3e20 4769 7448 7562 2043 6f70 696c  --> GitHub Copil
+00000920: 6f74 2e0a 0a49 2068 6176 6520 646f 6e65  ot...I have done
+00000930: 2073 6f2e 0a                              so..
```

### Comparing `ogl-0.70.22/README.md` & `ogl-0.70.25/ogl.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,103 +1,148 @@
-00000000: 3c69 6d67 2073 7263 3d22 2e2f 6465 7665  <img src="./deve
-00000010: 6c6f 7065 722f 6167 706c 2d6c 6963 656e  loper/agpl-licen
-00000020: 7365 2d77 6562 2d62 6164 6765 2d76 6572  se-web-badge-ver
-00000030: 7369 6f6e 2d32 2d32 3536 7834 382e 706e  sion-2-256x48.pn
-00000040: 6722 2f3e 200a 0a5b 215b 4d61 696e 7465  g"/> ..[![Mainte
-00000050: 6e61 6e63 655d 2868 7474 7073 3a2f 2f69  nance](https://i
-00000060: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-00000070: 6467 652f 4d61 696e 7461 696e 6564 2533  dge/Maintained%3
-00000080: 462d 7965 732d 6772 6565 6e2e 7376 6729  F-yes-green.svg)
-00000090: 5d28 6874 7470 733a 2f2f 4769 7448 7562  ](https://GitHub
-000000a0: 2e63 6f6d 2f4e 6165 7265 656e 2f53 7472  .com/Naereen/Str
-000000b0: 6170 446f 776e 2e6a 732f 6772 6170 6873  apDown.js/graphs
-000000c0: 2f63 6f6d 6d69 742d 6163 7469 7669 7479  /commit-activity
-000000d0: 290a 5b21 5b43 6972 636c 6543 495d 2868  ).[![CircleCI](h
-000000e0: 7474 7073 3a2f 2f64 6c2e 6369 7263 6c65  ttps://dl.circle
-000000f0: 6369 2e63 6f6d 2f73 7461 7475 732d 6261  ci.com/status-ba
-00000100: 6467 652f 696d 672f 6768 2f68 6173 6969  dge/img/gh/hasii
-00000110: 3230 3131 2f6f 676c 2f74 7265 652f 6d61  2011/ogl/tree/ma
-00000120: 7374 6572 2e73 7667 3f73 7479 6c65 3d73  ster.svg?style=s
-00000130: 6869 656c 6429 5d28 6874 7470 733a 2f2f  hield)](https://
-00000140: 646c 2e63 6972 636c 6563 692e 636f 6d2f  dl.circleci.com/
-00000150: 7374 6174 7573 2d62 6164 6765 2f72 6564  status-badge/red
-00000160: 6972 6563 742f 6768 2f68 6173 6969 3230  irect/gh/hasii20
-00000170: 3131 2f6f 676c 2f74 7265 652f 6d61 7374  11/ogl/tree/mast
-00000180: 6572 290a 5b21 5b6d 6163 4f53 5d28 6874  er).[![macOS](ht
-00000190: 7470 733a 2f2f 7376 6773 6861 7265 2e63  tps://svgshare.c
-000001a0: 6f6d 2f69 2f5a 6a50 2e73 7667 295d 2868  om/i/ZjP.svg)](h
-000001b0: 7474 7073 3a2f 2f73 7667 7368 6172 652e  ttps://svgshare.
-000001c0: 636f 6d2f 692f 5a6a 502e 7376 6729 0a0a  com/i/ZjP.svg)..
-000001d0: 5b21 5b66 6f72 7468 6562 6164 6765 206d  [![forthebadge m
-000001e0: 6164 652d 7769 7468 2d70 7974 686f 6e5d  ade-with-python]
-000001f0: 2868 7474 703a 2f2f 466f 7254 6865 4261  (http://ForTheBa
-00000200: 6467 652e 636f 6d2f 696d 6167 6573 2f62  dge.com/images/b
-00000210: 6164 6765 732f 6d61 6465 2d77 6974 682d  adges/made-with-
-00000220: 7079 7468 6f6e 2e73 7667 295d 2868 7474  python.svg)](htt
-00000230: 7073 3a2f 2f77 7777 2e70 7974 686f 6e2e  ps://www.python.
-00000240: 6f72 672f 290a 0af0 9d93 9f20 f09d 93a8  org/)...... ....
-00000250: 20f0 9d93 a420 f09d 93a3 2073 7461 6e64   .... .... stand
-00000260: 7320 666f 7220 5079 7468 6f6e 2055 4d4c  s for Python UML
-00000270: 2054 6f6f 6c2e 2054 6869 7320 6973 2074   Tool. This is t
-00000280: 6865 2065 7874 6572 6e61 6c20 6772 6170  he external grap
-00000290: 6869 6361 6c20 7368 6170 6573 206d 6f64  hical shapes mod
-000002a0: 756c 6520 666f 7220 5079 7574 0a74 6861  ule for Pyut.tha
-000002b0: 7420 616c 6c6f 7773 2066 6f72 2065 7874  t allows for ext
-000002c0: 6572 6e61 6c20 706c 7567 696e 2064 6576  ernal plugin dev
-000002d0: 656c 6f70 6d65 6e74 3b0a 0a54 6869 7320  elopment;..This 
-000002e0: 7072 6f6a 6563 7420 6465 7065 6e64 7320  project depends 
-000002f0: 6f6e 2070 7975 746d 6f64 656c 2061 6e64  on pyutmodel and
-00000300: 2077 7850 7974 686f 6e0a 0a0a 2d2d 2d2d   wxPython...----
-00000310: 2d2d 0a0a 0a21 5b48 756d 6265 7274 6f27  --...![Humberto'
-00000320: 7320 4d6f 6469 6669 6564 204c 6f67 6f5d  s Modified Logo]
-00000330: 2868 7474 7073 3a2f 2f72 6177 2e67 6974  (https://raw.git
-00000340: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00000350: 6f6d 2f77 696b 692f 6861 7369 6932 3031  om/wiki/hasii201
-00000360: 312f 6769 7474 6f64 6f69 7374 636c 6f6e  1/gittodoistclon
-00000370: 652f 696d 6167 6573 2f53 696c 6c79 4769  e/images/SillyGi
-00000380: 7448 7562 2e70 6e67 290a 0a49 2061 6d20  tHub.png)..I am 
-00000390: 636f 6e63 6572 6e65 6420 6162 6f75 7420  concerned about 
-000003a0: 4769 7448 7562 2773 2043 6f70 696c 6f74  GitHub's Copilot
-000003b0: 2070 726f 6a65 6374 0a0a 0a0a 4920 7572   project....I ur
-000003c0: 6765 2079 6f75 2074 6f20 7265 6164 2061  ge you to read a
-000003d0: 626f 7574 2074 6865 0a5b 4769 7665 2075  bout the.[Give u
-000003e0: 7020 4769 7448 7562 5d28 6874 7470 733a  p GitHub](https:
-000003f0: 2f2f 4769 7665 5570 4769 7448 7562 2e6f  //GiveUpGitHub.o
-00000400: 7267 2920 6361 6d70 6169 676e 2066 726f  rg) campaign fro
-00000410: 6d0a 5b74 6865 2053 6f66 7477 6172 6520  m.[the Software 
-00000420: 4672 6565 646f 6d20 436f 6e73 6572 7661  Freedom Conserva
-00000430: 6e63 795d 2868 7474 7073 3a2f 2f73 6663  ncy](https://sfc
-00000440: 6f6e 7365 7276 616e 6379 2e6f 7267 292e  onservancy.org).
-00000450: 0a0a 5768 696c 6520 4920 646f 206e 6f74  ..While I do not
-00000460: 2061 6476 6f63 6174 6520 666f 7220 616c   advocate for al
-00000470: 6c20 7468 6520 6973 7375 6573 206c 6973  l the issues lis
-00000480: 7465 6420 7468 6572 6520 4920 646f 206e  ted there I do n
-00000490: 6f74 206c 696b 6520 7468 6174 0a61 2063  ot like that.a c
-000004a0: 6f6d 7061 6e79 206c 696b 6520 4d69 6372  ompany like Micr
-000004b0: 6f73 6f66 7420 6d61 7920 7072 6f66 6974  osoft may profit
-000004c0: 2066 726f 6d20 6f70 656e 2073 6f75 7263   from open sourc
-000004d0: 6520 7072 6f6a 6563 7473 2e0a 0a49 2063  e projects...I c
-000004e0: 6f6e 7469 6e75 6520 746f 2075 7365 2047  ontinue to use G
-000004f0: 6974 4875 6220 6265 6361 7573 6520 6974  itHub because it
-00000500: 206f 6666 6572 7320 7468 6520 7365 7276   offers the serv
-00000510: 6963 6573 2049 206e 6565 6420 666f 7220  ices I need for 
-00000520: 6672 6565 2e20 2042 7574 2c20 4920 636f  free.  But, I co
-00000530: 6e74 696e 7565 0a74 6f20 6d6f 6e69 746f  ntinue.to monito
-00000540: 7220 7468 6569 7220 7465 726d 7320 6f66  r their terms of
-00000550: 2073 6572 7669 6365 2e0a 0a41 6e79 2075   service...Any u
-00000560: 7365 206f 6620 7468 6973 2070 726f 6a65  se of this proje
-00000570: 6374 2773 2063 6f64 6520 6279 2047 6974  ct's code by Git
-00000580: 4875 6220 436f 7069 6c6f 742c 2070 6173  Hub Copilot, pas
-00000590: 7420 6f72 2070 7265 7365 6e74 2c20 6973  t or present, is
-000005a0: 2064 6f6e 650a 7769 7468 6f75 7420 6d79   done.without my
-000005b0: 2070 6572 6d69 7373 696f 6e2e 2020 4920   permission.  I 
-000005c0: 646f 206e 6f74 2063 6f6e 7365 6e74 2074  do not consent t
-000005d0: 6f20 4769 7448 7562 2773 2075 7365 206f  o GitHub's use o
-000005e0: 6620 7468 6973 2070 726f 6a65 6374 2773  f this project's
-000005f0: 0a63 6f64 6520 696e 2043 6f70 696c 6f74  .code in Copilot
-00000600: 2e0a 0a41 2072 6570 6f73 6974 6f72 7920  ...A repository 
-00000610: 6f77 6e65 7220 6d61 7920 6f70 7420 6f75  owner may opt ou
-00000620: 7420 6f66 2043 6f70 696c 6f74 2062 7920  t of Copilot by 
-00000630: 6368 616e 6769 6e67 2053 6574 7469 6e67  changing Setting
-00000640: 7320 2d2d 3e20 4769 7448 7562 2043 6f70  s --> GitHub Cop
-00000650: 696c 6f74 2e0a 0a49 2068 6176 6520 646f  ilot...I have do
-00000660: 6e65 2073 6f2e 0a                        ne so..
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6f67 6c0a  : 2.1.Name: ogl.
+00000020: 5665 7273 696f 6e3a 2030 2e37 302e 3235  Version: 0.70.25
+00000030: 0a53 756d 6d61 7279 3a20 4578 7465 726e  .Summary: Extern
+00000040: 616c 2050 7975 7420 4772 6170 6869 6361  al Pyut Graphica
+00000050: 6c20 5368 6170 6573 0a48 6f6d 652d 7061  l Shapes.Home-pa
+00000060: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
+00000070: 7562 2e63 6f6d 2f68 6173 6969 3230 3131  ub.com/hasii2011
+00000080: 2f6f 676c 0a41 7574 686f 723a 2048 756d  /ogl.Author: Hum
+00000090: 6265 7274 6f20 412e 2053 616e 6368 657a  berto A. Sanchez
+000000a0: 2049 490a 4175 7468 6f72 2d65 6d61 696c   II.Author-email
+000000b0: 3a20 4875 6d62 6572 746f 2e41 2e53 616e  : Humberto.A.San
+000000c0: 6368 657a 2e49 4940 676d 6169 6c2e 636f  chez.II@gmail.co
+000000d0: 6d0a 4d61 696e 7461 696e 6572 3a20 4875  m.Maintainer: Hu
+000000e0: 6d62 6572 746f 2041 2e20 5361 6e63 6865  mberto A. Sanche
+000000f0: 7a20 4949 0a4d 6169 6e74 6169 6e65 722d  z II.Maintainer-
+00000100: 656d 6169 6c3a 2068 756d 6265 7274 6f2e  email: humberto.
+00000110: 612e 7361 6e63 6865 7a2e 6969 4067 6d61  a.sanchez.ii@gma
+00000120: 696c 2e63 6f6d 0a44 6573 6372 6970 7469  il.com.Descripti
+00000130: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
+00000140: 2074 6578 742f 6d61 726b 646f 776e 0a4c   text/markdown.L
+00000150: 6963 656e 7365 2d46 696c 653a 204c 4943  icense-File: LIC
+00000160: 454e 5345 0a0a 3c69 6d67 2073 7263 3d22  ENSE..<img src="
+00000170: 2e2f 6465 7665 6c6f 7065 722f 6167 706c  ./developer/agpl
+00000180: 2d6c 6963 656e 7365 2d77 6562 2d62 6164  -license-web-bad
+00000190: 6765 2d76 6572 7369 6f6e 2d32 2d32 3536  ge-version-2-256
+000001a0: 7834 382e 706e 6722 2f3e 200a 0a5b 215b  x48.png"/> ..[![
+000001b0: 4d61 696e 7465 6e61 6e63 655d 2868 7474  Maintenance](htt
+000001c0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000001d0: 2e69 6f2f 6261 6467 652f 4d61 696e 7461  .io/badge/Mainta
+000001e0: 696e 6564 2533 462d 7965 732d 6772 6565  ined%3F-yes-gree
+000001f0: 6e2e 7376 6729 5d28 6874 7470 733a 2f2f  n.svg)](https://
+00000200: 4769 7448 7562 2e63 6f6d 2f4e 6165 7265  GitHub.com/Naere
+00000210: 656e 2f53 7472 6170 446f 776e 2e6a 732f  en/StrapDown.js/
+00000220: 6772 6170 6873 2f63 6f6d 6d69 742d 6163  graphs/commit-ac
+00000230: 7469 7669 7479 290a 5b21 5b43 6972 636c  tivity).[![Circl
+00000240: 6543 495d 2868 7474 7073 3a2f 2f64 6c2e  eCI](https://dl.
+00000250: 6369 7263 6c65 6369 2e63 6f6d 2f73 7461  circleci.com/sta
+00000260: 7475 732d 6261 6467 652f 696d 672f 6768  tus-badge/img/gh
+00000270: 2f68 6173 6969 3230 3131 2f6f 676c 2f74  /hasii2011/ogl/t
+00000280: 7265 652f 6d61 7374 6572 2e73 7667 3f73  ree/master.svg?s
+00000290: 7479 6c65 3d73 6869 656c 6429 5d28 6874  tyle=shield)](ht
+000002a0: 7470 733a 2f2f 646c 2e63 6972 636c 6563  tps://dl.circlec
+000002b0: 692e 636f 6d2f 7374 6174 7573 2d62 6164  i.com/status-bad
+000002c0: 6765 2f72 6564 6972 6563 742f 6768 2f68  ge/redirect/gh/h
+000002d0: 6173 6969 3230 3131 2f6f 676c 2f74 7265  asii2011/ogl/tre
+000002e0: 652f 6d61 7374 6572 290a 5b21 5b6d 6163  e/master).[![mac
+000002f0: 4f53 5d28 6874 7470 733a 2f2f 7376 6773  OS](https://svgs
+00000300: 6861 7265 2e63 6f6d 2f69 2f5a 6a50 2e73  hare.com/i/ZjP.s
+00000310: 7667 295d 2868 7474 7073 3a2f 2f73 7667  vg)](https://svg
+00000320: 7368 6172 652e 636f 6d2f 692f 5a6a 502e  share.com/i/ZjP.
+00000330: 7376 6729 0a0a 5b21 5b66 6f72 7468 6562  svg)..[![fortheb
+00000340: 6164 6765 206d 6164 652d 7769 7468 2d70  adge made-with-p
+00000350: 7974 686f 6e5d 2868 7474 703a 2f2f 466f  ython](http://Fo
+00000360: 7254 6865 4261 6467 652e 636f 6d2f 696d  rTheBadge.com/im
+00000370: 6167 6573 2f62 6164 6765 732f 6d61 6465  ages/badges/made
+00000380: 2d77 6974 682d 7079 7468 6f6e 2e73 7667  -with-python.svg
+00000390: 295d 2868 7474 7073 3a2f 2f77 7777 2e70  )](https://www.p
+000003a0: 7974 686f 6e2e 6f72 672f 290a 0af0 9d93  ython.org/).....
+000003b0: 9f20 f09d 93a8 20f0 9d93 a420 f09d 93a3  . .... .... ....
+000003c0: 2073 7461 6e64 7320 666f 7220 5079 7468   stands for Pyth
+000003d0: 6f6e 2055 4d4c 2054 6f6f 6c2e 2054 6869  on UML Tool. Thi
+000003e0: 7320 6973 2074 6865 2065 7874 6572 6e61  s is the externa
+000003f0: 6c20 6772 6170 6869 6361 6c20 7368 6170  l graphical shap
+00000400: 6573 206d 6f64 756c 6520 666f 7220 5079  es module for Py
+00000410: 7574 0a74 6861 7420 616c 6c6f 7773 2066  ut.that allows f
+00000420: 6f72 2065 7874 6572 6e61 6c20 706c 7567  or external plug
+00000430: 696e 2064 6576 656c 6f70 6d65 6e74 3b0a  in development;.
+00000440: 0a54 6869 7320 7072 6f6a 6563 7420 6465  .This project de
+00000450: 7065 6e64 7320 6f6e 2070 7975 746d 6f64  pends on pyutmod
+00000460: 656c 2061 6e64 2077 7850 7974 686f 6e0a  el and wxPython.
+00000470: 0a5f 5f5f 0a0a 2323 2044 6576 656c 6f70  .___..## Develop
+00000480: 6572 204e 6f74 6573 0a54 6869 7320 7072  er Notes.This pr
+00000490: 6f6a 6563 7420 7573 6573 205b 6275 696c  oject uses [buil
+000004a0: 646c 6163 6b65 795d 2868 7474 7073 3a2f  dlackey](https:/
+000004b0: 2f67 6974 6875 622e 636f 6d2f 6861 7369  /github.com/hasi
+000004c0: 6932 3031 312f 6275 696c 646c 6163 6b65  i2011/buildlacke
+000004d0: 7929 2066 6f72 2064 6179 2074 6f20 6461  y) for day to da
+000004e0: 7920 6465 7665 6c6f 706d 656e 7420 6275  y development bu
+000004f0: 696c 6473 0a0a 5f5f 5f0a 0a57 7269 7474  ilds..___..Writt
+00000500: 656e 2062 7920 3c61 2068 7265 663d 226d  en by <a href="m
+00000510: 6169 6c74 6f3a 656d 6169 6c40 6875 6d62  ailto:email@humb
+00000520: 6572 746f 2e61 2e73 616e 6368 657a 2e69  erto.a.sanchez.i
+00000530: 6940 676d 6169 6c2e 636f 6d3f 7375 626a  i@gmail.com?subj
+00000540: 6563 743d 4865 6c6c 6f20 4875 6d62 6572  ect=Hello Humber
+00000550: 746f 223e 4875 6d62 6572 746f 2041 2e20  to">Humberto A. 
+00000560: 5361 6e63 6865 7a20 4949 3c2f 613e 2020  Sanchez II</a>  
+00000570: 2843 2920 3230 3233 0a0a 2323 204e 6f74  (C) 2023..## Not
+00000580: 650a 466f 7220 616c 6c20 6b69 6e64 206f  e.For all kind o
+00000590: 6620 7072 6f62 6c65 6d73 2c20 7265 7175  f problems, requ
+000005a0: 6573 7473 2c20 656e 6861 6e63 656d 656e  ests, enhancemen
+000005b0: 7473 2c20 6275 6720 7265 706f 7274 732c  ts, bug reports,
+000005c0: 2065 7463 2e2c 0a70 6c65 6173 6520 6472   etc.,.please dr
+000005d0: 6f70 206d 6520 616e 2065 2d6d 6169 6c2e  op me an e-mail.
+000005e0: 0a0a 0a21 5b48 756d 6265 7274 6f27 7320  ...![Humberto's 
+000005f0: 4d6f 6469 6669 6564 204c 6f67 6f5d 2868  Modified Logo](h
+00000600: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00000610: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00000620: 2f77 696b 692f 6861 7369 6932 3031 312f  /wiki/hasii2011/
+00000630: 6769 7474 6f64 6f69 7374 636c 6f6e 652f  gittodoistclone/
+00000640: 696d 6167 6573 2f53 696c 6c79 4769 7448  images/SillyGitH
+00000650: 7562 2e70 6e67 290a 0a49 2061 6d20 636f  ub.png)..I am co
+00000660: 6e63 6572 6e65 6420 6162 6f75 7420 4769  ncerned about Gi
+00000670: 7448 7562 2773 2043 6f70 696c 6f74 2070  tHub's Copilot p
+00000680: 726f 6a65 6374 0a0a 0a0a 4920 7572 6765  roject....I urge
+00000690: 2079 6f75 2074 6f20 7265 6164 2061 626f   you to read abo
+000006a0: 7574 2074 6865 205b 4769 7665 2075 7020  ut the [Give up 
+000006b0: 4769 7448 7562 5d28 6874 7470 733a 2f2f  GitHub](https://
+000006c0: 4769 7665 5570 4769 7448 7562 2e6f 7267  GiveUpGitHub.org
+000006d0: 2920 6361 6d70 6169 676e 2066 726f 6d20  ) campaign from 
+000006e0: 5b74 6865 2053 6f66 7477 6172 6520 4672  [the Software Fr
+000006f0: 6565 646f 6d20 436f 6e73 6572 7661 6e63  eedom Conservanc
+00000700: 795d 2868 7474 7073 3a2f 2f73 6663 6f6e  y](https://sfcon
+00000710: 7365 7276 616e 6379 2e6f 7267 292e 0a0a  servancy.org)...
+00000720: 5768 696c 6520 4920 646f 206e 6f74 2061  While I do not a
+00000730: 6476 6f63 6174 6520 666f 7220 616c 6c20  dvocate for all 
+00000740: 7468 6520 6973 7375 6573 206c 6973 7465  the issues liste
+00000750: 6420 7468 6572 6520 4920 646f 206e 6f74  d there I do not
+00000760: 206c 696b 6520 7468 6174 2061 2063 6f6d   like that a com
+00000770: 7061 6e79 206c 696b 6520 4d69 6372 6f73  pany like Micros
+00000780: 6f66 7420 6d61 7920 7072 6f66 6974 2066  oft may profit f
+00000790: 726f 6d20 6f70 656e 2073 6f75 7263 6520  rom open source 
+000007a0: 7072 6f6a 6563 7473 2e0a 0a49 2063 6f6e  projects...I con
+000007b0: 7469 6e75 6520 746f 2075 7365 2047 6974  tinue to use Git
+000007c0: 4875 6220 6265 6361 7573 6520 6974 206f  Hub because it o
+000007d0: 6666 6572 7320 7468 6520 7365 7276 6963  ffers the servic
+000007e0: 6573 2049 206e 6565 6420 666f 7220 6672  es I need for fr
+000007f0: 6565 2e20 2042 7574 2c20 4920 636f 6e74  ee.  But, I cont
+00000800: 696e 7565 2074 6f20 6d6f 6e69 746f 7220  inue to monitor 
+00000810: 7468 6569 7220 7465 726d 7320 6f66 2073  their terms of s
+00000820: 6572 7669 6365 2e0a 0a41 6e79 2075 7365  ervice...Any use
+00000830: 206f 6620 7468 6973 2070 726f 6a65 6374   of this project
+00000840: 2773 2063 6f64 6520 6279 2047 6974 4875  's code by GitHu
+00000850: 6220 436f 7069 6c6f 742c 2070 6173 7420  b Copilot, past 
+00000860: 6f72 2070 7265 7365 6e74 2c20 6973 2064  or present, is d
+00000870: 6f6e 6520 7769 7468 6f75 7420 6d79 2070  one without my p
+00000880: 6572 6d69 7373 696f 6e2e 2020 4920 646f  ermission.  I do
+00000890: 206e 6f74 2063 6f6e 7365 6e74 2074 6f20   not consent to 
+000008a0: 4769 7448 7562 2773 2075 7365 206f 6620  GitHub's use of 
+000008b0: 7468 6973 2070 726f 6a65 6374 2773 0a63  this project's.c
+000008c0: 6f64 6520 696e 2043 6f70 696c 6f74 2e0a  ode in Copilot..
+000008d0: 0a41 2072 6570 6f73 6974 6f72 7920 6f77  .A repository ow
+000008e0: 6e65 7220 6d61 7920 6f70 7420 6f75 7420  ner may opt out 
+000008f0: 6f66 2043 6f70 696c 6f74 2062 7920 6368  of Copilot by ch
+00000900: 616e 6769 6e67 2053 6574 7469 6e67 7320  anging Settings 
+00000910: 2d2d 3e20 4769 7448 7562 2043 6f70 696c  --> GitHub Copil
+00000920: 6f74 2e0a 0a49 2068 6176 6520 646f 6e65  ot...I have done
+00000930: 2073 6f2e 0a                              so..
```

### Comparing `ogl-0.70.22/miniogl/AnchorPoint.py` & `ogl-0.70.25/miniogl/AnchorPoint.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/miniogl/AttachmentSide.py` & `ogl-0.70.25/miniogl/AttachmentSide.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/miniogl/Common.py` & `ogl-0.70.25/miniogl/Common.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/miniogl/ControlPoint.py` & `ogl-0.70.25/miniogl/ControlPoint.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/miniogl/Diagram.py` & `ogl-0.70.25/miniogl/Diagram.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/miniogl/DiagramFrame.py` & `ogl-0.70.25/miniogl/DiagramFrame.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/miniogl/DlgDebugDiagramFrame.py` & `ogl-0.70.25/miniogl/DlgDebugDiagramFrame.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/miniogl/LinePoint.py` & `ogl-0.70.25/miniogl/LinePoint.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/miniogl/LineShape.py` & `ogl-0.70.25/miniogl/LineShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/miniogl/LollipopLine.py` & `ogl-0.70.25/miniogl/LollipopLine.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/miniogl/MiniOglColorEnum.py` & `ogl-0.70.25/miniogl/MiniOglColorEnum.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/miniogl/MiniOglPenStyle.py` & `ogl-0.70.25/miniogl/MiniOglPenStyle.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/miniogl/PointShape.py` & `ogl-0.70.25/miniogl/PointShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/miniogl/RectangleShape.py` & `ogl-0.70.25/miniogl/RectangleShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/miniogl/RectangleShapeModel.py` & `ogl-0.70.25/miniogl/RectangleShapeModel.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/miniogl/RotatableShape.py` & `ogl-0.70.25/miniogl/RotatableShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/miniogl/SelectAnchorPoint.py` & `ogl-0.70.25/miniogl/SelectAnchorPoint.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/miniogl/Shape.py` & `ogl-0.70.25/miniogl/Shape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/miniogl/ShapeEventHandler.py` & `ogl-0.70.25/miniogl/ShapeEventHandler.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/miniogl/ShapeModel.py` & `ogl-0.70.25/miniogl/ShapeModel.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/miniogl/SizerShape.py` & `ogl-0.70.25/miniogl/SizerShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/miniogl/TextShape.py` & `ogl-0.70.25/miniogl/TextShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/miniogl/TextShapeModel.py` & `ogl-0.70.25/miniogl/TextShapeModel.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/miniogl/VShapes.py` & `ogl-0.70.25/miniogl/VShapes.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/OglActor.py` & `ogl-0.70.25/ogl/OglActor.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/OglAggregation.py` & `ogl-0.70.25/ogl/OglAggregation.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/OglAssociation.py` & `ogl-0.70.25/ogl/OglAssociation.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/OglClass.py` & `ogl-0.70.25/ogl/OglClass.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/OglComposition.py` & `ogl-0.70.25/ogl/OglComposition.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/OglConstants.py` & `ogl-0.70.25/ogl/OglConstants.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/OglDimensions.py` & `ogl-0.70.25/ogl/OglDimensions.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/OglInheritance.py` & `ogl-0.70.25/ogl/OglInheritance.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/OglInterface.py` & `ogl-0.70.25/ogl/OglInterface.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from wx import PENSTYLE_LONG_DASH
 from wx import RED_PEN
 from wx import BLACK_PEN
 from wx import WHITE_BRUSH
 
 from pyutmodel.PyutLink import PyutLink
 
+from miniogl.TextShape import TextShape
+
 from ogl.OglLink import OglLink
 from ogl.OglClass import OglClass
 
 # Kind of labels
 [CENTER] = list(range(1))
 
 
@@ -51,18 +53,19 @@
         self.updateLabels()
         self.SetDrawArrow(True)
 
     def updateLabels(self):
         """
         Update the labels according to the link.
         """
-        def prepareLabel(textShape, text):
+        def prepareLabel(textShape: TextShape, text):
             # If label should be drawn
             if text.strip() != "":
-                textShape.SetText(text)
+                # textShape.SetText(text)
+                textShape.text = text
                 # textShape.Show(True)
                 textShape.SetVisible(True)
             else:
                 # textShape.Show(False)
                 textShape.SetVisible(False)
 
         # Prepares labels
```

### Comparing `ogl-0.70.22/ogl/OglInterface2.py` & `ogl-0.70.25/ogl/OglInterface2.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/OglLink.py` & `ogl-0.70.25/ogl/OglLink.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/OglLinkFactory.py` & `ogl-0.70.25/ogl/OglLinkFactory.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/OglNote.py` & `ogl-0.70.25/ogl/OglNote.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/OglNoteLink.py` & `ogl-0.70.25/ogl/OglNoteLink.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/OglObject.py` & `ogl-0.70.25/ogl/OglObject.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/OglText.py` & `ogl-0.70.25/ogl/OglText.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/OglUseCase.py` & `ogl-0.70.25/ogl/OglUseCase.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/OglUtils.py` & `ogl-0.70.25/ogl/OglUtils.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/events/IOglEventEngine.py` & `ogl-0.70.25/ogl/events/IOglEventEngine.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/events/OglEventEngine.py` & `ogl-0.70.25/ogl/events/OglEventEngine.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/events/OglEvents.py` & `ogl-0.70.25/ogl/events/OglEvents.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/preferences/OglPreferences.py` & `ogl-0.70.25/ogl/preferences/OglPreferences.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/resources/img/Display.py` & `ogl-0.70.25/ogl/resources/img/Display.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/resources/img/DoNotDisplay.py` & `ogl-0.70.25/ogl/resources/img/DoNotDisplay.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/resources/img/UnSpecified.py` & `ogl-0.70.25/ogl/resources/img/UnSpecified.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/resources/img/textdetails/DecreaseTextSize.py` & `ogl-0.70.25/ogl/resources/img/textdetails/DecreaseTextSize.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/resources/img/textdetails/IncreaseTextSize.py` & `ogl-0.70.25/ogl/resources/img/textdetails/IncreaseTextSize.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/sd/OglInstanceName.py` & `ogl-0.70.25/ogl/sd/OglInstanceName.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/sd/OglSDInstance.py` & `ogl-0.70.25/ogl/sd/OglSDInstance.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/sd/OglSDMessage.py` & `ogl-0.70.25/ogl/sd/OglSDMessage.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/ui/BaseOglPreferencesPage.py` & `ogl-0.70.25/ogl/ui/BaseOglPreferencesPage.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/ui/DefaultValuesPreferencesPage.py` & `ogl-0.70.25/ogl/ui/DefaultValuesPreferencesPage.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/ui/DiagramPreferencesPage.py` & `ogl-0.70.25/ogl/ui/DiagramPreferencesPage.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/ui/valuecontrols/AssociationAttributesControl.py` & `ogl-0.70.25/ogl/ui/valuecontrols/AssociationAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/ui/valuecontrols/ClassAttributesControl.py` & `ogl-0.70.25/ogl/ui/valuecontrols/ClassAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/ui/valuecontrols/DefaultNamesControl.py` & `ogl-0.70.25/ogl/ui/valuecontrols/DefaultNamesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/ui/valuecontrols/NoteAttributesControl.py` & `ogl-0.70.25/ogl/ui/valuecontrols/NoteAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/ui/valuecontrols/SDAttributesControl.py` & `ogl-0.70.25/ogl/ui/valuecontrols/SDAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl/ui/valuecontrols/TextAttributesControl.py` & `ogl-0.70.25/ogl/ui/valuecontrols/TextAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/ogl.egg-info/PKG-INFO` & `ogl-0.70.25/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6f67 6c0a  : 2.1.Name: ogl.
-00000020: 5665 7273 696f 6e3a 2030 2e37 302e 3232  Version: 0.70.22
-00000030: 0a53 756d 6d61 7279 3a20 4578 7465 726e  .Summary: Extern
-00000040: 616c 2050 7975 7420 4772 6170 6869 6361  al Pyut Graphica
-00000050: 6c20 5368 6170 6573 0a48 6f6d 652d 7061  l Shapes.Home-pa
-00000060: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
-00000070: 7562 2e63 6f6d 2f68 6173 6969 3230 3131  ub.com/hasii2011
-00000080: 2f6f 676c 0a41 7574 686f 723a 2048 756d  /ogl.Author: Hum
-00000090: 6265 7274 6f20 412e 2053 616e 6368 657a  berto A. Sanchez
-000000a0: 2049 490a 4175 7468 6f72 2d65 6d61 696c   II.Author-email
-000000b0: 3a20 4875 6d62 6572 746f 2e41 2e53 616e  : Humberto.A.San
-000000c0: 6368 657a 2e49 4940 676d 6169 6c2e 636f  chez.II@gmail.co
-000000d0: 6d0a 4d61 696e 7461 696e 6572 3a20 4875  m.Maintainer: Hu
-000000e0: 6d62 6572 746f 2041 2e20 5361 6e63 6865  mberto A. Sanche
-000000f0: 7a20 4949 0a4d 6169 6e74 6169 6e65 722d  z II.Maintainer-
-00000100: 656d 6169 6c3a 2068 756d 6265 7274 6f2e  email: humberto.
-00000110: 612e 7361 6e63 6865 7a2e 6969 4067 6d61  a.sanchez.ii@gma
-00000120: 696c 2e63 6f6d 0a44 6573 6372 6970 7469  il.com.Descripti
-00000130: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
-00000140: 2074 6578 742f 6d61 726b 646f 776e 0a4c   text/markdown.L
-00000150: 6963 656e 7365 2d46 696c 653a 204c 4943  icense-File: LIC
-00000160: 454e 5345 0a0a 3c69 6d67 2073 7263 3d22  ENSE..<img src="
-00000170: 2e2f 6465 7665 6c6f 7065 722f 6167 706c  ./developer/agpl
-00000180: 2d6c 6963 656e 7365 2d77 6562 2d62 6164  -license-web-bad
-00000190: 6765 2d76 6572 7369 6f6e 2d32 2d32 3536  ge-version-2-256
-000001a0: 7834 382e 706e 6722 2f3e 200a 0a5b 215b  x48.png"/> ..[![
-000001b0: 4d61 696e 7465 6e61 6e63 655d 2868 7474  Maintenance](htt
-000001c0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-000001d0: 2e69 6f2f 6261 6467 652f 4d61 696e 7461  .io/badge/Mainta
-000001e0: 696e 6564 2533 462d 7965 732d 6772 6565  ined%3F-yes-gree
-000001f0: 6e2e 7376 6729 5d28 6874 7470 733a 2f2f  n.svg)](https://
-00000200: 4769 7448 7562 2e63 6f6d 2f4e 6165 7265  GitHub.com/Naere
-00000210: 656e 2f53 7472 6170 446f 776e 2e6a 732f  en/StrapDown.js/
-00000220: 6772 6170 6873 2f63 6f6d 6d69 742d 6163  graphs/commit-ac
-00000230: 7469 7669 7479 290a 5b21 5b43 6972 636c  tivity).[![Circl
-00000240: 6543 495d 2868 7474 7073 3a2f 2f64 6c2e  eCI](https://dl.
-00000250: 6369 7263 6c65 6369 2e63 6f6d 2f73 7461  circleci.com/sta
-00000260: 7475 732d 6261 6467 652f 696d 672f 6768  tus-badge/img/gh
-00000270: 2f68 6173 6969 3230 3131 2f6f 676c 2f74  /hasii2011/ogl/t
-00000280: 7265 652f 6d61 7374 6572 2e73 7667 3f73  ree/master.svg?s
-00000290: 7479 6c65 3d73 6869 656c 6429 5d28 6874  tyle=shield)](ht
-000002a0: 7470 733a 2f2f 646c 2e63 6972 636c 6563  tps://dl.circlec
-000002b0: 692e 636f 6d2f 7374 6174 7573 2d62 6164  i.com/status-bad
-000002c0: 6765 2f72 6564 6972 6563 742f 6768 2f68  ge/redirect/gh/h
-000002d0: 6173 6969 3230 3131 2f6f 676c 2f74 7265  asii2011/ogl/tre
-000002e0: 652f 6d61 7374 6572 290a 5b21 5b6d 6163  e/master).[![mac
-000002f0: 4f53 5d28 6874 7470 733a 2f2f 7376 6773  OS](https://svgs
-00000300: 6861 7265 2e63 6f6d 2f69 2f5a 6a50 2e73  hare.com/i/ZjP.s
-00000310: 7667 295d 2868 7474 7073 3a2f 2f73 7667  vg)](https://svg
-00000320: 7368 6172 652e 636f 6d2f 692f 5a6a 502e  share.com/i/ZjP.
-00000330: 7376 6729 0a0a 5b21 5b66 6f72 7468 6562  svg)..[![fortheb
-00000340: 6164 6765 206d 6164 652d 7769 7468 2d70  adge made-with-p
-00000350: 7974 686f 6e5d 2868 7474 703a 2f2f 466f  ython](http://Fo
-00000360: 7254 6865 4261 6467 652e 636f 6d2f 696d  rTheBadge.com/im
-00000370: 6167 6573 2f62 6164 6765 732f 6d61 6465  ages/badges/made
-00000380: 2d77 6974 682d 7079 7468 6f6e 2e73 7667  -with-python.svg
-00000390: 295d 2868 7474 7073 3a2f 2f77 7777 2e70  )](https://www.p
-000003a0: 7974 686f 6e2e 6f72 672f 290a 0af0 9d93  ython.org/).....
-000003b0: 9f20 f09d 93a8 20f0 9d93 a420 f09d 93a3  . .... .... ....
-000003c0: 2073 7461 6e64 7320 666f 7220 5079 7468   stands for Pyth
-000003d0: 6f6e 2055 4d4c 2054 6f6f 6c2e 2054 6869  on UML Tool. Thi
-000003e0: 7320 6973 2074 6865 2065 7874 6572 6e61  s is the externa
-000003f0: 6c20 6772 6170 6869 6361 6c20 7368 6170  l graphical shap
-00000400: 6573 206d 6f64 756c 6520 666f 7220 5079  es module for Py
-00000410: 7574 0a74 6861 7420 616c 6c6f 7773 2066  ut.that allows f
-00000420: 6f72 2065 7874 6572 6e61 6c20 706c 7567  or external plug
-00000430: 696e 2064 6576 656c 6f70 6d65 6e74 3b0a  in development;.
-00000440: 0a54 6869 7320 7072 6f6a 6563 7420 6465  .This project de
-00000450: 7065 6e64 7320 6f6e 2070 7975 746d 6f64  pends on pyutmod
-00000460: 656c 2061 6e64 2077 7850 7974 686f 6e0a  el and wxPython.
-00000470: 0a0a 2d2d 2d2d 2d2d 0a0a 0a21 5b48 756d  ..------...![Hum
-00000480: 6265 7274 6f27 7320 4d6f 6469 6669 6564  berto's Modified
-00000490: 204c 6f67 6f5d 2868 7474 7073 3a2f 2f72   Logo](https://r
-000004a0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-000004b0: 7465 6e74 2e63 6f6d 2f77 696b 692f 6861  tent.com/wiki/ha
-000004c0: 7369 6932 3031 312f 6769 7474 6f64 6f69  sii2011/gittodoi
-000004d0: 7374 636c 6f6e 652f 696d 6167 6573 2f53  stclone/images/S
-000004e0: 696c 6c79 4769 7448 7562 2e70 6e67 290a  illyGitHub.png).
-000004f0: 0a49 2061 6d20 636f 6e63 6572 6e65 6420  .I am concerned 
-00000500: 6162 6f75 7420 4769 7448 7562 2773 2043  about GitHub's C
-00000510: 6f70 696c 6f74 2070 726f 6a65 6374 0a0a  opilot project..
-00000520: 0a0a 4920 7572 6765 2079 6f75 2074 6f20  ..I urge you to 
-00000530: 7265 6164 2061 626f 7574 2074 6865 0a5b  read about the.[
-00000540: 4769 7665 2075 7020 4769 7448 7562 5d28  Give up GitHub](
-00000550: 6874 7470 733a 2f2f 4769 7665 5570 4769  https://GiveUpGi
-00000560: 7448 7562 2e6f 7267 2920 6361 6d70 6169  tHub.org) campai
-00000570: 676e 2066 726f 6d0a 5b74 6865 2053 6f66  gn from.[the Sof
-00000580: 7477 6172 6520 4672 6565 646f 6d20 436f  tware Freedom Co
-00000590: 6e73 6572 7661 6e63 795d 2868 7474 7073  nservancy](https
-000005a0: 3a2f 2f73 6663 6f6e 7365 7276 616e 6379  ://sfconservancy
-000005b0: 2e6f 7267 292e 0a0a 5768 696c 6520 4920  .org)...While I 
-000005c0: 646f 206e 6f74 2061 6476 6f63 6174 6520  do not advocate 
-000005d0: 666f 7220 616c 6c20 7468 6520 6973 7375  for all the issu
-000005e0: 6573 206c 6973 7465 6420 7468 6572 6520  es listed there 
-000005f0: 4920 646f 206e 6f74 206c 696b 6520 7468  I do not like th
-00000600: 6174 0a61 2063 6f6d 7061 6e79 206c 696b  at.a company lik
-00000610: 6520 4d69 6372 6f73 6f66 7420 6d61 7920  e Microsoft may 
-00000620: 7072 6f66 6974 2066 726f 6d20 6f70 656e  profit from open
-00000630: 2073 6f75 7263 6520 7072 6f6a 6563 7473   source projects
-00000640: 2e0a 0a49 2063 6f6e 7469 6e75 6520 746f  ...I continue to
-00000650: 2075 7365 2047 6974 4875 6220 6265 6361   use GitHub beca
-00000660: 7573 6520 6974 206f 6666 6572 7320 7468  use it offers th
-00000670: 6520 7365 7276 6963 6573 2049 206e 6565  e services I nee
-00000680: 6420 666f 7220 6672 6565 2e20 2042 7574  d for free.  But
-00000690: 2c20 4920 636f 6e74 696e 7565 0a74 6f20  , I continue.to 
-000006a0: 6d6f 6e69 746f 7220 7468 6569 7220 7465  monitor their te
-000006b0: 726d 7320 6f66 2073 6572 7669 6365 2e0a  rms of service..
-000006c0: 0a41 6e79 2075 7365 206f 6620 7468 6973  .Any use of this
-000006d0: 2070 726f 6a65 6374 2773 2063 6f64 6520   project's code 
-000006e0: 6279 2047 6974 4875 6220 436f 7069 6c6f  by GitHub Copilo
-000006f0: 742c 2070 6173 7420 6f72 2070 7265 7365  t, past or prese
-00000700: 6e74 2c20 6973 2064 6f6e 650a 7769 7468  nt, is done.with
-00000710: 6f75 7420 6d79 2070 6572 6d69 7373 696f  out my permissio
-00000720: 6e2e 2020 4920 646f 206e 6f74 2063 6f6e  n.  I do not con
-00000730: 7365 6e74 2074 6f20 4769 7448 7562 2773  sent to GitHub's
-00000740: 2075 7365 206f 6620 7468 6973 2070 726f   use of this pro
-00000750: 6a65 6374 2773 0a63 6f64 6520 696e 2043  ject's.code in C
-00000760: 6f70 696c 6f74 2e0a 0a41 2072 6570 6f73  opilot...A repos
-00000770: 6974 6f72 7920 6f77 6e65 7220 6d61 7920  itory owner may 
-00000780: 6f70 7420 6f75 7420 6f66 2043 6f70 696c  opt out of Copil
-00000790: 6f74 2062 7920 6368 616e 6769 6e67 2053  ot by changing S
-000007a0: 6574 7469 6e67 7320 2d2d 3e20 4769 7448  ettings --> GitH
-000007b0: 7562 2043 6f70 696c 6f74 2e0a 0a49 2068  ub Copilot...I h
-000007c0: 6176 6520 646f 6e65 2073 6f2e 0a         ave done so..
+00000000: 3c69 6d67 2073 7263 3d22 2e2f 6465 7665  <img src="./deve
+00000010: 6c6f 7065 722f 6167 706c 2d6c 6963 656e  loper/agpl-licen
+00000020: 7365 2d77 6562 2d62 6164 6765 2d76 6572  se-web-badge-ver
+00000030: 7369 6f6e 2d32 2d32 3536 7834 382e 706e  sion-2-256x48.pn
+00000040: 6722 2f3e 200a 0a5b 215b 4d61 696e 7465  g"/> ..[![Mainte
+00000050: 6e61 6e63 655d 2868 7474 7073 3a2f 2f69  nance](https://i
+00000060: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+00000070: 6467 652f 4d61 696e 7461 696e 6564 2533  dge/Maintained%3
+00000080: 462d 7965 732d 6772 6565 6e2e 7376 6729  F-yes-green.svg)
+00000090: 5d28 6874 7470 733a 2f2f 4769 7448 7562  ](https://GitHub
+000000a0: 2e63 6f6d 2f4e 6165 7265 656e 2f53 7472  .com/Naereen/Str
+000000b0: 6170 446f 776e 2e6a 732f 6772 6170 6873  apDown.js/graphs
+000000c0: 2f63 6f6d 6d69 742d 6163 7469 7669 7479  /commit-activity
+000000d0: 290a 5b21 5b43 6972 636c 6543 495d 2868  ).[![CircleCI](h
+000000e0: 7474 7073 3a2f 2f64 6c2e 6369 7263 6c65  ttps://dl.circle
+000000f0: 6369 2e63 6f6d 2f73 7461 7475 732d 6261  ci.com/status-ba
+00000100: 6467 652f 696d 672f 6768 2f68 6173 6969  dge/img/gh/hasii
+00000110: 3230 3131 2f6f 676c 2f74 7265 652f 6d61  2011/ogl/tree/ma
+00000120: 7374 6572 2e73 7667 3f73 7479 6c65 3d73  ster.svg?style=s
+00000130: 6869 656c 6429 5d28 6874 7470 733a 2f2f  hield)](https://
+00000140: 646c 2e63 6972 636c 6563 692e 636f 6d2f  dl.circleci.com/
+00000150: 7374 6174 7573 2d62 6164 6765 2f72 6564  status-badge/red
+00000160: 6972 6563 742f 6768 2f68 6173 6969 3230  irect/gh/hasii20
+00000170: 3131 2f6f 676c 2f74 7265 652f 6d61 7374  11/ogl/tree/mast
+00000180: 6572 290a 5b21 5b6d 6163 4f53 5d28 6874  er).[![macOS](ht
+00000190: 7470 733a 2f2f 7376 6773 6861 7265 2e63  tps://svgshare.c
+000001a0: 6f6d 2f69 2f5a 6a50 2e73 7667 295d 2868  om/i/ZjP.svg)](h
+000001b0: 7474 7073 3a2f 2f73 7667 7368 6172 652e  ttps://svgshare.
+000001c0: 636f 6d2f 692f 5a6a 502e 7376 6729 0a0a  com/i/ZjP.svg)..
+000001d0: 5b21 5b66 6f72 7468 6562 6164 6765 206d  [![forthebadge m
+000001e0: 6164 652d 7769 7468 2d70 7974 686f 6e5d  ade-with-python]
+000001f0: 2868 7474 703a 2f2f 466f 7254 6865 4261  (http://ForTheBa
+00000200: 6467 652e 636f 6d2f 696d 6167 6573 2f62  dge.com/images/b
+00000210: 6164 6765 732f 6d61 6465 2d77 6974 682d  adges/made-with-
+00000220: 7079 7468 6f6e 2e73 7667 295d 2868 7474  python.svg)](htt
+00000230: 7073 3a2f 2f77 7777 2e70 7974 686f 6e2e  ps://www.python.
+00000240: 6f72 672f 290a 0af0 9d93 9f20 f09d 93a8  org/)...... ....
+00000250: 20f0 9d93 a420 f09d 93a3 2073 7461 6e64   .... .... stand
+00000260: 7320 666f 7220 5079 7468 6f6e 2055 4d4c  s for Python UML
+00000270: 2054 6f6f 6c2e 2054 6869 7320 6973 2074   Tool. This is t
+00000280: 6865 2065 7874 6572 6e61 6c20 6772 6170  he external grap
+00000290: 6869 6361 6c20 7368 6170 6573 206d 6f64  hical shapes mod
+000002a0: 756c 6520 666f 7220 5079 7574 0a74 6861  ule for Pyut.tha
+000002b0: 7420 616c 6c6f 7773 2066 6f72 2065 7874  t allows for ext
+000002c0: 6572 6e61 6c20 706c 7567 696e 2064 6576  ernal plugin dev
+000002d0: 656c 6f70 6d65 6e74 3b0a 0a54 6869 7320  elopment;..This 
+000002e0: 7072 6f6a 6563 7420 6465 7065 6e64 7320  project depends 
+000002f0: 6f6e 2070 7975 746d 6f64 656c 2061 6e64  on pyutmodel and
+00000300: 2077 7850 7974 686f 6e0a 0a5f 5f5f 0a0a   wxPython..___..
+00000310: 2323 2044 6576 656c 6f70 6572 204e 6f74  ## Developer Not
+00000320: 6573 0a54 6869 7320 7072 6f6a 6563 7420  es.This project 
+00000330: 7573 6573 205b 6275 696c 646c 6163 6b65  uses [buildlacke
+00000340: 795d 2868 7474 7073 3a2f 2f67 6974 6875  y](https://githu
+00000350: 622e 636f 6d2f 6861 7369 6932 3031 312f  b.com/hasii2011/
+00000360: 6275 696c 646c 6163 6b65 7929 2066 6f72  buildlackey) for
+00000370: 2064 6179 2074 6f20 6461 7920 6465 7665   day to day deve
+00000380: 6c6f 706d 656e 7420 6275 696c 6473 0a0a  lopment builds..
+00000390: 5f5f 5f0a 0a57 7269 7474 656e 2062 7920  ___..Written by 
+000003a0: 3c61 2068 7265 663d 226d 6169 6c74 6f3a  <a href="mailto:
+000003b0: 656d 6169 6c40 6875 6d62 6572 746f 2e61  email@humberto.a
+000003c0: 2e73 616e 6368 657a 2e69 6940 676d 6169  .sanchez.ii@gmai
+000003d0: 6c2e 636f 6d3f 7375 626a 6563 743d 4865  l.com?subject=He
+000003e0: 6c6c 6f20 4875 6d62 6572 746f 223e 4875  llo Humberto">Hu
+000003f0: 6d62 6572 746f 2041 2e20 5361 6e63 6865  mberto A. Sanche
+00000400: 7a20 4949 3c2f 613e 2020 2843 2920 3230  z II</a>  (C) 20
+00000410: 3233 0a0a 2323 204e 6f74 650a 466f 7220  23..## Note.For 
+00000420: 616c 6c20 6b69 6e64 206f 6620 7072 6f62  all kind of prob
+00000430: 6c65 6d73 2c20 7265 7175 6573 7473 2c20  lems, requests, 
+00000440: 656e 6861 6e63 656d 656e 7473 2c20 6275  enhancements, bu
+00000450: 6720 7265 706f 7274 732c 2065 7463 2e2c  g reports, etc.,
+00000460: 0a70 6c65 6173 6520 6472 6f70 206d 6520  .please drop me 
+00000470: 616e 2065 2d6d 6169 6c2e 0a0a 0a21 5b48  an e-mail....![H
+00000480: 756d 6265 7274 6f27 7320 4d6f 6469 6669  umberto's Modifi
+00000490: 6564 204c 6f67 6f5d 2868 7474 7073 3a2f  ed Logo](https:/
+000004a0: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+000004b0: 6f6e 7465 6e74 2e63 6f6d 2f77 696b 692f  ontent.com/wiki/
+000004c0: 6861 7369 6932 3031 312f 6769 7474 6f64  hasii2011/gittod
+000004d0: 6f69 7374 636c 6f6e 652f 696d 6167 6573  oistclone/images
+000004e0: 2f53 696c 6c79 4769 7448 7562 2e70 6e67  /SillyGitHub.png
+000004f0: 290a 0a49 2061 6d20 636f 6e63 6572 6e65  )..I am concerne
+00000500: 6420 6162 6f75 7420 4769 7448 7562 2773  d about GitHub's
+00000510: 2043 6f70 696c 6f74 2070 726f 6a65 6374   Copilot project
+00000520: 0a0a 0a0a 4920 7572 6765 2079 6f75 2074  ....I urge you t
+00000530: 6f20 7265 6164 2061 626f 7574 2074 6865  o read about the
+00000540: 205b 4769 7665 2075 7020 4769 7448 7562   [Give up GitHub
+00000550: 5d28 6874 7470 733a 2f2f 4769 7665 5570  ](https://GiveUp
+00000560: 4769 7448 7562 2e6f 7267 2920 6361 6d70  GitHub.org) camp
+00000570: 6169 676e 2066 726f 6d20 5b74 6865 2053  aign from [the S
+00000580: 6f66 7477 6172 6520 4672 6565 646f 6d20  oftware Freedom 
+00000590: 436f 6e73 6572 7661 6e63 795d 2868 7474  Conservancy](htt
+000005a0: 7073 3a2f 2f73 6663 6f6e 7365 7276 616e  ps://sfconservan
+000005b0: 6379 2e6f 7267 292e 0a0a 5768 696c 6520  cy.org)...While 
+000005c0: 4920 646f 206e 6f74 2061 6476 6f63 6174  I do not advocat
+000005d0: 6520 666f 7220 616c 6c20 7468 6520 6973  e for all the is
+000005e0: 7375 6573 206c 6973 7465 6420 7468 6572  sues listed ther
+000005f0: 6520 4920 646f 206e 6f74 206c 696b 6520  e I do not like 
+00000600: 7468 6174 2061 2063 6f6d 7061 6e79 206c  that a company l
+00000610: 696b 6520 4d69 6372 6f73 6f66 7420 6d61  ike Microsoft ma
+00000620: 7920 7072 6f66 6974 2066 726f 6d20 6f70  y profit from op
+00000630: 656e 2073 6f75 7263 6520 7072 6f6a 6563  en source projec
+00000640: 7473 2e0a 0a49 2063 6f6e 7469 6e75 6520  ts...I continue 
+00000650: 746f 2075 7365 2047 6974 4875 6220 6265  to use GitHub be
+00000660: 6361 7573 6520 6974 206f 6666 6572 7320  cause it offers 
+00000670: 7468 6520 7365 7276 6963 6573 2049 206e  the services I n
+00000680: 6565 6420 666f 7220 6672 6565 2e20 2042  eed for free.  B
+00000690: 7574 2c20 4920 636f 6e74 696e 7565 2074  ut, I continue t
+000006a0: 6f20 6d6f 6e69 746f 7220 7468 6569 7220  o monitor their 
+000006b0: 7465 726d 7320 6f66 2073 6572 7669 6365  terms of service
+000006c0: 2e0a 0a41 6e79 2075 7365 206f 6620 7468  ...Any use of th
+000006d0: 6973 2070 726f 6a65 6374 2773 2063 6f64  is project's cod
+000006e0: 6520 6279 2047 6974 4875 6220 436f 7069  e by GitHub Copi
+000006f0: 6c6f 742c 2070 6173 7420 6f72 2070 7265  lot, past or pre
+00000700: 7365 6e74 2c20 6973 2064 6f6e 6520 7769  sent, is done wi
+00000710: 7468 6f75 7420 6d79 2070 6572 6d69 7373  thout my permiss
+00000720: 696f 6e2e 2020 4920 646f 206e 6f74 2063  ion.  I do not c
+00000730: 6f6e 7365 6e74 2074 6f20 4769 7448 7562  onsent to GitHub
+00000740: 2773 2075 7365 206f 6620 7468 6973 2070  's use of this p
+00000750: 726f 6a65 6374 2773 0a63 6f64 6520 696e  roject's.code in
+00000760: 2043 6f70 696c 6f74 2e0a 0a41 2072 6570   Copilot...A rep
+00000770: 6f73 6974 6f72 7920 6f77 6e65 7220 6d61  ository owner ma
+00000780: 7920 6f70 7420 6f75 7420 6f66 2043 6f70  y opt out of Cop
+00000790: 696c 6f74 2062 7920 6368 616e 6769 6e67  ilot by changing
+000007a0: 2053 6574 7469 6e67 7320 2d2d 3e20 4769   Settings --> Gi
+000007b0: 7448 7562 2043 6f70 696c 6f74 2e0a 0a49  tHub Copilot...I
+000007c0: 2068 6176 6520 646f 6e65 2073 6f2e 0a     have done so..
```

### Comparing `ogl-0.70.22/ogl.egg-info/SOURCES.txt` & `ogl-0.70.25/ogl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ogl-0.70.22/setup.py` & `ogl-0.70.25/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 LICENSE = (HERE / 'LICENSE').read_text()
 
 setup(
     name="ogl",
-    version="0.70.22",
+    version="0.70.25",
     author='Humberto A. Sanchez II',
     author_email='Humberto.A.Sanchez.II@gmail.com',
     maintainer='Humberto A. Sanchez II',
     maintainer_email='humberto.a.sanchez.ii@gmail.com',
     description='External Pyut Graphical Shapes',
     long_description=README,
     long_description_content_type="text/markdown",
@@ -37,9 +37,9 @@
         'ogl',
         'ogl.events',
         'ogl.preferences',
         'ogl.resources', 'ogl.resources.img', 'ogl.resources.img.textdetails',
         'ogl.sd',
         'ogl.ui', 'ogl.ui.valuecontrols',
     ],
-    install_requires=['Deprecated~=1.2.13', 'pyutmodel==1.4.2', 'hasiihelper==0.1.0', 'hasiicommon==0.2.1', 'wxPython~=4.2.0'],
+    install_requires=['Deprecated~=1.2.13', 'pyutmodel==1.4.3', 'hasiihelper==0.2.0', 'hasiicommon==0.2.2', 'wxPython~=4.2.0'],
 )
```

