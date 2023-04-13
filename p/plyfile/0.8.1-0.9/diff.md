# Comparing `tmp/plyfile-0.8.1.tar.gz` & `tmp/plyfile-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plyfile-0.8.1.tar", last modified: Sun Mar 19 06:26:00 2023, max compression
+gzip compressed data, was "plyfile-0.9.tar", last modified: Thu Apr 13 06:51:39 2023, max compression
```

## Comparing `plyfile-0.8.1.tar` & `plyfile-0.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35147 2019-08-03 21:55:54.506719 plyfile-0.8.1/COPYING
--rw-r--r--   0        0        0    20282 2023-03-19 06:23:29.481207 plyfile-0.8.1/README.md
--rw-r--r--   0        0        0    31054 2023-03-17 16:03:59.737669 plyfile-0.8.1/plyfile.py
--rw-r--r--   0        0        0      936 2023-03-19 06:23:35.733136 plyfile-0.8.1/pyproject.toml
--rw-r--r--   0        0        0    21035 1970-01-01 00:00:00.000000 plyfile-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    35147 2019-08-03 21:55:54.506719 plyfile-0.9/COPYING
+-rw-r--r--   0        0        0    20787 2023-04-13 05:53:27.177994 plyfile-0.9/README.md
+-rw-r--r--   0        0        0    42475 2023-04-13 06:18:18.158979 plyfile-0.9/plyfile.py
+-rw-r--r--   0        0        0      934 2023-04-13 06:47:02.102832 plyfile-0.9/pyproject.toml
+-rw-r--r--   0        0        0    21538 1970-01-01 00:00:00.000000 plyfile-0.9/PKG-INFO
```

### Comparing `plyfile-0.8.1/COPYING` & `plyfile-0.9/COPYING`

 * *Files identical despite different names*

### Comparing `plyfile-0.8.1/README.md` & `plyfile-0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: plyfile
+Version: 0.9
+Summary: PLY file reader/writer
+Keywords: ply,numpy
+Author-email: Darsh Ranjan <dranjan@berkeley.edu>
+Requires-Python: >=3.7
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering
+Project-URL: Homepage, https://github.com/dranjan/python-plyfile
+Description-Content-Type: text/markdown
+
 ![Build Status](https://github.com/dranjan/python-plyfile/actions/workflows/python-package.yml/badge.svg)
 
 Welcome to the `plyfile` Python module, which provides a simple facility
 for reading and writing ASCII and binary PLY files.
 
 The PLY format is documented
 [elsewhere](https://web.archive.org/web/20161221115231/http://www.cs.virginia.edu/~gfx/Courses/2001/Advanced.spring.01/plylib/Ply.txt).
@@ -44,15 +63,17 @@
 
 # Usage
 
 Both deserialization and serialization of PLY file data is done through
 `PlyData` and `PlyElement` instances.
 
 ```Python Console
+>>> import numpy
 >>> from plyfile import PlyData, PlyElement
+>>>
 ```
 
 For the code examples that follow, assume the file `tet.ply` contains
 the following text:
 
     ply
     format ascii 1.0
@@ -79,21 +100,23 @@
 
 (This file is available under the `examples` directory.)
 
 ## Reading a PLY file
 
 ```Python Console
 >>> plydata = PlyData.read('tet.ply')
+>>>
 ```
 
 or
 
 ```Python Console
 >>> with open('tet.ply', 'rb') as f:
 ...     plydata = PlyData.read(f)
+>>>
 ```
 
 The static method `PlyData.read` returns a `PlyData` instance, which is
 `plyfile`'s representation of the data in a PLY file.  A `PlyData`
 instance has an attribute `elements`, which is a list of `PlyElement`
 instances, each of which has a `data` attribute which is a `numpy`
 structured array containing the numerical data.  PLY file elements map
@@ -104,59 +127,63 @@
 
 Concretely:
 
 ```Python Console
 >>> plydata.elements[0].name
 'vertex'
 >>> plydata.elements[0].data[0]
-(0.0, 0.0, 0.0)
+(0., 0., 0.)
 >>> plydata.elements[0].data['x']
-array([ 0.,  0.,  1.,  1.], dtype=float32)
+array([0., 0., 1., 1.], dtype=float32)
 >>> plydata['face'].data['vertex_indices'][0]
 array([0, 1, 2], dtype=int32)
+>>>
 ```
 
 For convenience, elements and properties can be looked up by name:
 
 ```Python Console
 >>> plydata['vertex']['x']
-array([ 0.,  0.,  1.,  1.], dtype=float32)
+array([0., 0., 1., 1.], dtype=float32)
+>>>
 ```
 
 and elements can be indexed directly without explicitly going through
 the `data` attribute:
 
 ```Python Console
 >>> plydata['vertex'][0]
-(0.0, 0.0, 0.0)
+(0., 0., 0.)
+>>>
 ```
 
 The above expression is equivalent to `plydata['vertex'].data[0]`.
 
 `PlyElement` instances also contain metadata:
 
 ```Python Console
 >>> plydata.elements[0].properties
-(PlyProperty('x', 'float'), PlyProperty('y', 'float'),
- PlyProperty('z', 'float'))
+(PlyProperty('x', 'float'), PlyProperty('y', 'float'), PlyProperty('z', 'float'))
 >>> plydata.elements[0].count
 4
+>>>
 ```
 
 `PlyProperty` and `PlyListProperty` instances are used internally as a
 convenient intermediate representation of PLY element properties that
 can easily be serialized to a PLY header (using `str`) or converted to
 `numpy`-compatible type descriptions (via the `dtype` method).  It's not
 extremely common to manipulate them directly, but if needed, the
 property metadata of an element can be accessed as a tuple via the
 `properties` attribute (as illustrated above) or looked up by name:
 
 ```Python Console
 >>> plydata.elements[0].ply_property('x')
 PlyProperty('x', 'float')
+>>>
 ```
 
 Many (but not necessarily all) types of malformed input files will raise
 `PlyParseError` when `PlyData.read` is called.  The string value of the
 `PlyParseError` instance (as well as attributes `element`, `row`, and
 `prop`) provides additional context for the error if applicable.
 
@@ -176,34 +203,36 @@
 
 ```Python Console
 >>> plydata.text = False
 >>> plydata.byte_order = '<'
 >>> plydata.write('tet_binary.ply')
 >>>
 >>> # `mmap=True` is the default:
->>> plydata = PlyData.read('tet_binary_ply')
+>>> plydata = PlyData.read('tet_binary.ply')
 >>> isinstance(plydata['vertex'].data, numpy.memmap)
 True
->>> plydata = PlyData.read('tet_binary_ply', mmap=False)
+>>> plydata = PlyData.read('tet_binary.ply', mmap=False)
 >>> isinstance(plydata['vertex'].data, numpy.memmap)
 False
+>>>
 ```
 
 #### Case 2: elements with list properties
 
 In the general case, elements with list properties cannot be
 memory-mapped as `numpy` arrays, except in one important case: when
 all list properties have fixed and known lengths. In that case, the
 `known_list_len` argument can be given to `PlyData.read`:
 
 ```Python Console
 >>> plydata = PlyData.read('tet_binary.ply',
 ...                        known_list_len={'face': {'vertex_indices': 3}})
 >>> isinstance(plydata['face'].data, numpy.memmap)
 True
+>>>
 ```
 
 The implementation will validate the data: if any instance of the list
 property has a length other than the value specified, then
 `PlyParseError` will be raised.
 
 Note that in order to enable memory mapping for a given element,
@@ -250,84 +279,91 @@
 >>> face = numpy.array([([0, 1, 2], 255, 255, 255),
 ...                     ([0, 2, 3], 255,   0,   0),
 ...                     ([0, 1, 3],   0, 255,   0),
 ...                     ([1, 2, 3],   0,   0, 255)],
 ...                    dtype=[('vertex_indices', 'i4', (3,)),
 ...                           ('red', 'u1'), ('green', 'u1'),
 ...                           ('blue', 'u1')])
+>>>
 ```
 
 Once you have suitably structured array, the static method
 `PlyElement.describe` can then be used to create the necessary
 `PlyElement` instances:
 
 ```Python Console
->>> el = PlyElement.describe(some_array, 'some_name')
+>>> el = PlyElement.describe(vertex, 'vertex')
+>>>
 ```
 
 or
 
 ```Python Console
->>> el = PlyElement.describe(some_array, 'some_name',
+>>> el = PlyElement.describe(vertex, 'vertex',
 ...                          comments=['comment1',
 ...                                    'comment2'])
+>>>
 ```
 
 Note that there's no need to create `PlyProperty` instances explicitly.
 This is all done behind the scenes by examining `some_array.dtype.descr`.
 One slight hiccup here is that variable-length fields in a `numpy` array
 (i.e., our representation of PLY list properties)
 must have a type of `object`, so the types of the list length and values
 in the serialized PLY file can't be obtained from the array's `dtype`
 attribute alone.  For simplicity and predictability, the length
 defaults to 8-bit unsigned integer, and the value defaults to 32-bit
 signed integer, which covers the majority of use cases.  Exceptions must
 be stated explicitly:
 
 ```Python Console
->>> el = PlyElement.describe(some_array, 'some_name',
-...                          val_dtypes={'some_property': 'f8'},
-...                          len_dtypes={'some_property': 'u4'})
+>>> el = PlyElement.describe(face, 'face',
+...                          val_types={'vertex_indices': 'u2'},
+...                          len_types={'vertex_indices': 'u4'})
+>>>
 ```
 
 Now you can instantiate `PlyData` and serialize:
 
 ```Python Console
 >>> PlyData([el]).write('some_binary.ply')
 >>> PlyData([el], text=True).write('some_ascii.ply')
 >>>
 >>> # Force the byte order of the output to big-endian, independently of
 >>> # the machine's native byte order
 >>> PlyData([el],
 ...         byte_order='>').write('some_big_endian_binary.ply')
 >>>
->>> # Use a file object.  Binary mode is used here, which will cause
+>>> # Use a file object. Binary mode is used here, which will cause
 >>> # Unix-style line endings to be written on all systems.
 >>> with open('some_ascii.ply', mode='wb') as f:
 ...     PlyData([el], text=True).write(f)
+>>>
 ```
 
 ## Miscellaneous
 
 ### Comments
 
 Header comments are supported:
 
 ```Python Console
 >>> ply = PlyData([el], comments=['header comment'])
 >>> ply.comments
 ['header comment']
+>>>
 ```
 
 As of version 0.3, "obj_info" comments are supported as well:
 
 ```Python Console
 >>> ply = PlyData([el], obj_info=['obj_info1', 'obj_info2'])
 >>> ply.obj_info
 ['obj_info1', 'obj_info2']
+>>>
 ```
 
 When written, they will be placed after regular comments after the
 "format" line.
 
 Comments can have leading whitespace, but trailing whitespace may be
 stripped and should not be relied upon.  Comments may not contain
@@ -344,14 +380,15 @@
 pretty easy way to obtain a two dimensional array, assuming we know the
 row length in advance:
 
 ```Python Console
 >>> plydata = PlyData.read('tet.ply')
 >>> tri_data = plydata['face'].data['vertex_indices']
 >>> triangles = numpy.vstack(tri_data)
+>>>
 ```
 
 ### Instance mutability
 
 A plausible code pattern is to read a PLY file into a `PlyData`
 instance, perform some operations on it, possibly modifying data and
 metadata in place, and write the result to a new file.  This pattern is
@@ -397,14 +434,15 @@
 >>> face = plydata['face']
 >>> face.properties = ()
 >>> face.data.dtype.names = ['idx', 'r', 'g', 'b']
 >>> face.properties = (PlyListProperty('idx', 'uchar', 'int'),
 ...                    PlyProperty('r', 'uchar'),
 ...                    PlyProperty('g', 'uchar'),
 ...                    PlyProperty('b', 'uchar'))
+>>>
 ```
 
 Note that it is always safe to create a new `PlyElement` or `PlyData`
 instance instead of modifying one in place, and this is the recommended
 style:
 
 ```Python Console
@@ -414,70 +452,79 @@
 >>>
 >>> # Also supported:
 >>> plydata.elements = [plydata['face'], plydata['vertex']]
 >>> plydata.text = False
 >>> plydata.byte_order = '<'
 >>> plydata.comments = []
 >>> plydata.obj_info = []
+>>>
 ```
 
 Objects created by this library don't claim ownership of the other
 objects they refer to, which has implications for both styles (creating
 new instances and modifying in place).  For example, a single
 `PlyElement` instance can be contained by multiple `PlyData` instances,
 but modifying that instance will then affect all of those containing
 `PlyData` instances.
 
+### Text-mode streams
+
+Input and output on text-mode streams is supported for ASCII-format
+PLY files, but not binary-format PLY files. Input and output on
+binary streams is supported for all valid PLY files. Note that
+`sys.stdout` and `sys.stdin` are text streams, so they can only be
+used directly for ASCII-format PLY files.
+
 # FAQ
 
 ## How do I initialize a list property from two-dimensional array?
 
 ```Python Console
 >>> # Here's a two-dimensional array containing vertex indices.
 >>> face_data = numpy.array([[0, 1, 2], [3, 4, 5]], dtype='i4')
 >>>
 >>> # PlyElement.describe requires a one-dimensional structured array.
->>> ply_faces = numpy.empty(len(faces),
+>>> ply_faces = numpy.empty(len(face_data),
 ...                         dtype=[('vertex_indices', 'i4', (3,))])
 >>> ply_faces['vertex_indices'] = face_data
 >>> face = PlyElement.describe(ply_faces, 'face')
+>>>
 ```
 
 ## Can I save a PLY file directly to `sys.stdout`?
 
-On Python 3, you will probably run into issues because `sys.stdout` is a
-text-mode stream and `plyfile` outputs binary data, even for
-ASCII-format PLY files:
-
-```Python Console
->>> import sys
->>> plydata.write(sys.stdout)
-Traceback (most recent call last):
-  File "<stdin>", line 1, in <module>
-    File ".../python-plyfile/plyfile.py", line 411, in write
-        stream.write(self.header.encode('ascii'))
-        TypeError: write() argument must be str, not bytes
-```
+Yes, for an ASCII-format PLY file. For binary-format files, it won't
+work directly, since `sys.stdout` is a text-mode stream and binary-format
+files can only be output to binary streams. (ASCII-format files can be
+output to text or binary streams.)
 
 There are a few ways around this.
 - Write to a named file instead. On Linux and some other Unix-likes, you
   can access `stdout` via the named file `/dev/stdout`:
 
     ```Python Console
-    >>> plydata.write('/dev/stdout')
+    >>> plydata.write('/dev/stdout')  # doctest: +SKIP
     ```
 
 - Use `sys.stdout.buffer`:
 
     ```Python Console
-    >>> plydata.write(sys.stdout.buffer)
+    >>> plydata.write(sys.stdout.buffer)  # doctest: +SKIP
     ```
 
   (source: https://bugs.python.org/issue4571)
 
+## Can I read a PLY file from `sys.stdin`?
+
+The answer is exactly analogous to the situation with writing to
+`sys.stdout`: it works for ASCII-format PLY files but not binary-format
+files. The two workarounds given above also apply: use a named file like
+`/dev/stdin`, or use `sys.stdin.buffer`.
+
+
 # Design philosophy and rationale
 
 The design philosophy of `plyfile` can be summed up as follows.
 - Be familiar to users of `numpy` and reuse existing idioms and concepts
   when possible.
 - Favor simplicity over power or user-friendliness.
 - Support all valid PLY files.
@@ -565,7 +612,8 @@
 
 # License
 
 Copyright Darsh Ranjan.
 
 This software is released under the terms of the GNU General Public
 License, version 3.  See the file `COPYING` for details.
+
```

### Comparing `plyfile-0.8.1/pyproject.toml` & `plyfile-0.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm]
 
 [project]
 name = "plyfile"
-version = "0.8.1"
+version = "0.9"
 description = "PLY file reader/writer"
 authors = [
     { name = "Darsh Ranjan", email = "dranjan@berkeley.edu" },
 ]
 dependencies = [
     "numpy>=1.17",
 ]
```

### Comparing `plyfile-0.8.1/PKG-INFO` & `plyfile-0.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: plyfile
-Version: 0.8.1
-Summary: PLY file reader/writer
-Keywords: ply,numpy
-Author-email: Darsh Ranjan <dranjan@berkeley.edu>
-Requires-Python: >=3.7
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering
-Project-URL: Homepage, https://github.com/dranjan/python-plyfile
-Description-Content-Type: text/markdown
-
 ![Build Status](https://github.com/dranjan/python-plyfile/actions/workflows/python-package.yml/badge.svg)
 
 Welcome to the `plyfile` Python module, which provides a simple facility
 for reading and writing ASCII and binary PLY files.
 
 The PLY format is documented
 [elsewhere](https://web.archive.org/web/20161221115231/http://www.cs.virginia.edu/~gfx/Courses/2001/Advanced.spring.01/plylib/Ply.txt).
@@ -63,15 +44,17 @@
 
 # Usage
 
 Both deserialization and serialization of PLY file data is done through
 `PlyData` and `PlyElement` instances.
 
 ```Python Console
+>>> import numpy
 >>> from plyfile import PlyData, PlyElement
+>>>
 ```
 
 For the code examples that follow, assume the file `tet.ply` contains
 the following text:
 
     ply
     format ascii 1.0
@@ -98,21 +81,23 @@
 
 (This file is available under the `examples` directory.)
 
 ## Reading a PLY file
 
 ```Python Console
 >>> plydata = PlyData.read('tet.ply')
+>>>
 ```
 
 or
 
 ```Python Console
 >>> with open('tet.ply', 'rb') as f:
 ...     plydata = PlyData.read(f)
+>>>
 ```
 
 The static method `PlyData.read` returns a `PlyData` instance, which is
 `plyfile`'s representation of the data in a PLY file.  A `PlyData`
 instance has an attribute `elements`, which is a list of `PlyElement`
 instances, each of which has a `data` attribute which is a `numpy`
 structured array containing the numerical data.  PLY file elements map
@@ -123,59 +108,63 @@
 
 Concretely:
 
 ```Python Console
 >>> plydata.elements[0].name
 'vertex'
 >>> plydata.elements[0].data[0]
-(0.0, 0.0, 0.0)
+(0., 0., 0.)
 >>> plydata.elements[0].data['x']
-array([ 0.,  0.,  1.,  1.], dtype=float32)
+array([0., 0., 1., 1.], dtype=float32)
 >>> plydata['face'].data['vertex_indices'][0]
 array([0, 1, 2], dtype=int32)
+>>>
 ```
 
 For convenience, elements and properties can be looked up by name:
 
 ```Python Console
 >>> plydata['vertex']['x']
-array([ 0.,  0.,  1.,  1.], dtype=float32)
+array([0., 0., 1., 1.], dtype=float32)
+>>>
 ```
 
 and elements can be indexed directly without explicitly going through
 the `data` attribute:
 
 ```Python Console
 >>> plydata['vertex'][0]
-(0.0, 0.0, 0.0)
+(0., 0., 0.)
+>>>
 ```
 
 The above expression is equivalent to `plydata['vertex'].data[0]`.
 
 `PlyElement` instances also contain metadata:
 
 ```Python Console
 >>> plydata.elements[0].properties
-(PlyProperty('x', 'float'), PlyProperty('y', 'float'),
- PlyProperty('z', 'float'))
+(PlyProperty('x', 'float'), PlyProperty('y', 'float'), PlyProperty('z', 'float'))
 >>> plydata.elements[0].count
 4
+>>>
 ```
 
 `PlyProperty` and `PlyListProperty` instances are used internally as a
 convenient intermediate representation of PLY element properties that
 can easily be serialized to a PLY header (using `str`) or converted to
 `numpy`-compatible type descriptions (via the `dtype` method).  It's not
 extremely common to manipulate them directly, but if needed, the
 property metadata of an element can be accessed as a tuple via the
 `properties` attribute (as illustrated above) or looked up by name:
 
 ```Python Console
 >>> plydata.elements[0].ply_property('x')
 PlyProperty('x', 'float')
+>>>
 ```
 
 Many (but not necessarily all) types of malformed input files will raise
 `PlyParseError` when `PlyData.read` is called.  The string value of the
 `PlyParseError` instance (as well as attributes `element`, `row`, and
 `prop`) provides additional context for the error if applicable.
 
@@ -195,34 +184,36 @@
 
 ```Python Console
 >>> plydata.text = False
 >>> plydata.byte_order = '<'
 >>> plydata.write('tet_binary.ply')
 >>>
 >>> # `mmap=True` is the default:
->>> plydata = PlyData.read('tet_binary_ply')
+>>> plydata = PlyData.read('tet_binary.ply')
 >>> isinstance(plydata['vertex'].data, numpy.memmap)
 True
->>> plydata = PlyData.read('tet_binary_ply', mmap=False)
+>>> plydata = PlyData.read('tet_binary.ply', mmap=False)
 >>> isinstance(plydata['vertex'].data, numpy.memmap)
 False
+>>>
 ```
 
 #### Case 2: elements with list properties
 
 In the general case, elements with list properties cannot be
 memory-mapped as `numpy` arrays, except in one important case: when
 all list properties have fixed and known lengths. In that case, the
 `known_list_len` argument can be given to `PlyData.read`:
 
 ```Python Console
 >>> plydata = PlyData.read('tet_binary.ply',
 ...                        known_list_len={'face': {'vertex_indices': 3}})
 >>> isinstance(plydata['face'].data, numpy.memmap)
 True
+>>>
 ```
 
 The implementation will validate the data: if any instance of the list
 property has a length other than the value specified, then
 `PlyParseError` will be raised.
 
 Note that in order to enable memory mapping for a given element,
@@ -269,84 +260,91 @@
 >>> face = numpy.array([([0, 1, 2], 255, 255, 255),
 ...                     ([0, 2, 3], 255,   0,   0),
 ...                     ([0, 1, 3],   0, 255,   0),
 ...                     ([1, 2, 3],   0,   0, 255)],
 ...                    dtype=[('vertex_indices', 'i4', (3,)),
 ...                           ('red', 'u1'), ('green', 'u1'),
 ...                           ('blue', 'u1')])
+>>>
 ```
 
 Once you have suitably structured array, the static method
 `PlyElement.describe` can then be used to create the necessary
 `PlyElement` instances:
 
 ```Python Console
->>> el = PlyElement.describe(some_array, 'some_name')
+>>> el = PlyElement.describe(vertex, 'vertex')
+>>>
 ```
 
 or
 
 ```Python Console
->>> el = PlyElement.describe(some_array, 'some_name',
+>>> el = PlyElement.describe(vertex, 'vertex',
 ...                          comments=['comment1',
 ...                                    'comment2'])
+>>>
 ```
 
 Note that there's no need to create `PlyProperty` instances explicitly.
 This is all done behind the scenes by examining `some_array.dtype.descr`.
 One slight hiccup here is that variable-length fields in a `numpy` array
 (i.e., our representation of PLY list properties)
 must have a type of `object`, so the types of the list length and values
 in the serialized PLY file can't be obtained from the array's `dtype`
 attribute alone.  For simplicity and predictability, the length
 defaults to 8-bit unsigned integer, and the value defaults to 32-bit
 signed integer, which covers the majority of use cases.  Exceptions must
 be stated explicitly:
 
 ```Python Console
->>> el = PlyElement.describe(some_array, 'some_name',
-...                          val_dtypes={'some_property': 'f8'},
-...                          len_dtypes={'some_property': 'u4'})
+>>> el = PlyElement.describe(face, 'face',
+...                          val_types={'vertex_indices': 'u2'},
+...                          len_types={'vertex_indices': 'u4'})
+>>>
 ```
 
 Now you can instantiate `PlyData` and serialize:
 
 ```Python Console
 >>> PlyData([el]).write('some_binary.ply')
 >>> PlyData([el], text=True).write('some_ascii.ply')
 >>>
 >>> # Force the byte order of the output to big-endian, independently of
 >>> # the machine's native byte order
 >>> PlyData([el],
 ...         byte_order='>').write('some_big_endian_binary.ply')
 >>>
->>> # Use a file object.  Binary mode is used here, which will cause
+>>> # Use a file object. Binary mode is used here, which will cause
 >>> # Unix-style line endings to be written on all systems.
 >>> with open('some_ascii.ply', mode='wb') as f:
 ...     PlyData([el], text=True).write(f)
+>>>
 ```
 
 ## Miscellaneous
 
 ### Comments
 
 Header comments are supported:
 
 ```Python Console
 >>> ply = PlyData([el], comments=['header comment'])
 >>> ply.comments
 ['header comment']
+>>>
 ```
 
 As of version 0.3, "obj_info" comments are supported as well:
 
 ```Python Console
 >>> ply = PlyData([el], obj_info=['obj_info1', 'obj_info2'])
 >>> ply.obj_info
 ['obj_info1', 'obj_info2']
+>>>
 ```
 
 When written, they will be placed after regular comments after the
 "format" line.
 
 Comments can have leading whitespace, but trailing whitespace may be
 stripped and should not be relied upon.  Comments may not contain
@@ -363,14 +361,15 @@
 pretty easy way to obtain a two dimensional array, assuming we know the
 row length in advance:
 
 ```Python Console
 >>> plydata = PlyData.read('tet.ply')
 >>> tri_data = plydata['face'].data['vertex_indices']
 >>> triangles = numpy.vstack(tri_data)
+>>>
 ```
 
 ### Instance mutability
 
 A plausible code pattern is to read a PLY file into a `PlyData`
 instance, perform some operations on it, possibly modifying data and
 metadata in place, and write the result to a new file.  This pattern is
@@ -416,14 +415,15 @@
 >>> face = plydata['face']
 >>> face.properties = ()
 >>> face.data.dtype.names = ['idx', 'r', 'g', 'b']
 >>> face.properties = (PlyListProperty('idx', 'uchar', 'int'),
 ...                    PlyProperty('r', 'uchar'),
 ...                    PlyProperty('g', 'uchar'),
 ...                    PlyProperty('b', 'uchar'))
+>>>
 ```
 
 Note that it is always safe to create a new `PlyElement` or `PlyData`
 instance instead of modifying one in place, and this is the recommended
 style:
 
 ```Python Console
@@ -433,70 +433,79 @@
 >>>
 >>> # Also supported:
 >>> plydata.elements = [plydata['face'], plydata['vertex']]
 >>> plydata.text = False
 >>> plydata.byte_order = '<'
 >>> plydata.comments = []
 >>> plydata.obj_info = []
+>>>
 ```
 
 Objects created by this library don't claim ownership of the other
 objects they refer to, which has implications for both styles (creating
 new instances and modifying in place).  For example, a single
 `PlyElement` instance can be contained by multiple `PlyData` instances,
 but modifying that instance will then affect all of those containing
 `PlyData` instances.
 
+### Text-mode streams
+
+Input and output on text-mode streams is supported for ASCII-format
+PLY files, but not binary-format PLY files. Input and output on
+binary streams is supported for all valid PLY files. Note that
+`sys.stdout` and `sys.stdin` are text streams, so they can only be
+used directly for ASCII-format PLY files.
+
 # FAQ
 
 ## How do I initialize a list property from two-dimensional array?
 
 ```Python Console
 >>> # Here's a two-dimensional array containing vertex indices.
 >>> face_data = numpy.array([[0, 1, 2], [3, 4, 5]], dtype='i4')
 >>>
 >>> # PlyElement.describe requires a one-dimensional structured array.
->>> ply_faces = numpy.empty(len(faces),
+>>> ply_faces = numpy.empty(len(face_data),
 ...                         dtype=[('vertex_indices', 'i4', (3,))])
 >>> ply_faces['vertex_indices'] = face_data
 >>> face = PlyElement.describe(ply_faces, 'face')
+>>>
 ```
 
 ## Can I save a PLY file directly to `sys.stdout`?
 
-On Python 3, you will probably run into issues because `sys.stdout` is a
-text-mode stream and `plyfile` outputs binary data, even for
-ASCII-format PLY files:
-
-```Python Console
->>> import sys
->>> plydata.write(sys.stdout)
-Traceback (most recent call last):
-  File "<stdin>", line 1, in <module>
-    File ".../python-plyfile/plyfile.py", line 411, in write
-        stream.write(self.header.encode('ascii'))
-        TypeError: write() argument must be str, not bytes
-```
+Yes, for an ASCII-format PLY file. For binary-format files, it won't
+work directly, since `sys.stdout` is a text-mode stream and binary-format
+files can only be output to binary streams. (ASCII-format files can be
+output to text or binary streams.)
 
 There are a few ways around this.
 - Write to a named file instead. On Linux and some other Unix-likes, you
   can access `stdout` via the named file `/dev/stdout`:
 
     ```Python Console
-    >>> plydata.write('/dev/stdout')
+    >>> plydata.write('/dev/stdout')  # doctest: +SKIP
     ```
 
 - Use `sys.stdout.buffer`:
 
     ```Python Console
-    >>> plydata.write(sys.stdout.buffer)
+    >>> plydata.write(sys.stdout.buffer)  # doctest: +SKIP
     ```
 
   (source: https://bugs.python.org/issue4571)
 
+## Can I read a PLY file from `sys.stdin`?
+
+The answer is exactly analogous to the situation with writing to
+`sys.stdout`: it works for ASCII-format PLY files but not binary-format
+files. The two workarounds given above also apply: use a named file like
+`/dev/stdin`, or use `sys.stdin.buffer`.
+
+
 # Design philosophy and rationale
 
 The design philosophy of `plyfile` can be summed up as follows.
 - Be familiar to users of `numpy` and reuse existing idioms and concepts
   when possible.
 - Favor simplicity over power or user-friendliness.
 - Support all valid PLY files.
@@ -584,8 +593,7 @@
 
 # License
 
 Copyright Darsh Ranjan.
 
 This software is released under the terms of the GNU General Public
 License, version 3.  See the file `COPYING` for details.
-
```

