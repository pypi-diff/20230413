# Comparing `tmp/dspawpy-0.8.6-py3-none-any.whl.zip` & `tmp/dspawpy-0.8.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 61941 bytes, number of entries: 20
+Zip file size: 67612 bytes, number of entries: 20
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 06:32 dspawpy/__init__.py
 -rw-rw-rw-  2.0 fat    27378 b- defN 23-Apr-06 03:08 dspawpy/plot.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 06:32 dspawpy/analysis/__init__.py
--rw-rw-rw-  2.0 fat    47068 b- defN 23-Apr-11 01:30 dspawpy/analysis/aimdtools.py
+-rw-rw-rw-  2.0 fat    47545 b- defN 23-Apr-13 03:15 dspawpy/analysis/aimdtools.py
 -rw-rw-rw-  2.0 fat    20152 b- defN 23-Apr-04 06:32 dspawpy/analysis/vacf.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 06:32 dspawpy/diffusion/__init__.py
--rw-rw-rw-  2.0 fat     9574 b- defN 23-Apr-04 06:32 dspawpy/diffusion/neb.py
--rw-rw-rw-  2.0 fat    47341 b- defN 23-Apr-06 03:08 dspawpy/diffusion/nebtools.py
--rw-rw-rw-  2.0 fat    10966 b- defN 23-Apr-04 06:32 dspawpy/diffusion/pathfinder.py
+-rw-rw-rw-  2.0 fat     9607 b- defN 23-Apr-13 05:59 dspawpy/diffusion/neb.py
+-rw-rw-rw-  2.0 fat    48170 b- defN 23-Apr-11 08:22 dspawpy/diffusion/nebtools.py
+-rw-rw-rw-  2.0 fat    10993 b- defN 23-Apr-13 05:52 dspawpy/diffusion/pathfinder.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 08:25 dspawpy/io/__init__.py
 -rw-rw-rw-  2.0 fat    21646 b- defN 23-Apr-04 06:32 dspawpy/io/read.py
 -rw-rw-rw-  2.0 fat     7910 b- defN 23-Apr-04 06:32 dspawpy/io/read_json.py
 -rw-rw-rw-  2.0 fat    10331 b- defN 23-Apr-04 06:32 dspawpy/io/structure.py
--rw-rw-rw-  2.0 fat     9407 b- defN 23-Apr-07 09:23 dspawpy/io/utils.py
+-rw-rw-rw-  2.0 fat    29355 b- defN 23-Apr-13 03:18 dspawpy/io/utils.py
 -rw-rw-rw-  2.0 fat    11049 b- defN 23-Apr-04 09:19 dspawpy/io/write.py
 -rw-rw-rw-  2.0 fat     1794 b- defN 23-Apr-04 06:32 dspawpy/io/write_json.py
--rw-rw-rw-  2.0 fat      754 b- defN 23-Apr-11 01:32 dspawpy-0.8.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-11 01:32 dspawpy-0.8.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-11 01:32 dspawpy-0.8.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1580 b- defN 23-Apr-11 01:32 dspawpy-0.8.6.dist-info/RECORD
-20 files, 227050 bytes uncompressed, 59391 bytes compressed:  73.8%
+-rw-rw-rw-  2.0 fat      754 b- defN 23-Apr-13 06:08 dspawpy-0.8.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 06:08 dspawpy-0.8.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-13 06:08 dspawpy-0.8.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1581 b- defN 23-Apr-13 06:08 dspawpy-0.8.7.dist-info/RECORD
+20 files, 248365 bytes uncompressed, 65062 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: dspawpy/io/write.py
 Comment: 
 
 Filename: dspawpy/io/write_json.py
 Comment: 
 
-Filename: dspawpy-0.8.6.dist-info/METADATA
+Filename: dspawpy-0.8.7.dist-info/METADATA
 Comment: 
 
-Filename: dspawpy-0.8.6.dist-info/WHEEL
+Filename: dspawpy-0.8.7.dist-info/WHEEL
 Comment: 
 
-Filename: dspawpy-0.8.6.dist-info/top_level.txt
+Filename: dspawpy-0.8.7.dist-info/top_level.txt
 Comment: 
 
-Filename: dspawpy-0.8.6.dist-info/RECORD
+Filename: dspawpy-0.8.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dspawpy/analysis/aimdtools.py

```diff
@@ -919,25 +919,25 @@
                 positions[i, j, :] = np.dot(wrapped_spos[:, sli], lats)
 
         return Nstep, elements, positions, lattices
 
 
 # 2. 写轨迹文件
 def write_xyz_traj(
-    datafile: str = "aimd.h5",
+    datafile="aimd.h5",
     ai=None,
     ele=None,
     index=None,
     xyzfile="aimdTraj.xyz",
 ):
     """保存xyz格式的轨迹文件
 
     Parameters
     ----------
-    datafile : str
+    datafile : str or list
         DSPAW计算完成后保存的h5/json文件或包含它们的文件夹路径
     ai : int
         原子编号列表（体系中的第几号原子，不是质子数）
     ele : str
         元素，例如 'C'，'H'，'O'，'N'
     index : int
         优化过程中的第几步
@@ -948,30 +948,34 @@
         写入xyz格式的轨迹文件，默认为aimdTraj.xyz
 
     Example
     -------
     >>> from dspawpy.analysis.aimdtools import write_xyz_traj
     >>> write_xyz_traj(datafile='aimd.h5', ai=[1,2,3], index=1, xyzfile='aimdTraj.xyz')
     """
+    if isinstance(datafile, list):
+        for i, df in enumerate(datafile):
+            write_xyz_traj(df, ai, ele, index, str(i+1)+xyzfile)
+        return f"{xyzfile} 文件已保存！"
     # search datafile in the given directory
-    if os.path.isdir(datafile):
+    elif os.path.isdir(datafile):
         directory = datafile  # specified datafile is actually a directory
         print("您指定了一个文件夹，正在查找相关h5或json文件...")
         if os.path.exists(os.path.join(directory, "aimd.h5")):
             datafile = os.path.join(directory, "aimd.h5")
             print("Reading aimd.h5...")
         elif os.path.exists(os.path.join(directory, "aimd.json")):
             datafile = os.path.join(directory, "aimd.json")
             print("Reading aimd.json...")
         else:
             raise FileNotFoundError("未找到aimd.h5/aimd.json文件！")
     if datafile.endswith(".h5"):
         Nstep, eles, poses, lats = read_h5(datafile, index, ele, ai)
     elif datafile.endswith(".json"):
-        raise NotImplementedError("json文件暂不支持写入xyz文件！")
+        Nstep, eles, poses, lats = _read_json(datafile, index, ele, ai)
     else:
         raise TypeError("仅支持读取h5或json文件！")
     
     # 写入文件
     with open(xyzfile, "w") as f:
         # Nstep
         for n in range(Nstep):
@@ -994,28 +998,29 @@
             )
             # position and element
             for i in range(len(eles)):
                 f.write(
                     "%s %f %f %f\n"
                     % (eles[i], poses[n, i, 0], poses[n, i, 1], poses[n, i, 2])
                 )
+    print(f"{xyzfile} 文件已保存！")
 
 
 def write_dump_traj(
     datafile="aimd.h5",
     ai=None,
     ele=None,
     index=None,
     dumpfile="aimdTraj.dump",
 ):
     """保存为lammps的dump格式的轨迹文件，暂时只支持正交晶胞
 
     Parameters
     ----------
-    datafile : str
+    datafile : str or list
         DSPAW计算完成后保存的h5/json文件或包含它们的文件夹路径
     ai : int
         原子编号列表（体系中的第几号原子，不是质子数）
     ele : str
         元素，例如 'C'，'H'，'O'，'N'
     index : int
         优化过程中的第几步
@@ -1026,30 +1031,34 @@
         写入xyz格式的轨迹文件，默认为aimdTraj.xyz
 
     Example
     -------
     >>> from dspawpy.analysis.aimdtools import write_dump_traj
     >>> write_dump_traj(datafile='aimd.h5', ai=[1,2,3], index=1, dumpfile='aimdTraj.dump')
     """
+    if isinstance(datafile, list):
+        for i, df in enumerate(datafile):
+            write_dump_traj(df, ai, ele, index, str(i+1)+dumpfile)
+        return f"{dumpfile} 文件已保存！"
     # search datafile in the given directory
-    if os.path.isdir(datafile):
+    elif os.path.isdir(datafile):
         directory = datafile  # specified datafile is actually a directory
         print("您指定了一个文件夹，正在查找相关h5或json文件...")
         if os.path.exists(os.path.join(directory, "aimd.h5")):
             datafile = os.path.join(directory, "aimd.h5")
             print("Reading aimd.h5...")
         elif os.path.exists(os.path.join(directory, "aimd.json")):
             datafile = os.path.join(directory, "aimd.json")
             print("Reading aimd.json...")
         else:
             raise FileNotFoundError("未找到aimd.h5/aimd.json文件！")
     if datafile.endswith(".h5"):
         Nstep, eles, poses, lats = read_h5(datafile, index, ele, ai)
     elif datafile.endswith(".json"):
-        raise NotImplementedError("json文件暂不支持写入xyz文件！")
+        Nstep, eles, poses, lats = _read_json(datafile, index, ele, ai)
     else:
         raise TypeError("仅支持读取h5或json文件！")
 
     # 写入文件
     with open(dumpfile, "w") as f:
         for n in range(Nstep):
             box_bounds = _get_lammps_non_orthogonal_box(lats[n])
@@ -1072,15 +1081,15 @@
             )
             f.write("ITEM: ATOMS type x y z id\n")
             for i in range(len(eles)):
                 f.write(
                     "%s %f %f %f %d\n"
                     % (eles[i], poses[n, i, 0], poses[n, i, 1], poses[n, i, 2], i + 1)
                 )
-
+    print(f"{dumpfile} 文件已保存！")
 
 def _get_structure_list(df: str = "aimd.h5") -> List[Structure]:
     """get pymatgen structures from single datafile
 
     Parameters
     ----------
     df : str, optional
```

## dspawpy/diffusion/neb.py

```diff
@@ -41,15 +41,15 @@
             initial_structure:
             final_structure:
             nimages: number of images,contain initial and final structure
         """
 
         self.nimages = nimages
         self.iddp = IDPPSolver.from_endpoints(
-            endpoints=[initial_structure, final_structure], nimages=self.nimages - 2
+            endpoints=[initial_structure, final_structure], nimages=self.nimages - 2, sort_tol=0 # 锁定原子编号
         )
 
     def linear_interpolate(self):
         return self.iddp.structures
 
     def idpp_interpolate(
         self,
```

## dspawpy/diffusion/nebtools.py

```diff
@@ -394,37 +394,37 @@
     for i in range(len(subfolders)):  # 注意格式化输出，对齐
         print(
             "%s\t%8.4f\t%8.4f\t%12.4f\t%20.4f"
             % (subfolders[i], resort_mfs[i], rcs[i], ens[i][0], dEs[i])
         )
 
 
-def restart(direrctory: str, inputin: str, output: str):
+def restart(directory: str, inputin: str, output: str):
     """将旧NEB任务归档压缩，并在原路径下准备续算
 
     Parameters
     ----------
-    direrctory : str
+    directory : str
         旧NEB任务所在路径，默认当前路径
     inputin : str
         输入参数文件名，默认input.in
     output : str
         备份文件夹路径
 
     Examples
     ----------
     >>> from dspawpy.diffusion.nebtools import restart
-    >>> restart(direrctory='source', inputin='input.in', output='backup')
+    >>> restart(directory='source', inputin='input.in', output='backup')
     """
     if output == "":
         raise ValueError("备份文件夹路径不能为空！")
     elif os.path.isdir(output):
         raise ValueError("备份文件夹已存在！")
 
-    if direrctory == "":
+    if directory == "":
         directory = os.getcwd()
     if inputin == "":
         inputin = "input.in"
 
     # 读取子文件夹名称列表，仅保留形如00，01数字文件夹路径
     subfolders = get_neb_subfolders(directory)
     # 创建备份文件夹并进入
@@ -616,15 +616,14 @@
                     raw = _from_json(directory, step)
                 except FileNotFoundError:
                     print("h5和json文件都不存在！")
                 except json.decoder.JSONDecodeError:
                     print("json文件格式错误！")
             except:
                 print("h5文件内容读取失败！")
-
     _dump_neb_movie_json(raw)
 
 
 def _from_structures(directory: str):
     """从structure00.as，structure01.as，...，中读取结构信息，
     写入neb_movie_init，以便用DeviceStudio打开观察
 
@@ -650,23 +649,33 @@
     MaxForces = np.zeros(shape=(nimage - 2, step + 1))  # optional
     TotalEnergies = np.zeros(shape=(nimage - 2, step + 1))  # optional
 
     Poses = []  # nimage x Natom x 3 , read
     Elems = []  # nimage x Natom, read
     Latvs = []  # nimage x 9, read
 
+    iDirects = [] # read coordinate type
     for i, folder in enumerate(subfolders):
         structure_path = os.path.join(directory, folder, f"structure{folder}.as")
         if not os.path.exists(structure_path):
             raise FileNotFoundError(f"请检查{structure_path}是否存在！")
         pos, ele, lat = get_pos_ele_lat(structure_path)
         Poses.append(pos)
         Elems.append(ele)
         Latvs.append(lat)
-
+        with open(structure_path, "r") as f:
+            lines = f.readlines()
+            coordinateType = lines[6].split()[0]
+            if coordinateType == "Direct":
+                iDirect = True
+            elif coordinateType == "Cartesian":
+                iDirect = False
+            else:
+                raise ValueError(f"请检查{structure_path}中的坐标类型！")
+            iDirects.append(iDirect)
     Natom = len(Elems[0])
 
     # reshape data
     Poses = np.array(Poses).reshape((nimage, Natom, 3))
     Elems = np.array(Elems).reshape((nimage, Natom))
     Latvs = np.array(Latvs).reshape((nimage, 9))
     Fixs = np.zeros(shape=(Natom, 3))  # optional
@@ -681,14 +690,15 @@
         Latvs,
         Elems,
         Fixs,
         reactionCoordinates,
         totalEnergies,
         maxForces,
         tangents,
+        iDirects
     )
 
 
 def _from_h5(directory: str, step: int):
     """从NEB路径下的h5文件读取指定step数的结构和能量信息，
     写入json文件，以便用DeviceStudio打开观察
 
@@ -808,14 +818,15 @@
         reactionCoordinates[i] += reactionCoordinates[i - 1]
 
     # reshape data
     Sposes = np.array(Sposes).reshape((nimage, Natom, 3))
     Elems = np.array(Elems).reshape((nimage, Natom))
     Latvs = np.array(Latvs).reshape((nimage, 9))
     Fixs = np.array(Fixs).reshape((Natom, 3))
+    iDirects = [True for i in range(Natom)] # only output direct coordinates
 
     return (
         output,
         subfolders,
         step,
         MaxForces,
         TotalEnergies,  #
@@ -823,14 +834,15 @@
         Latvs,
         Elems,
         Fixs,
         reactionCoordinates,
         totalEnergies,
         maxForces,
         tangents,
+        iDirects
     )
 
 
 def _from_json(directory: str, step: int):
     """从NEB路径下的json文件读取指定step数的结构和能量信息，
     写入json文件，以便用DeviceStudio打开观察
 
@@ -1014,14 +1026,15 @@
         reactionCoordinates[i] += reactionCoordinates[i - 1]
 
     # reshape data
     Sposes = np.array(Sposes).reshape((nimage, Natom, 3))
     Elems = np.array(Elems).reshape((nimage, Natom))
     Latvs = np.array(Latvs).reshape((nimage, 9))
     Fixs = np.array(Fixs).reshape((Natom, 3))
+    iDirects = [True for i in range(Natom)] # only output direct coordinates
 
     return (
         output,
         subfolders,
         step,
         MaxForces,
         TotalEnergies,
@@ -1029,14 +1042,15 @@
         Latvs,
         Elems,
         Fixs,
         reactionCoordinates,
         totalEnergies,
         maxForces,
         tangents,
+        iDirects,
     )
 
 
 def _dump_neb_movie_json(raw):
     """根据之前收集到的各数据列表，dump json文件到output"""
     (
         output,
@@ -1048,14 +1062,15 @@
         Latvs,
         Elems,
         Fixs,
         reactionCoordinates,
         totalEnergies,
         maxForces,
         tangents,
+        iDirects
     ) = raw
 
     IterDict = {}
     for s, sf in enumerate(subfolders):
         if sf == subfolders[0] or sf == subfolders[-1]:
             continue
         else:
@@ -1085,15 +1100,18 @@
                 "Element": elem[i],
                 "Fix": Fixs[i].tolist(),
                 "Mag": [],  # empty
                 "Position": pos[i].tolist(),
                 "Pot": "",
             }  # empty
             atoms.append(atom)
-        rs = {"Atoms": atoms, "CoordinateType": "Direct", "Lattice": lat.tolist()}
+        if iDirects[s]:
+            rs = {"Atoms": atoms, "CoordinateType": "Direct", "Lattice": lat.tolist()}
+        else:
+            rs = {"Atoms": atoms, "CoordinateType": "Cartesian", "Lattice": lat.tolist()}
         RSList.append(rs)
 
     URSList = []  # DS似乎并不读取这部分信息，空置即可
 
     data = {
         "Distance": {"ReactionCoordinate": reactionCoordinates.tolist()},
         "Energy": {"TotalEnergy": totalEnergies.tolist()},
```

## dspawpy/diffusion/pathfinder.py

```diff
@@ -192,15 +192,15 @@
             nimages (int): Number of images between the two end-points.
             sort_tol (float): Distance tolerance (in Angstrom) used to match the
                 atomic indices between start and end structures. Need
                 to increase the value in some cases.
         """
         try:
             images = endpoints[0].interpolate(
-                endpoints[1], nimages=nimages + 1, autosort_tol=sort_tol
+                endpoints[1], nimages=nimages + 1, interpolate_lattices=True, autosort_tol=sort_tol
             )
         except Exception as e:
             if "Unable to reliably match structures " in str(e):
                 warnings.warn(
                     "Auto sorting is turned off because it is unable"
                     " to match the end-point structures!",
                     UserWarning,
```

## dspawpy/io/utils.py

```diff
@@ -1,14 +1,560 @@
 from scipy import integrate
 import re
 from typing import List
 import numpy as np
 import os
 import pandas as pd
+import sys
 
+Na = 6.02214179e23  # 阿伏伽德罗常数 单位 /mol
+h = 6.6260696e-34  # 普朗克常数 单位J*s
+kB = 1.3806503e-23  # 玻尔兹曼常数 J/K
+R = Na * kB  # 理想气体常数 J/(K*mol)
+amu = 1.66053906660e-27  # 原子质量单位 kg
+k = 1.380649e-23/1.602176634e-19 # eV/K
+atomic_masses_iupac2016 = np.array([
+    1.0,  # X
+    1.008,  # H [1.00784, 1.00811]
+    4.002602,  # He
+    6.94,  # Li [6.938, 6.997]
+    9.0121831,  # Be
+    10.81,  # B [10.806, 10.821]
+    12.011,  # C [12.0096, 12.0116]
+    14.007,  # N [14.00643, 14.00728]
+    15.999,  # O [15.99903, 15.99977]
+    18.998403163,  # F
+    20.1797,  # Ne
+    22.98976928,  # Na
+    24.305,  # Mg [24.304, 24.307]
+    26.9815385,  # Al
+    28.085,  # Si [28.084, 28.086]
+    30.973761998,  # P
+    32.06,  # S [32.059, 32.076]
+    35.45,  # Cl [35.446, 35.457]
+    39.948,  # Ar
+    39.0983,  # K
+    40.078,  # Ca
+    44.955908,  # Sc
+    47.867,  # Ti
+    50.9415,  # V
+    51.9961,  # Cr
+    54.938044,  # Mn
+    55.845,  # Fe
+    58.933194,  # Co
+    58.6934,  # Ni
+    63.546,  # Cu
+    65.38,  # Zn
+    69.723,  # Ga
+    72.630,  # Ge
+    74.921595,  # As
+    78.971,  # Se
+    79.904,  # Br [79.901, 79.907]
+    83.798,  # Kr
+    85.4678,  # Rb
+    87.62,  # Sr
+    88.90584,  # Y
+    91.224,  # Zr
+    92.90637,  # Nb
+    95.95,  # Mo
+    97.90721,  # 98Tc
+    101.07,  # Ru
+    102.90550,  # Rh
+    106.42,  # Pd
+    107.8682,  # Ag
+    112.414,  # Cd
+    114.818,  # In
+    118.710,  # Sn
+    121.760,  # Sb
+    127.60,  # Te
+    126.90447,  # I
+    131.293,  # Xe
+    132.90545196,  # Cs
+    137.327,  # Ba
+    138.90547,  # La
+    140.116,  # Ce
+    140.90766,  # Pr
+    144.242,  # Nd
+    144.91276,  # 145Pm
+    150.36,  # Sm
+    151.964,  # Eu
+    157.25,  # Gd
+    158.92535,  # Tb
+    162.500,  # Dy
+    164.93033,  # Ho
+    167.259,  # Er
+    168.93422,  # Tm
+    173.054,  # Yb
+    174.9668,  # Lu
+    178.49,  # Hf
+    180.94788,  # Ta
+    183.84,  # W
+    186.207,  # Re
+    190.23,  # Os
+    192.217,  # Ir
+    195.084,  # Pt
+    196.966569,  # Au
+    200.592,  # Hg
+    204.38,  # Tl [204.382, 204.385]
+    207.2,  # Pb
+    208.98040,  # Bi
+    208.98243,  # 209Po
+    209.98715,  # 210At
+    222.01758,  # 222Rn
+    223.01974,  # 223Fr
+    226.02541,  # 226Ra
+    227.02775,  # 227Ac
+    232.0377,  # Th
+    231.03588,  # Pa
+    238.02891,  # U
+    237.04817,  # 237Np
+    244.06421,  # 244Pu
+    243.06138,  # 243Am
+    247.07035,  # 247Cm
+    247.07031,  # 247Bk
+    251.07959,  # 251Cf
+    252.0830,  # 252Es
+    257.09511,  # 257Fm
+    258.09843,  # 258Md
+    259.1010,  # 259No
+    262.110,  # 262Lr
+    267.122,  # 267Rf
+    268.126,  # 268Db
+    271.134,  # 271Sg
+    270.133,  # 270Bh
+    269.1338,  # 269Hs
+    278.156,  # 278Mt
+    281.165,  # 281Ds
+    281.166,  # 281Rg
+    285.177,  # 285Cn
+    286.182,  # 286Nh
+    289.190,  # 289Fl
+    289.194,  # 289Mc
+    293.204,  # 293Lv
+    293.208,  # 293Ts
+    294.214,  # 294Og
+])
+
+chemical_symbols = [
+    # 0
+    'X',
+    # 1
+    'H', 'He',
+    # 2
+    'Li', 'Be', 'B', 'C', 'N', 'O', 'F', 'Ne',
+    # 3
+    'Na', 'Mg', 'Al', 'Si', 'P', 'S', 'Cl', 'Ar',
+    # 4
+    'K', 'Ca', 'Sc', 'Ti', 'V', 'Cr', 'Mn', 'Fe', 'Co', 'Ni', 'Cu', 'Zn',
+    'Ga', 'Ge', 'As', 'Se', 'Br', 'Kr',
+    # 5
+    'Rb', 'Sr', 'Y', 'Zr', 'Nb', 'Mo', 'Tc', 'Ru', 'Rh', 'Pd', 'Ag', 'Cd',
+    'In', 'Sn', 'Sb', 'Te', 'I', 'Xe',
+    # 6
+    'Cs', 'Ba', 'La', 'Ce', 'Pr', 'Nd', 'Pm', 'Sm', 'Eu', 'Gd', 'Tb', 'Dy',
+    'Ho', 'Er', 'Tm', 'Yb', 'Lu',
+    'Hf', 'Ta', 'W', 'Re', 'Os', 'Ir', 'Pt', 'Au', 'Hg', 'Tl', 'Pb', 'Bi',
+    'Po', 'At', 'Rn',
+    # 7
+    'Fr', 'Ra', 'Ac', 'Th', 'Pa', 'U', 'Np', 'Pu', 'Am', 'Cm', 'Bk',
+    'Cf', 'Es', 'Fm', 'Md', 'No', 'Lr',
+    'Rf', 'Db', 'Sg', 'Bh', 'Hs', 'Mt', 'Ds', 'Rg', 'Cn', 'Nh', 'Fl', 'Mc',
+    'Lv', 'Ts', 'Og']
+
+atomic_numbers = {}
+for Z, symbol in enumerate(chemical_symbols):
+    atomic_numbers[symbol] = Z
+
+def symbols2numbers(symbols) -> List[int]:
+    numbers = []
+    for s in symbols:
+        if isinstance(s, str):
+            numbers.append(atomic_numbers[s])
+        else:
+            numbers.append(int(s))
+    return numbers
+
+def eles2masses(eles: List[str]) -> List[float]:
+    """将元素列表转换为质量列表
+
+    Parameters
+    ----------
+    eles : List[str]
+        元素列表
+
+    Returns
+    -------
+    List[float]
+        质量列表
+
+    Examples
+    --------
+    >>> from dspawpy.io.utils import eles2masses
+    >>> eles = ["H", "O"]
+    >>> masses = eles2masses(eles)
+    >>> print(masses)
+    [1.00794, 15.9994]
+    """
+    masses = []
+    for e in eles:
+        masses.append(atomic_masses_iupac2016[atomic_numbers[e]])
+    return np.array(masses)
+        
+def get_ma(elements, positions, Natom):
+    """Get the moments of inertia along the principal axes.
+
+    The three principal moments of inertia are computed from the
+    eigenvalues of the symmetric inertial tensor. Periodic boundary
+    conditions are ignored. Units of the moments of inertia are
+    amu*angstrom**2.
+    """
+    masses = eles2masses(elements)
+    com = np.dot(masses, positions) / masses.sum()
+    positions -= com  # translate center of mass to origin
+    masses = eles2masses(elements)
+
+    # Initialize elements of the inertial tensor
+    I11 = I22 = I33 = I12 = I13 = I23 = 0.0
+    for i in range(Natom):
+        x, y, z = positions[i]
+        m = masses[i]
+
+        I11 += m * (y ** 2 + z ** 2)
+        I22 += m * (x ** 2 + z ** 2)
+        I33 += m * (x ** 2 + y ** 2)
+        I12 += -m * x * y
+        I13 += -m * x * z
+        I23 += -m * y * z
+
+    I = np.array([[I11, I12, I13],
+                    [I12, I22, I23],
+                    [I13, I23, I33]])
+
+    evals, evecs = np.linalg.eigh(I)
+    return evals
+
+class IdealGasThermo(): # TODO remove atoms obj
+    """import from ase.thermochemistry.IdealGasThermo
+
+    Parameters
+    ----------
+    vib_energies : list
+        List of vibrational energies in eV.
+    geometry : str
+        One of 'linear', 'nonlinear', 'monatomic'
+    potentialenergy : float
+        Potential energy in eV.
+    elements : list
+        such as ['H', 'O'].
+    symmetrynumber : int
+        Symmetry number.
+    spin : int
+        Spin multiplicity.
+    Natom : int
+        Number of atoms.
+
+    Examples
+    --------
+    >>> from dspawpy.io.utils import IdealGasThermo
+    >>> thermo = IdealGasThermo(vib_energies=[0.1, 0.2, 0.3, 0.4, 0.5, 0.6],
+    ...                         geometry='linear', potentialenergy=0.,  # eV
+    ...                         elements=['H', 'O'], positions=[[0, 0, 0], [0, 0, 1]],  # angstrom
+    ...                         symmetrynumber=None, spin=None, Natom=None)
+    >>> thermo.get_free_energy(298.15)  # K
+
+    """
+    # 读取elements数组代替atoms
+    def __init__(self, vib_energies, geometry, potentialenergy=0.,
+                 elements=None, positions=None,symmetrynumber=None, spin=None, natoms=None):
+        self.potentialenergy = potentialenergy
+        self.geometry = geometry
+        self.elements = elements
+        if isinstance(positions, list):
+            self.positions = np.array(positions, dtype=float)
+        elif isinstance(positions, np.ndarray):
+            self.positions = positions
+        else:
+            raise TypeError('positions must be list or np.ndarray')
+        if isinstance(vib_energies, list):
+            vib_energies = np.array(vib_energies)
+        elif isinstance(vib_energies, np.ndarray):
+            pass
+        else:
+            raise TypeError('vib_energies must be list or np.ndarray')
+        self.sigma = symmetrynumber
+        self.spin = spin
+        if natoms is None:
+            if elements:
+                natoms = len(elements)
+        # Cut the vibrations to those needed from the geometry.
+        if natoms:
+            if geometry == 'nonlinear':
+                self.vib_energies = vib_energies[-(3 * natoms - 6):]
+            elif geometry == 'linear':
+                self.vib_energies = vib_energies[-(3 * natoms - 5):]
+            elif geometry == 'monatomic':
+                self.vib_energies = []
+        else:
+            self.vib_energies = vib_energies
+        # Make sure no imaginary frequencies remain.
+        if sum(np.iscomplex(self.vib_energies)):
+            raise ValueError('Imaginary frequencies are present.')
+        else:
+            self.vib_energies = np.real(self.vib_energies)  # clear +0.j
+        self.referencepressure = 1.0e5  # Pa
+        self.natoms = natoms
+
+    def get_ZPE_correction(self):
+        """Returns the zero-point vibrational energy correction in eV."""
+        zpe = 0.
+        for energy in self.vib_energies:
+            zpe += 0.5 * energy
+        return zpe
+    
+    def _vibrational_energy_contribution(self, temperature):
+        """Calculates the change in internal energy due to vibrations from
+        0K to the specified temperature for a set of vibrations given in
+        eV and a temperature given in Kelvin. Returns the energy change
+        in eV."""
+        kT = k * temperature
+        dU = 0.
+        for energy in self.vib_energies:
+            dU += energy / (np.exp(energy / kT) - 1.)
+        return dU
+    
+    def _vibrational_entropy_contribution(self, temperature):
+        """Calculates the entropy due to vibrations for a set of vibrations
+        given in eV and a temperature given in Kelvin.  Returns the entropy
+        in eV/K."""
+        kT = k * temperature
+        S_v = 0.
+        for energy in self.vib_energies:
+            x = energy / kT
+            S_v += x / (np.exp(x) - 1.) - np.log(1. - np.exp(-x))
+        S_v *= k
+        return S_v
+    
+    def get_enthalpy(self, temperature):
+        """Returns the enthalpy, in eV, in the ideal gas approximation
+        at a specified temperature (K)."""
+
+        fmt = '%-15s%13.3f eV'
+        print('Enthalpy components at T = %.2f K:' % temperature)
+        print('=' * 31)
+
+        H = 0.
+
+        print(fmt % ('E_pot', self.potentialenergy))
+        H += self.potentialenergy
+
+        zpe = self.get_ZPE_correction()
+        print(fmt % ('E_ZPE', zpe))
+        H += zpe
+
+        Cv_t = 3. / 2. * k  # translational heat capacity (3-d gas)
+        print(fmt % ('Cv_trans (0->T)', Cv_t * temperature))
+        H += Cv_t * temperature
+
+        if self.geometry == 'nonlinear':  # rotational heat capacity
+            Cv_r = 3. / 2. * k
+        elif self.geometry == 'linear':
+            Cv_r = k
+        elif self.geometry == 'monatomic':
+            Cv_r = 0.
+        print(fmt % ('Cv_rot (0->T)', Cv_r * temperature))
+        H += Cv_r * temperature
+
+        dH_v = self._vibrational_energy_contribution(temperature)
+        print(fmt % ('Cv_vib (0->T)', dH_v))
+        H += dH_v
+
+        Cp_corr = k * temperature
+        print(fmt % ('(C_v -> C_p)', Cp_corr))
+        H += Cp_corr
+
+        print('-' * 31)
+        print(fmt % ('H', H))
+        print('=' * 31)
+        return H
+
+    def get_entropy(self, temperature, pressure):
+        """Returns the entropy, in eV/K, in the ideal gas approximation
+        at a specified temperature (K) and pressure (Pa)."""
+
+        if self.elements is None or self.sigma is None or self.spin is None:
+            raise RuntimeError('elements, symmetrynumber, and spin must be '
+                               'specified for entropy and free energy '
+                               'calculations.')
+        S = 0.0
+        # Translational entropy (term inside the log is in SI units).
+        mass = sum(eles2masses(self.elements)) * amu  # kg/molecule
+        S_t = (2 * np.pi * mass * kB *
+               temperature / h**2)**(3.0 / 2)
+        S_t *= kB * temperature / self.referencepressure
+        S_t = k * (np.log(S_t) + 5.0 / 2.0)
+        S += S_t
+
+        # Rotational entropy (term inside the log is in SI units).
+        if self.geometry == 'monatomic':
+            S_r = 0.0
+        elif self.geometry == 'nonlinear':
+            inertias = (get_ma(self.elements, self.positions, self.natoms) * amu /
+                        (10.0**10)**2)  # kg m^2
+            S_r = np.sqrt(np.pi * np.product(inertias)) / self.sigma
+            S_r *= (8.0 * np.pi**2 * kB * temperature /
+                    h**2)**(3.0 / 2.0)
+            S_r = k * (np.log(S_r) + 3.0 / 2.0)
+        elif self.geometry == 'linear':
+            inertias = (get_ma(self.elements, self.positions, self.natoms) * amu /
+                        (10.0**10)**2)  # kg m^2
+            inertia = max(inertias)  # should be two identical and one zero
+            S_r = (8 * np.pi**2 * inertia * kB * temperature /
+                   self.sigma / h**2)
+            S_r = k * (np.log(S_r) + 1.)
+        S += S_r
+        # Electronic entropy.
+        S_e = k * np.log(2 * self.spin + 1)
+        S += S_e
+        # Vibrational entropy.
+        S_v = self._vibrational_entropy_contribution(temperature)
+        S += S_v
+        # Pressure correction to translational entropy.
+        S_p = - k * np.log(pressure / self.referencepressure)
+        S += S_p
+        return S
+
+    def get_gibbs_energy(self, temperature, pressure):
+        """Returns the Gibbs free energy, in eV, in the ideal gas
+        approximation at a specified temperature (K) and pressure (Pa)."""
+
+
+        H = self.get_enthalpy(temperature)
+        print('')
+        S = self.get_entropy(temperature, pressure)
+        G = H - temperature * S
+
+        print('')
+        print('Free energy components at T = %.2f K and P = %.1f Pa:' %
+              (temperature, pressure))
+        print('=' * 23)
+        fmt = '%5s%15.3f eV'
+        print(fmt % ('H', H))
+        print(fmt % ('-T*S', -temperature * S))
+        print('-' * 23)
+        print(fmt % ('G', G))
+        print('=' * 23)
+        return G
+
+def getTSgas(fretxt='frequency.txt',
+            datafile='.',
+            potentialenergy=0, # eV
+            elements=None,
+            geometry='linear',
+            positions=None, # Angstrom
+            symmetrynumber=1,
+            spin=1,
+            temperature=298.15,
+            pressure=101325):
+    """理想气体近似下，计算熵的能量贡献
+
+
+    Parameters
+    ----------
+    fretxt : str
+        记录频率信息的文件所在路径, 默认当前路径下的'frequency.txt'
+    datafile : str
+        计算结果json或h5文件或包含它们的文件夹路径, 默认当前路径；
+        如果设置为None，则需要传入elements和positions参数
+    potentialenergy : float
+        势能，单位eV
+    elements : list
+        元素列表，如果
+    geometry : str
+        分子几何，monatomic, linear, nonlinear
+    positions : list
+        原子坐标，单位Angstrom
+    symmetrynumber : int
+        对称数
+    spin : int
+        自旋数
+    temperature : float
+        温度，单位K
+    pressure : float
+        压强，单位Pa
+    
+    Returns
+    -------
+    TSgas : float
+        理想气体近似下，计算熵的能量贡献，单位eV
+
+    Examples
+    --------
+    >>> from dspawpy.io.utils import getTSgas
+    >>> TSgas = getTSgas(fretxt='frequency.txt', datafile=None, potentialenergy=-0.0, elements=['H', 'H'], geometry='linear', positions=[[0.0, 0.0, 0.0], [0.0, 0.0, 1.0]], symmetrynumber=1, spin=1, temperature=298.15, pressure=101325.0)
+    >>> TSgas
+    0.5037357905277046
+    >>> TSgas = getTSgas(fretxt='frequency.txt', datafile='.', potentialenergy=-0.0,  geometry='linear', symmetrynumber=1, spin=1, temperature=298.15, pressure=101325.0)
+    >>> TSgas
+    0.6790991704342505
+    """
+    ve = []
+    with open(fretxt) as ft:
+        lines = ft.readlines()
+        for i in range(2, len(lines)):
+            if lines[i].strip()[1] == 'f/i':
+                ve.append(complex(lines[i].split()[-1])/1000)
+            else:
+                ve.append(float(lines[i].split()[-1])/1000)
+
+    if datafile: # skip if datafile is None
+        # search datafile in the given directory
+        if os.path.isdir(datafile):
+            directory = datafile  # specified datafile is actually a directory
+            print("您指定了一个文件夹，正在查找相关h5或json文件...")
+            if os.path.exists(os.path.join(directory, "frequency.h5")):
+                datafile = os.path.join(directory, "frequency.h5")
+                print("Reading frequency.h5...")
+            elif os.path.exists(os.path.join(directory, "frequency.json")):
+                datafile = os.path.join(directory, "frequency.json")
+                print("Reading frequency.json...")
+            else:
+                raise FileNotFoundError("未找到frequency.h5/frequency.json文件！")
+        if datafile.endswith(".h5"):
+            eles = get_ele_from_h5(datafile)
+            import h5py
+            data = h5py.File(datafile)
+            poses = np.array(data.get("/AtomInfo/Position")).reshape(-1, 3)
+
+        elif datafile.endswith(".json"):
+            import json
+            with open(datafile) as f:
+                data = json.load(f)
+            atoms = data["AtomInfo"]['Atoms']
+            eles = []
+            poses = []
+            for i in range(len(atoms)):
+                eles.append(atoms[i]["Element"])
+                poses.append(atoms[i]["Position"])
+        else:
+            raise TypeError("仅支持读取h5或json文件！")
+    else:
+        eles = elements
+        poses = positions
+
+    # 计算熵的能量贡献
+    thermo = IdealGasThermo(vib_energies=ve, # eV
+                            potentialenergy=potentialenergy, # eV
+                            elements=eles,
+                            geometry=geometry,
+                            positions=poses, # Angstrom
+                            symmetrynumber=symmetrynumber,
+                            spin=spin)
+    S = thermo.get_entropy(temperature, pressure)
+
+    return S*temperature
 
 def d_band(spin, dos_data):  # 定义函数，括号里给出函数的两个变量
     """计算d带中心
 
     Parameters
     ----------
     spin : Spin.up或Spin.down
@@ -72,15 +618,15 @@
 
 
 def get_pos_ele_lat(spath: str):
     """从DSPAW的as结构文件中读取坐标、元素列表，和晶胞信息
 
     Parameters
     ----------
-    path : str
+    spath : str
         结构文件路径
 
     Returns
     -------
     pos : np.ndarray
         坐标分量数组，Natom x 3
     ele : list
@@ -175,91 +721,130 @@
             spos = coord
         else:
             raise ValueError(f"{spath}中的坐标类型未知！")
 
     return spos, ele, latv
 
 
-def thermo_correction(fretxt: str = "frequency.txt", T: float = 298.15):
-    """从fretext中读取数据，计算ZPE和TS
+def getZPE(fretxt: str = "frequency.txt"):
+    """从fretext中读取数据，计算ZPE
 
     将另外保存结果到 ZPE_TS.dat 中
 
     Parameters
     ----------
     fretxt : str
         记录频率信息的文件所在路径, 默认当前路径下的'frequency.txt'
-    T : float
-        温度，单位K, 默认298.15
 
     Returns
     -------
     ZPE: float
         零点能
-    TS: float
-        熵校正
 
     Examples
     --------
-    >>> from dspawpy.io.utils import thermo_correction
-    >>> ZPE, TS = thermo_correction(fretxt='frequency.txt', T=298.15)
+    >>> from dspawpy.io.utils import getZPE
+    >>> ZPE= getZPE(fretxt='frequency.txt', T=298.15)
     >>> ZPE
     0.8842567390000002
-    >>> TS
-    0.18362317157111566
     """
 
     # 1. read data
     data_get_ZPE = []
-    data_get_TS = []
-
     with open(fretxt, "r") as f:
         for line in f.readlines():
             data_line = line.strip().split()
             if len(data_line) != 6:
                 continue
             if data_line[1] == "f":
                 data_get_ZPE.append(float(data_line[5]))
-                data_get_TS.append(float(data_line[2]))
 
     data_get_ZPE = np.array(data_get_ZPE)
-    data_get_TS = np.array(data_get_TS)
 
     # 2. printout to check
     print(f"=== 从{fretxt}中读取到的相关如下 ===")
-    dt = pd.DataFrame({'Frequency (meV)':data_get_ZPE, 'Frequency (THz)':data_get_TS}, index=None)
+    dt = pd.DataFrame({'Frequency (meV)':data_get_ZPE}, index=None)
     print(dt)
 
     if len(data_get_ZPE) == 0:
         raise ValueError("全是虚频，请考虑重新优化结构...")
     else:
-        print("\n正在写入ZPE_TS.dat文件...")
+        print("\n正在写入ZPE.dat文件...")
         np.savetxt(
-            "ZPE_TS.dat",
-            np.array([data_get_ZPE, data_get_TS]).T,
+            "ZPE.dat",
+            np.array(data_get_ZPE).T,
             fmt="%.6f",
-            header="ZPE(meV) \t TS(THz)",
+            header="Frequency (meV)",
             comments=f"Data read from {os.path.abspath(fretxt)}\n",
         )
 
     # 3. calculate
     ZPE = 0
     for data in data_get_ZPE:
         ZPE += data / 2000.0
     print("\n--> Zero-point energy,  ZPE (eV):", ZPE)
 
-    # T = 298.15 #温度 单位：K
-    # S = 0
-    Na = 6.02214179e23  # 阿伏伽德罗常数 单位 /mol
-    h = 6.6260696e-34  # 普朗克常数 单位J*s
-    kB = 1.3806503e-23  # 玻尔兹曼常数 J/K
-    R = Na * kB  # 理想气体常数 J/(K*mol)
-    # THz = 1e+12 # 1 Hz = 1e+12 THz
-    # e = 1.60217653E-19 #单位 C
+    with open("ZPE.dat", "a") as f:
+        f.write(f"\n--> Zero-point energy,  ZPE (eV): {ZPE}")
+
+    return ZPE
 
+def getTSads(fretxt: str = "frequency.txt", T: float = 298.15):
+    """从fretext中读取数据，计算ZPE和TS
+
+    将另外保存结果到 ZPE_TS.dat 中
+
+    Parameters
+    ----------
+    fretxt : str
+        记录频率信息的文件所在路径, 默认当前路径下的'frequency.txt'
+    T : float
+        温度，单位K, 默认298.15
+
+    Returns
+    -------
+    TS: float
+        熵校正
+
+    Examples
+    --------
+    >>> from dspawpy.io.utils import getTSads
+    >>> TS = getTSads(fretxt='frequency.txt', T=298.15)
+    >>> TS
+    0.18362317157111566
+    """
+    data_get_TS = []
+    with open(fretxt, "r") as f:
+        for line in f.readlines():
+            data_line = line.strip().split()
+            if len(data_line) != 6:
+                continue
+            if data_line[1] == "f":
+                data_get_TS.append(float(data_line[2]))
+
+    data_get_TS = np.array(data_get_TS)
+
+    # 2. printout to check
+    print(f"=== 从{fretxt}中读取到的相关如下 ===")
+    dt = pd.DataFrame({'Frequency (THz)':data_get_TS}, index=None)
+    print(dt)
+
+    if len(data_get_TS) == 0:
+        raise ValueError("全是虚频，请考虑重新优化结构...")
+    else:
+        print("\n正在写入TS.dat文件...")
+        np.savetxt(
+            "TS.dat",
+            np.array(data_get_TS).T,
+            fmt="%.6f",
+            header="Frequency (THz)",
+            comments=f"Data read from {os.path.abspath(fretxt)}\n",
+        )
+
+    # 3. calculate
     sum_S = 0
     import math  # 因为要使用 e的多少次方，ln（）对数
 
     for vi_THz in data_get_TS:
         vi_Hz = vi_THz * 1e12
         m1 = h * Na * vi_Hz
         m2 = h * vi_Hz / (kB * T)
@@ -271,20 +856,54 @@
         m8 = m1 / m4 - m7  # S 单位J/(mol*K)
         m9 = (T * m8 / 1000) / 96.49  # T*S,将单位化为KJ/mol, 96.49 kJ/mol = 1 eV 单位eV
         sum_S += m9
 
     print("--> Entropy contribution, T*S (eV)：", sum_S)
 
     with open("ZPE_TS.dat", "a") as f:
-        f.write(f"\n--> Zero-point energy,  ZPE (eV): {ZPE}")
         f.write(f"\n--> Entropy contribution, T*S (eV): {sum_S}\n")
 
+    return sum_S
+
+
+def thermo_correction(fretxt: str = "frequency.txt", T: float = 298.15):
+    """从fretext中读取数据，计算ZPE和TS
+    将另外保存结果到 ZPE_TS.dat 中
+
+    Parameters
+    ----------
+    fretxt : str
+        记录频率信息的文件所在路径, 默认当前路径下的'frequency.txt'
+    T : float
+        温度，单位K, 默认298.15
+
+    Returns
+    -------
+    ZPE: float
+        零点能
+    TS: float
+        熵校正
+
+    Examples
+    --------
+    >>> from dspawpy.io.utils import thermo_correction
+    >>> ZPE, TS = thermo_correction(fretxt='frequency.txt', T=298.15)
+    >>> ZPE
+    0.8842567390000002
+    >>> TS
+    0.18362317157111566
+    """
+
+    ZPE = getZPE(fretxt=fretxt)
+    sum_S = getTSads(fretxt=fretxt, T=T)
+
     return ZPE, sum_S
 
 
+
 def get_lines_without_comment(filename: str, comment: str = "#") -> List[str]:
     lines = []
     with open(filename) as file:
         while True:
             line = file.readline()
             if line:
                 line = re.sub(comment + r".*$", "", line)  # remove comment
```

## Comparing `dspawpy-0.8.6.dist-info/METADATA` & `dspawpy-0.8.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspawpy
-Version: 0.8.6
+Version: 0.8.7
 Summary: Tools for dspaw
 Home-page: http://www.hzwtech.com/
 Author: Hzwtech
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Requires-Dist: pymatgen (>=2021.2.8.1)
```

