# Comparing `tmp/delaunay_watershed_3d-0.2.2.tar.gz` & `tmp/delaunay_watershed_3d-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/delaunay-watershed/dist/.tmp-3o4qv7iu/delaunay_watershed_3d-0.2.2.tar", last modified: Wed Apr 12 17:18:32 2023, max compression
+gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/delaunay-watershed/dist/.tmp-fkmjxki_/delaunay_watershed_3d-0.2.4.tar", last modified: Thu Apr 13 08:11:29 2023, max compression
```

## Comparing `delaunay_watershed_3d-0.2.2.tar` & `delaunay_watershed_3d-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 17:18:32.118678 delaunay_watershed_3d-0.2.2/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     6029 2023-04-12 17:18:32.118879 delaunay_watershed_3d-0.2.2/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     5343 2023-04-12 12:26:50.000000 delaunay_watershed_3d-0.2.2/README.md
--rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.2/pyproject.toml
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     1019 2023-04-12 17:18:32.119633 delaunay_watershed_3d-0.2.2/setup.cfg
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 17:18:32.102437 delaunay_watershed_3d-0.2.2/src/
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 17:18:32.106364 delaunay_watershed_3d-0.2.2/src/delaunay_watershed_3d.egg-info/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     6029 2023-04-12 17:18:32.000000 delaunay_watershed_3d-0.2.2/src/delaunay_watershed_3d.egg-info/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      531 2023-04-12 17:18:32.000000 delaunay_watershed_3d-0.2.2/src/delaunay_watershed_3d.egg-info/SOURCES.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-04-12 17:18:32.000000 delaunay_watershed_3d-0.2.2/src/delaunay_watershed_3d.egg-info/dependency_links.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      163 2023-04-12 17:18:32.000000 delaunay_watershed_3d-0.2.2/src/delaunay_watershed_3d.egg-info/requires.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        5 2023-04-12 17:18:32.000000 delaunay_watershed_3d-0.2.2/src/delaunay_watershed_3d.egg-info/top_level.txt
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-12 17:18:32.118228 delaunay_watershed_3d-0.2.2/src/dw3d/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    12409 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.2/src/dw3d/Curvature.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    21435 2023-04-12 12:16:26.000000 delaunay_watershed_3d-0.2.2/src/dw3d/Dcel.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     6880 2023-04-12 17:10:03.000000 delaunay_watershed_3d-0.2.2/src/dw3d/Geometric_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    13501 2023-04-12 17:17:47.000000 delaunay_watershed_3d-0.2.2/src/dw3d/Geometry.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     6334 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.2/src/dw3d/Graph_functions.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     2827 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.2/src/dw3d/Mask_reconstruction.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    10499 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.2/src/dw3d/Mesh_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     3506 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.2/src/dw3d/Networkx_functions.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)       87 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.2/src/dw3d/__init__.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     5033 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.2/src/dw3d/functions.py
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-13 08:11:29.288559 delaunay_watershed_3d-0.2.4/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     6029 2023-04-13 08:11:29.288720 delaunay_watershed_3d-0.2.4/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     5343 2023-04-12 12:26:50.000000 delaunay_watershed_3d-0.2.4/README.md
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.4/pyproject.toml
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     1019 2023-04-13 08:11:29.289679 delaunay_watershed_3d-0.2.4/setup.cfg
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-13 08:11:29.270991 delaunay_watershed_3d-0.2.4/src/
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-13 08:11:29.275760 delaunay_watershed_3d-0.2.4/src/delaunay_watershed_3d.egg-info/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     6029 2023-04-13 08:11:29.000000 delaunay_watershed_3d-0.2.4/src/delaunay_watershed_3d.egg-info/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      531 2023-04-13 08:11:29.000000 delaunay_watershed_3d-0.2.4/src/delaunay_watershed_3d.egg-info/SOURCES.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-04-13 08:11:29.000000 delaunay_watershed_3d-0.2.4/src/delaunay_watershed_3d.egg-info/dependency_links.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      163 2023-04-13 08:11:29.000000 delaunay_watershed_3d-0.2.4/src/delaunay_watershed_3d.egg-info/requires.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        5 2023-04-13 08:11:29.000000 delaunay_watershed_3d-0.2.4/src/delaunay_watershed_3d.egg-info/top_level.txt
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-13 08:11:29.288155 delaunay_watershed_3d-0.2.4/src/dw3d/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    12409 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.4/src/dw3d/Curvature.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    21891 2023-04-13 08:05:19.000000 delaunay_watershed_3d-0.2.4/src/dw3d/Dcel.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     6880 2023-04-12 17:10:03.000000 delaunay_watershed_3d-0.2.4/src/dw3d/Geometric_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    16784 2023-04-13 08:01:40.000000 delaunay_watershed_3d-0.2.4/src/dw3d/Geometry.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     6334 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.4/src/dw3d/Graph_functions.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     2827 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.4/src/dw3d/Mask_reconstruction.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    10499 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.4/src/dw3d/Mesh_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     3506 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.4/src/dw3d/Networkx_functions.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)       87 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.4/src/dw3d/__init__.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     5033 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.4/src/dw3d/functions.py
```

### Comparing `delaunay_watershed_3d-0.2.2/PKG-INFO` & `delaunay_watershed_3d-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delaunay_watershed_3d
-Version: 0.2.2
+Version: 0.2.4
 Summary: Geometrical reconstruction of cell assemblies from instance segmentations
 Home-page: https://github.com/VirtualEmbryo/delaunay-watershed
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `delaunay_watershed_3d-0.2.2/README.md` & `delaunay_watershed_3d-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.2/setup.cfg` & `delaunay_watershed_3d-0.2.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = delaunay_watershed_3d
-version = 0.2.2
+version = 0.2.4
 author = Sacha Ichbiah
 author_email = sacha.ichbiah@college-de-france.fr
 description = Geometrical reconstruction of cell assemblies from instance segmentations
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/VirtualEmbryo/delaunay-watershed
 project_urls =
```

### Comparing `delaunay_watershed_3d-0.2.2/src/delaunay_watershed_3d.egg-info/PKG-INFO` & `delaunay_watershed_3d-0.2.4/src/delaunay_watershed_3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delaunay-watershed-3d
-Version: 0.2.2
+Version: 0.2.4
 Summary: Geometrical reconstruction of cell assemblies from instance segmentations
 Home-page: https://github.com/VirtualEmbryo/delaunay-watershed
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `delaunay_watershed_3d-0.2.2/src/delaunay_watershed_3d.egg-info/SOURCES.txt` & `delaunay_watershed_3d-0.2.4/src/delaunay_watershed_3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.2/src/dw3d/Curvature.py` & `delaunay_watershed_3d-0.2.4/src/dw3d/Curvature.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.2/src/dw3d/Dcel.py` & `delaunay_watershed_3d-0.2.4/src/dw3d/Dcel.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from dataclasses import dataclass, field
 import math
 import pickle
 import numpy as np 
 from dw3d.Curvature import compute_curvature_interfaces
 from dw3d.Geometry import compute_areas_faces,compute_areas_cells,compute_angles_tri,compute_volume_cells, compute_volume_derivative_dict, compute_areas_interfaces,compute_area_derivative_dict, compute_length_trijunctions
+from dw3d.Geometry import compute_area_derivative_autodiff, compute_volume_derivative_autodiff_dict, compute_length_derivative_autodiff
 import networkx
 
 
 
 def separate_faces_dict(Faces,n_towers=10): 
     n_towers = np.amax(Faces[:,[3,4]])+1
    
@@ -373,19 +374,28 @@
 
     def compute_areas_interfaces(self): 
         return(compute_areas_interfaces(self))
     
     def compute_area_derivatives(self): 
         return(compute_area_derivative_dict(self))
 
+    def compute_area_derivatives_fast(self): 
+        return(compute_area_derivative_autodiff(self))
+
     def compute_volumes_cells(self): 
         return(compute_volume_cells(self))
     
     def compute_volume_derivatives(self):
         return(compute_volume_derivative_dict(self))
+    
+    def compute_volume_derivatives_fast(self):
+        return(compute_volume_derivative_autodiff_dict(self))
+    
+    def compute_length_derivatives(self):
+        return(compute_length_derivative_autodiff(self))
 
     def compute_angles_junctions(self,unique=True):
         return(compute_angles_tri(self,unique=unique)[0])
 
     def compute_angles_tri(self,unique=True):
         return(compute_angles_tri(self,unique=unique))
```

### Comparing `delaunay_watershed_3d-0.2.2/src/dw3d/Geometric_utilities.py` & `delaunay_watershed_3d-0.2.4/src/dw3d/Geometric_utilities.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.2/src/dw3d/Geometry.py` & `delaunay_watershed_3d-0.2.4/src/dw3d/Geometry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,91 @@
 #Sacha Ichbiah, Sept 2021
 import numpy as np 
 from tqdm import tqdm
+import torch
 
 def find_key_multiplier(num_points): 
     key_multiplier = 1
     while num_points//key_multiplier != 0 : 
         key_multiplier*=10
     return(key_multiplier)    
 
 ## LENGTHS AND DERIVATIVES
 
+def compute_area_derivative_autodiff(Mesh,device = 'cpu'):
+
+    #Faces_membranes = extract_faces_membranes(Mesh)
+    key_mult = np.amax(Mesh.f[:,3:])+1
+    keys = Mesh.f[:,3]+key_mult*Mesh.f[:,4]
+    Faces_membranes = {}
+    for key in np.unique(keys):
+        tup = (key%key_mult,key//key_mult)
+        Faces_membranes[tup]=Mesh.f[:,:3][np.arange(len(keys))[keys==key]]
+
+    verts = torch.tensor(Mesh.v,dtype=torch.float,requires_grad=True).to(device)
+    optimizer = torch.optim.SGD([verts],lr=1) # Useless, here just to reset the grad
+
+    Areas_derivatives = {}
+    for tup in sorted(Faces_membranes.keys()):
+
+        loss_area = (Compute_Area_Faces_torch(verts,torch.tensor(Faces_membranes[tup]))).sum()
+        loss_area.backward()
+        Areas_derivatives[tup] = (verts.grad).numpy().copy()
+        optimizer.zero_grad()
+
+    return(Areas_derivatives)
+
+
+
+
+def compute_volume_derivative_autodiff_dict(Mesh,device='cpu'):
+    
+    #Faces_manifolds = extract_faces_manifolds(Mesh)
+    Faces_manifolds = {key:[] for key in Mesh.materials}
+    for face in Mesh.f :
+        a,b,c,m1,m2 = face
+        Faces_manifolds[m1].append([a,b,c])
+        Faces_manifolds[m2].append([a,c,b])
+    
+    verts = torch.tensor(Mesh.v,dtype=torch.float,requires_grad=True).to(device)
+    optimizer = torch.optim.SGD([verts],lr=1) # Useless, here just to reset the grad
+
+    Volumes_derivatives = {}
+    for key in Mesh.materials:#1:] :
+        faces = Faces_manifolds[key]
+        assert len(faces)>0
+        loss_volume = -Compute_Volume_manifold_torch(verts,torch.tensor(faces))
+        loss_volume.backward()
+        Volumes_derivatives[key]=(verts.grad.numpy().copy())
+        optimizer.zero_grad()
+    
+    return(Volumes_derivatives)
+
+def compute_length_derivative_autodiff(Mesh,device = 'cpu'):
+
+    Edges_trijunctions = extract_edges_trijunctions(Mesh)
+
+    verts = torch.tensor(Mesh.v,dtype=torch.float,requires_grad=True).to(device)
+    optimizer = torch.optim.SGD([verts],lr=1) # Useless, here just to reset the grad
+
+    Length_derivatives = {}
+    for tup in sorted(Edges_trijunctions.keys()):
+        loss_length = (Compute_length_edges_trijunctions_torch(verts,torch.tensor(Edges_trijunctions[tup]))).sum()
+        loss_length.backward()
+        Length_derivatives[tup] = (verts.grad).numpy().copy()
+        optimizer.zero_grad()
+
+    return(Length_derivatives)
+def Compute_length_edges_trijunctions_torch(verts,Edges_trijunctions):
+    Pos = verts[Edges_trijunctions]
+    Lengths = torch.norm(Pos[:,0]-Pos[:,1],dim=1)
+    return(Lengths)
+
+
+
 def compute_length_trijunctions(Mesh,prints=False): 
     Length_trijunctions = {}
     Edges_trijunctions = extract_edges_trijunctions(Mesh,prints)
     for key in Edges_trijunctions.keys(): 
         Length_trijunctions[key] = np.sum(Compute_length_edges_trijunctions(Mesh.v,Edges_trijunctions[key]))
     return(Length_trijunctions)
 
@@ -115,14 +187,27 @@
     Diffs = np.zeros(Lengths_sides.shape)
     Diffs[:,0] = Half_perimeters - Lengths_sides[:,0]
     Diffs[:,1] = Half_perimeters - Lengths_sides[:,1]
     Diffs[:,2] = Half_perimeters - Lengths_sides[:,2]
     Areas = (Half_perimeters*Diffs[:,0]*Diffs[:,1]*Diffs[:,2])**(0.5)
     return(Areas)
 
+def Compute_Area_Faces_torch(Verts,Faces):
+    Pos = Verts[Faces]
+    Sides = Pos-Pos[:,[2,0,1]]
+
+    Lengths_sides =torch.norm(Sides,dim=2)
+    Half_perimeters = torch.sum(Lengths_sides,axis=1)/2
+    Diffs = torch.zeros(Lengths_sides.shape)
+    Diffs[:,0] = Half_perimeters - Lengths_sides[:,0]
+    Diffs[:,1] = Half_perimeters - Lengths_sides[:,1]
+    Diffs[:,2] = Half_perimeters - Lengths_sides[:,2]
+    Areas = (Half_perimeters*Diffs[:,0]*Diffs[:,1]*Diffs[:,2])**(0.5)
+    return(Areas)
+
 
 
 def compute_areas_faces(Mesh):
     Pos = Mesh.v[Mesh.f[:,[0,1,2]]]
     Sides = Pos-Pos[:,[2,0,1]]
     Lengths_sides = np.linalg.norm(Sides,axis = 2)
     Half_perimeters = np.sum(Lengths_sides,axis=1)/2
@@ -186,14 +271,21 @@
 def Compute_Volume_manifold(Verts,Faces):
     Coords = Verts[Faces]
     cross_prods = np.cross(Coords[:,1],Coords[:,2],axis=1)
     dots = np.sum(cross_prods*Coords[:,0],axis=1)
     Vol = -np.sum(dots)/6
     return(Vol)
 
+def Compute_Volume_manifold_torch(Verts,Faces):
+    Coords = Verts[Faces]
+    cross_prods = torch.cross(Coords[:,1],Coords[:,2],axis=1)
+    dots = torch.sum(cross_prods*Coords[:,0],axis=1)
+    Vol = -torch.sum(dots)/6
+    return(Vol)
+
 def Compute_Volume_manifold_sequential(Verts,Faces):
     Volume = np.zeros(len(Faces))
     for i,face in enumerate(Faces) :
         index = Faces[i,[0,1,2]]
         Coords = Verts[index]
         inc = np.linalg.det(Coords)
         Volume [i]-=inc
```

### Comparing `delaunay_watershed_3d-0.2.2/src/dw3d/Graph_functions.py` & `delaunay_watershed_3d-0.2.4/src/dw3d/Graph_functions.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.2/src/dw3d/Mask_reconstruction.py` & `delaunay_watershed_3d-0.2.4/src/dw3d/Mask_reconstruction.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.2/src/dw3d/Mesh_utilities.py` & `delaunay_watershed_3d-0.2.4/src/dw3d/Mesh_utilities.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.2/src/dw3d/Networkx_functions.py` & `delaunay_watershed_3d-0.2.4/src/dw3d/Networkx_functions.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.2/src/dw3d/functions.py` & `delaunay_watershed_3d-0.2.4/src/dw3d/functions.py`

 * *Files identical despite different names*

