# Comparing `tmp/fplore-0.4a1.tar.gz` & `tmp/fplore-0.5b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fplore-0.4a1.tar", last modified: Wed Dec 14 14:45:56 2022, max compression
+gzip compressed data, was "fplore-0.5b1.tar", last modified: Thu Apr 13 15:59:23 2023, max compression
```

## Comparing `fplore-0.4a1.tar` & `fplore-0.5b1.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 14:45:56.026899 fplore-0.4a1/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2022-12-14 14:45:42.000000 fplore-0.4a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2022-12-14 14:45:56.026899 fplore-0.4a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2022-12-14 14:45:42.000000 fplore-0.4a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 14:45:56.022899 fplore-0.4a1/fplore/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2022-12-14 14:45:42.000000 fplore-0.4a1/fplore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 14:45:56.026899 fplore-0.4a1/fplore/files/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2022-12-14 14:45:42.000000 fplore-0.4a1/fplore/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19545 2022-12-14 14:45:42.000000 fplore-0.4a1/fplore/files/band.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2022-12-14 14:45:42.000000 fplore-0.4a1/fplore/files/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2022-12-14 14:45:42.000000 fplore-0.4a1/fplore/files/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2022-12-14 14:45:42.000000 fplore-0.4a1/fplore/files/dos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2022-12-14 14:45:42.000000 fplore-0.4a1/fplore/files/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2022-12-14 14:45:42.000000 fplore-0.4a1/fplore/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2022-12-14 14:45:42.000000 fplore-0.4a1/fplore/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2022-12-14 14:45:42.000000 fplore-0.4a1/fplore/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    14501 2022-12-14 14:45:42.000000 fplore-0.4a1/fplore/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 14:45:56.022899 fplore-0.4a1/fplore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2022-12-14 14:45:56.000000 fplore-0.4a1/fplore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2022-12-14 14:45:56.000000 fplore-0.4a1/fplore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 14:45:56.000000 fplore-0.4a1/fplore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      204 2022-12-14 14:45:56.000000 fplore-0.4a1/fplore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-14 14:45:56.000000 fplore-0.4a1/fplore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-14 14:45:56.026899 fplore-0.4a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2022-12-14 14:45:42.000000 fplore-0.4a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:59:23.940894 fplore-0.5b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-13 15:59:15.000000 fplore-0.5b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-13 15:59:23.940894 fplore-0.5b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-13 15:59:15.000000 fplore-0.5b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:59:23.936893 fplore-0.5b1/fplore/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-13 15:59:15.000000 fplore-0.5b1/fplore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:59:23.940894 fplore-0.5b1/fplore/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-13 15:59:15.000000 fplore-0.5b1/fplore/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18963 2023-04-13 15:59:15.000000 fplore-0.5b1/fplore/files/band.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-04-13 15:59:15.000000 fplore-0.5b1/fplore/files/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-13 15:59:15.000000 fplore-0.5b1/fplore/files/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-13 15:59:15.000000 fplore-0.5b1/fplore/files/dos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-13 15:59:15.000000 fplore-0.5b1/fplore/files/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-13 15:59:15.000000 fplore-0.5b1/fplore/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-04-13 15:59:15.000000 fplore-0.5b1/fplore/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-04-13 15:59:15.000000 fplore-0.5b1/fplore/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-04-13 15:59:15.000000 fplore-0.5b1/fplore/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:59:23.936893 fplore-0.5b1/fplore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-13 15:59:23.000000 fplore-0.5b1/fplore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-13 15:59:23.000000 fplore-0.5b1/fplore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:59:23.000000 fplore-0.5b1/fplore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-13 15:59:23.000000 fplore-0.5b1/fplore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 15:59:23.000000 fplore-0.5b1/fplore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 15:59:23.940894 fplore-0.5b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-13 15:59:15.000000 fplore-0.5b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:59:23.940894 fplore-0.5b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-13 15:59:15.000000 fplore-0.5b1/tests/test_band.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-13 15:59:15.000000 fplore-0.5b1/tests/test_util.py
```

### Comparing `fplore-0.4a1/LICENSE` & `fplore-0.5b1/LICENSE`

 * *Files identical despite different names*

### Comparing `fplore-0.4a1/PKG-INFO` & `fplore-0.5b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: fplore
-Version: 0.4a1
+Version: 0.5b1
 Summary: FPLO run evaluation
 Home-page: https://github.com/mueslo/fplore
 License: GPLv3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Provides-Extra: tests
```

### Comparing `fplore-0.4a1/README.md` & `fplore-0.5b1/README.md`

 * *Files identical despite different names*

### Comparing `fplore-0.4a1/fplore/files/band.py` & `fplore-0.5b1/fplore/files/band.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from functools import cached_property
 
 import numpy as np
 from numpy.lib.recfunctions import merge_arrays
 import progressbar
 from scipy.stats.distributions import norm
 from scipy.interpolate import RegularGridInterpolator, LinearNDInterpolator
-from pymatgen.symmetry.groups import PointGroup
 from pymatgen.core import Lattice
 
 from .base import FPLOFile, writeable, loads
 from ..logging import log
 from ..util import (cartesian_product, find_basis, detect_grid,
                     remove_duplicates, snap_to_grid, fill_bz,
                     find_lattice)
@@ -65,16 +64,15 @@
     def bands_within(self, e_lower=-0.025, e_upper=0.025):
         e = (e_lower + e_upper) / 2
         tol = np.abs(e_upper - e_lower) / 2
         return self.bands_at_energy(e=e, tol=tol)
 
 
 class BandWeights(BandBase, FPLOFile):
-    __fplo_file__ = ("+bweights", "+bweights_kp", "+bweightslms", "+bwsum",
-                     "+bweights_unfold")
+    __fplo_file__ = re.compile(r"\+bw(eights(lms)?|sum)(_kp)?(_unfold)?")
 
     @loads('data', 'labels', disk_cache=True, mem_map={'data'})
     def load(self):
         weights_file = open(self.filepath, 'r')
         header_str = next(weights_file)
         _0, _1, n_k, n_weights, n_bands, n_spinstates, _6, size2 = (
             f(x) for f, x in zip((int, float, int, int, int, int, int, int),
@@ -195,28 +193,19 @@
         return merge_arrays([self._data, k_structured], flatten=True)
 
     @cached_property
     def symm_data(self):
         """Returns the band data folded back to the first BZ and applies
         symmetry operations. Returns an index array to reduce memory usage."""
 
-        base_lattice = self.run.lattice
-        basis = None  # skip basis transformation for cartesian-aligned lattices
-        # for body/face centered cubic, symm_ops are in non-primitive simple cubic axes
-        
-        if self.run.spacegroup.crystal_system in ('trigonal', 'hexagonal'):
-            # symm ops are in primitive (rhombohedral) basis vectors (hkl)
-            base_lattice = self.run.primitive_lattice
-            basis = base_lattice.reciprocal_lattice.matrix
-        elif self.run.spacegroup.crystal_system not in ('cubic', 'tetragonal'):
-            log.warning('untested crystal system, k-space symmetrization may be wrong')
-        symm_ops = base_lattice.get_recp_symmetry_operation()
-        
+        # get symmetry operations from point group, in rotated cartesian coords
+        symm_ops = self.run.point_group_operations
+
         # apply symmetry operations from point group
-        data = self.apply_symmetry(self.data, symm_ops, basis=basis)
+        data = self.apply_symmetry(self.data, symm_ops)
         data['k'] = self.run.backfold_k(data['k'])
         data = remove_duplicates(data)
         return data
 
     @cached_property
     def padded_symm_data(self):
         k = self.symm_data['k']
@@ -257,15 +246,17 @@
         return dict(zip(lattice_ijk, data['idx']))  # map sampling lattice ijk to unique index
 
     def reshape_gridded_data(self, data='padded_symm', missing_coords_strategy='backfold'):
         """Tries to detect if the band data coordinates form a regular,
         rectangular grid, and returns the band data `indexes` reshaped to that
         grid."""
 
-        if data in ('padded_symm', None):
+        if isinstance(data, np.ndarray):
+            pass
+        elif data in ('padded_symm', None):
             data = self.padded_symm_data
         elif data == 'symm':
             data = self.symm_data
         elif data in ('raw', 'data'):
             data = self._gen_band_data_array(len(self.data),
                                              k_coords=True, index=True)
             data['k'] = self.data['k']
@@ -442,15 +433,15 @@
         num_k = len(k_points)
 
         k_idx = np.arange(num_k)
         new_data_idx = cls._gen_band_data_array(num_k*len(symm_ops),
                                                 k_coords=True, index=True)
         for i, op in enumerate(symm_ops):
             rot = op.rotation_matrix
-            new_k_points = k_points @ rot
+            new_k_points = k_points @ rot.T    # .T important! == op.operate_multi(k_points)
             new_data_idx['k'][num_k*i:num_k*(i+1)] = new_k_points
             new_data_idx['idx'][num_k*i:num_k*(i+1)] = k_idx
 
         log.debug('applied {} symm ops to {} k points', len(symm_ops), num_k)
         new_data_idx = remove_duplicates(new_data_idx)
 
         if basis is not None:
```

### Comparing `fplore-0.4a1/fplore/files/base.py` & `fplore-0.5b1/fplore/files/base.py`

 * *Files identical despite different names*

### Comparing `fplore-0.4a1/fplore/files/config.py` & `fplore-0.5b1/fplore/files/config.py`

 * *Files identical despite different names*

### Comparing `fplore-0.4a1/fplore/files/misc.py` & `fplore-0.5b1/fplore/files/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
                 data[key.strip()] = value.strip()
 
         return data
 
 
 class Dens(FPLOConfig, FPLOFile):
     __fplo_file__ = "=.dens"
+    load_default = False
 
 
 class Points(FPLOFile):
     __fplo_file__ = "+points"
 
     @loads('data')
     def load(self):
@@ -71,13 +72,15 @@
     @loads('_data')
     def load(self):
         data = super(InFile, self).load()['_data']
 
         self.run.version = (data.header.version.mainversion,
                             data.header.version.subversion)
         log.info("Detected FPLO run with version {}-{}", *self.run.version)
+        if float(self.run.version[0]) < 14:
+            log.warning("FPLO version <14 is not supported. Things may break.")
 
         return data
 
 
 class SymFile(FPLOConfig, FPLOFile):
     __fplo_file__ = "=.sym"
```

### Comparing `fplore-0.4a1/fplore/plot.py` & `fplore-0.5b1/fplore/plot.py`

 * *Files identical despite different names*

### Comparing `fplore-0.4a1/fplore/util.py` & `fplore-0.5b1/fplore/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import itertools
 
 import numpy as np
 from scipy.ndimage import map_coordinates
 from scipy.spatial.distance import cdist
+from scipy.spatial.transform import Rotation
 from scipy.spatial import Delaunay, Voronoi
 import scipy.cluster.hierarchy as hcluster
 from scipy.constants import hbar, m_e, eV, angstrom, c
 from pymatgen.core import Lattice
 
 from .logging import log
 
@@ -89,26 +90,39 @@
     order = np.argsort(dists[partition])
     smallest = lattice_points[partition][order]
     
     basis = None
     for basis_candidate in itertools.permutations(smallest, 3):
         if np.linalg.matrix_rank(basis_candidate) < 3:
             continue
-        basis = np.array(basis_candidate) 
+        basis = np.array(basis_candidate, dtype=np.float64)
         break
     else:
         raise Exception('Points do not span a volume')
 
     try:
         # diff to grid
         inv_basis = np.linalg.inv(basis)
         frac = lattice_points @ inv_basis
-        diff = frac - np.rint(frac)
+        frac_int = np.rint(frac)
+
+        # finetune basis for numerical accuracy
+        # solve matrix equation for best fit
+        # diff = frac - frac_int
+        # delta_basis, res, rank, s = np.linalg.lstsq(frac_int, diff @ basis)
+        basis, res2, rank2, s2 = np.linalg.lstsq(frac_int, lattice_points, rcond=None)
+
+        # diff to grid (finetuned basis)
+        inv_basis = np.linalg.inv(basis)
+        frac = lattice_points @ inv_basis
+        frac_int = np.rint(frac)
+        diff = frac - frac_int
+
         max_diff = np.linalg.norm(diff, axis=1).max()
-        assert max_diff < 1e-4, f'max_diff {max_diff}'
+        assert max_diff < 1e-4, f'max_diff {max_diff}'  # absolute error
 
         # assert grid has no major holes (e.g. basis too small)
         uniq_x, uniq_y, uniq_z = [np.unique(frac[:, i].round(decimals=4)) for i in range(3)]
         assert np.allclose(uniq_x, np.arange(uniq_x[0], uniq_x[-1]+1)), 'x'
         assert np.allclose(uniq_y, np.arange(uniq_y[0], uniq_y[-1]+1)), 'y'
         assert np.allclose(uniq_z, np.arange(uniq_z[0], uniq_z[-1]+1)), 'z'
     except AssertionError as ae:
@@ -383,23 +397,44 @@
     Partitions BZ into irreducible wedges.
     :return: List of irreducible wedges with matrix to transform coordinates
     to the 'primary' wedge.
     """
     raise NotImplementedError
 
 
+def get_perp_vector(v):
+    """
+    Returns an arbitrary normalized vector perpendicular to v
+    """
+    v = np.array(v)
+    if v[0] == 0:
+        return np.array([1, 0, 0])
+    elif v[1] == 0:
+        return np.array([0, 1, 0])
+    elif v[2] == 0:
+        return np.array([0, 0, 1])
+    else:
+        return np.array([v[1], -v[0], 0])/np.sqrt(v[0]**2 + v[1]**2)
+
+
 def rot_v1_v2(v1, v2):
     """Returns rotation matrix which rotates v1 onto v2"""
     v1 = np.array(v1)
     v2 = np.array(v2)
     v1 = v1 / np.linalg.norm(v1)
     v2 = v2 / np.linalg.norm(v2)
-    cp = np.cross(v1, v2)
+    cp = np.cross(v1, v2)  # sine * rot axis
     c = np.dot(v1, v2)  # cosine
 
+    if np.isclose(c, -1.0):
+        log.debug(f'v1={v1} and v2={v2} are antiparallel')
+        n = get_perp_vector(v1)
+        return Rotation.from_rotvec(n*np.pi).as_matrix()
+
+    # rodrigues rotation formula
     cpm = np.array([[0, -cp[2], cp[1]],
                    [cp[2], 0, -cp[0]],
                    [-cp[1], cp[0], 0]])
 
     return np.eye(3) + cpm + np.dot(cpm, cpm) * 1 / (1 + c)
```

### Comparing `fplore-0.4a1/fplore.egg-info/PKG-INFO` & `fplore-0.5b1/fplore.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: fplore
-Version: 0.4a1
+Version: 0.5b1
 Summary: FPLO run evaluation
 Home-page: https://github.com/mueslo/fplore
 License: GPLv3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Provides-Extra: tests
```

### Comparing `fplore-0.4a1/setup.py` & `fplore-0.5b1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,14 +50,17 @@
             'Pillow',
         ],
     },
     classifiers=[
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Physics",
         "Topic :: Scientific/Engineering :: Chemistry",
     ],
 )
```

