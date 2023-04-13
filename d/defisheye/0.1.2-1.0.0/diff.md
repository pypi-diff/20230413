# Comparing `tmp/defisheye-0.1.2.tar.gz` & `tmp/defisheye-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defisheye-0.1.2.tar", last modified: Thu Apr 13 12:46:03 2023, max compression
+gzip compressed data, was "dist/defisheye-1.0.0.tar", last modified: Wed Oct 28 19:32:13 2020, max compression
```

## Comparing `defisheye-0.1.2.tar` & `defisheye-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-13 12:46:03.053816 defisheye-0.1.2/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5067 2023-04-13 12:46:03.053816 defisheye-0.1.2/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4774 2023-04-13 12:43:38.000000 defisheye-0.1.2/README.md
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2023-04-13 12:46:03.053816 defisheye-0.1.2/setup.cfg
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      705 2023-04-13 12:44:58.000000 defisheye-0.1.2/setup.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-13 12:46:03.053816 defisheye-0.1.2/src/
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-13 12:46:03.053816 defisheye-0.1.2/src/defisheye/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      750 2023-04-13 12:40:23.000000 defisheye-0.1.2/src/defisheye/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5201 2023-04-13 12:41:03.000000 defisheye-0.1.2/src/defisheye/defisheye.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-13 12:46:03.053816 defisheye-0.1.2/src/defisheye.egg-info/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5067 2023-04-13 12:46:03.000000 defisheye-0.1.2/src/defisheye.egg-info/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      255 2023-04-13 12:46:03.000000 defisheye-0.1.2/src/defisheye.egg-info/SOURCES.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2023-04-13 12:46:03.000000 defisheye-0.1.2/src/defisheye.egg-info/dependency_links.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       20 2023-04-13 12:46:03.000000 defisheye-0.1.2/src/defisheye.egg-info/requires.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       10 2023-04-13 12:46:03.000000 defisheye-0.1.2/src/defisheye.egg-info/top_level.txt
+drwxrwxrwx   0 eduardo   (1000) eduardo   (1000)        0 2020-10-28 19:32:13.977264 defisheye-1.0.0/
+-rwxrwxrwx   0 eduardo   (1000) eduardo   (1000)     6191 2020-10-28 19:32:13.976723 defisheye-1.0.0/PKG-INFO
+-rwxrwxrwx   0 eduardo   (1000) eduardo   (1000)     4671 2020-03-23 14:25:09.000000 defisheye-1.0.0/README.md
+-rwxrwxrwx   0 eduardo   (1000) eduardo   (1000)       38 2020-10-28 19:32:13.977362 defisheye-1.0.0/setup.cfg
+-rwxrwxrwx   0 eduardo   (1000) eduardo   (1000)      705 2020-10-28 19:28:17.000000 defisheye-1.0.0/setup.py
+drwxrwxrwx   0 eduardo   (1000) eduardo   (1000)        0 2020-10-28 19:32:13.946562 defisheye-1.0.0/src/
+drwxrwxrwx   0 eduardo   (1000) eduardo   (1000)        0 2020-10-28 19:32:13.954196 defisheye-1.0.0/src/defisheye/
+-rwxrwxrwx   0 eduardo   (1000) eduardo   (1000)      750 2020-03-23 14:25:10.000000 defisheye-1.0.0/src/defisheye/__init__.py
+-rwxrwxrwx   0 eduardo   (1000) eduardo   (1000)     5610 2020-09-11 22:06:18.000000 defisheye-1.0.0/src/defisheye/defisheye.py
+drwxrwxrwx   0 eduardo   (1000) eduardo   (1000)        0 2020-10-28 19:32:13.975711 defisheye-1.0.0/src/defisheye.egg-info/
+-rwxrwxrwx   0 eduardo   (1000) eduardo   (1000)     6191 2020-10-28 19:32:13.000000 defisheye-1.0.0/src/defisheye.egg-info/PKG-INFO
+-rwxrwxrwx   0 eduardo   (1000) eduardo   (1000)      255 2020-10-28 19:32:13.000000 defisheye-1.0.0/src/defisheye.egg-info/SOURCES.txt
+-rwxrwxrwx   0 eduardo   (1000) eduardo   (1000)        1 2020-10-28 19:32:13.000000 defisheye-1.0.0/src/defisheye.egg-info/dependency_links.txt
+-rwxrwxrwx   0 eduardo   (1000) eduardo   (1000)       20 2020-10-28 19:32:13.000000 defisheye-1.0.0/src/defisheye.egg-info/requires.txt
+-rwxrwxrwx   0 eduardo   (1000) eduardo   (1000)       10 2020-10-28 19:32:13.000000 defisheye-1.0.0/src/defisheye.egg-info/top_level.txt
```

### Comparing `defisheye-0.1.2/PKG-INFO` & `defisheye-1.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: defisheye
-Version: 0.1.2
-Summary: Fast defisheye algorithm
-Home-page: https://github.com/duducosmos/defisheye
-Author: Eduardo S. Pereira
-Author-email: pereira.somoza@gmail.com
-License: Apache License 2.0
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # Defisheye
 
 Fast Corrects for fisheye distortion in an image.
 
 Defisheye is designed to transform a fisheye image into a normal perspective
 view looking towards the center of the fisheye image.
 
@@ -38,25 +27,17 @@
 fov = 180
 pfov = 120
 
 img = "./images/example3.jpg"
 img_out = f"./images/out/example3_{dtype}_{format}_{pfov}_{fov}.jpg"
 
 obj = Defisheye(img, dtype=dtype, format=format, fov=fov, pfov=pfov)
-
-# To save image locally 
-obj.convert(outfile=img_out)
-
-# To use the converted image in memory
-
-new_image = obj.convert()
+obj.convert(img_out)
 ```
 
-
-
 ## Constructor atributes:
 ### fov
 fisheye field of view (aperture) in degrees.
 
 
 IFOV is the input fisheye image field of view in degrees. A value of 180
 will correspond to a hemispherical fisheye image within the circular area.
@@ -165,9 +146,7 @@
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
-
-
```

### Comparing `defisheye-0.1.2/setup.py` & `defisheye-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 def read(filename):
     return open(os.path.join(os.path.dirname(__file__), filename)).read()
 
 setup(
     name="defisheye",
     license="Apache License 2.0",
-    version='0.1.2',
+    version='1.0.0',
     author='Eduardo S. Pereira',
     author_email='pereira.somoza@gmail.com',
     packages=find_packages("src"),
     package_dir={"":"src"},
     description="Fast defisheye algorithm",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
```

### Comparing `defisheye-0.1.2/src/defisheye/__init__.py` & `defisheye-1.0.0/src/defisheye/__init__.py`

 * *Files identical despite different names*

### Comparing `defisheye-0.1.2/src/defisheye/defisheye.py` & `defisheye-1.0.0/src/defisheye/defisheye.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,18 @@
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 """
 import cv2
 from numpy import arange, sqrt, arctan, sin, tan, zeros, array, meshgrid, pi
-from numpy import argwhere, hypot
+from numpy import argwhere, hypot, zeros_like, uint8, ndarray
+
+from numpy import hstack
+import matplotlib.pyplot as plt
 
 
 class Defisheye:
     """
     Defisheye
 
     fov: fisheye field of view (aperture) in degrees
@@ -55,21 +58,20 @@
         self._start_att(vkwargs, kwargs)
 
         if type(infile) == str:
             _image = cv2.imread(infile)
         elif type(infile) == ndarray:
             _image = infile
         else:
-            raise ImageError("Image format not recognized")
-
+            raise NameError("Image format not recognized")
 
         width = _image.shape[1]
         height = _image.shape[0]
         xcenter = width // 2
-        ycenter = height  // 2
+        ycenter = height // 2
 
         dim = min(width, height)
         x0 = xcenter - dim // 2
         xf = xcenter + dim // 2
         y0 = ycenter - dim // 2
         yf = ycenter + dim // 2
 
@@ -111,25 +113,27 @@
             ifoc = dim / (2.0 * tan(self._fov * pi / 720))
             rr = ifoc * tan(phiang / 2)
 
         rdmask = rd != 0
         xs = xd.copy()
         ys = yd.copy()
 
-        xs[rdmask] = (rr[rdmask] / rd[rdmask]) * xd[rdmask] + self._xcenter
-        ys[rdmask] = (rr[rdmask] / rd[rdmask]) * yd[rdmask] + self._ycenter
+        tmp = rr[rdmask] / rd[rdmask]
+
+        xs[rdmask] = tmp * xd[rdmask] + self._xcenter
+        ys[rdmask] = tmp * yd[rdmask] + self._ycenter
 
         xs[~rdmask] = 0
         ys[~rdmask] = 0
 
         xs = xs.astype(int)
         ys = ys.astype(int)
         return xs, ys
 
-    def convert(self, outfile=None):
+    def convert(self, outfile, circle=False):
         if self._format == "circular":
             dim = min(self._width, self._height)
         elif self._format == "fullframe":
             dim = sqrt(self._width ** 2.0 + self._height ** 2.0)
 
         if self._radius is not None:
             dim = 2 * self._radius
@@ -147,16 +151,25 @@
         j = arange(self._height)
         i, j = meshgrid(i, j)
 
         xs, ys, = self._map(i, j, ofocinv, dim)
         img = self._image.copy()
 
         img[i, j, :] = self._image[xs, ys, :]
-        if outfile is not None:
-            cv2.imwrite(outfile, img)
+
+        if circle is True:
+            center = (self._width // 2, self._height // 2)
+            radius = min(self._width // 2, self._height // 2)
+            color = (255, 255, 255)
+            thickness = -1
+            alpha = cv2.circle(zeros_like(img),
+                               center, radius, color, thickness)
+            img[alpha == 0] = 0
+
+        cv2.imwrite(outfile, img)
         return img
 
     def _start_att(self, vkwargs, kwargs):
         """
         Starting atributes
         """
         pin = []
```

