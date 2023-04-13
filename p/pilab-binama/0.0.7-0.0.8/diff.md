# Comparing `tmp/pilab-binama-0.0.7.tar.gz` & `tmp/pilab-binama-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilab-binama-0.0.7.tar", last modified: Mon Mar 27 15:20:23 2023, max compression
+gzip compressed data, was "pilab-binama-0.0.8.tar", last modified: Thu Apr 13 09:48:10 2023, max compression
```

## Comparing `pilab-binama-0.0.7.tar` & `pilab-binama-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 15:20:23.470000 pilab-binama-0.0.7/
--rw-rw-rw-   0        0        0    35823 2022-12-21 15:02:10.000000 pilab-binama-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     2566 2023-03-27 15:20:24.000000 pilab-binama-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2190 2023-02-01 10:39:52.000000 pilab-binama-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-03-27 15:20:23.480000 pilab-binama-0.0.7/binama/
--rw-rw-rw-   0        0        0       70 2023-03-27 15:20:00.000000 pilab-binama-0.0.7/binama/__init__.py
--rw-rw-rw-   0        0        0      553 2022-12-21 12:10:20.000000 pilab-binama-0.0.7/binama/example.py
--rw-rw-rw-   0        0        0    11975 2023-03-27 14:24:52.000000 pilab-binama-0.0.7/binama/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-27 15:20:23.480000 pilab-binama-0.0.7/pilab_binama.egg-info/
--rw-rw-rw-   0        0        0     2566 2023-03-27 15:20:24.000000 pilab-binama-0.0.7/pilab_binama.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-03-27 15:20:24.000000 pilab-binama-0.0.7/pilab_binama.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 15:20:24.000000 pilab-binama-0.0.7/pilab_binama.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-03-27 15:20:24.000000 pilab-binama-0.0.7/pilab_binama.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-27 15:20:24.000000 pilab-binama-0.0.7/pilab_binama.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-27 15:20:24.000000 pilab-binama-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      794 2022-12-21 14:34:36.000000 pilab-binama-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:48:10.200000 pilab-binama-0.0.8/
+-rw-rw-rw-   0        0        0    35823 2022-12-21 15:02:10.000000 pilab-binama-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2566 2023-04-13 09:48:12.000000 pilab-binama-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2190 2023-02-01 10:39:52.000000 pilab-binama-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 09:48:10.210000 pilab-binama-0.0.8/binama/
+-rw-rw-rw-   0        0        0       70 2023-04-13 09:47:42.000000 pilab-binama-0.0.8/binama/__init__.py
+-rw-rw-rw-   0        0        0      553 2022-12-21 12:10:20.000000 pilab-binama-0.0.8/binama/example.py
+-rw-rw-rw-   0        0        0    13722 2023-04-13 09:44:22.000000 pilab-binama-0.0.8/binama/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:48:10.210000 pilab-binama-0.0.8/pilab_binama.egg-info/
+-rw-rw-rw-   0        0        0     2566 2023-04-13 09:48:12.000000 pilab-binama-0.0.8/pilab_binama.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-04-13 09:48:12.000000 pilab-binama-0.0.8/pilab_binama.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 09:48:12.000000 pilab-binama-0.0.8/pilab_binama.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-13 09:48:12.000000 pilab-binama-0.0.8/pilab_binama.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-13 09:48:12.000000 pilab-binama-0.0.8/pilab_binama.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 09:48:12.000000 pilab-binama-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      794 2022-12-21 14:34:36.000000 pilab-binama-0.0.8/setup.py
```

### Comparing `pilab-binama-0.0.7/LICENSE` & `pilab-binama-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pilab-binama-0.0.7/PKG-INFO` & `pilab-binama-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilab-binama
-Version: 0.0.7
+Version: 0.0.8
 Home-page: https://github.com/PiLAB-Medical-Imaging/BinaryMasks
 Author: PiLAB
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `pilab-binama-0.0.7/README.md` & `pilab-binama-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pilab-binama-0.0.7/binama/example.py` & `pilab-binama-0.0.8/binama/example.py`

 * *Files identical despite different names*

### Comparing `pilab-binama-0.0.7/binama/utils.py` & `pilab-binama-0.0.8/binama/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,30 +25,46 @@
         voxelList = getVoxels(voxel, data_new, init_val, voxelList)
         data_new[voxel] = int(new_val)
         voxelList = [y for y in voxelList if y != voxel]
 
     return data_new
 
 
-def getVoxels(voxel, data, init_val, voxelList):
+def getVoxels(voxel, data, init_val: int, voxelList: list):
 
     (x, y, z) = voxel
 
     adjacentVoxelList = [(x+1, y, z), (x-1, y, z), (x, y+1, z),
                          (x, y-1, z), (x, y, z+1), (x, y, z-1)]
 
     for adja in adjacentVoxelList:
         if isInbound(adja, data):
             if data[adja] == init_val and data[voxel] == init_val:
                 voxelList.append(adja)
 
     return voxelList
 
 
-def isInbound(voxel, data):
+def isInbound(voxel, data) -> bool:
+    '''
+    Returns True if voxel is inside data volume.
+
+    Parameters
+    ----------
+    voxel : TYPE
+        Voxel coordinates
+    data : TYPE
+        Data volume
+
+    Returns
+    -------
+    bool
+        Returns True if voxel is inside data volume.
+
+    '''
 
     cond = (voxel[0] < data.shape[0] and voxel[0] >= 0 and
             voxel[1] < data.shape[1] and voxel[1] >= 0 and
             voxel[2] < data.shape[2] and voxel[2] >= 0)
 
     return cond
 
@@ -242,25 +258,72 @@
     Returns
     -------
     ROI : 3D array
         3D binary mask opened by a 3-wide cross kernel
 
     '''
 
+    warn('This function is deprecated, please use opening() instead.',
+         DeprecationWarning, stacklevel=1)
+
     return dilate3D(erode3D(ROI, repeat=repeat), repeat=repeat)
 
 
+def opening(ROI, repeat: int = 1):
+    '''
+    Applies the opening morphological operation on a binary mask.
+
+    Parameters
+    ----------
+    ROI : 3D array
+        3D array of size (x,y,z) containing a binary mask.
+    repeat : int, optional
+        Numbers of times the operation is repeated. The default is 1.
+
+    Returns
+    -------
+    ROI : 3D array
+        3D binary mask opened by a 3-wide cross kernel
+
+    '''
+
+    return dilation(erosion(ROI, repeat=repeat), repeat=repeat)
+
+
 def closing3D(ROI, repeat: int = 1):
 
+    warn('This function is deprecated, please use closing() instead.',
+         DeprecationWarning, stacklevel=1)
+
     return erode3D(dilate3D(ROI, repeat=repeat), repeat=repeat)
 
 
-def remove_inclusions(mask):
+def closing(ROI, repeat: int = 1):
+    '''
+    Applies the closing morphological operation on a binary mask.
+
+    Parameters
+    ----------
+    ROI : 3D array
+        3D array of size (x,y,z) containing a binary mask.
+    repeat : int, optional
+        Numbers of times the operation is repeated. The default is 1.
+
+    Returns
+    -------
+    ROI : 3D array
+        3D binary mask closed by a 3-wide cross kernel
     '''
 
+    return erosion(dilation(ROI, repeat=repeat), repeat=repeat)
+
+
+def remove_inclusions(mask):
+    '''
+    Removes inclusions in a binary mask.
 
     Parameters
     ----------
     mask : 3D array
         3D array of size (x,y,z) containing a binary mask.
 
     Returns
@@ -277,15 +340,15 @@
     mask = mask[tuple(slice(1, dim - 1) for dim in mask.shape)]
 
     return mask
 
 
 def convex_mask(mask):
     '''
-
+    Makes a mask convex.
 
     Parameters
     ----------
     mask : 3D array
         3D array of size (x,y,z) containing a binary mask.
 
     Returns
@@ -312,43 +375,43 @@
     mask = np.where(mask_filled == 0, 1, mask)
 
     return mask
 
 
 def center_of_mass(mask):
     '''
-
+    Returns center of mass coordinates.
 
     Parameters
     ----------
     mask : 3D array
         3D array of size (x,y,z) containing a binary mask.
 
     Returns
     -------
-    center : TYPE
-        DESCRIPTION.
+    center : tuple
+        Center of mass coordinates.
 
     '''
 
     center = tuple([np.average(indices) for indices in np.where(mask == 1)])
 
     return center
 
 
-def isolate_mass(mask, center, strict: bool = False):
+def isolate_mass(mask, center: tuple, strict: bool = False):
     '''
     Return the region of connected 1s at tne center point.
 
     Parameters
     ----------
     mask : 3D array
         3D array of size (x,y,z) containing a binary mask.
-    center : TYPE
-        DESCRIPTION.
+    center : tuple
+        Center of mass coordinates.
     strict : bool, optional
         If True, only direct contact is considered as a conenction.
         The default is False.
 
     Returns
     -------
     mask_bis : 3D array
@@ -458,15 +521,15 @@
         fuse += flood(mask, tuple(idx), tolerance=1)
 
     return fuse
 
 
 def clean_mask(mask, strict: bool = False):
     '''
-
+    Makes a mask convex and removes small clusters.
 
     Parameters
     ----------
     mask : 3D array
         3D array of size (x,y,z) containing a binary mask.
     strict : bool, optional
         DESCRIPTION. The default is False.
```

### Comparing `pilab-binama-0.0.7/pilab_binama.egg-info/PKG-INFO` & `pilab-binama-0.0.8/pilab_binama.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilab-binama
-Version: 0.0.7
+Version: 0.0.8
 Home-page: https://github.com/PiLAB-Medical-Imaging/BinaryMasks
 Author: PiLAB
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `pilab-binama-0.0.7/setup.py` & `pilab-binama-0.0.8/setup.py`

 * *Files identical despite different names*

