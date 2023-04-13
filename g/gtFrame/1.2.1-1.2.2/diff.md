# Comparing `tmp/gtFrame-1.2.1.tar.gz` & `tmp/gtFrame-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtFrame-1.2.1.tar", last modified: Sun Apr  2 12:53:38 2023, max compression
+gzip compressed data, was "gtFrame-1.2.2.tar", last modified: Thu Apr 13 17:52:40 2023, max compression
```

## Comparing `gtFrame-1.2.1.tar` & `gtFrame-1.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 12:53:38.452631 gtFrame-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-02 12:53:21.000000 gtFrame-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-02 12:53:38.452631 gtFrame-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-02 12:53:21.000000 gtFrame-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 12:53:38.452631 gtFrame-1.2.1/gtFrame/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-02 12:53:21.000000 gtFrame-1.2.1/gtFrame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21879 2023-04-02 12:53:21.000000 gtFrame-1.2.1/gtFrame/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-04-02 12:53:21.000000 gtFrame-1.2.1/gtFrame/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-04-02 12:53:21.000000 gtFrame-1.2.1/gtFrame/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-04-02 12:53:21.000000 gtFrame-1.2.1/gtFrame/rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 12:53:38.452631 gtFrame-1.2.1/gtFrame.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-02 12:53:38.000000 gtFrame-1.2.1/gtFrame.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-02 12:53:38.000000 gtFrame-1.2.1/gtFrame.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 12:53:38.000000 gtFrame-1.2.1/gtFrame.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-02 12:53:38.000000 gtFrame-1.2.1/gtFrame.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-02 12:53:38.000000 gtFrame-1.2.1/gtFrame.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-02 12:53:21.000000 gtFrame-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 12:53:38.452631 gtFrame-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 12:53:21.000000 gtFrame-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 12:53:38.452631 gtFrame-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    46338 2023-04-02 12:53:21.000000 gtFrame-1.2.1/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    23157 2023-04-02 12:53:21.000000 gtFrame-1.2.1/tests/test_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20554 2023-04-02 12:53:21.000000 gtFrame-1.2.1/tests/test_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-04-02 12:53:21.000000 gtFrame-1.2.1/tests/test_rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:52:40.043404 gtFrame-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-13 17:52:30.000000 gtFrame-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-13 17:52:40.043404 gtFrame-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-13 17:52:30.000000 gtFrame-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:52:40.043404 gtFrame-1.2.2/gtFrame/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-13 17:52:30.000000 gtFrame-1.2.2/gtFrame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22991 2023-04-13 17:52:30.000000 gtFrame-1.2.2/gtFrame/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-04-13 17:52:30.000000 gtFrame-1.2.2/gtFrame/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14238 2023-04-13 17:52:30.000000 gtFrame-1.2.2/gtFrame/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-04-13 17:52:30.000000 gtFrame-1.2.2/gtFrame/rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:52:40.043404 gtFrame-1.2.2/gtFrame.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-13 17:52:40.000000 gtFrame-1.2.2/gtFrame.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-13 17:52:40.000000 gtFrame-1.2.2/gtFrame.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:52:40.000000 gtFrame-1.2.2/gtFrame.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 17:52:40.000000 gtFrame-1.2.2/gtFrame.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 17:52:40.000000 gtFrame-1.2.2/gtFrame.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-13 17:52:30.000000 gtFrame-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 17:52:40.043404 gtFrame-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 17:52:30.000000 gtFrame-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:52:40.043404 gtFrame-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    48296 2023-04-13 17:52:30.000000 gtFrame-1.2.2/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23157 2023-04-13 17:52:30.000000 gtFrame-1.2.2/tests/test_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35544 2023-04-13 17:52:30.000000 gtFrame-1.2.2/tests/test_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-04-13 17:52:30.000000 gtFrame-1.2.2/tests/test_rotation.py
```

### Comparing `gtFrame-1.2.1/LICENSE` & `gtFrame-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gtFrame-1.2.1/PKG-INFO` & `gtFrame-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtFrame
-Version: 1.2.1
+Version: 1.2.2
 Summary: A simple library for working with frames of reference
 Author-email: "Roko Jukic (bluePlatinum)" <jukic.rok@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Roko Jukic. All rights reserved
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gtFrame-1.2.1/gtFrame/basic.py` & `gtFrame-1.2.2/gtFrame/basic.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,26 @@
     def __init__(self):
         """
         Constructor method. Sets position to [0, 0] and rotation to 0.
         """
         self.position = np.array([0, 0], dtype=np.float64)
         self.rotation = gtFrame.rotation.Rotation2d(0)
 
+    def __deepcopy__(self, memo):
+        """
+        The deepcopy method for RootFrame2d just returns itself, as is does not
+        make any sense to copy a root frame.
+
+        :param memo: required memo argument
+        :type memo: dict
+        :return: the deepcopy of RootFrame2d, which is just self
+        :rtype: RootFrame2d
+        """
+        return self
+
     def find_transform_path(self, frame):
         """
         Finds the transform path from this frame of reference to the given
         frame.
 
         :param frame: the frame of reference to find a transform path to
         :type frame: Frame2d
@@ -48,14 +60,23 @@
         current_frame = frame
         while current_frame != self:
             path.append((current_frame, "from"))
             current_frame = current_frame.parent()
 
         return path[::-1]      # path is generated in reverse
 
+    def parent(self):
+        """
+        Returns the parent of the Frame. For RootFrame2d this is self.
+
+        :return: self
+        :rtype: RootFrame2d
+        """
+        return self
+
     def transform_from(self, frame, vector):
         """
         Transform a vector expressed in an arbitrary frame of reference into
         this frame.
         :param frame: the frame of reference, in which the vector is defined
         :type frame: Frame2d
         :param vector: the vector to be transformed
@@ -339,14 +360,26 @@
         Constructor method
         """
         self.position = np.array([0, 0, 0], dtype=np.float64)
         self.rotation = Rotation3d.from_euler('xyz', np.array(
                                                         [0, 0, 0],
                                                         dtype=np.float64))
 
+    def __deepcopy__(self, memo):
+        """
+        The deepcopy method for RootFrame3d just returns itself, as is does not
+        make any sense to copy a root frame.
+
+        :param memo: required memo argument
+        :type memo: dict
+        :return: the deepcopy of RootFrame3d, which is just self
+        :rtype: RootFrame3d
+        """
+        return self
+
     def find_transform_path(self, frame):
         """
         Finds the transform path from this frame of reference to the given
         frame.
 
         :param frame: the frame of reference to find a transform path to
         :type frame: Frame3d
@@ -357,14 +390,23 @@
         current_frame = frame
         while current_frame != self:
             path.append((current_frame, "from"))
             current_frame = current_frame.parent()
 
         return path[::-1]      # path is generated in reverse
 
+    def parent(self):
+        """
+        Returns the parent of the Frame. For RootFrame3d this is self.
+
+        :return: self
+        :rtype: RootFrame3d
+        """
+        return self
+
     def transform_from(self, frame, vector):
         """
         Transform a vector expressed in an arbitrary frame of reference into
         this frame.
         :param frame: the frame of reference, in which the vector is defined
         :type frame: Frame3d
         :param vector: the vector to be transformed
```

### Comparing `gtFrame-1.2.1/gtFrame/direction.py` & `gtFrame-1.2.2/gtFrame/direction.py`

 * *Files identical despite different names*

### Comparing `gtFrame-1.2.1/gtFrame/position.py` & `gtFrame-1.2.2/gtFrame/position.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 Module Contents
 ---------------
 Classes:
     * Position2d
     * Position3d
 
 """
+import copy
 import numpy as np
 
 from gtFrame import DEFAULT_RTOL
+from gtFrame.basic import RootFrame2d, RootFrame3d
 from gtFrame.direction import Direction2d, Direction3d
 
 
 class Position2d:
     """
     This class holds the coordinates of a 2d vector in a numpy array and the
     frame of reference in which they have been defined.
@@ -126,14 +128,74 @@
         :type reference: gtFrame.basic.Frame2d
         :return: the transformed coordinates
         :rtype: np.ndarray
         """
         return self.reference.transform_to(reference, self.coordinates)
 
 
+class BoundPosition2d(Position2d):
+    """
+    This is a wrapper class for Position2d. It has the same functionality as
+    :class:`gtFrame.position.BoundPosition2d`, only that the frame is bound to
+    the position and gets updated instead of the coordinates.
+
+    :param coordinates: the coordinates of the 2d-vector representing a point
+        in space
+    :type coordinates: np.ndarray
+    :param reference: the reference in which the coordinates are defined
+    :type reference: gtFrame.basic.Frame2d
+    :param rtol: The relative tolerance to be used when comparing
+        Position2d objects. The default is set to the global variable
+        DEFAULT_RTOL.
+    :type rtol: float
+    """
+    def __init__(self, coordinates, reference, rtol=DEFAULT_RTOL):
+        """
+        Constructor method.
+        """
+        if isinstance(reference, RootFrame2d):
+            raise TypeError("BoundPosition2d cannot take RootFrame2d as "
+                            "reference")
+
+        super().__init__(coordinates, reference, rtol)
+
+    def add_direction(self, direction):
+        """
+        Returns the point that results in adding a direction vector to this
+        point.
+
+        :param direction: a direction vector to be added to the point
+        :type direction: gtFrame.direction.Direction2d
+        :return: The resulting point from the addition with a direction vector.
+            The returned Position2d object will inherit the reference and rtol
+            of this (self) object.
+        :rtype: BoundPosition2d
+        """
+        rotated = direction.transform_to(self.reference.parent())
+        new = copy.deepcopy(self)
+        new.reference.position += rotated
+        return new
+
+    def apply_direction(self, direction):
+        """
+        Adds a given direction vector to this Position2d object. This results
+        in the same point as would be returned by the .add_direction method.
+        The difference is that .apply_direction applies the changes to the
+        coordinates from this object, while .add_direction creates a new
+        :class:`gtFrame.direction.Position2d` object with the modified
+        coordinates.
+
+        :param direction: a direction vector to be added to the point
+        :type direction: gtFrame.direction.Direction2d
+        :return: None
+        """
+        rotated = direction.transform_to(self.reference.parent())
+        self.reference.position = self.reference.position + rotated
+
+
 class Position3d:
     """
     This class holds the coordinates of a 3d vector in a numpy array and the
     frame of reference in which they have been defined.
 
     :param coordinates: the coordinates of the 3d-vector representing a point
         in space
@@ -237,7 +299,67 @@
         :param reference: the desired reference for the coordinates to be
             transformed into
         :type reference: gtFrame.basic.Frame3d
         :return: the transformed coordinates
         :rtype: np.ndarray
         """
         return self.reference.transform_to(reference, self.coordinates)
+
+
+class BoundPosition3d(Position3d):
+    """
+    This is a wrapper class for Position3d. It has the same functionality as
+    :class:`gtFrame.position.BoundPosition3d`, only that the frame is bound to
+    the position and gets updated instead of the coordinates.
+
+    :param coordinates: the coordinates of the 3d-vector representing a point
+        in space
+    :type coordinates: np.ndarray
+    :param reference: the reference in which the coordinates are defined
+    :type reference: gtFrame.basic.Frame3d
+    :param rtol: The relative tolerance to be used when comparing
+        Position3d objects. The default is set to the global variable
+        DEFAULT_RTOL.
+    :type rtol: float
+    """
+    def __init__(self, coordinates, reference, rtol=DEFAULT_RTOL):
+        """
+        Constructor method.
+        """
+        if isinstance(reference, RootFrame3d):
+            raise TypeError("BoundPosition3d cannot take RootFrame3d as "
+                            "reference")
+
+        super().__init__(coordinates, reference, rtol)
+
+    def add_direction(self, direction):
+        """
+        Returns the point that results in adding a direction vector to this
+        point.
+
+        :param direction: a direction vector to be added to the point
+        :type direction: gtFrame.direction.Direction3d
+        :return: The resulting point from the addition with a direction vector.
+            The returned Position3d object will inherit the reference and rtol
+            of this (self) object.
+        :rtype: BoundPosition3d
+        """
+        rotated = direction.transform_to(self.reference.parent())
+        new = copy.deepcopy(self)
+        new.reference.position += rotated
+        return new
+
+    def apply_direction(self, direction):
+        """
+        Adds a given direction vector to this Position3d object. This results
+        in the same point as would be returned by the .add_direction method.
+        The difference is that .apply_direction applies the changes to the
+        coordinates from this object, while .add_direction creates a new
+        :class:`gtFrame.direction.Position3d` object with the modified
+        coordinates.
+
+        :param direction: a direction vector to be added to the point
+        :type direction: gtFrame.direction.Direction3d
+        :return: None
+        """
+        rotated = direction.transform_to(self.reference.parent())
+        self.reference.position = self.reference.position + rotated
```

### Comparing `gtFrame-1.2.1/gtFrame/rotation.py` & `gtFrame-1.2.2/gtFrame/rotation.py`

 * *Files identical despite different names*

### Comparing `gtFrame-1.2.1/gtFrame.egg-info/PKG-INFO` & `gtFrame-1.2.2/gtFrame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtFrame
-Version: 1.2.1
+Version: 1.2.2
 Summary: A simple library for working with frames of reference
 Author-email: "Roko Jukic (bluePlatinum)" <jukic.rok@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Roko Jukic. All rights reserved
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gtFrame-1.2.1/pyproject.toml` & `gtFrame-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'gtFrame'
-version = '1.2.1'
+version = '1.2.2'
 authors = [
     { name='Roko Jukic (bluePlatinum)', email='jukic.rok@gmail.com'},
 ]
 description = 'A simple library for working with frames of reference'
 readme = 'README.md'
 license = {file='LICENSE'}
 requires-python = '>=3.7'
```

### Comparing `gtFrame-1.2.1/tests/test_basic.py` & `gtFrame-1.2.2/tests/test_basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """
 Tests for the :mod:`gtFrame.basic` module.
 """
+import copy
 import math
 import random
 
 import numpy as np
 import pytest
 from scipy.spatial.transform import Rotation as Rotation3d
 
 import gtFrame.basic
 from gtFrame.basic import Frame2d
 from gtFrame.basic import Frame3d
 from gtFrame.basic import origin2d
 from gtFrame.basic import origin3d
 from gtFrame.basic import RootFrame2d
 from gtFrame.basic import RootFrame3d
+from gtFrame.position import Position2d
+from gtFrame.position import Position3d
 from gtFrame.rotation import Rotation2d
 
 # TOLERANCES
 RTOL = 1e-12
 
 
 def generate_frame2d(parent=origin2d):
@@ -186,14 +189,40 @@
         :return: None
         """
         root_frame = RootFrame2d()
 
         assert np.allclose(root_frame.position, np.array([0, 0]), rtol=RTOL)
         assert root_frame.rotation.as_rad() == 0
 
+    def test_deepcopy_simple(self):
+        """
+        Test the :meth:`gtFrame.basic.RootFrame2d.__deepcopy__` method with a
+        simple `copy.deepcopy()` call.
+
+        :return: None
+        """
+        root_frame = RootFrame2d()
+
+        assert copy.deepcopy(root_frame) == root_frame
+
+    def test_deepcopy_nested(self):
+        """
+        Test the :meth:`gtFrame.basic.RootFrame2d.__deepcopy__` method with a
+        nested `copy.deepcopy()` call.
+
+        :return: None
+        """
+        coordinates = np.random.random(2)
+        frame = generate_frame2d(parent=origin2d)
+        position = Position2d(coordinates, frame)
+
+        copy_position = copy.deepcopy(position)
+
+        assert copy_position.reference.parent() == origin2d
+
     def test_find_transform_path(self, frame2d_system):
         """
         Test the find_transform_path method of RootFrame2d with static
         system-structure but random positions and rotations.
 
         :return: None
         """
@@ -218,14 +247,22 @@
         assert expected2 == origin2d.find_transform_path(frame2)
         assert expected3 == origin2d.find_transform_path(frame3)
         assert expected4 == origin2d.find_transform_path(frame4)
         assert expected5 == origin2d.find_transform_path(frame5)
         assert expected6 == origin2d.find_transform_path(frame6)
         assert expected7 == origin2d.find_transform_path(frame7)
 
+    def test_parent(self):
+        """
+        Test the :meth:`gtFrame.basic.RootFrame2d.parent` method.
+        """
+        frame = RootFrame2d()
+
+        assert frame.parent() == frame
+
     def test_transform_from(self, frame2d_system):
         """
         Test the .transform_from method with random vectors and random paths.
         :return: None
         """
         vectors = [np.random.random(2) for _ in range(10)]
 
@@ -737,14 +774,40 @@
         frame = RootFrame3d()
 
         assert np.allclose(frame.position,
                            np.array([0, 0, 0], dtype=np.float64), rtol=RTOL)
         assert np.allclose(frame.rotation.as_matrix(), np.identity(3),
                            rtol=RTOL)
 
+    def test_deepcopy_simple(self):
+        """
+        Test the :meth:`gtFrame.basic.RootFrame2d.__deepcopy__` method with a
+        simple `copy.deepcopy()` call.
+
+        :return: None
+        """
+        root_frame = RootFrame3d()
+
+        assert copy.deepcopy(root_frame) == root_frame
+
+    def test_deepcopy_nested(self):
+        """
+        Test the :meth:`gtFrame.basic.RootFrame2d.__deepcopy__` method with a
+        nested `copy.deepcopy()` call.
+
+        :return: None
+        """
+        coordinates = np.random.random(3)
+        frame = generate_frame3d(parent=origin3d)
+        position = Position3d(coordinates, frame)
+
+        copy_position = copy.deepcopy(position)
+
+        assert copy_position.reference.parent() == origin3d
+
     def test_find_transform_path(self, frame3d_system):
         """
         Test the find_transform_path method of RootFrame3d with static
         system-structure but random positions and rotations.
 
         :return: None
         """
@@ -769,14 +832,22 @@
         assert expected2 == origin3d.find_transform_path(frame2)
         assert expected3 == origin3d.find_transform_path(frame3)
         assert expected4 == origin3d.find_transform_path(frame4)
         assert expected5 == origin3d.find_transform_path(frame5)
         assert expected6 == origin3d.find_transform_path(frame6)
         assert expected7 == origin3d.find_transform_path(frame7)
 
+    def test_parent(self):
+        """
+        Test the :meth:`gtFrame.basic.RootFrame3d.parent` method.
+        """
+        frame = RootFrame3d()
+
+        assert frame.parent() == frame
+
     def test_transform_from(self, frame3d_system):
         """
         Test the .transform_from method with random vectors and random paths.
         :return: None
         """
         vectors = [np.random.random(3) for _ in range(10)]
```

### Comparing `gtFrame-1.2.1/tests/test_direction.py` & `gtFrame-1.2.2/tests/test_direction.py`

 * *Files identical despite different names*

### Comparing `gtFrame-1.2.1/tests/test_position.py` & `gtFrame-1.2.2/tests/test_position.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+import copy
 import math
 import random
 
 import numpy as np
 import pytest
 from scipy.spatial.transform import Rotation as Rotation3d
 
 from gtFrame import DEFAULT_RTOL
 from gtFrame.basic import Frame2d, Frame3d, origin2d, origin3d
+from gtFrame.basic import RootFrame2d, RootFrame3d
 from gtFrame.direction import Direction2d, Direction3d
+from gtFrame.position import BoundPosition2d, BoundPosition3d
 from gtFrame.position import Position2d, Position3d
 from gtFrame.rotation import Rotation2d
 
 # TOLERANCES
 RTOL = 1e-12
 
 # Defines how many iterations tests should run which run multiple times.
@@ -91,14 +94,48 @@
     :rtype: gtFrame.basic.Frame3d
     """
     rotation = Rotation3d.from_rotvec(np.random.random(3))
     position = np.random.random(3)
     return Frame3d(position, rotation, parent_frame=parent)
 
 
+def random_boundposition2d(coordinates=None, reference=None):
+    """
+    Generates a random BoundPosition2d object with random values.
+
+    :param coordinates: override random coordinates assigned to object
+    :type coordinates: np.ndarray
+    :param reference: override random reference assigned to object
+    :type reference: gtFrame.basic.Frame2d
+    """
+    if coordinates is None:
+        coordinates = np.random.random(2)
+    if reference is None:
+        reference = random_frame2d()
+
+    return BoundPosition2d(coordinates, reference)
+
+
+def random_boundposition3d(coordinates=None, reference=None):
+    """
+    Generates a random BoundPosition3d object with random values.
+
+    :param coordinates: override random coordinates assigned to object
+    :type coordinates: np.ndarray
+    :param reference: override random reference assigned to object
+    :type reference: gtFrame.basic.Frame3d
+    """
+    if coordinates is None:
+        coordinates = np.random.random(3)
+    if reference is None:
+        reference = random_frame3d()
+
+    return BoundPosition3d(coordinates, reference)
+
+
 def random_position2d(coordinates=None, reference=None):
     """
     Generates a random Position2d object with random values.
 
     :param coordinates: override random coordinates assigned to object
     :type coordinates: np.ndarray
     :param reference: override random reference assigned to object
@@ -125,14 +162,211 @@
         coordinates = np.random.random(3)
     if reference is None:
         reference = random_frame3d()
 
     return Position3d(coordinates, reference)
 
 
+class TestBoundPosition2d:
+    """
+    Holds tests for BoundPosition2d
+    """
+    def test_constructor_assign(self):
+        """
+        Tests whether the constructor correctly assigns the attributes.
+
+        :return: None
+        """
+        coordinates = np.random.random(2)
+        frame = random_frame2d()
+
+        position = BoundPosition2d(coordinates, frame)
+
+        assert np.allclose(position.coordinates, coordinates, rtol=RTOL)
+        assert position.reference == frame
+
+    def test_constructor_exception_coordinates(self):
+        """
+        Tests whether the constructor raises an error if the wrong dimension
+        vector is passed.
+
+        :return: None
+        """
+        coordinates = np.random.random(random.randint(3, 100))
+        frame = random_frame2d()
+
+        with pytest.raises(ValueError):
+            position = BoundPosition2d(coordinates, frame)       # noqa: F841
+
+    def test_construction_exception_reference(self):
+        """
+        Tests whether the constructor raises an error if a RootFrame2d is
+        passed as a reference.
+        """
+        coordinates = np.random.random(2)
+        frame = RootFrame2d()
+
+        with pytest.raises(TypeError):
+            BoundPosition2d(coordinates, frame)
+
+    def test_constructor_tolerances(self):
+        """
+        Test the assignment of the rtol attribute on init.
+        """
+        coordinates = np.random.random(2)
+        frame = random_frame2d()
+        rtol = random.random()
+
+        position_a = BoundPosition2d(coordinates, frame)
+        position_b = BoundPosition2d(coordinates, frame, rtol=rtol)
+
+        assert position_a.rtol == DEFAULT_RTOL
+        assert position_b.rtol == rtol
+
+    def test_eq(self):
+        """
+        Tests the == operator (i.e. the __eq__ method).
+
+        :return: None
+        """
+        coordinates = np.random.random(2)
+        frame_a = random_frame2d()
+        frame_b = random_frame2d()
+
+        position_a = BoundPosition2d(coordinates, frame_a)
+        position_b = BoundPosition2d(frame_b.transform_from(frame_a,
+                                                            coordinates),
+                                     frame_b)
+
+        assert position_a == position_b
+
+    def test_eq_agnostic(self):
+        """
+        Test the == operator with agnostic Position types. So compare Position
+        with BoundPosition.
+        """
+        coordinates = np.random.random(2)
+        frame_a = random_frame2d()
+        frame_b = random_frame2d()
+
+        position_a = Position2d(coordinates, frame_a)
+        position_b = BoundPosition2d(frame_b.transform_from(frame_a,
+                                                            coordinates),
+                                     frame_b)
+
+        assert position_a == position_b
+
+    def test_add_direction_static(self):
+        """
+        Tests the .add_direction method with static testcases. This test
+        assumes that the comparison between Position2d objects is valid.
+        """
+        # Testcase 1 - 0-Direction
+        frame = Frame2d(np.zeros(2), Rotation2d(0), origin2d)
+        position = BoundPosition2d(np.random.random(2), frame)
+        direction = Direction2d(np.zeros(2), origin2d)
+
+        result = position.add_direction(direction)
+        expected = Position2d(position.coordinates, origin2d)
+
+        assert result == expected
+
+        # Testcase 2
+        frame = Frame2d(np.zeros(2), Rotation2d(0), origin2d)
+        position = BoundPosition2d(np.array([0, 1]), frame)
+        dir_frame = Frame2d(np.zeros(2), Rotation2d(math.pi / 2), origin2d)
+        direction = Direction2d(np.array([0, 1]), dir_frame)
+
+        result = position.add_direction(direction)
+        expected = Position2d(np.array([-1, 1]), origin2d)
+        expected_frame_pos = np.array([-1, 0], dtype=np.float64)
+
+        assert result == expected
+        assert np.allclose(result.reference.position, expected_frame_pos,
+                           rtol=RTOL)
+
+    def test_add_direction_inheritance(self):
+        """
+        Tests whether the returned objects from .add_direction method inherit
+        the reference and rtol from the calling object.
+        """
+        frame = random_frame2d()
+        position = BoundPosition2d(np.random.random(2), frame,
+                                   rtol=random.random())
+        direction = random_direction2d()
+
+        result = position.add_direction(direction)
+
+        assert np.allclose(position.coordinates, result.coordinates, rtol=RTOL)
+        assert result.rtol == position.rtol
+
+    def test_add_direction_random(self):
+        """
+        Tests the .add_direction method with random values.
+        """
+        for i in range(ITERS):
+            reference = random_frame2d()
+            copy_reference = copy.deepcopy(reference)
+            copy_reference._parent = origin2d
+            position = random_boundposition2d(reference=copy_reference)
+            direction = random_direction2d()
+
+            result = position.add_direction(direction)
+
+            transformed = direction.transform_to(reference)
+            expected_coordinates = position.coordinates + transformed
+            expected = Position2d(expected_coordinates, reference)
+
+            assert result == expected
+
+    def test_add_direction_reversible(self):
+        """
+        Tests whether adding the direction gained from .get_direction method
+        results in the other position coordinates. This test relies on the
+        validity of .get_direction.
+        """
+        for i in range(ITERS):
+            position_a = random_boundposition2d()
+            position_b = random_boundposition2d()
+
+            direction = position_a.get_direction(position_b)
+
+            assert position_a.add_direction(direction) == position_b
+
+    def test_add_direction_sanity_check(self):
+        """
+        Assures that the :meth:`gtFrame.position.BoundPosition2d` only alters
+        the reference position and does not alter the coordinates.
+        """
+        for i in range(ITERS):
+            position = random_boundposition2d()
+            coordinates = position.coordinates
+            direction = random_direction2d()
+
+            result = position.add_direction(direction)
+
+            assert np.allclose(position.coordinates, coordinates, rtol=RTOL)
+            assert result != position
+
+    def test_apply_direction(self):
+        """
+        Tests the .apply_direction method by comparing it to results from
+        the .add_direction method. This test therefore relies on the validity
+        of the .add_direction method.
+        """
+        for i in range(ITERS):
+            position = random_boundposition2d()
+            direction = random_direction2d()
+
+            expected = position.add_direction(direction)
+            position.apply_direction(direction)
+
+            assert position == expected
+
+
 class TestPosition2d:
     """
     Holds tests for Position2d.
     """
     def test_constructor_assign(self):
         """
         Tests whether the constructor correctly assigns the attributes.
@@ -359,14 +593,213 @@
 
         transformed = position.transform_to(foreign_frame)
         expected = foreign_frame.transform_from(frame, coordinates)
 
         assert np.allclose(transformed, expected, rtol=RTOL)
 
 
+class TestBoundPosition3d:
+    """
+    Holds tests for BoundPosition3d
+    """
+    def test_constructor_assign(self):
+        """
+        Tests whether the constructor correctly assigns the attributes.
+
+        :return: None
+        """
+        coordinates = np.random.random(3)
+        frame = random_frame3d()
+
+        position = BoundPosition3d(coordinates, frame)
+
+        assert np.allclose(position.coordinates, coordinates, rtol=RTOL)
+        assert position.reference == frame
+
+    def test_constructor_exception_coordinates(self):
+        """
+        Tests whether the constructor raises an error if the wrong dimension
+        vector is passed.
+
+        :return: None
+        """
+        coordinates = np.random.random(random.randint(3, 100))
+        frame = random_frame3d()
+
+        with pytest.raises(ValueError):
+            position = BoundPosition3d(coordinates, frame)       # noqa: F841
+
+    def test_construction_exception_reference(self):
+        """
+        Tests whether the constructor raises an error if a RootFrame2d is
+        passed as a reference.
+        """
+        coordinates = np.random.random(3)
+        frame = RootFrame3d()
+
+        with pytest.raises(TypeError):
+            BoundPosition3d(coordinates, frame)
+
+    def test_constructor_tolerances(self):
+        """
+        Test the assignment of the rtol attribute on init.
+        """
+        coordinates = np.random.random(3)
+        frame = random_frame3d()
+        rtol = random.random()
+
+        position_a = BoundPosition3d(coordinates, frame)
+        position_b = BoundPosition3d(coordinates, frame, rtol=rtol)
+
+        assert position_a.rtol == DEFAULT_RTOL
+        assert position_b.rtol == rtol
+
+    def test_eq(self):
+        """
+        Tests the == operator (i.e. the __eq__ method).
+
+        :return: None
+        """
+        coordinates = np.random.random(3)
+        frame_a = random_frame3d()
+        frame_b = random_frame3d()
+
+        position_a = BoundPosition3d(coordinates, frame_a)
+        position_b = BoundPosition3d(frame_b.transform_from(frame_a,
+                                                            coordinates),
+                                     frame_b)
+
+        assert position_a == position_b
+
+    def test_eq_agnostic(self):
+        """
+        Test the == operator with agnostic Position types. So compare Position
+        with BoundPosition.
+        """
+        coordinates = np.random.random(3)
+        frame_a = random_frame3d()
+        frame_b = random_frame3d()
+
+        position_a = Position3d(coordinates, frame_a)
+        position_b = BoundPosition3d(frame_b.transform_from(frame_a,
+                                                            coordinates),
+                                     frame_b)
+
+        assert position_a == position_b
+
+    def test_add_direction_static(self):
+        """
+        Tests the .add_direction method with static testcases. This test
+        assumes that the comparison between Position3d objects is valid.
+        """
+        # Testcase 1 - 0-Direction
+        frame = Frame3d(np.zeros(3), Rotation3d.from_rotvec([0, 0, 0]),
+                        parent_frame=origin3d)
+        position = BoundPosition3d(np.random.random(3), frame)
+        direction = Direction3d(np.zeros(3), origin3d)
+
+        result = position.add_direction(direction)
+        expected = Position3d(position.coordinates, origin3d)
+
+        assert result == expected
+
+        # Testcase 2
+        frame = Frame3d(np.zeros(3), Rotation3d.from_rotvec([0, 0, 0]),
+                        parent_frame=origin3d)
+        position = BoundPosition3d(np.array([0, 1, 0]), frame)
+        dir_frame = Frame3d(np.zeros(3),
+                            Rotation3d.from_rotvec(
+                                np.array([0, 0, math.pi / 2])),
+                            origin3d)
+        direction = Direction3d(np.array([0, 1, 0]), dir_frame)
+
+        result = position.add_direction(direction)
+        expected = Position3d(np.array([-1, 1, 0]), origin3d)
+
+        assert result == expected
+
+    def test_add_direction_inheritance(self):
+        """
+        Tests whether the returned objects from .add_direction method inherit
+        the reference and rtol from the calling object.
+        """
+        frame = random_frame3d()
+        position = BoundPosition3d(np.random.random(3), frame,
+                                   rtol=random.random())
+        direction = random_direction3d()
+
+        result = position.add_direction(direction)
+
+        assert np.allclose(position.coordinates, result.coordinates, rtol=RTOL)
+        assert result.rtol == position.rtol
+
+    def test_add_direction_random(self):
+        """
+        Tests the .add_direction method with random values.
+        """
+        for i in range(ITERS):
+            reference = random_frame3d()
+            copy_reference = copy.deepcopy(reference)
+            copy_reference._parent = origin3d
+            position = random_boundposition3d(reference=copy_reference)
+            direction = random_direction3d()
+
+            result = position.add_direction(direction)
+
+            transformed = direction.transform_to(reference)
+            expected_coordinates = position.coordinates + transformed
+            expected = Position3d(expected_coordinates, reference)
+
+            assert result == expected
+
+    def test_add_direction_reversible(self):
+        """
+        Tests whether adding the direction gained from .get_direction method
+        results in the other position coordinates. This test relies on the
+        validity of .get_direction.
+        """
+        for i in range(ITERS):
+            position_a = random_boundposition3d()
+            position_b = random_boundposition3d()
+
+            direction = position_a.get_direction(position_b)
+
+            assert position_a.add_direction(direction) == position_b
+
+    def test_add_direction_sanity_check(self):
+        """
+        Assures that the :meth:`gtFrame.position.BoundPosition2d` only alters
+        the reference position and does not alter the coordinates.
+        """
+        for i in range(ITERS):
+            position = random_boundposition3d()
+            coordinates = position.coordinates
+            direction = random_direction3d()
+
+            result = position.add_direction(direction)
+
+            assert np.allclose(position.coordinates, coordinates, rtol=RTOL)
+            assert result != position
+
+    def test_apply_direction(self):
+        """
+        Tests the .apply_direction method by comparing it to results from
+        the .add_direction method. This test therefore relies on the validity
+        of the .add_direction method.
+        """
+        for i in range(ITERS):
+            position = random_boundposition3d()
+            direction = random_direction3d()
+
+            expected = position.add_direction(direction)
+            position.apply_direction(direction)
+
+            assert position == expected
+
+
 class TestPosition3d:
     """
     Holds tests for Position3d.
     """
     def test_constructor_assign(self):
         """
         Tests whether the constructor correctly assigns the attributes.
```

### Comparing `gtFrame-1.2.1/tests/test_rotation.py` & `gtFrame-1.2.2/tests/test_rotation.py`

 * *Files identical despite different names*

