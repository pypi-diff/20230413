# Comparing `tmp/pyutmodel-1.4.2.tar.gz` & `tmp/pyutmodel-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyutmodel-1.4.2.tar", last modified: Sun Mar 26 21:00:03 2023, max compression
+gzip compressed data, was "pyutmodel-1.4.3.tar", last modified: Thu Apr 13 18:25:21 2023, max compression
```

## Comparing `pyutmodel-1.4.2.tar` & `pyutmodel-1.4.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-26 21:00:03.998727 pyutmodel-1.4.2/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-23 19:00:15.000000 pyutmodel-1.4.2/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1916 2023-03-26 21:00:03.998571 pyutmodel-1.4.2/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1585 2023-01-12 22:10:43.000000 pyutmodel-1.4.2/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-26 21:00:03.997545 pyutmodel-1.4.2/pyutmodel/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      174 2022-03-03 03:11:12.000000 pyutmodel-1.4.2/pyutmodel/DisplayMethodParameters.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      237 2023-01-26 17:37:55.000000 pyutmodel-1.4.2/pyutmodel/ModelTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      485 2022-05-18 15:25:38.000000 pyutmodel-1.4.2/pyutmodel/PyutActor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4721 2023-01-26 17:31:28.000000 pyutmodel-1.4.2/pyutmodel/PyutClass.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3270 2023-01-26 17:38:43.000000 pyutmodel-1.4.2/pyutmodel/PyutClassCommon.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1464 2022-03-14 02:19:43.000000 pyutmodel-1.4.2/pyutmodel/PyutDisplayParameters.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2178 2023-02-07 02:28:42.000000 pyutmodel-1.4.2/pyutmodel/PyutField.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1300 2023-01-26 17:31:00.000000 pyutmodel-1.4.2/pyutmodel/PyutInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5259 2023-03-22 16:22:13.000000 pyutmodel-1.4.2/pyutmodel/PyutLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1413 2022-03-27 17:27:56.000000 pyutmodel-1.4.2/pyutmodel/PyutLinkType.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3852 2023-01-26 17:32:44.000000 pyutmodel-1.4.2/pyutmodel/PyutLinkedObject.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8981 2023-02-06 15:37:30.000000 pyutmodel-1.4.2/pyutmodel/PyutMethod.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      828 2023-01-08 04:44:45.000000 pyutmodel-1.4.2/pyutmodel/PyutModifier.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1020 2023-01-26 16:44:25.000000 pyutmodel-1.4.2/pyutmodel/PyutNote.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2420 2022-03-15 21:36:23.000000 pyutmodel-1.4.2/pyutmodel/PyutObject.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2438 2023-02-07 16:16:50.000000 pyutmodel-1.4.2/pyutmodel/PyutParameter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2929 2022-05-18 01:48:45.000000 pyutmodel-1.4.2/pyutmodel/PyutSDInstance.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6123 2023-03-11 02:14:00.000000 pyutmodel-1.4.2/pyutmodel/PyutSDMessage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2747 2023-02-05 20:11:42.000000 pyutmodel-1.4.2/pyutmodel/PyutStereotype.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      591 2022-05-18 15:25:38.000000 pyutmodel-1.4.2/pyutmodel/PyutText.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      762 2022-03-14 02:23:07.000000 pyutmodel-1.4.2/pyutmodel/PyutType.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      184 2022-04-05 20:39:40.000000 pyutmodel-1.4.2/pyutmodel/PyutUseCase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1512 2022-03-23 16:04:17.000000 pyutmodel-1.4.2/pyutmodel/PyutVisibilityEnum.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2020-05-01 18:22:04.000000 pyutmodel-1.4.2/pyutmodel/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 pyutmodel-1.4.2/pyutmodel/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-26 21:00:03.998350 pyutmodel-1.4.2/pyutmodel.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1916 2023-03-26 21:00:03.000000 pyutmodel-1.4.2/pyutmodel.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      837 2023-03-26 21:00:03.000000 pyutmodel-1.4.2/pyutmodel.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-03-26 21:00:03.000000 pyutmodel-1.4.2/pyutmodel.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-03-26 21:00:03.000000 pyutmodel-1.4.2/pyutmodel.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       10 2023-03-26 21:00:03.000000 pyutmodel-1.4.2/pyutmodel.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-03-26 21:00:03.998763 pyutmodel-1.4.2/setup.cfg
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      780 2023-03-26 17:52:35.000000 pyutmodel-1.4.2/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:25:21.845472 pyutmodel-1.4.3/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-23 19:00:15.000000 pyutmodel-1.4.3/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2270 2023-04-13 18:25:21.845359 pyutmodel-1.4.3/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1939 2023-04-12 01:20:33.000000 pyutmodel-1.4.3/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:25:21.844572 pyutmodel-1.4.3/pyutmodel/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      174 2022-03-03 03:11:12.000000 pyutmodel-1.4.3/pyutmodel/DisplayMethodParameters.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      237 2023-01-26 17:37:55.000000 pyutmodel-1.4.3/pyutmodel/ModelTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      485 2022-05-18 15:25:38.000000 pyutmodel-1.4.3/pyutmodel/PyutActor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4721 2023-01-26 17:31:28.000000 pyutmodel-1.4.3/pyutmodel/PyutClass.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3270 2023-01-26 17:38:43.000000 pyutmodel-1.4.3/pyutmodel/PyutClassCommon.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1464 2022-03-14 02:19:43.000000 pyutmodel-1.4.3/pyutmodel/PyutDisplayParameters.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2178 2023-02-07 02:28:42.000000 pyutmodel-1.4.3/pyutmodel/PyutField.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1300 2023-01-26 17:31:00.000000 pyutmodel-1.4.3/pyutmodel/PyutInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5259 2023-03-22 16:22:13.000000 pyutmodel-1.4.3/pyutmodel/PyutLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1413 2022-03-27 17:27:56.000000 pyutmodel-1.4.3/pyutmodel/PyutLinkType.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3852 2023-01-26 17:32:44.000000 pyutmodel-1.4.3/pyutmodel/PyutLinkedObject.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8981 2023-02-06 15:37:30.000000 pyutmodel-1.4.3/pyutmodel/PyutMethod.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      828 2023-01-08 04:44:45.000000 pyutmodel-1.4.3/pyutmodel/PyutModifier.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1020 2023-01-26 16:44:25.000000 pyutmodel-1.4.3/pyutmodel/PyutNote.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2420 2022-03-15 21:36:23.000000 pyutmodel-1.4.3/pyutmodel/PyutObject.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2438 2023-02-07 16:16:50.000000 pyutmodel-1.4.3/pyutmodel/PyutParameter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2929 2022-05-18 01:48:45.000000 pyutmodel-1.4.3/pyutmodel/PyutSDInstance.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6123 2023-03-11 02:14:00.000000 pyutmodel-1.4.3/pyutmodel/PyutSDMessage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2747 2023-02-05 20:11:42.000000 pyutmodel-1.4.3/pyutmodel/PyutStereotype.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      591 2022-05-18 15:25:38.000000 pyutmodel-1.4.3/pyutmodel/PyutText.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      762 2022-03-14 02:23:07.000000 pyutmodel-1.4.3/pyutmodel/PyutType.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      184 2022-04-05 20:39:40.000000 pyutmodel-1.4.3/pyutmodel/PyutUseCase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1512 2022-03-23 16:04:17.000000 pyutmodel-1.4.3/pyutmodel/PyutVisibilityEnum.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2020-05-01 18:22:04.000000 pyutmodel-1.4.3/pyutmodel/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 pyutmodel-1.4.3/pyutmodel/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:25:21.845164 pyutmodel-1.4.3/pyutmodel.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2270 2023-04-13 18:25:21.000000 pyutmodel-1.4.3/pyutmodel.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      837 2023-04-13 18:25:21.000000 pyutmodel-1.4.3/pyutmodel.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-04-13 18:25:21.000000 pyutmodel-1.4.3/pyutmodel.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-04-13 18:25:21.000000 pyutmodel-1.4.3/pyutmodel.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       10 2023-04-13 18:25:21.000000 pyutmodel-1.4.3/pyutmodel.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-04-13 18:25:21.845501 pyutmodel-1.4.3/setup.cfg
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      780 2023-04-13 17:50:57.000000 pyutmodel-1.4.3/setup.py
```

### Comparing `pyutmodel-1.4.2/LICENSE` & `pyutmodel-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.2/PKG-INFO` & `pyutmodel-1.4.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 7574  : 2.1.Name: pyut
 00000020: 6d6f 6465 6c0a 5665 7273 696f 6e3a 2031  model.Version: 1
-00000030: 2e34 2e32 0a53 756d 6d61 7279 3a20 4578  .4.2.Summary: Ex
+00000030: 2e34 2e33 0a53 756d 6d61 7279 3a20 4578  .4.3.Summary: Ex
 00000040: 7465 726e 616c 2050 7975 7420 4461 7461  ternal Pyut Data
 00000050: 204d 6f64 656c 0a48 6f6d 652d 7061 6765   Model.Home-page
 00000060: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
 00000070: 2e63 6f6d 2f68 6173 6969 3230 3131 2f70  .com/hasii2011/p
 00000080: 7975 746d 6f64 656c 0a41 7574 686f 722d  yutmodel.Author-
 00000090: 656d 6169 6c3a 2048 756d 6265 7274 6f2e  email: Humberto.
 000000a0: 412e 5361 6e63 6865 7a2e 4949 4067 6d61  A.Sanchez.II@gma
@@ -59,62 +59,84 @@
 000003a0: 93a8 20f0 9d93 a420 f09d 93a3 2073 7461  .. .... .... sta
 000003b0: 6e64 7320 666f 7220 5079 7468 6f6e 2055  nds for Python U
 000003c0: 4d4c 2054 6f6f 6c2e 2054 6869 7320 6973  ML Tool. This is
 000003d0: 2074 6865 2065 7874 6572 6e61 6c20 6461   the external da
 000003e0: 7461 206d 6f64 656c 2066 6f72 2050 7975  ta model for Pyu
 000003f0: 740a 7468 6174 2061 6c6c 6f77 7320 666f  t.that allows fo
 00000400: 7220 6578 7465 726e 616c 2070 6c75 6769  r external plugi
-00000410: 6e20 6465 7665 6c6f 706d 656e 740a 0a0a  n development...
-00000420: 0a2d 2d2d 2d2d 2d0a 0a0a 215b 4875 6d62  .------...![Humb
-00000430: 6572 746f 2773 204d 6f64 6966 6965 6420  erto's Modified 
-00000440: 4c6f 676f 5d28 6874 7470 733a 2f2f 7261  Logo](https://ra
-00000450: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00000460: 656e 742e 636f 6d2f 7769 6b69 2f68 6173  ent.com/wiki/has
-00000470: 6969 3230 3131 2f67 6974 746f 646f 6973  ii2011/gittodois
-00000480: 7463 6c6f 6e65 2f69 6d61 6765 732f 5369  tclone/images/Si
-00000490: 6c6c 7947 6974 4875 622e 706e 6729 0a0a  llyGitHub.png)..
-000004a0: 4920 616d 2063 6f6e 6365 726e 6564 2061  I am concerned a
-000004b0: 626f 7574 2047 6974 4875 6227 7320 436f  bout GitHub's Co
-000004c0: 7069 6c6f 7420 7072 6f6a 6563 740a 0a0a  pilot project...
-000004d0: 0a49 2075 7267 6520 796f 7520 746f 2072  .I urge you to r
-000004e0: 6561 6420 6162 6f75 7420 7468 650a 5b47  ead about the.[G
-000004f0: 6976 6520 7570 2047 6974 4875 625d 2868  ive up GitHub](h
-00000500: 7474 7073 3a2f 2f47 6976 6555 7047 6974  ttps://GiveUpGit
-00000510: 4875 622e 6f72 6729 2063 616d 7061 6967  Hub.org) campaig
-00000520: 6e20 6672 6f6d 0a5b 7468 6520 536f 6674  n from.[the Soft
-00000530: 7761 7265 2046 7265 6564 6f6d 2043 6f6e  ware Freedom Con
-00000540: 7365 7276 616e 6379 5d28 6874 7470 733a  servancy](https:
-00000550: 2f2f 7366 636f 6e73 6572 7661 6e63 792e  //sfconservancy.
-00000560: 6f72 6729 2e0a 0a57 6869 6c65 2049 2064  org)...While I d
-00000570: 6f20 6e6f 7420 6164 766f 6361 7465 2066  o not advocate f
-00000580: 6f72 2061 6c6c 2074 6865 2069 7373 7565  or all the issue
-00000590: 7320 6c69 7374 6564 2074 6865 7265 2049  s listed there I
-000005a0: 2064 6f20 6e6f 7420 6c69 6b65 2074 6861   do not like tha
-000005b0: 740a 6120 636f 6d70 616e 7920 6c69 6b65  t.a company like
-000005c0: 204d 6963 726f 736f 6674 206d 6179 2070   Microsoft may p
-000005d0: 726f 6669 7420 6672 6f6d 206f 7065 6e20  rofit from open 
-000005e0: 736f 7572 6365 2070 726f 6a65 6374 732e  source projects.
-000005f0: 0a0a 4920 636f 6e74 696e 7565 2074 6f20  ..I continue to 
-00000600: 7573 6520 4769 7448 7562 2062 6563 6175  use GitHub becau
-00000610: 7365 2069 7420 6f66 6665 7273 2074 6865  se it offers the
-00000620: 2073 6572 7669 6365 7320 4920 6e65 6564   services I need
-00000630: 2066 6f72 2066 7265 652e 2020 4275 742c   for free.  But,
-00000640: 2049 2063 6f6e 7469 6e75 650a 746f 206d   I continue.to m
-00000650: 6f6e 6974 6f72 2074 6865 6972 2074 6572  onitor their ter
-00000660: 6d73 206f 6620 7365 7276 6963 652e 0a0a  ms of service...
-00000670: 416e 7920 7573 6520 6f66 2074 6869 7320  Any use of this 
-00000680: 7072 6f6a 6563 7427 7320 636f 6465 2062  project's code b
-00000690: 7920 4769 7448 7562 2043 6f70 696c 6f74  y GitHub Copilot
-000006a0: 2c20 7061 7374 206f 7220 7072 6573 656e  , past or presen
-000006b0: 742c 2069 7320 646f 6e65 0a77 6974 686f  t, is done.witho
-000006c0: 7574 206d 7920 7065 726d 6973 7369 6f6e  ut my permission
-000006d0: 2e20 2049 2064 6f20 6e6f 7420 636f 6e73  .  I do not cons
-000006e0: 656e 7420 746f 2047 6974 4875 6227 7320  ent to GitHub's 
-000006f0: 7573 6520 6f66 2074 6869 7320 7072 6f6a  use of this proj
-00000700: 6563 7427 730a 636f 6465 2069 6e20 436f  ect's.code in Co
-00000710: 7069 6c6f 742e 0a0a 4120 7265 706f 7369  pilot...A reposi
-00000720: 746f 7279 206f 776e 6572 206d 6179 206f  tory owner may o
-00000730: 7074 206f 7574 206f 6620 436f 7069 6c6f  pt out of Copilo
-00000740: 7420 6279 2063 6861 6e67 696e 6720 5365  t by changing Se
-00000750: 7474 696e 6773 202d 2d3e 2047 6974 4875  ttings --> GitHu
-00000760: 6220 436f 7069 6c6f 742e 0a0a 4920 6861  b Copilot...I ha
-00000770: 7665 2064 6f6e 6520 736f 2e0a            ve done so..
+00000410: 6e20 6465 7665 6c6f 706d 656e 740a 0a23  n development..#
+00000420: 2320 4465 7665 6c6f 7065 7220 4e6f 7465  # Developer Note
+00000430: 730a 5468 6973 2070 726f 6a65 6374 2075  s.This project u
+00000440: 7365 7320 5b62 7569 6c64 6c61 636b 6579  ses [buildlackey
+00000450: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000460: 2e63 6f6d 2f68 6173 6969 3230 3131 2f62  .com/hasii2011/b
+00000470: 7569 6c64 6c61 636b 6579 2920 666f 7220  uildlackey) for 
+00000480: 6461 7920 746f 2064 6179 2064 6576 656c  day to day devel
+00000490: 6f70 6d65 6e74 2062 7569 6c64 730a 0a5f  opment builds.._
+000004a0: 5f5f 0a0a 5772 6974 7465 6e20 6279 203c  __..Written by <
+000004b0: 6120 6872 6566 3d22 6d61 696c 746f 3a65  a href="mailto:e
+000004c0: 6d61 696c 4068 756d 6265 7274 6f2e 612e  mail@humberto.a.
+000004d0: 7361 6e63 6865 7a2e 6969 4067 6d61 696c  sanchez.ii@gmail
+000004e0: 2e63 6f6d 3f73 7562 6a65 6374 3d48 656c  .com?subject=Hel
+000004f0: 6c6f 2048 756d 6265 7274 6f22 3e48 756d  lo Humberto">Hum
+00000500: 6265 7274 6f20 412e 2053 616e 6368 657a  berto A. Sanchez
+00000510: 2049 493c 2f61 3e20 2028 4329 2032 3032   II</a>  (C) 202
+00000520: 330a 0a23 2320 4e6f 7465 0a46 6f72 2061  3..## Note.For a
+00000530: 6c6c 206b 696e 6420 6f66 2070 726f 626c  ll kind of probl
+00000540: 656d 732c 2072 6571 7565 7374 732c 2065  ems, requests, e
+00000550: 6e68 616e 6365 6d65 6e74 732c 2062 7567  nhancements, bug
+00000560: 2072 6570 6f72 7473 2c20 6574 632e 2c0a   reports, etc.,.
+00000570: 706c 6561 7365 2064 726f 7020 6d65 2061  please drop me a
+00000580: 6e20 652d 6d61 696c 2e0a 0a0a 215b 4875  n e-mail....![Hu
+00000590: 6d62 6572 746f 2773 204d 6f64 6966 6965  mberto's Modifie
+000005a0: 6420 4c6f 676f 5d28 6874 7470 733a 2f2f  d Logo](https://
+000005b0: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
+000005c0: 6e74 656e 742e 636f 6d2f 7769 6b69 2f68  ntent.com/wiki/h
+000005d0: 6173 6969 3230 3131 2f67 6974 746f 646f  asii2011/gittodo
+000005e0: 6973 7463 6c6f 6e65 2f69 6d61 6765 732f  istclone/images/
+000005f0: 5369 6c6c 7947 6974 4875 622e 706e 6729  SillyGitHub.png)
+00000600: 0a0a 4920 616d 2063 6f6e 6365 726e 6564  ..I am concerned
+00000610: 2061 626f 7574 2047 6974 4875 6227 7320   about GitHub's 
+00000620: 436f 7069 6c6f 7420 7072 6f6a 6563 740a  Copilot project.
+00000630: 0a0a 0a49 2075 7267 6520 796f 7520 746f  ...I urge you to
+00000640: 2072 6561 6420 6162 6f75 7420 7468 650a   read about the.
+00000650: 5b47 6976 6520 7570 2047 6974 4875 625d  [Give up GitHub]
+00000660: 2868 7474 7073 3a2f 2f47 6976 6555 7047  (https://GiveUpG
+00000670: 6974 4875 622e 6f72 6729 2063 616d 7061  itHub.org) campa
+00000680: 6967 6e20 6672 6f6d 0a5b 7468 6520 536f  ign from.[the So
+00000690: 6674 7761 7265 2046 7265 6564 6f6d 2043  ftware Freedom C
+000006a0: 6f6e 7365 7276 616e 6379 5d28 6874 7470  onservancy](http
+000006b0: 733a 2f2f 7366 636f 6e73 6572 7661 6e63  s://sfconservanc
+000006c0: 792e 6f72 6729 2e0a 0a57 6869 6c65 2049  y.org)...While I
+000006d0: 2064 6f20 6e6f 7420 6164 766f 6361 7465   do not advocate
+000006e0: 2066 6f72 2061 6c6c 2074 6865 2069 7373   for all the iss
+000006f0: 7565 7320 6c69 7374 6564 2074 6865 7265  ues listed there
+00000700: 2049 2064 6f20 6e6f 7420 6c69 6b65 2074   I do not like t
+00000710: 6861 740a 6120 636f 6d70 616e 7920 6c69  hat.a company li
+00000720: 6b65 204d 6963 726f 736f 6674 206d 6179  ke Microsoft may
+00000730: 2070 726f 6669 7420 6672 6f6d 206f 7065   profit from ope
+00000740: 6e20 736f 7572 6365 2070 726f 6a65 6374  n source project
+00000750: 732e 0a0a 4920 636f 6e74 696e 7565 2074  s...I continue t
+00000760: 6f20 7573 6520 4769 7448 7562 2062 6563  o use GitHub bec
+00000770: 6175 7365 2069 7420 6f66 6665 7273 2074  ause it offers t
+00000780: 6865 2073 6572 7669 6365 7320 4920 6e65  he services I ne
+00000790: 6564 2066 6f72 2066 7265 652e 2020 4275  ed for free.  Bu
+000007a0: 742c 2049 2063 6f6e 7469 6e75 650a 746f  t, I continue.to
+000007b0: 206d 6f6e 6974 6f72 2074 6865 6972 2074   monitor their t
+000007c0: 6572 6d73 206f 6620 7365 7276 6963 652e  erms of service.
+000007d0: 0a0a 416e 7920 7573 6520 6f66 2074 6869  ..Any use of thi
+000007e0: 7320 7072 6f6a 6563 7427 7320 636f 6465  s project's code
+000007f0: 2062 7920 4769 7448 7562 2043 6f70 696c   by GitHub Copil
+00000800: 6f74 2c20 7061 7374 206f 7220 7072 6573  ot, past or pres
+00000810: 656e 742c 2069 7320 646f 6e65 0a77 6974  ent, is done.wit
+00000820: 686f 7574 206d 7920 7065 726d 6973 7369  hout my permissi
+00000830: 6f6e 2e20 2049 2064 6f20 6e6f 7420 636f  on.  I do not co
+00000840: 6e73 656e 7420 746f 2047 6974 4875 6227  nsent to GitHub'
+00000850: 7320 7573 6520 6f66 2074 6869 7320 7072  s use of this pr
+00000860: 6f6a 6563 7427 730a 636f 6465 2069 6e20  oject's.code in 
+00000870: 436f 7069 6c6f 742e 0a0a 4120 7265 706f  Copilot...A repo
+00000880: 7369 746f 7279 206f 776e 6572 206d 6179  sitory owner may
+00000890: 206f 7074 206f 7574 206f 6620 436f 7069   opt out of Copi
+000008a0: 6c6f 7420 6279 2063 6861 6e67 696e 6720  lot by changing 
+000008b0: 5365 7474 696e 6773 202d 2d3e 2047 6974  Settings --> Git
+000008c0: 4875 6220 436f 7069 6c6f 742e 0a0a 4920  Hub Copilot...I 
+000008d0: 6861 7665 2064 6f6e 6520 736f 2e0a       have done so..
```

### Comparing `pyutmodel-1.4.2/README.md` & `pyutmodel-1.4.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -39,62 +39,84 @@
 00000260: a320 7374 616e 6473 2066 6f72 2050 7974  . stands for Pyt
 00000270: 686f 6e20 554d 4c20 546f 6f6c 2e20 5468  hon UML Tool. Th
 00000280: 6973 2069 7320 7468 6520 6578 7465 726e  is is the extern
 00000290: 616c 2064 6174 6120 6d6f 6465 6c20 666f  al data model fo
 000002a0: 7220 5079 7574 0a74 6861 7420 616c 6c6f  r Pyut.that allo
 000002b0: 7773 2066 6f72 2065 7874 6572 6e61 6c20  ws for external 
 000002c0: 706c 7567 696e 2064 6576 656c 6f70 6d65  plugin developme
-000002d0: 6e74 0a0a 0a0a 2d2d 2d2d 2d2d 0a0a 0a21  nt....------...!
-000002e0: 5b48 756d 6265 7274 6f27 7320 4d6f 6469  [Humberto's Modi
-000002f0: 6669 6564 204c 6f67 6f5d 2868 7474 7073  fied Logo](https
-00000300: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
-00000310: 7263 6f6e 7465 6e74 2e63 6f6d 2f77 696b  rcontent.com/wik
-00000320: 692f 6861 7369 6932 3031 312f 6769 7474  i/hasii2011/gitt
-00000330: 6f64 6f69 7374 636c 6f6e 652f 696d 6167  odoistclone/imag
-00000340: 6573 2f53 696c 6c79 4769 7448 7562 2e70  es/SillyGitHub.p
-00000350: 6e67 290a 0a49 2061 6d20 636f 6e63 6572  ng)..I am concer
-00000360: 6e65 6420 6162 6f75 7420 4769 7448 7562  ned about GitHub
-00000370: 2773 2043 6f70 696c 6f74 2070 726f 6a65  's Copilot proje
-00000380: 6374 0a0a 0a0a 4920 7572 6765 2079 6f75  ct....I urge you
-00000390: 2074 6f20 7265 6164 2061 626f 7574 2074   to read about t
-000003a0: 6865 0a5b 4769 7665 2075 7020 4769 7448  he.[Give up GitH
-000003b0: 7562 5d28 6874 7470 733a 2f2f 4769 7665  ub](https://Give
-000003c0: 5570 4769 7448 7562 2e6f 7267 2920 6361  UpGitHub.org) ca
-000003d0: 6d70 6169 676e 2066 726f 6d0a 5b74 6865  mpaign from.[the
-000003e0: 2053 6f66 7477 6172 6520 4672 6565 646f   Software Freedo
-000003f0: 6d20 436f 6e73 6572 7661 6e63 795d 2868  m Conservancy](h
-00000400: 7474 7073 3a2f 2f73 6663 6f6e 7365 7276  ttps://sfconserv
-00000410: 616e 6379 2e6f 7267 292e 0a0a 5768 696c  ancy.org)...Whil
-00000420: 6520 4920 646f 206e 6f74 2061 6476 6f63  e I do not advoc
-00000430: 6174 6520 666f 7220 616c 6c20 7468 6520  ate for all the 
-00000440: 6973 7375 6573 206c 6973 7465 6420 7468  issues listed th
-00000450: 6572 6520 4920 646f 206e 6f74 206c 696b  ere I do not lik
-00000460: 6520 7468 6174 0a61 2063 6f6d 7061 6e79  e that.a company
-00000470: 206c 696b 6520 4d69 6372 6f73 6f66 7420   like Microsoft 
-00000480: 6d61 7920 7072 6f66 6974 2066 726f 6d20  may profit from 
-00000490: 6f70 656e 2073 6f75 7263 6520 7072 6f6a  open source proj
-000004a0: 6563 7473 2e0a 0a49 2063 6f6e 7469 6e75  ects...I continu
-000004b0: 6520 746f 2075 7365 2047 6974 4875 6220  e to use GitHub 
-000004c0: 6265 6361 7573 6520 6974 206f 6666 6572  because it offer
-000004d0: 7320 7468 6520 7365 7276 6963 6573 2049  s the services I
-000004e0: 206e 6565 6420 666f 7220 6672 6565 2e20   need for free. 
-000004f0: 2042 7574 2c20 4920 636f 6e74 696e 7565   But, I continue
-00000500: 0a74 6f20 6d6f 6e69 746f 7220 7468 6569  .to monitor thei
-00000510: 7220 7465 726d 7320 6f66 2073 6572 7669  r terms of servi
-00000520: 6365 2e0a 0a41 6e79 2075 7365 206f 6620  ce...Any use of 
-00000530: 7468 6973 2070 726f 6a65 6374 2773 2063  this project's c
-00000540: 6f64 6520 6279 2047 6974 4875 6220 436f  ode by GitHub Co
-00000550: 7069 6c6f 742c 2070 6173 7420 6f72 2070  pilot, past or p
-00000560: 7265 7365 6e74 2c20 6973 2064 6f6e 650a  resent, is done.
-00000570: 7769 7468 6f75 7420 6d79 2070 6572 6d69  without my permi
-00000580: 7373 696f 6e2e 2020 4920 646f 206e 6f74  ssion.  I do not
-00000590: 2063 6f6e 7365 6e74 2074 6f20 4769 7448   consent to GitH
-000005a0: 7562 2773 2075 7365 206f 6620 7468 6973  ub's use of this
-000005b0: 2070 726f 6a65 6374 2773 0a63 6f64 6520   project's.code 
-000005c0: 696e 2043 6f70 696c 6f74 2e0a 0a41 2072  in Copilot...A r
-000005d0: 6570 6f73 6974 6f72 7920 6f77 6e65 7220  epository owner 
-000005e0: 6d61 7920 6f70 7420 6f75 7420 6f66 2043  may opt out of C
-000005f0: 6f70 696c 6f74 2062 7920 6368 616e 6769  opilot by changi
-00000600: 6e67 2053 6574 7469 6e67 7320 2d2d 3e20  ng Settings --> 
-00000610: 4769 7448 7562 2043 6f70 696c 6f74 2e0a  GitHub Copilot..
-00000620: 0a49 2068 6176 6520 646f 6e65 2073 6f2e  .I have done so.
-00000630: 0a                                       .
+000002d0: 6e74 0a0a 2323 2044 6576 656c 6f70 6572  nt..## Developer
+000002e0: 204e 6f74 6573 0a54 6869 7320 7072 6f6a   Notes.This proj
+000002f0: 6563 7420 7573 6573 205b 6275 696c 646c  ect uses [buildl
+00000300: 6163 6b65 795d 2868 7474 7073 3a2f 2f67  ackey](https://g
+00000310: 6974 6875 622e 636f 6d2f 6861 7369 6932  ithub.com/hasii2
+00000320: 3031 312f 6275 696c 646c 6163 6b65 7929  011/buildlackey)
+00000330: 2066 6f72 2064 6179 2074 6f20 6461 7920   for day to day 
+00000340: 6465 7665 6c6f 706d 656e 7420 6275 696c  development buil
+00000350: 6473 0a0a 5f5f 5f0a 0a57 7269 7474 656e  ds..___..Written
+00000360: 2062 7920 3c61 2068 7265 663d 226d 6169   by <a href="mai
+00000370: 6c74 6f3a 656d 6169 6c40 6875 6d62 6572  lto:email@humber
+00000380: 746f 2e61 2e73 616e 6368 657a 2e69 6940  to.a.sanchez.ii@
+00000390: 676d 6169 6c2e 636f 6d3f 7375 626a 6563  gmail.com?subjec
+000003a0: 743d 4865 6c6c 6f20 4875 6d62 6572 746f  t=Hello Humberto
+000003b0: 223e 4875 6d62 6572 746f 2041 2e20 5361  ">Humberto A. Sa
+000003c0: 6e63 6865 7a20 4949 3c2f 613e 2020 2843  nchez II</a>  (C
+000003d0: 2920 3230 3233 0a0a 2323 204e 6f74 650a  ) 2023..## Note.
+000003e0: 466f 7220 616c 6c20 6b69 6e64 206f 6620  For all kind of 
+000003f0: 7072 6f62 6c65 6d73 2c20 7265 7175 6573  problems, reques
+00000400: 7473 2c20 656e 6861 6e63 656d 656e 7473  ts, enhancements
+00000410: 2c20 6275 6720 7265 706f 7274 732c 2065  , bug reports, e
+00000420: 7463 2e2c 0a70 6c65 6173 6520 6472 6f70  tc.,.please drop
+00000430: 206d 6520 616e 2065 2d6d 6169 6c2e 0a0a   me an e-mail...
+00000440: 0a21 5b48 756d 6265 7274 6f27 7320 4d6f  .![Humberto's Mo
+00000450: 6469 6669 6564 204c 6f67 6f5d 2868 7474  dified Logo](htt
+00000460: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00000470: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f77  sercontent.com/w
+00000480: 696b 692f 6861 7369 6932 3031 312f 6769  iki/hasii2011/gi
+00000490: 7474 6f64 6f69 7374 636c 6f6e 652f 696d  ttodoistclone/im
+000004a0: 6167 6573 2f53 696c 6c79 4769 7448 7562  ages/SillyGitHub
+000004b0: 2e70 6e67 290a 0a49 2061 6d20 636f 6e63  .png)..I am conc
+000004c0: 6572 6e65 6420 6162 6f75 7420 4769 7448  erned about GitH
+000004d0: 7562 2773 2043 6f70 696c 6f74 2070 726f  ub's Copilot pro
+000004e0: 6a65 6374 0a0a 0a0a 4920 7572 6765 2079  ject....I urge y
+000004f0: 6f75 2074 6f20 7265 6164 2061 626f 7574  ou to read about
+00000500: 2074 6865 0a5b 4769 7665 2075 7020 4769   the.[Give up Gi
+00000510: 7448 7562 5d28 6874 7470 733a 2f2f 4769  tHub](https://Gi
+00000520: 7665 5570 4769 7448 7562 2e6f 7267 2920  veUpGitHub.org) 
+00000530: 6361 6d70 6169 676e 2066 726f 6d0a 5b74  campaign from.[t
+00000540: 6865 2053 6f66 7477 6172 6520 4672 6565  he Software Free
+00000550: 646f 6d20 436f 6e73 6572 7661 6e63 795d  dom Conservancy]
+00000560: 2868 7474 7073 3a2f 2f73 6663 6f6e 7365  (https://sfconse
+00000570: 7276 616e 6379 2e6f 7267 292e 0a0a 5768  rvancy.org)...Wh
+00000580: 696c 6520 4920 646f 206e 6f74 2061 6476  ile I do not adv
+00000590: 6f63 6174 6520 666f 7220 616c 6c20 7468  ocate for all th
+000005a0: 6520 6973 7375 6573 206c 6973 7465 6420  e issues listed 
+000005b0: 7468 6572 6520 4920 646f 206e 6f74 206c  there I do not l
+000005c0: 696b 6520 7468 6174 0a61 2063 6f6d 7061  ike that.a compa
+000005d0: 6e79 206c 696b 6520 4d69 6372 6f73 6f66  ny like Microsof
+000005e0: 7420 6d61 7920 7072 6f66 6974 2066 726f  t may profit fro
+000005f0: 6d20 6f70 656e 2073 6f75 7263 6520 7072  m open source pr
+00000600: 6f6a 6563 7473 2e0a 0a49 2063 6f6e 7469  ojects...I conti
+00000610: 6e75 6520 746f 2075 7365 2047 6974 4875  nue to use GitHu
+00000620: 6220 6265 6361 7573 6520 6974 206f 6666  b because it off
+00000630: 6572 7320 7468 6520 7365 7276 6963 6573  ers the services
+00000640: 2049 206e 6565 6420 666f 7220 6672 6565   I need for free
+00000650: 2e20 2042 7574 2c20 4920 636f 6e74 696e  .  But, I contin
+00000660: 7565 0a74 6f20 6d6f 6e69 746f 7220 7468  ue.to monitor th
+00000670: 6569 7220 7465 726d 7320 6f66 2073 6572  eir terms of ser
+00000680: 7669 6365 2e0a 0a41 6e79 2075 7365 206f  vice...Any use o
+00000690: 6620 7468 6973 2070 726f 6a65 6374 2773  f this project's
+000006a0: 2063 6f64 6520 6279 2047 6974 4875 6220   code by GitHub 
+000006b0: 436f 7069 6c6f 742c 2070 6173 7420 6f72  Copilot, past or
+000006c0: 2070 7265 7365 6e74 2c20 6973 2064 6f6e   present, is don
+000006d0: 650a 7769 7468 6f75 7420 6d79 2070 6572  e.without my per
+000006e0: 6d69 7373 696f 6e2e 2020 4920 646f 206e  mission.  I do n
+000006f0: 6f74 2063 6f6e 7365 6e74 2074 6f20 4769  ot consent to Gi
+00000700: 7448 7562 2773 2075 7365 206f 6620 7468  tHub's use of th
+00000710: 6973 2070 726f 6a65 6374 2773 0a63 6f64  is project's.cod
+00000720: 6520 696e 2043 6f70 696c 6f74 2e0a 0a41  e in Copilot...A
+00000730: 2072 6570 6f73 6974 6f72 7920 6f77 6e65   repository owne
+00000740: 7220 6d61 7920 6f70 7420 6f75 7420 6f66  r may opt out of
+00000750: 2043 6f70 696c 6f74 2062 7920 6368 616e   Copilot by chan
+00000760: 6769 6e67 2053 6574 7469 6e67 7320 2d2d  ging Settings --
+00000770: 3e20 4769 7448 7562 2043 6f70 696c 6f74  > GitHub Copilot
+00000780: 2e0a 0a49 2068 6176 6520 646f 6e65 2073  ...I have done s
+00000790: 6f2e 0a                                  o..
```

### Comparing `pyutmodel-1.4.2/pyutmodel/PyutClass.py` & `pyutmodel-1.4.3/pyutmodel/PyutClass.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.2/pyutmodel/PyutClassCommon.py` & `pyutmodel-1.4.3/pyutmodel/PyutClassCommon.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.2/pyutmodel/PyutDisplayParameters.py` & `pyutmodel-1.4.3/pyutmodel/PyutDisplayParameters.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.2/pyutmodel/PyutField.py` & `pyutmodel-1.4.3/pyutmodel/PyutField.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.2/pyutmodel/PyutInterface.py` & `pyutmodel-1.4.3/pyutmodel/PyutInterface.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.2/pyutmodel/PyutLink.py` & `pyutmodel-1.4.3/pyutmodel/PyutLink.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.2/pyutmodel/PyutLinkType.py` & `pyutmodel-1.4.3/pyutmodel/PyutLinkType.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.2/pyutmodel/PyutLinkedObject.py` & `pyutmodel-1.4.3/pyutmodel/PyutLinkedObject.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.2/pyutmodel/PyutMethod.py` & `pyutmodel-1.4.3/pyutmodel/PyutMethod.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.2/pyutmodel/PyutModifier.py` & `pyutmodel-1.4.3/pyutmodel/PyutModifier.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.2/pyutmodel/PyutNote.py` & `pyutmodel-1.4.3/pyutmodel/PyutNote.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.2/pyutmodel/PyutObject.py` & `pyutmodel-1.4.3/pyutmodel/PyutObject.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.2/pyutmodel/PyutParameter.py` & `pyutmodel-1.4.3/pyutmodel/PyutParameter.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.2/pyutmodel/PyutSDInstance.py` & `pyutmodel-1.4.3/pyutmodel/PyutSDInstance.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.2/pyutmodel/PyutSDMessage.py` & `pyutmodel-1.4.3/pyutmodel/PyutSDMessage.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.2/pyutmodel/PyutStereotype.py` & `pyutmodel-1.4.3/pyutmodel/PyutStereotype.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.2/pyutmodel/PyutText.py` & `pyutmodel-1.4.3/pyutmodel/PyutText.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.2/pyutmodel/PyutType.py` & `pyutmodel-1.4.3/pyutmodel/PyutType.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.2/pyutmodel/PyutVisibilityEnum.py` & `pyutmodel-1.4.3/pyutmodel/PyutVisibilityEnum.py`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.2/pyutmodel.egg-info/PKG-INFO` & `pyutmodel-1.4.3/pyutmodel.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 7574  : 2.1.Name: pyut
 00000020: 6d6f 6465 6c0a 5665 7273 696f 6e3a 2031  model.Version: 1
-00000030: 2e34 2e32 0a53 756d 6d61 7279 3a20 4578  .4.2.Summary: Ex
+00000030: 2e34 2e33 0a53 756d 6d61 7279 3a20 4578  .4.3.Summary: Ex
 00000040: 7465 726e 616c 2050 7975 7420 4461 7461  ternal Pyut Data
 00000050: 204d 6f64 656c 0a48 6f6d 652d 7061 6765   Model.Home-page
 00000060: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
 00000070: 2e63 6f6d 2f68 6173 6969 3230 3131 2f70  .com/hasii2011/p
 00000080: 7975 746d 6f64 656c 0a41 7574 686f 722d  yutmodel.Author-
 00000090: 656d 6169 6c3a 2048 756d 6265 7274 6f2e  email: Humberto.
 000000a0: 412e 5361 6e63 6865 7a2e 4949 4067 6d61  A.Sanchez.II@gma
@@ -59,62 +59,84 @@
 000003a0: 93a8 20f0 9d93 a420 f09d 93a3 2073 7461  .. .... .... sta
 000003b0: 6e64 7320 666f 7220 5079 7468 6f6e 2055  nds for Python U
 000003c0: 4d4c 2054 6f6f 6c2e 2054 6869 7320 6973  ML Tool. This is
 000003d0: 2074 6865 2065 7874 6572 6e61 6c20 6461   the external da
 000003e0: 7461 206d 6f64 656c 2066 6f72 2050 7975  ta model for Pyu
 000003f0: 740a 7468 6174 2061 6c6c 6f77 7320 666f  t.that allows fo
 00000400: 7220 6578 7465 726e 616c 2070 6c75 6769  r external plugi
-00000410: 6e20 6465 7665 6c6f 706d 656e 740a 0a0a  n development...
-00000420: 0a2d 2d2d 2d2d 2d0a 0a0a 215b 4875 6d62  .------...![Humb
-00000430: 6572 746f 2773 204d 6f64 6966 6965 6420  erto's Modified 
-00000440: 4c6f 676f 5d28 6874 7470 733a 2f2f 7261  Logo](https://ra
-00000450: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00000460: 656e 742e 636f 6d2f 7769 6b69 2f68 6173  ent.com/wiki/has
-00000470: 6969 3230 3131 2f67 6974 746f 646f 6973  ii2011/gittodois
-00000480: 7463 6c6f 6e65 2f69 6d61 6765 732f 5369  tclone/images/Si
-00000490: 6c6c 7947 6974 4875 622e 706e 6729 0a0a  llyGitHub.png)..
-000004a0: 4920 616d 2063 6f6e 6365 726e 6564 2061  I am concerned a
-000004b0: 626f 7574 2047 6974 4875 6227 7320 436f  bout GitHub's Co
-000004c0: 7069 6c6f 7420 7072 6f6a 6563 740a 0a0a  pilot project...
-000004d0: 0a49 2075 7267 6520 796f 7520 746f 2072  .I urge you to r
-000004e0: 6561 6420 6162 6f75 7420 7468 650a 5b47  ead about the.[G
-000004f0: 6976 6520 7570 2047 6974 4875 625d 2868  ive up GitHub](h
-00000500: 7474 7073 3a2f 2f47 6976 6555 7047 6974  ttps://GiveUpGit
-00000510: 4875 622e 6f72 6729 2063 616d 7061 6967  Hub.org) campaig
-00000520: 6e20 6672 6f6d 0a5b 7468 6520 536f 6674  n from.[the Soft
-00000530: 7761 7265 2046 7265 6564 6f6d 2043 6f6e  ware Freedom Con
-00000540: 7365 7276 616e 6379 5d28 6874 7470 733a  servancy](https:
-00000550: 2f2f 7366 636f 6e73 6572 7661 6e63 792e  //sfconservancy.
-00000560: 6f72 6729 2e0a 0a57 6869 6c65 2049 2064  org)...While I d
-00000570: 6f20 6e6f 7420 6164 766f 6361 7465 2066  o not advocate f
-00000580: 6f72 2061 6c6c 2074 6865 2069 7373 7565  or all the issue
-00000590: 7320 6c69 7374 6564 2074 6865 7265 2049  s listed there I
-000005a0: 2064 6f20 6e6f 7420 6c69 6b65 2074 6861   do not like tha
-000005b0: 740a 6120 636f 6d70 616e 7920 6c69 6b65  t.a company like
-000005c0: 204d 6963 726f 736f 6674 206d 6179 2070   Microsoft may p
-000005d0: 726f 6669 7420 6672 6f6d 206f 7065 6e20  rofit from open 
-000005e0: 736f 7572 6365 2070 726f 6a65 6374 732e  source projects.
-000005f0: 0a0a 4920 636f 6e74 696e 7565 2074 6f20  ..I continue to 
-00000600: 7573 6520 4769 7448 7562 2062 6563 6175  use GitHub becau
-00000610: 7365 2069 7420 6f66 6665 7273 2074 6865  se it offers the
-00000620: 2073 6572 7669 6365 7320 4920 6e65 6564   services I need
-00000630: 2066 6f72 2066 7265 652e 2020 4275 742c   for free.  But,
-00000640: 2049 2063 6f6e 7469 6e75 650a 746f 206d   I continue.to m
-00000650: 6f6e 6974 6f72 2074 6865 6972 2074 6572  onitor their ter
-00000660: 6d73 206f 6620 7365 7276 6963 652e 0a0a  ms of service...
-00000670: 416e 7920 7573 6520 6f66 2074 6869 7320  Any use of this 
-00000680: 7072 6f6a 6563 7427 7320 636f 6465 2062  project's code b
-00000690: 7920 4769 7448 7562 2043 6f70 696c 6f74  y GitHub Copilot
-000006a0: 2c20 7061 7374 206f 7220 7072 6573 656e  , past or presen
-000006b0: 742c 2069 7320 646f 6e65 0a77 6974 686f  t, is done.witho
-000006c0: 7574 206d 7920 7065 726d 6973 7369 6f6e  ut my permission
-000006d0: 2e20 2049 2064 6f20 6e6f 7420 636f 6e73  .  I do not cons
-000006e0: 656e 7420 746f 2047 6974 4875 6227 7320  ent to GitHub's 
-000006f0: 7573 6520 6f66 2074 6869 7320 7072 6f6a  use of this proj
-00000700: 6563 7427 730a 636f 6465 2069 6e20 436f  ect's.code in Co
-00000710: 7069 6c6f 742e 0a0a 4120 7265 706f 7369  pilot...A reposi
-00000720: 746f 7279 206f 776e 6572 206d 6179 206f  tory owner may o
-00000730: 7074 206f 7574 206f 6620 436f 7069 6c6f  pt out of Copilo
-00000740: 7420 6279 2063 6861 6e67 696e 6720 5365  t by changing Se
-00000750: 7474 696e 6773 202d 2d3e 2047 6974 4875  ttings --> GitHu
-00000760: 6220 436f 7069 6c6f 742e 0a0a 4920 6861  b Copilot...I ha
-00000770: 7665 2064 6f6e 6520 736f 2e0a            ve done so..
+00000410: 6e20 6465 7665 6c6f 706d 656e 740a 0a23  n development..#
+00000420: 2320 4465 7665 6c6f 7065 7220 4e6f 7465  # Developer Note
+00000430: 730a 5468 6973 2070 726f 6a65 6374 2075  s.This project u
+00000440: 7365 7320 5b62 7569 6c64 6c61 636b 6579  ses [buildlackey
+00000450: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000460: 2e63 6f6d 2f68 6173 6969 3230 3131 2f62  .com/hasii2011/b
+00000470: 7569 6c64 6c61 636b 6579 2920 666f 7220  uildlackey) for 
+00000480: 6461 7920 746f 2064 6179 2064 6576 656c  day to day devel
+00000490: 6f70 6d65 6e74 2062 7569 6c64 730a 0a5f  opment builds.._
+000004a0: 5f5f 0a0a 5772 6974 7465 6e20 6279 203c  __..Written by <
+000004b0: 6120 6872 6566 3d22 6d61 696c 746f 3a65  a href="mailto:e
+000004c0: 6d61 696c 4068 756d 6265 7274 6f2e 612e  mail@humberto.a.
+000004d0: 7361 6e63 6865 7a2e 6969 4067 6d61 696c  sanchez.ii@gmail
+000004e0: 2e63 6f6d 3f73 7562 6a65 6374 3d48 656c  .com?subject=Hel
+000004f0: 6c6f 2048 756d 6265 7274 6f22 3e48 756d  lo Humberto">Hum
+00000500: 6265 7274 6f20 412e 2053 616e 6368 657a  berto A. Sanchez
+00000510: 2049 493c 2f61 3e20 2028 4329 2032 3032   II</a>  (C) 202
+00000520: 330a 0a23 2320 4e6f 7465 0a46 6f72 2061  3..## Note.For a
+00000530: 6c6c 206b 696e 6420 6f66 2070 726f 626c  ll kind of probl
+00000540: 656d 732c 2072 6571 7565 7374 732c 2065  ems, requests, e
+00000550: 6e68 616e 6365 6d65 6e74 732c 2062 7567  nhancements, bug
+00000560: 2072 6570 6f72 7473 2c20 6574 632e 2c0a   reports, etc.,.
+00000570: 706c 6561 7365 2064 726f 7020 6d65 2061  please drop me a
+00000580: 6e20 652d 6d61 696c 2e0a 0a0a 215b 4875  n e-mail....![Hu
+00000590: 6d62 6572 746f 2773 204d 6f64 6966 6965  mberto's Modifie
+000005a0: 6420 4c6f 676f 5d28 6874 7470 733a 2f2f  d Logo](https://
+000005b0: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
+000005c0: 6e74 656e 742e 636f 6d2f 7769 6b69 2f68  ntent.com/wiki/h
+000005d0: 6173 6969 3230 3131 2f67 6974 746f 646f  asii2011/gittodo
+000005e0: 6973 7463 6c6f 6e65 2f69 6d61 6765 732f  istclone/images/
+000005f0: 5369 6c6c 7947 6974 4875 622e 706e 6729  SillyGitHub.png)
+00000600: 0a0a 4920 616d 2063 6f6e 6365 726e 6564  ..I am concerned
+00000610: 2061 626f 7574 2047 6974 4875 6227 7320   about GitHub's 
+00000620: 436f 7069 6c6f 7420 7072 6f6a 6563 740a  Copilot project.
+00000630: 0a0a 0a49 2075 7267 6520 796f 7520 746f  ...I urge you to
+00000640: 2072 6561 6420 6162 6f75 7420 7468 650a   read about the.
+00000650: 5b47 6976 6520 7570 2047 6974 4875 625d  [Give up GitHub]
+00000660: 2868 7474 7073 3a2f 2f47 6976 6555 7047  (https://GiveUpG
+00000670: 6974 4875 622e 6f72 6729 2063 616d 7061  itHub.org) campa
+00000680: 6967 6e20 6672 6f6d 0a5b 7468 6520 536f  ign from.[the So
+00000690: 6674 7761 7265 2046 7265 6564 6f6d 2043  ftware Freedom C
+000006a0: 6f6e 7365 7276 616e 6379 5d28 6874 7470  onservancy](http
+000006b0: 733a 2f2f 7366 636f 6e73 6572 7661 6e63  s://sfconservanc
+000006c0: 792e 6f72 6729 2e0a 0a57 6869 6c65 2049  y.org)...While I
+000006d0: 2064 6f20 6e6f 7420 6164 766f 6361 7465   do not advocate
+000006e0: 2066 6f72 2061 6c6c 2074 6865 2069 7373   for all the iss
+000006f0: 7565 7320 6c69 7374 6564 2074 6865 7265  ues listed there
+00000700: 2049 2064 6f20 6e6f 7420 6c69 6b65 2074   I do not like t
+00000710: 6861 740a 6120 636f 6d70 616e 7920 6c69  hat.a company li
+00000720: 6b65 204d 6963 726f 736f 6674 206d 6179  ke Microsoft may
+00000730: 2070 726f 6669 7420 6672 6f6d 206f 7065   profit from ope
+00000740: 6e20 736f 7572 6365 2070 726f 6a65 6374  n source project
+00000750: 732e 0a0a 4920 636f 6e74 696e 7565 2074  s...I continue t
+00000760: 6f20 7573 6520 4769 7448 7562 2062 6563  o use GitHub bec
+00000770: 6175 7365 2069 7420 6f66 6665 7273 2074  ause it offers t
+00000780: 6865 2073 6572 7669 6365 7320 4920 6e65  he services I ne
+00000790: 6564 2066 6f72 2066 7265 652e 2020 4275  ed for free.  Bu
+000007a0: 742c 2049 2063 6f6e 7469 6e75 650a 746f  t, I continue.to
+000007b0: 206d 6f6e 6974 6f72 2074 6865 6972 2074   monitor their t
+000007c0: 6572 6d73 206f 6620 7365 7276 6963 652e  erms of service.
+000007d0: 0a0a 416e 7920 7573 6520 6f66 2074 6869  ..Any use of thi
+000007e0: 7320 7072 6f6a 6563 7427 7320 636f 6465  s project's code
+000007f0: 2062 7920 4769 7448 7562 2043 6f70 696c   by GitHub Copil
+00000800: 6f74 2c20 7061 7374 206f 7220 7072 6573  ot, past or pres
+00000810: 656e 742c 2069 7320 646f 6e65 0a77 6974  ent, is done.wit
+00000820: 686f 7574 206d 7920 7065 726d 6973 7369  hout my permissi
+00000830: 6f6e 2e20 2049 2064 6f20 6e6f 7420 636f  on.  I do not co
+00000840: 6e73 656e 7420 746f 2047 6974 4875 6227  nsent to GitHub'
+00000850: 7320 7573 6520 6f66 2074 6869 7320 7072  s use of this pr
+00000860: 6f6a 6563 7427 730a 636f 6465 2069 6e20  oject's.code in 
+00000870: 436f 7069 6c6f 742e 0a0a 4120 7265 706f  Copilot...A repo
+00000880: 7369 746f 7279 206f 776e 6572 206d 6179  sitory owner may
+00000890: 206f 7074 206f 7574 206f 6620 436f 7069   opt out of Copi
+000008a0: 6c6f 7420 6279 2063 6861 6e67 696e 6720  lot by changing 
+000008b0: 5365 7474 696e 6773 202d 2d3e 2047 6974  Settings --> Git
+000008c0: 4875 6220 436f 7069 6c6f 742e 0a0a 4920  Hub Copilot...I 
+000008d0: 6861 7665 2064 6f6e 6520 736f 2e0a       have done so..
```

### Comparing `pyutmodel-1.4.2/pyutmodel.egg-info/SOURCES.txt` & `pyutmodel-1.4.3/pyutmodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyutmodel-1.4.2/setup.py` & `pyutmodel-1.4.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 LICENSE = (HERE / 'LICENSE').read_text()
 
 setup(
     name="pyutmodel",
-    version="1.4.2",
+    version="1.4.3",
     author_email='Humberto.A.Sanchez.II@gmail.com',
     maintainer='Humberto A. Sanchez II',
     maintainer_email='humberto.a.sanchez.ii@gmail.com',
     description='External Pyut Data Model',
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/hasii2011/pyutmodel",
     packages=[
         'pyutmodel',
     ],
     package_data={
         'pyutmodel': ['py.typed'],
     },
-    install_requires=['hasiihelper==0.1.0', 'Deprecated==1.2.13'],
+    install_requires=['hasiihelper~=0.2.0', 'Deprecated==1.2.13'],
 )
```

